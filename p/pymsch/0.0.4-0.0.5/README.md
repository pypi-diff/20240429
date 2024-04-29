# Comparing `tmp/pymsch-0.0.4.tar.gz` & `tmp/pymsch-0.0.5.tar.gz`

## Comparing `pymsch-0.0.4.tar` & `pymsch-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    37986 2020-02-02 00:00:00.000000 pymsch-0.0.4/src/pymsch/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pymsch-0.0.4/LICENSE
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymsch-0.0.4/README.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pymsch-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pymsch-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    39273 2020-02-02 00:00:00.000000 pymsch-0.0.5/src/pymsch/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pymsch-0.0.5/LICENSE
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymsch-0.0.5/README.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pymsch-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pymsch-0.0.5/PKG-INFO
```

### Comparing `pymsch-0.0.4/src/pymsch/__init__.py` & `pymsch-0.0.5/src/pymsch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,107 +8,110 @@
         self.y = y 
         self.config = config 
         self.rotation = rotation
 
     def get_block_name(self):
         return(self.block.name.lower().replace("_", "-"))
 
+    def set_config(self, config):
+        self.config = config
+
 class Schematic:
     pass
 
 class Schematic:
 
     def __init__(self):
         self.tiles = []
         self.tags = {}
-        self.types_list = []
+        self.labels = []
         self.filled_list = []
 
+    def copy(self):
+        a = Schematic()
+        a.tiles = self.tiles.copy()
+        a.tags = self.tags.copy()
+        a.labels = self.labels.copy()
+        a.filled_list = self.filled_list.copy()
+        return(a)
+
     def add_block(self, tile: Block, do_collision: bool = True):
-        if(len(self.types_list) >= 127 and tile.get_block_name() not in self.types_list):
-            raise Exception("Failed to add block (total block types can't exceed 127)")
+        if(self.test_block_collision(tile) == False or do_collision == False):
+            self.tiles.append(tile)
+            self.add_block_collision(tile)
+            return(tile)
         else:
-            if(self.test_block_collision(tile) == False or do_collision == False):
-                self.tiles.append(tile)
-                self.add_block_collision(tile)
-                if(tile.get_block_name() not in self.types_list):
-                    self.types_list.append(tile.get_block_name())
-                return(True)
-            else:
-                return(False)
+            return(None)
 
     def add_schem(self, schem: Schematic, x: int, y: int):
-        offset_x = 1000000
-        offset_y = 1000000
 
-        for block in self.tiles:
-            offset_x = min(offset_x, block.x + ((block.block.value.size - 1) // 2))
-            offset_y = min(offset_y, block.y + ((block.block.value.size - 1) // 2))
-        offset_x *= -1
-        offset_y *= -1
+        width, height, offset_x, offset_y = schem.get_dimensions(offsets = True)
 
-        for tile in list(schem.tiles):
-            self.add_block(Block(tile.block, tile.x + x - offset_x, tile.y + y - offset_y, tile.config, tile.rotation))
+        for tile in schem.tiles:
+            self.add_block(Block(tile.block, tile.x + x + offset_x, tile.y + y + offset_y, tile.config, tile.rotation))
 
     def write(self):
-        
-        width = -1000000
-        height = -1000000
-        offset_x = 1000000
-        offset_y = 1000000
 
-        for block in self.tiles:
-            offset_x = min(offset_x, block.x - ((block.block.value.size - 1) // 2))
-            offset_y = min(offset_y, block.y - ((block.block.value.size - 1) // 2))
-            width = max(width, block.x + (block.block.value.size // 2) + 1)
-            height = max(height, block.y + (block.block.value.size // 2) + 1)
-        offset_x *= -1
-        offset_y *= -1
-        width += offset_x
-        height += offset_y
+        schem = self.copy()
 
-        for block in self.tiles:
+        types_list = []
+        for tile in schem.tiles:
+            if(tile.get_block_name() not in types_list):
+                types_list.append(tile.get_block_name())
+        
+        width, height, offset_x, offset_y = schem.get_dimensions(offsets = True)
+
+        for block in schem.tiles:
             block.x = block.x + offset_x
             block.y = block.y + offset_y
 
         buffer = ByteBuffer()
 
         buffer.writeShort(width)
         buffer.writeShort(height)
 
-        buffer.writeByte(len(self.tags))
-        for k, v in self.tags.items():
+        labels = "["
+        for label in schem.labels:
+            labels += f"{label}, "
+        labels = labels.rstrip(', ') + ']'
+
+        schem.set_tag('labels', labels)
+
+        buffer.writeByte(len(schem.tags))
+        for k, v in schem.tags.items():
             buffer.writeUTF(k)
             buffer.writeUTF(v)
-        buffer.writeByte(len(self.types_list)) #dictionary
-        for t in self.types_list:
+        buffer.writeByte(len(types_list)) #dictionary
+        for t in types_list:
             buffer.writeUTF(t)
         
-        buffer.writeInt(len(self.tiles))
-        for t in self.tiles:
-            buffer.writeByte(self.types_list.index(t.get_block_name())) #dictionary index
+        buffer.writeInt(len(schem.tiles))
+        for t in schem.tiles:
+            buffer.writeByte(types_list.index(t.get_block_name())) #dictionary index
             buffer.writeShort(t.x) #x
             buffer.writeShort(t.y) #y
-            buffer.writeObject(t.config) #config, idk yet
+            buffer.writeObject(t.config) #config
             buffer.writeByte(t.rotation) #rotation
 
         return(b"msch\x01"+zlib.compress(buffer.data))
 
     def write_clipboard(self):
         s = base64.standard_b64encode(self.write()).decode()
-        #s = s[:6] + 'F' + s[7:] #no clue, but this makes it work
         pyperclip.copy(s)
 
     def write_file(self, file_path: str):
         file = open(file_path, 'wb')
         file.write(self.write())
 
     def set_tag(self, tag: str, value: str):
         self.tags[tag] = value
 
+    def add_label(self, label: str):
+        self.labels.append(label)
+
     def add_block_collision(self, block: Block):
         smallest_x = block.x - ((block.block.value.size - 1) // 2)
         smallest_y = block.y - ((block.block.value.size - 1) // 2)
 
         for x in range(smallest_x, smallest_x + block.block.value.size, 1):
             for y in range(smallest_y, smallest_y + block.block.value.size, 1):
                 if((x, y) not in self.filled_list):
@@ -120,14 +123,51 @@
 
         for x in range(smallest_x, smallest_x + block.block.value.size, 1):
             for y in range(smallest_y, smallest_y + block.block.value.size, 1):
                 if((x, y) in self.filled_list):
                     return(True)
         return(False)
 
+    def get_block(self, x: int, y: int):
+        for block in self.tiles:
+            smallest_x = block.x - ((block.block.value.size - 1) // 2)
+            smallest_y = block.y - ((block.block.value.size - 1) // 2)
+            if(x >= smallest_x and x < smallest_x + block.block.value.size and y >= smallest_y and y < smallest_y + block.block.value.size):
+                return(block)
+        return(None)
+
+    def get_dimensions(self, offsets = False):
+
+        if(len(self.tiles) == 0):
+            if(offsets == False):
+                return(0, 0)
+            else:
+                return(0, 0, 0, 0)
+
+        b = self.tiles[0]
+
+        width = b.x - ((b.block.value.size - 1) // 2)
+        height = b.y - ((b.block.value.size - 1) // 2)
+        offset_x = b.x + (b.block.value.size // 2) + 1
+        offset_y = b.y + (b.block.value.size // 2) + 1
+
+        for block in self.tiles:
+            offset_x = min(offset_x, block.x - ((block.block.value.size - 1) // 2))
+            offset_y = min(offset_y, block.y - ((block.block.value.size - 1) // 2))
+            width = max(width, block.x + (block.block.value.size // 2) + 1)
+            height = max(height, block.y + (block.block.value.size // 2) + 1)
+        offset_x *= -1
+        offset_y *= -1
+        width += offset_x
+        height += offset_y
+        if(offsets == False):
+            return(width, height)
+        else:
+            return(width, height, offset_x, offset_y)
+
 class ContentTypes(Enum):
     ITEM = 0
     BLOCK = 1
     MECH_UNUSED = 2
     BULLET = 3
     LIQUID = 4
     STATUS = 5
@@ -566,19 +606,19 @@
     ITEM_VOID = ContentBlock(384, 1)
     LIQUID_SOURCE = ContentBlock(385, 1)
     LIQUID_VOID = ContentBlock(386, 1)
     PAYLOAD_SOURCE = ContentBlock(387, 5)
     PAYLOAD_VOID = ContentBlock(388, 5)
     HEAT_SOURCE = ContentBlock(389, 1)
     ILLUMINATOR = ContentBlock(390, 1)
-    LEGACY_MECH_PAD = ContentBlock(391, 1)
-    LEGACY_UNIT_FACTORY = ContentBlock(392, 1)
-    LEGACY_UNIT_FACTORY_AIR = ContentBlock(393, 1)
-    LEGACY_UNIT_FACTORY_GROUND = ContentBlock(394, 1)
-    COMMAND_CENTER = ContentBlock(395, 2)
+    # LEGACY_MECH_PAD = ContentBlock(391, 1)
+    # LEGACY_UNIT_FACTORY = ContentBlock(392, 1)
+    # LEGACY_UNIT_FACTORY_AIR = ContentBlock(393, 1)
+    # LEGACY_UNIT_FACTORY_GROUND = ContentBlock(394, 1)
+    # COMMAND_CENTER = ContentBlock(395, 2)
     LAUNCH_PAD = ContentBlock(396, 3)
     INTERPLANETARY_ACCELERATOR = ContentBlock(397, 7)
     MESSAGE = ContentBlock(398, 1)
     SWITCH = ContentBlock(399, 1)
     MICRO_PROCESSOR = ContentBlock(400, 1)
     LOGIC_PROCESSOR = ContentBlock(401, 2)
     HYPER_PROCESSOR = ContentBlock(402, 3)
@@ -677,29 +717,29 @@
                 BLOCKS.append(content)
             elif(content.value.type == ContentTypes.ITEM):
                 ITEMS.append(content)
             elif(content.value.type == ContentTypes.UNIT):
                 UNITS.append(content)
             elif(content.value.type == ContentTypes.LIQUID):
                 LIQUIDS.append(content)
-        BUILDINGS = [Content.GRAPHITE_PRESS, Content.MULTI_PRESS, Content.SILICON_SMELTER, Content.SILICON_CRUCIBLE, Content.KILN, Content.PLASTANIUM_COMPRESSOR, Content.PHASE_WEAVER, Content.SURGE_SMELTER, Content.CRYOFLUID_MIXER, Content.PYRATITE_MIXER, Content.BLAST_MIXER, Content.MELTER, Content.SEPARATOR, Content.DISASSEMBLER, Content.SPORE_PRESS, Content.PULVERIZER, Content.COAL_CENTRIFUGE, Content.INCINERATOR, Content.SILICON_ARC_FURNACE, Content.ELECTROLYZER, Content.ATMOSPHERIC_CONCENTRATOR, Content.OXIDATION_CHAMBER, Content.ELECTRIC_HEATER, Content.SLAG_HEATER, Content.PHASE_HEATER, Content.HEAT_REDIRECTOR, Content.HEAT_ROUTER, Content.SLAG_INCINERATOR, Content.CARBIDE_CRUCIBLE, Content.SLAG_CENTRIFUGE, Content.SURGE_CRUCIBLE, Content.CYANOGEN_SYNTHESIZER, Content.PHASE_SYNTHESIZER, Content.HEAT_REACTOR, Content.COPPER_WALL, Content.COPPER_WALL_LARGE, Content.TITANIUM_WALL, Content.TITANIUM_WALL_LARGE, Content.PLASTANIUM_WALL, Content.PLASTANIUM_WALL_LARGE, Content.THORIUM_WALL, Content.THORIUM_WALL_LARGE, Content.PHASE_WALL, Content.PHASE_WALL_LARGE, Content.SURGE_WALL, Content.SURGE_WALL_LARGE, Content.DOOR, Content.DOOR_LARGE, Content.SCRAP_WALL, Content.SCRAP_WALL_LARGE, Content.SCRAP_WALL_HUGE, Content.SCRAP_WALL_GIGANTIC, Content.THRUSTER, Content.BERYLLIUM_WALL, Content.BERYLLIUM_WALL_LARGE, Content.TUNGSTEN_WALL, Content.TUNGSTEN_WALL_LARGE, Content.BLAST_DOOR, Content.REINFORCED_SURGE_WALL, Content.REINFORCED_SURGE_WALL_LARGE, Content.CARBIDE_WALL, Content.CARBIDE_WALL_LARGE, Content.SHIELDED_WALL, Content.MENDER, Content.MEND_PROJECTOR, Content.OVERDRIVE_PROJECTOR, Content.OVERDRIVE_DOME, Content.FORCE_PROJECTOR, Content.SHOCK_MINE, Content.RADAR, Content.BUILD_TOWER, Content.REGEN_PROJECTOR, Content.SHOCKWAVE_TOWER, Content.SHIELD_PROJECTOR, Content.LARGE_SHIELD_PROJECTOR, Content.CONVEYOR, Content.TITANIUM_CONVEYOR, Content.PLASTANIUM_CONVEYOR, Content.ARMORED_CONVEYOR, Content.JUNCTION, Content.BRIDGE_CONVEYOR, Content.PHASE_CONVEYOR, Content.SORTER, Content.INVERTED_SORTER, Content.ROUTER, Content.DISTRIBUTOR, Content.OVERFLOW_GATE, Content.UNDERFLOW_GATE, Content.MASS_DRIVER, Content.DUCT, Content.ARMORED_DUCT, Content.DUCT_ROUTER, Content.OVERFLOW_DUCT, Content.UNDERFLOW_DUCT, Content.DUCT_BRIDGE, Content.DUCT_UNLOADER, Content.SURGE_CONVEYOR, Content.SURGE_ROUTER, Content.UNIT_CARGO_LOADER, Content.UNIT_CARGO_UNLOAD_POINT, Content.MECHANICAL_PUMP, Content.ROTARY_PUMP, Content.IMPULSE_PUMP, Content.CONDUIT, Content.PULSE_CONDUIT, Content.PLATED_CONDUIT, Content.LIQUID_ROUTER, Content.LIQUID_CONTAINER, Content.LIQUID_TANK, Content.LIQUID_JUNCTION, Content.BRIDGE_CONDUIT, Content.PHASE_CONDUIT, Content.REINFORCED_PUMP, Content.REINFORCED_CONDUIT, Content.REINFORCED_LIQUID_JUNCTION, Content.REINFORCED_BRIDGE_CONDUIT, Content.REINFORCED_LIQUID_ROUTER, Content.REINFORCED_LIQUID_CONTAINER, Content.REINFORCED_LIQUID_TANK, Content.POWER_NODE, Content.POWER_NODE_LARGE, Content.SURGE_TOWER, Content.DIODE, Content.BATTERY, Content.BATTERY_LARGE, Content.COMBUSTION_GENERATOR, Content.THERMAL_GENERATOR, Content.STEAM_GENERATOR, Content.DIFFERENTIAL_GENERATOR, Content.RTG_GENERATOR, Content.SOLAR_PANEL, Content.SOLAR_PANEL_LARGE, Content.THORIUM_REACTOR, Content.IMPACT_REACTOR, Content.BEAM_NODE, Content.BEAM_TOWER, Content.BEAM_LINK, Content.TURBINE_CONDENSER, Content.CHEMICAL_COMBUSTION_CHAMBER, Content.PYROLYSIS_GENERATOR, Content.FLUX_REACTOR, Content.NEOPLASIA_REACTOR, Content.MECHANICAL_DRILL, Content.PNEUMATIC_DRILL, Content.LASER_DRILL, Content.BLAST_DRILL, Content.WATER_EXTRACTOR, Content.CULTIVATOR, Content.OIL_EXTRACTOR, Content.VENT_CONDENSER, Content.CLIFF_CRUSHER, Content.PLASMA_BORE, Content.LARGE_PLASMA_BORE, Content.IMPACT_DRILL, Content.ERUPTION_DRILL, Content.CORE_SHARD, Content.CORE_FOUNDATION, Content.CORE_NUCLEUS, Content.CORE_BASTION, Content.CORE_CITADEL, Content.CORE_ACROPOLIS, Content.CONTAINER, Content.VAULT, Content.UNLOADER, Content.REINFORCED_CONTAINER, Content.REINFORCED_VAULT, Content.DUO, Content.SCATTER, Content.SCORCH, Content.HAIL, Content.WAVE, Content.LANCER, Content.ARC, Content.PARALLAX, Content.SWARMER, Content.SALVO, Content.SEGMENT, Content.TSUNAMI, Content.FUSE, Content.RIPPLE, Content.CYCLONE, Content.FORESHADOW, Content.SPECTRE, Content.MELTDOWN, Content.BREACH, Content.DIFFUSE, Content.SUBLIMATE, Content.TITAN, Content.DISPERSE, Content.AFFLICT, Content.LUSTRE, Content.SCATHE, Content.SMITE, Content.MALIGN, Content.GROUND_FACTORY, Content.AIR_FACTORY, Content.NAVAL_FACTORY, Content.ADDITIVE_RECONSTRUCTOR, Content.MULTIPLICATIVE_RECONSTRUCTOR, Content.EXPONENTIAL_RECONSTRUCTOR, Content.TETRATIVE_RECONSTRUCTOR, Content.REPAIR_POINT, Content.REPAIR_TURRET, Content.TANK_FABRICATOR, Content.SHIP_FABRICATOR, Content.MECH_FABRICATOR, Content.TANK_REFABRICATOR, Content.SHIP_REFABRICATOR, Content.MECH_REFABRICATOR, Content.PRIME_REFABRICATOR, Content.TANK_ASSEMBLER, Content.SHIP_ASSEMBLER, Content.MECH_ASSEMBLER, Content.BASIC_ASSEMBLER_MODULE, Content.UNIT_REPAIR_TOWER, Content.PAYLOAD_CONVEYOR, Content.PAYLOAD_ROUTER, Content.REINFORCED_PAYLOAD_CONVEYOR, Content.REINFORCED_PAYLOAD_ROUTER, Content.PAYLOAD_MASS_DRIVER, Content.LARGE_PAYLOAD_MASS_DRIVER, Content.SMALL_DECONSTRUCTOR, Content.DECONSTRUCTOR, Content.CONSTRUCTOR, Content.LARGE_CONSTRUCTOR, Content.PAYLOAD_LOADER, Content.PAYLOAD_UNLOADER, Content.POWER_SOURCE, Content.POWER_VOID, Content.ITEM_SOURCE, Content.ITEM_VOID, Content.LIQUID_SOURCE, Content.LIQUID_VOID, Content.PAYLOAD_SOURCE, Content.PAYLOAD_VOID, Content.HEAT_SOURCE, Content.ILLUMINATOR, Content.LEGACY_MECH_PAD, Content.LEGACY_UNIT_FACTORY, Content.LEGACY_UNIT_FACTORY_AIR, Content.LEGACY_UNIT_FACTORY_GROUND, Content.COMMAND_CENTER, Content.LAUNCH_PAD, Content.INTERPLANETARY_ACCELERATOR, Content.MESSAGE, Content.SWITCH, Content.MICRO_PROCESSOR, Content.LOGIC_PROCESSOR, Content.HYPER_PROCESSOR, Content.MEMORY_CELL, Content.MEMORY_BANK, Content.LOGIC_DISPLAY, Content.LARGE_LOGIC_DISPLAY, Content.CANVAS, Content.REINFORCED_MESSAGE, Content.WORLD_PROCESSOR, Content.WORLD_CELL, Content.WORLD_MESSAGE, Content.WORLD_SWITCH]
+        BUILDINGS = [Content.GRAPHITE_PRESS, Content.MULTI_PRESS, Content.SILICON_SMELTER, Content.SILICON_CRUCIBLE, Content.KILN, Content.PLASTANIUM_COMPRESSOR, Content.PHASE_WEAVER, Content.SURGE_SMELTER, Content.CRYOFLUID_MIXER, Content.PYRATITE_MIXER, Content.BLAST_MIXER, Content.MELTER, Content.SEPARATOR, Content.DISASSEMBLER, Content.SPORE_PRESS, Content.PULVERIZER, Content.COAL_CENTRIFUGE, Content.INCINERATOR, Content.SILICON_ARC_FURNACE, Content.ELECTROLYZER, Content.ATMOSPHERIC_CONCENTRATOR, Content.OXIDATION_CHAMBER, Content.ELECTRIC_HEATER, Content.SLAG_HEATER, Content.PHASE_HEATER, Content.HEAT_REDIRECTOR, Content.HEAT_ROUTER, Content.SLAG_INCINERATOR, Content.CARBIDE_CRUCIBLE, Content.SLAG_CENTRIFUGE, Content.SURGE_CRUCIBLE, Content.CYANOGEN_SYNTHESIZER, Content.PHASE_SYNTHESIZER, Content.HEAT_REACTOR, Content.COPPER_WALL, Content.COPPER_WALL_LARGE, Content.TITANIUM_WALL, Content.TITANIUM_WALL_LARGE, Content.PLASTANIUM_WALL, Content.PLASTANIUM_WALL_LARGE, Content.THORIUM_WALL, Content.THORIUM_WALL_LARGE, Content.PHASE_WALL, Content.PHASE_WALL_LARGE, Content.SURGE_WALL, Content.SURGE_WALL_LARGE, Content.DOOR, Content.DOOR_LARGE, Content.SCRAP_WALL, Content.SCRAP_WALL_LARGE, Content.SCRAP_WALL_HUGE, Content.SCRAP_WALL_GIGANTIC, Content.THRUSTER, Content.BERYLLIUM_WALL, Content.BERYLLIUM_WALL_LARGE, Content.TUNGSTEN_WALL, Content.TUNGSTEN_WALL_LARGE, Content.BLAST_DOOR, Content.REINFORCED_SURGE_WALL, Content.REINFORCED_SURGE_WALL_LARGE, Content.CARBIDE_WALL, Content.CARBIDE_WALL_LARGE, Content.SHIELDED_WALL, Content.MENDER, Content.MEND_PROJECTOR, Content.OVERDRIVE_PROJECTOR, Content.OVERDRIVE_DOME, Content.FORCE_PROJECTOR, Content.SHOCK_MINE, Content.RADAR, Content.BUILD_TOWER, Content.REGEN_PROJECTOR, Content.SHOCKWAVE_TOWER, Content.SHIELD_PROJECTOR, Content.LARGE_SHIELD_PROJECTOR, Content.CONVEYOR, Content.TITANIUM_CONVEYOR, Content.PLASTANIUM_CONVEYOR, Content.ARMORED_CONVEYOR, Content.JUNCTION, Content.BRIDGE_CONVEYOR, Content.PHASE_CONVEYOR, Content.SORTER, Content.INVERTED_SORTER, Content.ROUTER, Content.DISTRIBUTOR, Content.OVERFLOW_GATE, Content.UNDERFLOW_GATE, Content.MASS_DRIVER, Content.DUCT, Content.ARMORED_DUCT, Content.DUCT_ROUTER, Content.OVERFLOW_DUCT, Content.UNDERFLOW_DUCT, Content.DUCT_BRIDGE, Content.DUCT_UNLOADER, Content.SURGE_CONVEYOR, Content.SURGE_ROUTER, Content.UNIT_CARGO_LOADER, Content.UNIT_CARGO_UNLOAD_POINT, Content.MECHANICAL_PUMP, Content.ROTARY_PUMP, Content.IMPULSE_PUMP, Content.CONDUIT, Content.PULSE_CONDUIT, Content.PLATED_CONDUIT, Content.LIQUID_ROUTER, Content.LIQUID_CONTAINER, Content.LIQUID_TANK, Content.LIQUID_JUNCTION, Content.BRIDGE_CONDUIT, Content.PHASE_CONDUIT, Content.REINFORCED_PUMP, Content.REINFORCED_CONDUIT, Content.REINFORCED_LIQUID_JUNCTION, Content.REINFORCED_BRIDGE_CONDUIT, Content.REINFORCED_LIQUID_ROUTER, Content.REINFORCED_LIQUID_CONTAINER, Content.REINFORCED_LIQUID_TANK, Content.POWER_NODE, Content.POWER_NODE_LARGE, Content.SURGE_TOWER, Content.DIODE, Content.BATTERY, Content.BATTERY_LARGE, Content.COMBUSTION_GENERATOR, Content.THERMAL_GENERATOR, Content.STEAM_GENERATOR, Content.DIFFERENTIAL_GENERATOR, Content.RTG_GENERATOR, Content.SOLAR_PANEL, Content.SOLAR_PANEL_LARGE, Content.THORIUM_REACTOR, Content.IMPACT_REACTOR, Content.BEAM_NODE, Content.BEAM_TOWER, Content.BEAM_LINK, Content.TURBINE_CONDENSER, Content.CHEMICAL_COMBUSTION_CHAMBER, Content.PYROLYSIS_GENERATOR, Content.FLUX_REACTOR, Content.NEOPLASIA_REACTOR, Content.MECHANICAL_DRILL, Content.PNEUMATIC_DRILL, Content.LASER_DRILL, Content.BLAST_DRILL, Content.WATER_EXTRACTOR, Content.CULTIVATOR, Content.OIL_EXTRACTOR, Content.VENT_CONDENSER, Content.CLIFF_CRUSHER, Content.PLASMA_BORE, Content.LARGE_PLASMA_BORE, Content.IMPACT_DRILL, Content.ERUPTION_DRILL, Content.CORE_SHARD, Content.CORE_FOUNDATION, Content.CORE_NUCLEUS, Content.CORE_BASTION, Content.CORE_CITADEL, Content.CORE_ACROPOLIS, Content.CONTAINER, Content.VAULT, Content.UNLOADER, Content.REINFORCED_CONTAINER, Content.REINFORCED_VAULT, Content.DUO, Content.SCATTER, Content.SCORCH, Content.HAIL, Content.WAVE, Content.LANCER, Content.ARC, Content.PARALLAX, Content.SWARMER, Content.SALVO, Content.SEGMENT, Content.TSUNAMI, Content.FUSE, Content.RIPPLE, Content.CYCLONE, Content.FORESHADOW, Content.SPECTRE, Content.MELTDOWN, Content.BREACH, Content.DIFFUSE, Content.SUBLIMATE, Content.TITAN, Content.DISPERSE, Content.AFFLICT, Content.LUSTRE, Content.SCATHE, Content.SMITE, Content.MALIGN, Content.GROUND_FACTORY, Content.AIR_FACTORY, Content.NAVAL_FACTORY, Content.ADDITIVE_RECONSTRUCTOR, Content.MULTIPLICATIVE_RECONSTRUCTOR, Content.EXPONENTIAL_RECONSTRUCTOR, Content.TETRATIVE_RECONSTRUCTOR, Content.REPAIR_POINT, Content.REPAIR_TURRET, Content.TANK_FABRICATOR, Content.SHIP_FABRICATOR, Content.MECH_FABRICATOR, Content.TANK_REFABRICATOR, Content.SHIP_REFABRICATOR, Content.MECH_REFABRICATOR, Content.PRIME_REFABRICATOR, Content.TANK_ASSEMBLER, Content.SHIP_ASSEMBLER, Content.MECH_ASSEMBLER, Content.BASIC_ASSEMBLER_MODULE, Content.UNIT_REPAIR_TOWER, Content.PAYLOAD_CONVEYOR, Content.PAYLOAD_ROUTER, Content.REINFORCED_PAYLOAD_CONVEYOR, Content.REINFORCED_PAYLOAD_ROUTER, Content.PAYLOAD_MASS_DRIVER, Content.LARGE_PAYLOAD_MASS_DRIVER, Content.SMALL_DECONSTRUCTOR, Content.DECONSTRUCTOR, Content.CONSTRUCTOR, Content.LARGE_CONSTRUCTOR, Content.PAYLOAD_LOADER, Content.PAYLOAD_UNLOADER, Content.POWER_SOURCE, Content.POWER_VOID, Content.ITEM_SOURCE, Content.ITEM_VOID, Content.LIQUID_SOURCE, Content.LIQUID_VOID, Content.PAYLOAD_SOURCE, Content.PAYLOAD_VOID, Content.HEAT_SOURCE, Content.ILLUMINATOR, Content.LAUNCH_PAD, Content.INTERPLANETARY_ACCELERATOR, Content.MESSAGE, Content.SWITCH, Content.MICRO_PROCESSOR, Content.LOGIC_PROCESSOR, Content.HYPER_PROCESSOR, Content.MEMORY_CELL, Content.MEMORY_BANK, Content.LOGIC_DISPLAY, Content.LARGE_LOGIC_DISPLAY, Content.CANVAS, Content.REINFORCED_MESSAGE, Content.WORLD_PROCESSOR, Content.WORLD_CELL, Content.WORLD_MESSAGE, Content.WORLD_SWITCH]
 
 class double(float):
     pass
 
 class long(int):
     pass
 
 class Point:
     def __init__(self, x: float, y: float):
         self.x = x
         self.y = y
 
 class PointArray:
-    def __init__(self, array):
+    def __init__(self, array = []):
         self.array = []
         a = 0
         for i in array:
             self.insert(a, i)
             a += 1
 
     def __getitem__(self, index):
@@ -713,14 +753,17 @@
 
     def __iter__(self):
         return(iter(self.array))
 
     def __len__(self):
         return(len(self.array))
 
+    def append(self, item):
+        self.array.append(item)
+
 class ProcessorConfig:
     def __init__(self, code: str, links: list):
         self.code = code
         self.links = links
 
     def compress(self):
         buffer = ByteBuffer()
@@ -728,16 +771,16 @@
         buffer.writeByte(1)
 
         buffer.writeBytesFromStr(self.code)
 
         buffer.writeInt(len(self.links))
         for link in self.links:
             buffer.writeUTF(link.name)
-            buffer.writeShort(link.x)
-            buffer.writeShort(link.y)
+            buffer.writeSShort(link.x)
+            buffer.writeSShort(link.y)
 
         return(bytearray(zlib.compress(buffer.data)))
 
 class ProcessorLink:
     def __init__(self, x, y, name):
         self.x = x
         self.y = y
@@ -753,14 +796,18 @@
     def writeSShort(self, var: int):
         self.data += struct.pack(">h", var)
 
     def writeUTF(self, var: str):
         self.writeShort(len(var))
         self.data += bytes(var.encode("UTF"))
 
+    def writeString(self, var: str):
+        self.writeByte(1)
+        self.writeUTF(var)
+
     def writeBytesFromStr(self, var: str):
         self.writeInt(len(var))
         self.data.extend(map(ord, var))
         
     def writeByte(self, var: int):
         self.data += struct.pack("b", var)
 
@@ -792,15 +839,15 @@
             self.writeByte(2)
             self.writeLong(obj)
         elif(type(obj) is float):
             self.writeByte(3)
             self.writeFloat(obj)
         elif(type(obj) is str):
             self.writeByte(4)
-            self.writeUTF(obj)
+            self.writeString(obj)
         elif(type(obj).__name__ == 'Content'):
             self.writeByte(5)
             self.writeByte(obj.value.type.value)
             self.writeShort(obj.value.id)
         #elif(type(obj) is str): #intSeq
         #    self.writeByte(6)
         elif(type(obj).__name__ == 'Point'):
@@ -828,14 +875,20 @@
         #elif(type(obj) is str): #LAccess
         #    self.writeByte(13)
         elif(type(obj) is bytearray): #Byte array
             self.writeByte(14)
             self.writeInt(len(obj))
             for b in obj:
                 self.writeUByte(b)
+        elif(type(obj).__name__ == "ProcessorConfig"): #Byte array
+            self.writeByte(14)
+            data = obj.compress()
+            self.writeInt(len(data))
+            for b in data:
+                self.writeUByte(b)
         #elif(type(obj) is str): #Bool array
         #    self.writeByte(16)
         #elif(type(obj) is str): #Unit
         #    self.writeByte(17)
         #elif(type(obj) is str): #Vec2 array
         #    self.writeByte(18)
         #elif(type(obj) is str): #Vec2
```

### Comparing `pymsch-0.0.4/LICENSE` & `pymsch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymsch-0.0.4/PKG-INFO` & `pymsch-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pymsch
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for creating mindustry schematic files
 Author: skyethefoxyfox
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

