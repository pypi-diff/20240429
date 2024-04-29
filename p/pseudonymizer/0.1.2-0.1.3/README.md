# Comparing `tmp/pseudonymizer-0.1.2-py3-none-any.whl.zip` & `tmp/pseudonymizer-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 76287 bytes, number of entries: 51
+Zip file size: 76285 bytes, number of entries: 51
 -rw-r--r--  2.0 unx        1 b- defN 24-Jan-14 10:42 pseudonymizer/__init__.py
 -rw-r--r--  2.0 unx     3616 b- defN 24-Apr-21 07:22 pseudonymizer/anonymizationSecurityMeasure.py
 -rw-r--r--  2.0 unx     5589 b- defN 24-Apr-21 11:47 pseudonymizer/createMappingTable.py
 -rw-r--r--  2.0 unx     6332 b- defN 24-Apr-21 11:34 pseudonymizer/extractJoinDatafromDB.py
 -rw-r--r--  2.0 unx     5131 b- defN 24-Apr-21 11:52 pseudonymizer/joinTargetTables.py
 -rw-r--r--  2.0 unx     9509 b- defN 24-Apr-21 12:11 pseudonymizer/privacyPreservingModels.py
 -rw-r--r--  2.0 unx     5267 b- defN 24-Apr-21 13:36 pseudonymizer/pseudonym.py
@@ -42,12 +42,12 @@
 -rw-r--r--  2.0 unx      612 b- defN 24-Apr-13 04:53 pseudonymizer/pseudonymizers/nameMasking.py
 -rw-r--r--  2.0 unx     5485 b- defN 24-Apr-21 13:14 pseudonymizer/pseudonymizers/numcategorization.py
 -rw-r--r--  2.0 unx     1627 b- defN 24-Apr-18 11:00 pseudonymizer/pseudonymizers/phoneNumMasking.py
 -rw-r--r--  2.0 unx     1707 b- defN 24-Apr-21 13:38 pseudonymizer/pseudonymizers/randomRoundingPseudonymizer.py
 -rw-r--r--  2.0 unx     1058 b- defN 24-Apr-21 13:49 pseudonymizer/pseudonymizers/residentNumMasking.py
 -rw-r--r--  2.0 unx     5739 b- defN 24-Apr-21 13:35 pseudonymizer/pseudonymizers/topandBottomCoding.py
 -rw-r--r--  2.0 unx        1 b- defN 24-Jan-14 10:42 tests/__init__.py
--rw-r--r--  2.0 unx    57762 b- defN 24-Apr-29 13:19 pseudonymizer-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 13:19 pseudonymizer-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-Apr-29 13:19 pseudonymizer-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5207 b- defN 24-Apr-29 13:19 pseudonymizer-0.1.2.dist-info/RECORD
-51 files, 203385 bytes uncompressed, 67621 bytes compressed:  66.8%
+-rw-r--r--  2.0 unx    57763 b- defN 24-Apr-29 13:39 pseudonymizer-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 13:39 pseudonymizer-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-29 13:39 pseudonymizer-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5207 b- defN 24-Apr-29 13:39 pseudonymizer-0.1.3.dist-info/RECORD
+51 files, 203386 bytes uncompressed, 67619 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -135,20 +135,20 @@
 
 Filename: pseudonymizer/pseudonymizers/topandBottomCoding.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: pseudonymizer-0.1.2.dist-info/METADATA
+Filename: pseudonymizer-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pseudonymizer-0.1.2.dist-info/WHEEL
+Filename: pseudonymizer-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pseudonymizer-0.1.2.dist-info/top_level.txt
+Filename: pseudonymizer-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pseudonymizer-0.1.2.dist-info/RECORD
+Filename: pseudonymizer-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pseudonymizer-0.1.2.dist-info/METADATA` & `pseudonymizer-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pseudonymizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: pseudonymizer-to-protect-private-personal-data
 Home-page: https://github.com/ksydata/pseudonymizer
 Author: ksydata
 Author-email: ksydata01@gmail.com
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas (==1.4.4)
 Requires-Dist: PyMySQL (==1.1.0)
 Requires-Dist: numpy (==1.22.3)
-Requires-Dist: scipy (==1.9.1)
+Requires-Dist: scipy (==1.10.0)
 Requires-Dist: matplotlib (==3.5.2)
 Requires-Dist: seaborn (==0.11.2)
 Requires-Dist: setuptools (==63.4.1)
 Requires-Dist: prettytable (==3.9.0)
 
 # 가명처리∙결합 오픈소스 라이브러리 프로젝트
```

## Comparing `pseudonymizer-0.1.2.dist-info/RECORD` & `pseudonymizer-0.1.3.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -41,11 +41,11 @@
 pseudonymizer/pseudonymizers/nameMasking.py,sha256=L1qQkEzkCC6SsNmaXrV9yrxa_7So71-8_XexprgpToU,612
 pseudonymizer/pseudonymizers/numcategorization.py,sha256=TFCeOmowWxnKly_rqufF7ZRNS6X480TMR8sJ2xufuBI,5485
 pseudonymizer/pseudonymizers/phoneNumMasking.py,sha256=zV9QLprrYsXI1UmFLrGVZAlMr8Rn1zd9Wt-17EPzZTQ,1627
 pseudonymizer/pseudonymizers/randomRoundingPseudonymizer.py,sha256=HaTDeCTfU0pkWN31z9JlcmJoQ_INtUk1fpDzJpOoIOA,1707
 pseudonymizer/pseudonymizers/residentNumMasking.py,sha256=2SAsjEAJf-ikhSSy7LxLFe1f8_J9Uxj4bEuUIDUOOEk,1058
 pseudonymizer/pseudonymizers/topandBottomCoding.py,sha256=FoiC0oWSy4zxIFYc5hvOTuoYjWv3m6I0M5fWxk6fnJs,5739
 tests/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pseudonymizer-0.1.2.dist-info/METADATA,sha256=DbNMFBJw4c1tLL6SKSJOfQIrS7okbgLZEZUy0DqSsxo,57762
-pseudonymizer-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pseudonymizer-0.1.2.dist-info/top_level.txt,sha256=CTpFPZ-varEcVizfZO3Y3rH1wKmbj5LwTov_xQ4d_IA,20
-pseudonymizer-0.1.2.dist-info/RECORD,,
+pseudonymizer-0.1.3.dist-info/METADATA,sha256=H25a2IruLeltN-huSxhqC1CD2eo9w7X61l-Z3roZUSc,57763
+pseudonymizer-0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pseudonymizer-0.1.3.dist-info/top_level.txt,sha256=CTpFPZ-varEcVizfZO3Y3rH1wKmbj5LwTov_xQ4d_IA,20
+pseudonymizer-0.1.3.dist-info/RECORD,,
```

