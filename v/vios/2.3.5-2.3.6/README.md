# Comparing `tmp/vios-2.3.5-py3-none-any.whl.zip` & `tmp/vios-2.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 45407 bytes, number of entries: 24
+Zip file size: 45409 bytes, number of entries: 24
 -rw-rw-rw-  2.0 fat    18569 b- defN 24-Apr-25 14:44 quark/proxy.py
--rw-rw-rw-  2.0 fat    18867 b- defN 24-Apr-28 13:53 quark/app/__init__.py
+-rw-rw-rw-  2.0 fat    18867 b- defN 24-Apr-29 13:27 quark/app/__init__.py
 -rw-rw-rw-  2.0 fat     2575 b- defN 24-Mar-19 11:19 quark/app/_data.py
--rw-rw-rw-  2.0 fat    10205 b- defN 24-Mar-19 11:19 quark/app/demo.py
--rw-rw-rw-  2.0 fat     8790 b- defN 24-Apr-28 13:40 quark/app/task.py
+-rw-rw-rw-  2.0 fat    10205 b- defN 24-Mar-19 11:19 quark/app/_demo.py
+-rw-rw-rw-  2.0 fat     8790 b- defN 24-Apr-28 13:40 quark/app/_task.py
 -rw-rw-rw-  2.0 fat     5876 b- defN 24-Mar-19 11:19 quark/app/uapi.py
 -rw-rw-rw-  2.0 fat     7914 b- defN 24-Mar-19 11:19 quark/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat      386 b- defN 24-Mar-19 11:19 quark/driver/__init__.py
 -rw-rw-rw-  2.0 fat      217 b- defN 24-Mar-19 11:19 quark/driver/common/__init__.py
 -rw-rw-rw-  2.0 fat     4478 b- defN 24-Mar-19 11:19 quark/driver/common/basedriver.py
 -rw-rw-rw-  2.0 fat     4663 b- defN 24-Mar-19 11:19 quark/driver/common/quantity.py
 -rw-rw-rw-  2.0 fat     5432 b- defN 24-Mar-19 11:19 quark/driver/common/visadriver.py
 -rw-rw-rw-  2.0 fat     1188 b- defN 24-Mar-19 11:19 quark/envelope/__init__.py
 -rw-rw-rw-  2.0 fat    15111 b- defN 24-Mar-19 11:19 quark/envelope/assembler.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 24-Mar-19 11:19 quark/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1106 b- defN 24-Mar-19 11:19 quark/envelope/device.py
 -rw-rw-rw-  2.0 fat     3733 b- defN 24-Apr-25 14:44 quark/envelope/processor.py
 -rw-rw-rw-  2.0 fat     4320 b- defN 24-Apr-25 14:44 quark/envelope/router.py
 -rw-rw-rw-  2.0 fat     2841 b- defN 24-Mar-21 12:16 quark/envelope/systemq.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-28 14:00 vios-2.3.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1211 b- defN 24-Apr-28 14:00 vios-2.3.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 14:00 vios-2.3.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-28 14:00 vios-2.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1921 b- defN 24-Apr-28 14:00 vios-2.3.5.dist-info/RECORD
-24 files, 124908 bytes uncompressed, 42341 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-29 13:34 vios-2.3.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1211 b- defN 24-Apr-29 13:34 vios-2.3.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 13:34 vios-2.3.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-29 13:34 vios-2.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1923 b- defN 24-Apr-29 13:34 vios-2.3.6.dist-info/RECORD
+24 files, 124910 bytes uncompressed, 42339 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -3,18 +3,18 @@
 
 Filename: quark/app/__init__.py
 Comment: 
 
 Filename: quark/app/_data.py
 Comment: 
 
-Filename: quark/app/demo.py
+Filename: quark/app/_demo.py
 Comment: 
 
-Filename: quark/app/task.py
+Filename: quark/app/_task.py
 Comment: 
 
 Filename: quark/app/uapi.py
 Comment: 
 
 Filename: quark/driver/VirtualDevice.py
 Comment: 
@@ -51,23 +51,23 @@
 
 Filename: quark/envelope/router.py
 Comment: 
 
 Filename: quark/envelope/systemq.py
 Comment: 
 
-Filename: vios-2.3.5.dist-info/LICENSE
+Filename: vios-2.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: vios-2.3.5.dist-info/METADATA
+Filename: vios-2.3.6.dist-info/METADATA
 Comment: 
 
-Filename: vios-2.3.5.dist-info/WHEEL
+Filename: vios-2.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: vios-2.3.5.dist-info/top_level.txt
+Filename: vios-2.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-2.3.5.dist-info/RECORD
+Filename: vios-2.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `quark/app/demo.py` & `quark/app/_demo.py`

 * *Files identical despite different names*

## Comparing `quark/app/task.py` & `quark/app/_task.py`

 * *Files identical despite different names*

## Comparing `vios-2.3.5.dist-info/LICENSE` & `vios-2.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-2.3.5.dist-info/METADATA` & `vios-2.3.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 2.3.5
+Version: 2.3.6
 Summary: runtime requirements for systemq
 Author-email: YL Feng <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-2.3.5.dist-info/RECORD` & `vios-2.3.6.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 quark/proxy.py,sha256=4rpjQK0m_5OU1DAF4x4-jjjewDa9HxnKLWKHxyi4COo,18569
 quark/app/__init__.py,sha256=QwShGh3X6VQ1k8ltdDSP9l_xQLeXemXkpPeuutwhnWg,18867
 quark/app/_data.py,sha256=EGGTD2FrZ8vlbMh4jlmWhYk4fEG3FolGoWaQ26qxoss,2575
-quark/app/demo.py,sha256=eod5vSXKB0XI-Rr8UVKkNc9tOUfWCjI109Imd8bKmuo,10205
-quark/app/task.py,sha256=OT3e7QWgyeP1aw5L4DlS8-2RvCyOmJKN3YNzaR_Tdj0,8790
+quark/app/_demo.py,sha256=eod5vSXKB0XI-Rr8UVKkNc9tOUfWCjI109Imd8bKmuo,10205
+quark/app/_task.py,sha256=OT3e7QWgyeP1aw5L4DlS8-2RvCyOmJKN3YNzaR_Tdj0,8790
 quark/app/uapi.py,sha256=itjEa89SUXozZqBGLH-3o4mKtRssNQODDj60knC-cGE,5876
 quark/driver/VirtualDevice.py,sha256=Cswl_ykFhIsocGV6Okh_YS1b48FeLm2fh1ruXqmNoyw,7914
 quark/driver/__init__.py,sha256=p1pVx1xTulBT8-qdp_zJ859tdIsA92XdvwrkqcVHL4s,386
 quark/driver/common/__init__.py,sha256=eSw0oQ4qSq6QMOlqmk01wys4EbWT9h1g-ITdrmtaiwI,217
 quark/driver/common/basedriver.py,sha256=h8YabyzreB4_vjLzbkieXrMrdWBYF5Lh3SYBgyE6IDs,4478
 quark/driver/common/quantity.py,sha256=fV9DMmjys44efe7TTvzXmFdozqGdS2QUm23wtfLxeBE,4663
 quark/driver/common/visadriver.py,sha256=LRyYDBF0u9EYf6p47LeGGKhx9pHiq4pux_pzDakaICY,5432
 quark/envelope/__init__.py,sha256=5_cs0tZ7mV4GjOsY2isx8sUQu4u6Y3WN-9DUGG27SQM,1188
 quark/envelope/assembler.py,sha256=ENwX7FutJvpg6_Wcm42_Zx-ddq40JozuYqHPwJp09ZA,15111
 quark/envelope/calculator.py,sha256=0rZAA46sWh_X8wOBmpBvmljqCV53ID4VHPX1cE_abEc,4322
 quark/envelope/device.py,sha256=5E3oWZ84IYnQdzlmzltgPyayYz_au7p7UIbFVpJUa0Q,1106
 quark/envelope/processor.py,sha256=QTBsW0mUwg1xCZ6k3oEBzGc13DDP60dT-QP61tjwe2s,3733
 quark/envelope/router.py,sha256=XtTaZWRXQtqBpAkHCnEj99xmTuctNUFCrbXpoz49unY,4320
 quark/envelope/systemq.py,sha256=QAaHLv68C9UjMp9qHt9t-HJkOTpCkbHZTlNVOsAzIBc,2841
-vios-2.3.5.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
-vios-2.3.5.dist-info/METADATA,sha256=UDdJtk94ZkFGq7KXwkjAcO2JjikDoHzD0Zqw5EXYo5M,1211
-vios-2.3.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-vios-2.3.5.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
-vios-2.3.5.dist-info/RECORD,,
+vios-2.3.6.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
+vios-2.3.6.dist-info/METADATA,sha256=p3mYUQgTvso8FAxvsgjkVU2NV3a76EMwgjCSK7VM5-Y,1211
+vios-2.3.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+vios-2.3.6.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
+vios-2.3.6.dist-info/RECORD,,
```

