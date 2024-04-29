# Comparing `tmp/pyneople-0.2.7.tar.gz` & `tmp/pyneople-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.2.7.tar", last modified: Sat Apr 27 10:48:10 2024, max compression
+gzip compressed data, was "pyneople-0.2.8.tar", last modified: Mon Apr 29 03:27:11 2024, max compression
```

## Comparing `pyneople-0.2.7.tar` & `pyneople-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:48:10.984887 pyneople-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-27 10:48:01.000000 pyneople-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-27 10:48:10.984887 pyneople-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-27 10:48:01.000000 pyneople-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 10:48:01.000000 pyneople-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:48:10.984887 pyneople-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-27 10:48:01.000000 pyneople-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:48:10.980887 pyneople-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:48:10.980887 pyneople-0.2.7/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34094 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:48:10.980887 pyneople-0.2.7/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-27 10:48:10.000000 pyneople-0.2.7/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-27 10:48:10.000000 pyneople-0.2.7/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:48:10.000000 pyneople-0.2.7/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 10:48:10.000000 pyneople-0.2.7/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:27:11.305623 pyneople-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 03:27:01.000000 pyneople-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 03:27:11.305623 pyneople-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-29 03:27:01.000000 pyneople-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 03:27:01.000000 pyneople-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:27:11.305623 pyneople-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-29 03:27:01.000000 pyneople-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:27:11.301623 pyneople-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:27:11.301623 pyneople-0.2.8/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-29 03:27:01.000000 pyneople-0.2.8/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 03:27:01.000000 pyneople-0.2.8/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41313 2024-04-29 03:27:01.000000 pyneople-0.2.8/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-04-29 03:27:01.000000 pyneople-0.2.8/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-29 03:27:01.000000 pyneople-0.2.8/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:27:11.305623 pyneople-0.2.8/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 03:27:11.000000 pyneople-0.2.8/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 03:27:11.000000 pyneople-0.2.8/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:27:11.000000 pyneople-0.2.8/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 03:27:11.000000 pyneople-0.2.8/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.2.7/LICENSE` & `pyneople-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.7/PKG-INFO` & `pyneople-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.7
+Version: 0.2.8
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.2.7/setup.py` & `pyneople-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.2.7",
+    version="0.2.8",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.2.7/src/pyneople/METADATA.py` & `pyneople-0.2.8/src/pyneople/METADATA.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 # 직업명 문자열 길이의 최대값
 JOB_NAME_LENGTH = max(list(map(lambda x : len(x), list(JOBCLASS.keys()))))
 
 del jobclass_list
 
 # 착용가능 장비
-EQUIPMENT_LIST = ['weapon', 'title', 'jacket', 'shoulder', 'pants', 'shoes', 'waist', 'amulet', 'wrist', 'ring', 'support', 'magic_ston', 'earring']
+EQUIPMENT_LIST = ['weapon', 'title', 'jacket', 'shoulder', 'pants', 'shoes', 'waist', 'amulet', 'wrist', 'ring', 'support', 'magic_ston', 'earring', 'set_item_info']
 
 # 착용가능 아바타
 AVATAR_LIST = ['headgear', 'hair', 'face', 'jacket', 'pants', 'shoes', 'breast', 'waist', 'skin', 'aurora', 'weapon']
 
 # 플래티넘 엠블렘 착용 가능 부위
 PLATINUM_AVATAR_LIST = ['jacket', 'pants']
 
@@ -170,8 +170,45 @@
     'water_element_damage': '수속성 피해',
     'light_element_damage': '명속성 피해',
     'dark_element_damage': '암속성 피해',
     'bleed_damage': '출혈 피해',
     'poison_damage': '중독 피해',
     'burn_damage': '화상 피해',
     'electrocution_damage': '감전 피해'
- }
+ }
+
+BASE_EQUIPMENT_NAME = {
+    'item_name' :'itemName',
+    'item_available_level' :'itemAvailableLevel',
+    'item_rarity' :'itemRarity',
+    'reinforce' :'reinforce',
+    'amplification_name' :'amplificationName',
+    'refine' :'refine', 
+    'item_grade_name' :'itemGradeName',
+    'enchant' : 'enchant'
+}
+
+EQUIPMENT_NAME = {
+    'upgrade_info' : 'upgrade_info',
+    'mist_gear' :  'mist_gear',
+    'grow_info' : 'grow_info'
+}
+
+WEAPON_NAME = {
+    'bakal_info' : 'bakal_info',
+    'asrahan_info':'asrahan_info'
+}
+
+AVATAR_NAME = {
+        'item_name' : "itemName",
+        'item_rarity' : "itemRarity",
+        'option_ability' : "optionAbility",
+        'emblems' : 'emblems'
+}
+
+PLATINUM_AVATAR_NAME = {
+        'item_name' : "itemName",
+        'item_rarity' : "itemRarity",
+        'option_ability' : "optionAbility",
+        'emblems' : 'emblems',
+        'platinum_emblem' : 'emblems'
+}
```

### Comparing `pyneople-0.2.7/src/pyneople/character.py` & `pyneople-0.2.8/src/pyneople/character.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import urllib.parse
 from typing import Iterable, Union
 from .functions import get_request, explain_enchant
-from .METADATA import SERVER_NAME_2_ID, CHARACTER_SEARCH_NAME, CHARACTER_INFORMATION_NAME, STATUS_NAME, EQUIPMENT_LIST, AVATAR_LIST, PLATINUM_AVATAR_LIST
+from .METADATA import SERVER_NAME_2_ID, CHARACTER_SEARCH_NAME, \
+                    CHARACTER_INFORMATION_NAME, STATUS_NAME, EQUIPMENT_LIST, AVATAR_LIST, PLATINUM_AVATAR_LIST, BASE_EQUIPMENT_NAME, EQUIPMENT_NAME, WEAPON_NAME, AVATAR_NAME, PLATINUM_AVATAR_NAME
 
 __all__ = [
     "CharacterSearch",
     "CharacterInformation",
     "Timeline",
     "Status",
     "Equipments",
@@ -60,32 +61,36 @@
         url = f"https://api.neople.co.kr/df/servers/{arg_server_name}/characters?characterName={urllib.parse.quote(arg_character_name)}&limit=1&apikey={self._api_key}"
         
         # parse_data에 매개변수로 사용 될 것을 생각해서 dict를 받을 수 있도록 정보 다듬어서 제공
         try:
             return get_request(url).get("rows")[0]
         except IndexError:
             return dict()
+    sub_attribute_list = CHARACTER_SEARCH_NAME.keys()
     
-    def parse_data(self, arg_data : dict, attribute_list : Iterable[str] = CHARACTER_SEARCH_NAME.keys()):
+    @classmethod
+    def set_sub_attributes(cls, new_attribute_list : list[str]):
+        cls.sub_attribute_list = new_attribute_list
+
+    def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 속성에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
                 attribute_list(iterable of str) : 원하는 하위 속성 명
         """
         # 하위 속성에 데이터 할당
-        for attribute_name in attribute_list:            
+        for attribute_name in CharacterSearch.sub_attribute_list:            
             setattr(self, attribute_name, arg_data.get(CHARACTER_SEARCH_NAME[attribute_name]))
 
 
 class CharacterInformation(PyNeople):
     """
     Neople Open API 03. 캐릭터 '기본정보' 조회
     """
-
     def __init__(self, arg_api_key : str):
         super().__init__(arg_api_key)
     
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 기본 정보를 반환
             Args : 
@@ -93,23 +98,30 @@
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """    
         self._server_id = arg_server_id
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}?apikey={self._api_key}"
         return get_request(url)
     
-    def parse_data(self, arg_data : dict, attribute_list : Iterable[str] = CHARACTER_INFORMATION_NAME.keys()):
+    sub_attribute_list = CHARACTER_INFORMATION_NAME.keys()
+    
+    @classmethod
+    def set_sub_attributes(cls, new_attribute_list : list[str]):
+        cls.sub_attribute_list = new_attribute_list
+
+    def parse_data(self, arg_data : dict):
+
         """
         데이터를 정리해서 하위 속성에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
                 attribute_list(iterable of str) : 원하는 하위 속성 명
         """
         # 하위 속성에 데이터 할당
-        for attribute_name in attribute_list:
+        for attribute_name in CharacterInformation.sub_attribute_list:
             setattr(self, attribute_name, arg_data.get(CHARACTER_INFORMATION_NAME[attribute_name]))
 
 
 class Timeline(PyNeople):
     """
     Neople Open API 04. 캐릭터 '타임라인 정보' 조회
     """    
@@ -206,15 +218,23 @@
                 arg_server_id(str) :  서버 ID
                 
                 arg_character_id(str) : 캐릭터 ID
         """
         self._server_id = arg_server_id
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/status?apikey={self._api_key}'
         return get_request(url)
-    def parse_data(self, arg_data : dict, attribute_list : Iterable[str] = STATUS_NAME.keys()):
+
+    sub_attribute_list = STATUS_NAME.keys()
+    
+    @classmethod
+    def set_sub_attributes(cls, new_attribute_list : list[str]):
+        cls.sub_attribute_list = new_attribute_list
+
+
+    def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
                 attribute_list(iterable of str) : 원하는 하위 속성 명
         """
         
@@ -232,15 +252,15 @@
         
         # 상세 스탯 정리
         if arg_data.get('status'):
             for item in arg_data['status']:
                 arg_data[item['name']] = item['value']   
         
         # 하위 속성에 데이터 할당
-        for attribute_name in attribute_list:
+        for attribute_name in Status.sub_attribute_list:
             setattr(self, attribute_name, arg_data.get(STATUS_NAME[attribute_name]))
 
 class OptionInfo():
     """
     Equipments를 위해 사용되는 Class
     """
 
@@ -271,63 +291,124 @@
             for i, option in enumerate(arg_grow_info_dict.get('options')):
                 if option.get('transfer') == True:
                     setattr(self, 'transfer', i+1)
                 else:
                     pass    
                 setattr(self, f'option_{i+1}', option.get('explain')) 
 
-class Equipment():
+class BaseEquipment():
     """
     Equipments를 위해 사용되는 Class
-    """
-
+    가장 기초적인 장비 정보를 담으며 다른 장비에 부모클래스로 이용된다.
+    """    
+    sub_attribute_list = BASE_EQUIPMENT_NAME.keys()
     def __init__(self):
-        self.item_name = None
-        self.item_available_level = None
-        self.item_rarity = None
-        self.reinforce = None
-        self.item_grade_name = None
-        self.enchant = None
-        self.amplification_name = None
-        self.refine = None
-        self.upgrade_info = None
-        self.mist_gear = None
-        self.grow_info = GrowInfo()
-    
+        print(BaseEquipment.sub_attribute_list)
+        for sub_attribute in BaseEquipment.sub_attribute_list:
+            setattr(self, sub_attribute, None)
+    
+    @classmethod
+    def set_sub_attributes(cls, new_attribute_list : list[str]):
+        cls.sub_attribute_list = new_attribute_list
+
     def get_equipment_data(self, arg_equipment_dict : dict):
-        self.item_name = arg_equipment_dict.get('itemName') # 이름
-        self.item_available_level = arg_equipment_dict.get('itemAvailableLevel') # 레벨 제한
-        self.item_rarity = arg_equipment_dict.get('itemRarity') # 레어도
-        self.reinforce = arg_equipment_dict.get('reinforce') # 강화수치             
-        self.amplification_name = arg_equipment_dict.get('amplificationName') # 차원의 기운 여부 ex 차원의 힘, 차원의 지능, None
-        self.refine = arg_equipment_dict.get('refine') # 제련   
-        self.item_grade_name = arg_equipment_dict.get('itemGradeName') # 등급(최상~최하)
-        self.enchant = explain_enchant(arg_equipment_dict.get('enchant')) # 마법부여
-
-        # 미스트 기어 정보
-        if arg_equipment_dict.get('mistGear'):
-            self.mist_gear = 'mist_gear'
-        elif arg_equipment_dict.get('pureMistGear'):
-            self.mist_gear = 'pure_mist_gear'   
-        elif arg_equipment_dict.get('refinedMistGear'):
-            self.mist_gear = 'refined_mistgear'                   
-        else :
-            pass    
-
-
-        if arg_equipment_dict.get("upgradeInfo"):
-            self.upgrade_info = arg_equipment_dict.get("upgradeInfo").get('itemName') # 융합장비
-        
-        # 105제 성장 장비 정보
-        if arg_equipment_dict.get("customOption"):
-            self.grow_info.get_grow_info_data(arg_equipment_dict.get('customOption'))
-        elif arg_equipment_dict.get("fixedOption"):
-            self.grow_info.get_grow_info_data(arg_equipment_dict.get("fixedOption"))
-        else :
-            pass
+        
+        for sub_attribute in BaseEquipment.sub_attribute_list:
+            if sub_attribute == 'enchant':
+                setattr(self, sub_attribute, explain_enchant(arg_equipment_dict.get('enchant')))
+                pass
+            else:    
+                setattr(self, sub_attribute, arg_equipment_dict.get(BASE_EQUIPMENT_NAME[sub_attribute]))
+
+class Equipment(BaseEquipment):
+    """
+    Equipments를 위해 사용되는 Class
+    """
+    sub_attribute_list = EQUIPMENT_NAME.keys()
+    def __init__(self):
+        super().__init__()
+        print(Equipment.sub_attribute_list)
+        for sub_attribute in Equipment.sub_attribute_list:
+            if sub_attribute == 'grow_info':
+                setattr(self, sub_attribute, GrowInfo())
+            else:
+                setattr(self, sub_attribute, None)
+
+    # @classmethod
+    # def set_sub_attributes(cls, new_attribute_list : list[str]):
+    #     cls.sub_attribute_list = new_attribute_list
+
+    def get_equipment_data(self, arg_equipment_dict):
+        super().get_equipment_data(arg_equipment_dict)
+        
+        for sub_attribute in Equipment.sub_attribute_list:
+            if sub_attribute == 'upgrade_info':
+                setattr(self, sub_attribute, arg_equipment_dict.get("upgradeInfo", dict()).get('itemName'))
+            elif sub_attribute == 'mist_gear':
+                if arg_equipment_dict.get('mistGear'):
+                    setattr(self, sub_attribute, 'mist_gear')    
+                elif arg_equipment_dict.get('pureMistGear'):
+                    setattr(self, sub_attribute, 'pure_mist_gear')
+                elif arg_equipment_dict.get('refinedMistGear'):
+                    setattr(self, sub_attribute, 'refined_mistgear')
+                else :
+                    pass                
+            elif sub_attribute == 'grow_info':
+                if arg_equipment_dict.get("customOption"):
+                    getattr(self, sub_attribute).get_grow_info_data(arg_equipment_dict.get('customOption'))
+                elif arg_equipment_dict.get("fixedOption"):
+                    getattr(self, sub_attribute).get_grow_info_data(arg_equipment_dict.get("fixedOption"))
+                else :
+                    pass
+            else:
+                pass    
+    # def __init__(self):
+    #     self.item_name = None
+    #     self.item_available_level = None
+    #     self.item_rarity = None
+    #     self.reinforce = None
+    #     self.item_grade_name = None
+    #     self.enchant = None
+    #     self.amplification_name = None
+    #     self.refine = None
+    #     self.upgrade_info = None
+    #     self.mist_gear = None
+    #     self.grow_info = GrowInfo()
+    
+    # def get_equipment_data(self, arg_equipment_dict : dict):
+    #     self.item_name = arg_equipment_dict.get('itemName') # 이름
+    #     self.item_available_level = arg_equipment_dict.get('itemAvailableLevel') # 레벨 제한
+    #     self.item_rarity = arg_equipment_dict.get('itemRarity') # 레어도
+    #     self.reinforce = arg_equipment_dict.get('reinforce') # 강화수치             
+    #     self.amplification_name = arg_equipment_dict.get('amplificationName') # 차원의 기운 여부 ex 차원의 힘, 차원의 지능, None
+    #     self.refine = arg_equipment_dict.get('refine') # 제련   
+    #     self.item_grade_name = arg_equipment_dict.get('itemGradeName') # 등급(최상~최하)
+    #     self.enchant = explain_enchant(arg_equipment_dict.get('enchant')) # 마법부여
+
+    #     # 미스트 기어 정보
+    #     if arg_equipment_dict.get('mistGear'):
+    #         self.mist_gear = 'mist_gear'
+    #     elif arg_equipment_dict.get('pureMistGear'):
+    #         self.mist_gear = 'pure_mist_gear'   
+    #     elif arg_equipment_dict.get('refinedMistGear'):
+    #         self.mist_gear = 'refined_mistgear'                   
+    #     else :
+    #         pass    
+
+
+    #     if arg_equipment_dict.get("upgradeInfo"):
+    #         self.upgrade_info = arg_equipment_dict.get("upgradeInfo").get('itemName') # 융합장비
+        
+    #     # 105제 성장 장비 정보
+    #     if arg_equipment_dict.get("customOption"):
+    #         self.grow_info.get_grow_info_data(arg_equipment_dict.get('customOption'))
+    #     elif arg_equipment_dict.get("fixedOption"):
+    #         self.grow_info.get_grow_info_data(arg_equipment_dict.get("fixedOption"))
+    #     else :
+    #         pass
 
 class BakalInfo():
     """
     Equipments를 위해 사용되는 Class
     """
 
     def __init__(self):
@@ -336,116 +417,190 @@
         self.option_3 = None
 
     def get_bakal_info_data(self, arg_bakal_info_dict):
         if arg_bakal_info_dict.get('options'):
             for i, option in enumerate(arg_bakal_info_dict.get('options')):
                 setattr(self, f'option_{i+1}',option.get('explain'))                
 
-class Weapon(Equipment):
+class Asrahan_Info():
     """
     Equipments를 위해 사용되는 Class
     """
+    def __init__(self):
+        self.memory_cluster = None
+        self.memory_destination = None
 
+    def get_asrahan_info_data(self, arg_asrahan_info_dict):
+        for asrahan_info in arg_asrahan_info_dict.get('options'):
+            if asrahan_info.get('name') == '기억의 종착지':
+                self.memory_destination = asrahan_info.get('step')     
+            else:
+                self.memory_cluster = asrahan_info.get('step')     
+
+class Weapon(Equipment):
+    """
+    Equipments를 위해 사용되는 Class
+    """
+    sub_attribute_list = WEAPON_NAME.keys()
     def __init__(self):
         super().__init__()
-        self.bakal_info = BakalInfo()
+        for sub_attribute in Weapon.sub_attribute_list:
+            if sub_attribute == 'bakal_info':
+                self.bakal_info = BakalInfo()
+            elif sub_attribute == 'asrahan_info':
+                self.asrahan_info = Asrahan_Info()
+            else:
+                pass    
 
     def get_equipment_data(self, arg_equipment_dict):
         super().get_equipment_data(arg_equipment_dict)
-        self.bakal_info.get_bakal_info_data(arg_equipment_dict.get("bakalInfo", dict())) # 바칼 무기 융합
-
+        for sub_attribute in Weapon.sub_attribute_list:
+            if sub_attribute == 'bakal_info':
+                self.bakal_info.get_bakal_info_data(arg_equipment_dict.get("bakalInfo", dict())) # 바칼 무기 융합
+            elif sub_attribute == 'asrahan_info':
+                self.asrahan_info.get_asrahan_info_data(arg_equipment_dict.get("asrahanOption", dict()))
+            else:
+                pass    
 
 class Equipments(PyNeople):
     """
     Neople Open API 06. 캐릭터 '장착 장비' 조회
     """    
-
+    sub_attribute_list = EQUIPMENT_LIST
     def __init__(self, arg_api_key : str):
         super().__init__(arg_api_key)
-
+    
+    @classmethod
+    def set_sub_attributes(cls, new_attribute_list : list[str]):
+        cls.sub_attribute_list = new_attribute_list
+    
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 장비 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """        
         self._server_id = arg_server_id
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment?apikey={self._api_key}'
         return get_request(url)
-
+    
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
         """
         # 하위 속성 생성
-        for equipment in EQUIPMENT_LIST:
+        
+        for equipment in Equipments.sub_attribute_list:
             if equipment == 'weapon':
                 setattr(self, equipment, Weapon())
+            elif equipment == 'title':
+                setattr(self, equipment, BaseEquipment())
+            elif equipment == 'set_item_info':
+                setattr(self, equipment, None)
             else:
                 setattr(self, equipment, Equipment())
                 
         # 장착 장비 정보 할당        
         for equipment in arg_data.get('equipment', list()):
-            getattr(self, equipment['slotId'].lower()).get_equipment_data(equipment)
+            if equipment['slotId'].lower() in Equipments.sub_attribute_list:
+                getattr(self, equipment['slotId'].lower()).get_equipment_data(equipment)
             # setattr(self, equipment['slotId'].lower(), equipment_data)
-        
-        # 세트 아이템 정보 할당
-        if arg_data.get('setItemInfo'):
-            set_item_info_list = []
-            for set_item_info in arg_data.get('setItemInfo'):
-                set_item_name_list = set_item_info.get('setItemName').split()
-                set_item_name_list.insert(-1, f"{set_item_info.get('activeSetNo')}")
-                set_item_info_list.append(" ".join(set_item_name_list))
-            setattr(self, 'set_item_info', ", ".join(set_item_info_list))
-        else:
-            setattr(self, 'set_item_info', None)
-
+            elif equipment == "set_item_info":
+                # 세트 아이템 정보 할당
+                if arg_data.get('setItemInfo'):
+                    set_item_info_list = []
+                    for set_item_info in arg_data.get('setItemInfo'):
+                        set_item_name_list = set_item_info.get('setItemName').split()
+                        set_item_name_list.insert(-1, f"{set_item_info.get('activeSetNo')}")
+                        set_item_info_list.append(" ".join(set_item_name_list))
+                    setattr(self, 'set_item_info', ", ".join(set_item_info_list))
+                else:
+                    pass
+            else:
+                pass        
 
 class Avatar():
     """
     Avatars를 위해 사용되는 Class
     """
-
+    sub_attribute_list = AVATAR_NAME.keys()
+    
     def __init__(self):
-        self.item_name = None       # 아바타 이름
-        self.item_rarity = None     # 아바타 레어도
-        self.option_ability = None  # 아바타 옵션
-        self.emblem_1 = None        # 엠블렘1 옵션
-        self.emblem_2 = None        # 엠블렘2 옵션
-        
+        for sub_attribute in Avatar.sub_attribute_list:
+            if sub_attribute == "emblem":
+                for i in range(1,3):
+                    setattr(self, f"{sub_attribute}_{i}", None)
+            else:
+                setattr(self, sub_attribute, None)
+
+        # self.item_name = None       # 아바타 이름
+        # self.item_rarity = None     # 아바타 레어도
+        # self.option_ability = None  # 아바타 옵션
+        # self.emblem_1 = None        # 엠블렘1 옵션
+        # self.emblem_2 = None        # 엠블렘2 옵션
+    @classmethod
+    def set_sub_attributes(cls, new_attribute_list : list[str]):
+        cls.sub_attribute_list = new_attribute_list
+
     def get_avatar_data(self, arg_avatar_dict):
-        self.item_name = arg_avatar_dict.get("itemName")
-        self.item_rarity = arg_avatar_dict.get("itemRarity")
-        self.option_ability = arg_avatar_dict.get("optionAbility")
-        for i, emblem in enumerate(arg_avatar_dict.get('emblems', dict())):
-            setattr(self, f'emblem_{i+1}', emblem.get('itemName'))
+        for sub_attribute in Avatar.sub_attribute_list:
+            if sub_attribute == 'emblem':
+                for emblem in arg_avatar_dict.get('emblems', dict()):
+                    setattr(self, f"emblem_{emblem.get('slotId')}", emblem.get('itemName'))
+            else:    
+                setattr(self, sub_attribute, arg_avatar_dict.get(AVATAR_NAME[sub_attribute]))
+        # self.item_name = arg_avatar_dict.get("itemName")
+        # self.item_rarity = arg_avatar_dict.get("itemRarity")
+        # self.option_ability = arg_avatar_dict.get("optionAbility")
+
+
 
 class PlatinumAvatar(Avatar):
     """
     Avatars를 위해 사용되는 Class
     """   
-
+    sub_attribute_list = PLATINUM_AVATAR_NAME
     def __init__(self):
-        super().__init__()
-        self.emblem_3 = None # 플래티넘 엠블렘 옵션
+        for sub_attribute in PlatinumAvatar.sub_attribute_list:
+            if sub_attribute == "emblem":
+                for i in range(1,3):
+                    setattr(self, f"{sub_attribute}_{i}", None)
+            elif sub_attribute == "platinum_emblem":
+                setattr(self, sub_attribute, None)    
+            else:
+                setattr(self, sub_attribute, None)
 
     def get_avatar_data(self, arg_avatar_dict):
-        super().get_avatar_data(arg_avatar_dict)
+        for sub_attribute in Avatar.sub_attribute_list:
+            if sub_attribute == 'emblem':
+                for emblem in arg_avatar_dict.get(PLATINUM_AVATAR_NAME[sub_attribute], dict()):
+                    if emblem.get('slotColor') != '플래티넘':
+                        setattr(self, f"{sub_attribute}_{emblem.get('slotId')}", emblem.get('itemName'))
+            elif sub_attribute == "platinum_emblem":
+                for emblem in arg_avatar_dict.get(PLATINUM_AVATAR_NAME[sub_attribute], dict()):
+                    if emblem.get('slotColor') == '플래티넘':
+                        setattr(self, sub_attribute, emblem.get('itemName'))
+            else:    
+                setattr(self, sub_attribute, arg_avatar_dict.get(AVATAR_NAME[sub_attribute]))
 
 class Avatars(PyNeople):
     """
     Neople Open API 07. 캐릭터 '장착 아바타' 조회
     """       
-
+    sub_attribute_list = AVATAR_LIST
     def __init__(self, arg_api_key: str):
         super().__init__(arg_api_key)
+    
+    @classmethod
+    def set_sub_attributes(cls, new_attribute_list : list[str]):
+        cls.sub_attribute_list = new_attribute_list
 
     def get_data(self, arg_server_id: str, arg_character_id : str):    
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 아바타 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
@@ -458,23 +613,24 @@
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
         """        
         # 하위 속성 생성
-        for avatar in AVATAR_LIST:
-            if avatar in PlatinumAvatar:
+        for avatar in Avatars.sub_attribute_list:
+            if avatar in PLATINUM_AVATAR_LIST:
                 setattr(self, avatar, PlatinumAvatar())    
             else:
                 setattr(self, avatar, Avatar())
         
         # 하위 속성에 데이터 할당
         for avatar in arg_data.get('avatar', list()):
-            getattr(self, f'{avatar["slotId"].lower()}').get_avatar_data(avatar)
+            if f'{avatar["slotId"].lower()}' in Avatars.sub_attribute_list:
+                getattr(self, f'{avatar["slotId"].lower()}').get_avatar_data(avatar)
 
 
 class Creature(PyNeople):
     """
     Neople Open API 08. 캐릭터 '장착 크리쳐' 조회
     """
     
@@ -796,9 +952,8 @@
                 arg_is_all_job_grow(bool) : jobGrowId 입력 시 연계되는 전체 전직 포함 조회 ex) 검성 -> 웨펀마스터, 검성, 검신, 眞웨펀마스터
                 arg_is_buff(bool) : 버퍼만 조회(true), 딜러만 조회(false), 전체 조회(미 입력)	
                 arg_server_id(str) : 서버 아이디
                 arg_limit(int) : 반환 Row 수
         """
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters-fame?minFame={arg_min_fame}&maxFame={arg_max_fame}&jobId={arg_job_id}&jobGrowId={arg_job_grow_id}&isAllJobGrow={arg_is_all_job_grow}&isBuff={arg_is_buff}&limit={arg_limit}&apikey={self._api_key}"
         return get_request(url)
-
```

### Comparing `pyneople-0.2.7/src/pyneople/database_connecter.py` & `pyneople-0.2.8/src/pyneople/database_connecter.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.7/src/pyneople/functions.py` & `pyneople-0.2.8/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.7/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.2.8/src/pyneople.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.7
+Version: 0.2.8
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

