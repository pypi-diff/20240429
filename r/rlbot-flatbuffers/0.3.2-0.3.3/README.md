# Comparing `tmp/rlbot_flatbuffers-0.3.2.tar.gz` & `tmp/rlbot_flatbuffers-0.3.3.tar.gz`

## Comparing `rlbot_flatbuffers-0.3.2.tar` & `rlbot_flatbuffers-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.2/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/LICENSE
--rw-r--r--   0     1001      127      479 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/README.md
--rw-r--r--   0     1001      127    60199 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/build.rs
--rw-r--r--   0     1001      127      182 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/README.md
--rw-r--r--   0     1001      127      401 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/comms.fbs
--rw-r--r--   0     1001      127     1932 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/event.fbs
--rwxr-xr-x   0     1001      127  6681832 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc
--rw-r--r--   0     1001      127  3488256 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc.exe
--rw-r--r--   0     1001      127  6896752 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc_mac
--rw-r--r--   0     1001      127     1281 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/gamestate.fbs
--rw-r--r--   0     1001      127     5824 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/matchstart.fbs
--rw-r--r--   0     1001      127     1162 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/rendering.fbs
--rw-r--r--   0     1001      127     6296 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/rlbot.fbs
--rw-r--r--   0     1001      127     4770 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/src/lib.rs
--rw-r--r--   0     1001      127    12644 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/Cargo.lock
--rw-r--r--   0     1001      127      418 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.3/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-04-29 03:47:00.000000 rlbot_flatbuffers-0.3.3/LICENSE
+-rw-r--r--   0     1001      127      479 2024-04-29 03:47:00.000000 rlbot_flatbuffers-0.3.3/README.md
+-rw-r--r--   0     1001      127    60227 2024-04-29 03:47:00.000000 rlbot_flatbuffers-0.3.3/build.rs
+-rw-r--r--   0     1001      127      182 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/README.md
+-rw-r--r--   0     1001      127      401 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/comms.fbs
+-rw-r--r--   0     1001      127     1932 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/event.fbs
+-rwxr-xr-x   0     1001      127  6681832 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/flatc
+-rw-r--r--   0     1001      127  3488256 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/flatc.exe
+-rw-r--r--   0     1001      127  6896752 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/flatc_mac
+-rw-r--r--   0     1001      127     1281 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/gamestate.fbs
+-rw-r--r--   0     1001      127     5824 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/matchstart.fbs
+-rw-r--r--   0     1001      127     1162 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/rendering.fbs
+-rw-r--r--   0     1001      127     6296 2024-04-29 03:47:01.000000 rlbot_flatbuffers-0.3.3/flatbuffers-schema/rlbot.fbs
+-rw-r--r--   0     1001      127     4757 2024-04-29 03:47:00.000000 rlbot_flatbuffers-0.3.3/src/lib.rs
+-rw-r--r--   0     1001      127    13114 2024-04-29 03:47:00.000000 rlbot_flatbuffers-0.3.3/Cargo.lock
+-rw-r--r--   0     1001      127      418 2024-04-29 03:47:00.000000 rlbot_flatbuffers-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.3/PKG-INFO
```

### Comparing `rlbot_flatbuffers-0.3.2/Cargo.toml` & `rlbot_flatbuffers-0.3.3/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlbot-flatbuffers-py"
-version = "0.3.2"
+version = "0.3.3"
 edition = "2021"
 description = "A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers"
 repository = "https://github.com/VirxEC/rlbot-flatbuffers-py"
 license = "MIT"
 readme = "README.md"
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore", ".gitmodules"]
 publish = false
@@ -16,15 +16,15 @@
 [lib]
 name = "rlbot_flatbuffers"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = "0.21.0"
 serde = "1.0.197"
-flatbuffers = { git = "https://github.com/google/flatbuffers", branch = "master" }
+flatbuffers = "24.3.25"
 get-size = { version = "0.1.4", features = ["derive"] }
 
 [profile.release]
 lto = true
 strip = true
 codegen-units = 1
 panic = "abort"
```

### Comparing `rlbot_flatbuffers-0.3.2/LICENSE` & `rlbot_flatbuffers-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/build.rs` & `rlbot_flatbuffers-0.3.3/build.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1200,18 +1200,19 @@
 
     fs::write(format!("{PYTHON_OUT_FOLDER}/mod.rs"), file_contents.join("\n"))?;
 
     Ok(())
 }
 
 fn class_names_txt_generator(type_data: &[(String, String, Vec<Vec<String>>)]) -> io::Result<()> {
-    let class_names = type_data
+    let mut class_names = type_data
         .iter()
         .map(|(_, type_name, _)| format!("    {type_name}"))
         .collect::<Vec<_>>();
+    class_names.sort();
 
     let file_contents = format!("[\n{}\n]", class_names.join(",\n"));
 
     fs::write("classes.txt", file_contents)?;
 
     Ok(())
 }
```

### Comparing `rlbot_flatbuffers-0.3.2/flatbuffers-schema/event.fbs` & `rlbot_flatbuffers-0.3.3/flatbuffers-schema/event.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc` & `rlbot_flatbuffers-0.3.3/flatbuffers-schema/flatc`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc.exe` & `rlbot_flatbuffers-0.3.3/flatbuffers-schema/flatc.exe`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc_mac` & `rlbot_flatbuffers-0.3.3/flatbuffers-schema/flatc_mac`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/flatbuffers-schema/gamestate.fbs` & `rlbot_flatbuffers-0.3.3/flatbuffers-schema/gamestate.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/flatbuffers-schema/matchstart.fbs` & `rlbot_flatbuffers-0.3.3/flatbuffers-schema/matchstart.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/flatbuffers-schema/rendering.fbs` & `rlbot_flatbuffers-0.3.3/flatbuffers-schema/rendering.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/flatbuffers-schema/rlbot.fbs` & `rlbot_flatbuffers-0.3.3/flatbuffers-schema/rlbot.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.2/src/lib.rs` & `rlbot_flatbuffers-0.3.3/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -108,110 +108,110 @@
 }
 
 macro_rules! pynamedmodule {
     (doc: $doc:literal, name: $name:tt, classes: [$($class_name:ident),*], vars: [$(($var_name:literal, $value:expr)),*]) => {
         #[doc = $doc]
         #[pymodule]
         #[allow(redundant_semicolons)]
-        fn $name(_py: Python, m: Bound<PyModule>) -> PyResult<()> {
+        fn $name(m: Bound<PyModule>) -> PyResult<()> {
             $(m.add_class::<$class_name>()?);*;
             $(m.add($var_name, $value)?);*;
             Ok(())
         }
     };
 }
 
 pynamedmodule! {
     doc: "rlbot_flatbuffers is a Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers.",
     name: rlbot_flatbuffers,
     classes: [
-        ExistingMatchBehavior,
-        PlayerStatEvent,
-        MatchComm,
-        DesiredCarState,
-        RemoveRenderGroup,
+        AirState,
+        BallBouncinessOption,
+        BallInfo,
+        BallMaxSpeedOption,
         BallPrediction,
-        PlayerInfo,
-        GameStateType,
-        GameSpeedOption,
-        ScoreInfo,
-        MessagePacket,
-        DemolishOption,
-        Vector3Partial,
-        TextHAlign,
+        BallSizeOption,
+        BallTypeOption,
+        BallWeightOption,
+        Bool,
         BoostOption,
-        RumbleOption,
-        Vector3,
-        GravityOption,
-        BallInfo,
-        ReadyMessage,
-        StartCommand,
-        MatchSettings,
-        OvertimeOption,
-        PlayerSpectate,
-        SphereShape,
-        Touch,
-        TextVAlign,
+        BoostPad,
+        BoostPadState,
+        BoostStrengthOption,
+        BoxShape,
+        CollisionShape,
+        Color,
         ConsoleCommand,
-        DesiredGameInfoState,
-        PredictionSlice,
-        PolyLine3D,
-        Rotator,
-        BallTypeOption,
-        LoadoutPaint,
-        RotatorPartial,
-        RLBot,
+        ControllerState,
         CylinderShape,
-        PlayerInputChange,
+        DemolishOption,
         DesiredBallState,
-        CollisionShape,
-        RenderMessage,
-        BoostPadState,
-        GameMode,
-        ControllerState,
-        BoostStrengthOption,
-        GoalInfo,
-        BallBouncinessOption,
-        MaxScore,
-        SeriesLengthOption,
-        GameMessage,
         DesiredBoostState,
-        BallSizeOption,
-        BallMaxSpeedOption,
-        MatchLength,
-        BallWeightOption,
-        PlayerLoadout,
-        Psyonix,
+        DesiredCarState,
+        DesiredGameInfoState,
+        DesiredGameState,
         DesiredPhysics,
-        AirState,
+        ExistingMatchBehavior,
+        FieldInfo,
+        Float,
+        GameInfo,
+        GameMessage,
         GameMessageWrapper,
+        GameMode,
+        GameSpeedOption,
+        GameStateType,
         GameTickPacket,
+        GoalInfo,
+        GravityOption,
         Human,
-        String3D,
-        Float,
-        FieldInfo,
-        PlayerClass,
-        BoostPad,
-        Bool,
-        RespawnTimeOption,
-        String2D,
-        PartyMember,
-        GameInfo,
-        StopCommand,
-        PlayerInput,
-        Color,
+        Launcher,
         Line3D,
-        Physics,
+        LoadoutPaint,
+        MatchComm,
+        MatchLength,
+        MatchSettings,
+        MaxScore,
+        MessagePacket,
         MutatorSettings,
+        OvertimeOption,
+        PartyMember,
+        Physics,
+        PlayerClass,
         PlayerConfiguration,
-        DesiredGameState,
-        TeamInfo,
-        RenderType,
+        PlayerInfo,
+        PlayerInput,
+        PlayerInputChange,
+        PlayerLoadout,
+        PlayerSpectate,
+        PlayerStatEvent,
+        PolyLine3D,
+        PredictionSlice,
+        Psyonix,
+        RLBot,
+        ReadyMessage,
+        RemoveRenderGroup,
         RenderGroup,
+        RenderMessage,
+        RenderType,
+        RespawnTimeOption,
+        Rotator,
+        RotatorPartial,
+        RumbleOption,
+        ScoreInfo,
         ScriptConfiguration,
-        Launcher,
-        BoxShape
+        SeriesLengthOption,
+        SphereShape,
+        StartCommand,
+        StopCommand,
+        String2D,
+        String3D,
+        TeamInfo,
+        TextHAlign,
+        TextVAlign,
+        Touch,
+        Vector3,
+        Vector3Partial
     ],
     vars: [
         ("__version__", env!("CARGO_PKG_VERSION"))
     ]
 }
```

### Comparing `rlbot_flatbuffers-0.3.2/Cargo.lock` & `rlbot_flatbuffers-0.3.3/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c124f12ade4e670107b132722d0ad1a5c9790bcbc1b265336369ea05626b4498"
 dependencies = [
  "attribute-derive-macro",
  "proc-macro2",
  "quote",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "attribute-derive-macro"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b217a07446e0fb086f83401a98297e2d81492122f5874db5391bd270a185f88"
@@ -23,15 +23,15 @@
  "collection_literals",
  "interpolator",
  "proc-macro-error",
  "proc-macro-utils",
  "proc-macro2",
  "quote",
  "quote-use",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
@@ -39,14 +39,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "collection_literals"
@@ -58,23 +64,24 @@
 name = "derive-where"
 version = "1.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62d671cc41a825ebabc75757b62d3d168c577f9149b2d49ece1dad1f72119d25"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "flatbuffers"
 version = "24.3.25"
-source = "git+https://github.com/google/flatbuffers?branch=master#f4a9c5325b7cba8ae432466bdfb90f857da0d593"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8add37afff2d4ffa83bc748a70b4b1370984f6980768554182424ef71447c35f"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "rustc_version",
 ]
 
 [[package]]
 name = "get-size"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -87,15 +94,15 @@
 name = "get-size-derive"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13a1bcfb855c1f340d5913ab542e36f25a1c56f57de79022928297632435dec2"
 dependencies = [
  "attribute-derive",
  "quote",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
@@ -116,17 +123,17 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -141,27 +148,27 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
@@ -205,26 +212,26 @@
  "proc-macro2",
  "quote",
  "smallvec",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -232,101 +239,101 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "quote-use"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a7b5abe3fe82fdeeb93f44d66a7b444dedf2e4827defb0a8e69c437b2de2ef94"
 dependencies = [
  "quote",
  "quote-use-macros",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote-use-macros"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97ea44c7e20f16017a76a245bb42188517e13d16dcb1aa18044bc406cdc3f4af"
 dependencies = [
  "derive-where",
  "proc-macro2",
  "quote",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "rlbot-flatbuffers-py"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "flatbuffers",
  "get-size",
  "pyo3",
  "serde",
 ]
 
@@ -349,30 +356,30 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.57",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
@@ -385,17 +392,17 @@
 dependencies = [
  "proc-macro2",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.57"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -420,61 +427,68 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `rlbot_flatbuffers-0.3.2/PKG-INFO` & `rlbot_flatbuffers-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rlbot_flatbuffers
-Version: 0.3.2
+Version: 0.3.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers
 License: MIT
 Requires-Python: >=3.10
```

