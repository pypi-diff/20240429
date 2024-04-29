# Comparing `tmp/simplebox-0.0.1a202-py3-none-any.whl.zip` & `tmp/simplebox-0.0.1a203-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 460219 bytes, number of entries: 158
--rw-rw-rw-  2.0 fat     5191 b- defN 24-Apr-28 17:17 simplebox/__init__.py
+Zip file size: 460449 bytes, number of entries: 158
+-rw-rw-rw-  2.0 fat     5191 b- defN 24-Apr-28 17:35 simplebox/__init__.py
 -rw-rw-rw-  2.0 fat     2090 b- defN 24-Apr-07 16:46 simplebox/backend.py
 -rw-rw-rw-  2.0 fat    17626 b- defN 24-Apr-07 16:46 simplebox/character.py
 -rw-rw-rw-  2.0 fat     4829 b- defN 24-Apr-14 15:04 simplebox/classes.py
 -rw-rw-rw-  2.0 fat    16962 b- defN 24-Apr-20 14:21 simplebox/cmd.py
 -rw-rw-rw-  2.0 fat     5481 b- defN 23-Nov-14 15:01 simplebox/converter.py
 -rw-rw-rw-  2.0 fat     1638 b- defN 24-Apr-07 15:02 simplebox/enums.py
 -rw-rw-rw-  2.0 fat      306 b- defN 23-May-31 16:53 simplebox/generic.py
@@ -145,16 +145,16 @@
 -rw-rw-rw-  2.0 fat      783 b- defN 23-Mar-25 15:32 simplebox/scheduler/_cron/_fields.py
 -rw-rw-rw-  2.0 fat       47 b- defN 23-May-03 14:12 simplebox/utils/__init__.py
 -rw-rw-rw-  2.0 fat    16556 b- defN 24-Apr-18 15:30 simplebox/utils/computer.py
 -rw-rw-rw-  2.0 fat     2173 b- defN 24-Apr-07 15:48 simplebox/utils/enums.py
 -rw-rw-rw-  2.0 fat     2735 b- defN 24-Apr-27 14:18 simplebox/utils/locks.py
 -rw-rw-rw-  2.0 fat    14864 b- defN 24-Apr-28 15:25 simplebox/utils/objects.py
 -rw-rw-rw-  2.0 fat     3258 b- defN 24-Apr-14 14:42 simplebox/utils/optionals.py
--rw-rw-rw-  2.0 fat     3230 b- defN 24-Apr-28 17:10 simplebox/utils/reflect.py
+-rw-rw-rw-  2.0 fat     5653 b- defN 24-Apr-28 17:58 simplebox/utils/reflect.py
 -rw-rw-rw-  2.0 fat    19546 b- defN 24-Apr-07 15:48 simplebox/utils/strings.py
 -rw-rw-rw-  2.0 fat      247 b- defN 23-Feb-28 15:31 simplebox/valid/__init__.py
 -rw-rw-rw-  2.0 fat    16632 b- defN 24-Apr-15 17:12 simplebox/valid/_validator.py
--rw-rw-rw-  2.0 fat     1279 b- defN 24-Apr-28 17:17 simplebox-0.0.1a202.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 17:17 simplebox-0.0.1a202.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-28 17:17 simplebox-0.0.1a202.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    13755 b- defN 24-Apr-28 17:17 simplebox-0.0.1a202.dist-info/RECORD
-158 files, 1446627 bytes uncompressed, 438523 bytes compressed:  69.7%
+-rw-rw-rw-  2.0 fat     1279 b- defN 24-Apr-28 18:00 simplebox-0.0.1a203.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 18:00 simplebox-0.0.1a203.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-28 18:00 simplebox-0.0.1a203.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    13755 b- defN 24-Apr-28 18:00 simplebox-0.0.1a203.dist-info/RECORD
+158 files, 1449050 bytes uncompressed, 438753 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -456,20 +456,20 @@
 
 Filename: simplebox/valid/__init__.py
 Comment: 
 
 Filename: simplebox/valid/_validator.py
 Comment: 
 
-Filename: simplebox-0.0.1a202.dist-info/METADATA
+Filename: simplebox-0.0.1a203.dist-info/METADATA
 Comment: 
 
-Filename: simplebox-0.0.1a202.dist-info/WHEEL
+Filename: simplebox-0.0.1a203.dist-info/WHEEL
 Comment: 
 
-Filename: simplebox-0.0.1a202.dist-info/top_level.txt
+Filename: simplebox-0.0.1a203.dist-info/top_level.txt
 Comment: 
 
-Filename: simplebox-0.0.1a202.dist-info/RECORD
+Filename: simplebox-0.0.1a203.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplebox/__init__.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
-__version__ = "0.0.1.alpha202"
+__version__ = "0.0.1.alpha203"
 
 banner = f"""
  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------. 
 | .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. |
 | |    _______   | || |     _____    | || | ____    ____ | || |   ______     | || |   _____      | || |  _________   | || |   ______     | || |     ____     | || |  ____  ____  | |
 | |   /  ___  |  | || |    |_   _|   | || ||_   \  /   _|| || |  |_   __ \   | || |  |_   _|     | || | |_   ___  |  | || |  |_   _ \    | || |   .'    `.   | || | |_  _||_  _| | |
 | |  |  (__ \_|  | || |      | |     | || |  |   \/   |  | || |    | |__) |  | || |    | |       | || |   | |_  \_|  | || |    | |_) |   | || |  /  .--.  \  | || |   \ \  / /   | |
```

## simplebox/utils/reflect.py

```diff
@@ -37,14 +37,42 @@
                         super_field = True
                         break
                 if not super_field:
                     attributes[k] = v
         return attributes
 
     @staticmethod
+    def get_genealogy_private_attribute(obj, name) -> dict[str, Any]:
+        """
+        Gets the properties of the parent class that have been overridden by obj,
+        containing only the private attributes.
+        """
+
+        def get_class_name(clz: type, clzs: dict[type, str]):
+            classes = [clz]
+            classes.extend(clz.__bases__)
+            for clz_ in classes:
+                temp = [clz_.__name__]
+                while True:
+                    if temp[0][0] == "_":
+                        temp[0] = temp[0][1:]
+                    else:
+                        break
+                clzs[clz_] = f"_{temp[0]}"
+
+        class_names = {}
+        get_class_name(obj.__class__, class_names)
+        attributes = {}
+        for k, v in obj.__dict__.items():
+            for obj_type, obj_prefix in class_names.items():
+                if k.endswith(name) and k.startswith(obj_prefix):
+                    attributes[obj_type] = v
+        return attributes
+
+    @staticmethod
     def get_attribute(obj, name: str) -> Optional[Any]:
         """
         get attribute by name
         """
         return ReflectUtils.get_attributes(obj).get(name, None)
 
     @staticmethod
@@ -92,7 +120,44 @@
 
     @staticmethod
     def get_method(obj, name) -> callable:
         """
         get method by name.
         """
         return ReflectUtils.get_methods(obj).get(name, None)
+
+    @staticmethod
+    def get_genealogy_private_method(obj, name) -> dict[str, callable]:
+        """
+        Gets a method whose parent class has been overridden by obj, containing only private methods.
+        """
+        if issubclass(type(obj), type):
+            obj_class = obj
+        else:
+            obj_class = obj.__class__
+
+        def get_class_name(clz: type, clzs: dict[type, str]):
+            classes = [clz]
+            classes.extend(clz.__bases__)
+            for clz_ in classes:
+                temp = [clz_.__name__]
+                while True:
+                    if temp[0][0] == "_":
+                        temp[0] = temp[0][1:]
+                    else:
+                        break
+                clzs[clz_] = f"_{temp[0]}"
+
+        class_names = {}
+        get_class_name(obj_class, class_names)
+
+        all_func_names = [i for i in dir(obj_class) if
+                          isfunction(getattr(obj_class, i)) or ismethod(getattr(obj_class, i))]
+        all_funcs = {}
+        for func in all_func_names:
+            if func.startswith("__") and func.endswith("__"):
+                continue
+            for obj_type, obj_prefix in class_names.items():
+                if func.endswith(name) and func.startswith(obj_prefix):
+                    all_funcs[obj_type] = getattr(obj, func, None)
+        return all_funcs
+
```

## Comparing `simplebox-0.0.1a202.dist-info/METADATA` & `simplebox-0.0.1a203.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplebox
-Version: 0.0.1a202
+Version: 0.0.1a203
 Summary: 简易工具箱。
 Author: fuck
 License: MIT Licence
 Keywords: pip,simplebox,backend,fast,fasttools,box,simple
 Platform: any
 Requires-Python: >=3.9
 Requires-Dist: psutil (==5.9.2)
```

## Comparing `simplebox-0.0.1a202.dist-info/RECORD` & `simplebox-0.0.1a203.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-simplebox/__init__.py,sha256=qUTuapyqk8pfIuui1WMsjR8M6kcRmq2uFIuNs75GAbQ,5191
+simplebox/__init__.py,sha256=VfggSJFgQd0adtJ4M-DqVeGJSq8yGzR8Y1S7FKYNdII,5191
 simplebox/backend.py,sha256=yR3gveO0iKcTKWKW5K57513u-s7O3oGes84Kp8HUZho,2090
 simplebox/character.py,sha256=NEbQqFmD3rpkl_E3MeES7rRfAmtc_DJHoKcF8GNK92g,17626
 simplebox/classes.py,sha256=vGD0PVglh-Nlz8I3PTqDmDquQf_Z2BNoXIvp9aRS140,4829
 simplebox/cmd.py,sha256=5SK-ne4vAyjNdEztS0TyMWUuQC6bBc4RCtnbdQBvVF4,16962
 simplebox/converter.py,sha256=DZ_sb-ZBIorTZAlpuNyGjxnlPAjtSp7yKMIDSiwws0g,5481
 simplebox/enums.py,sha256=KzziG7TboPMIENPrc4HrsUagSEMd4JfLFG6Bn2T0HAs,1638
 simplebox/generic.py,sha256=tBDzlqFHQ7I6bb8_iC9PEqyMaD0sxJee9a7zR3YwxRw,306
@@ -144,15 +144,15 @@
 simplebox/scheduler/_cron/_fields.py,sha256=iYBrX15zyYSSwmwDc1fSl0tAux_0OXPBGbzF0Io1eGQ,783
 simplebox/utils/__init__.py,sha256=CtZuEO8oVkrRxwm4_fsQYg0wdQ6o3znWt5v6hZ1BBgc,47
 simplebox/utils/computer.py,sha256=WYBYAbZ2ViWUMjNW8LtutFpKHfgpr-wg4kcim3DKWk4,16556
 simplebox/utils/enums.py,sha256=rwMAmDqUFy2iJey9v0aThBCAFcR-tKqVI9LELw4BKcw,2173
 simplebox/utils/locks.py,sha256=KP_utNUBYeWjJhsWzu1-rn5sG6jzi2cDrFXtSmgJCHE,2735
 simplebox/utils/objects.py,sha256=jaTS8DaHdrdspANFzol2ad6UKRQnFCPCvHHnSu5R2d4,14864
 simplebox/utils/optionals.py,sha256=XDlteLGkfbWHOgJPdGykE-a79Ae-P7Fbfsabmiwdjuw,3258
-simplebox/utils/reflect.py,sha256=My7m5kCd08gjFfg31Pg0l-l0XjNmt971lneX6Wg6J5U,3230
+simplebox/utils/reflect.py,sha256=ih_-fw49DzYSNyauvDbpEW5ixf5wi5UVhE6nlq_zfUk,5653
 simplebox/utils/strings.py,sha256=yvdvMVI-ULs-DIWElpmjdYHp9CPLbETc5M-16L9gflk,19546
 simplebox/valid/__init__.py,sha256=7deSv2vW7Wj-83Db3JbO0SZK9Pf-G9pDqbCAgkxr8PI,247
 simplebox/valid/_validator.py,sha256=xj3ju6Lpx73bF3NZR9eGHJl_pTk6kPMsFL4hrhbM2cw,16632
-simplebox-0.0.1a202.dist-info/METADATA,sha256=il34JgelsjZRQi5RbUGRBciRxGooavaC-pRPM6vXUdM,1279
-simplebox-0.0.1a202.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-simplebox-0.0.1a202.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
-simplebox-0.0.1a202.dist-info/RECORD,,
+simplebox-0.0.1a203.dist-info/METADATA,sha256=KhVANXHB56uYCfUk7IwKPejT32U2T_QRQY1yabOCSv4,1279
+simplebox-0.0.1a203.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+simplebox-0.0.1a203.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
+simplebox-0.0.1a203.dist-info/RECORD,,
```

