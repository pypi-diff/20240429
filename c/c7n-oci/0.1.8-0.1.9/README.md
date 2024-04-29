# Comparing `tmp/c7n_oci-0.1.8-py3-none-any.whl.zip` & `tmp/c7n_oci-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 26736 bytes, number of entries: 21
+Zip file size: 26758 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      189 b- defN 80-Jan-01 00:00 c7n_oci/actions/__init__.py
 -rw-r--r--  2.0 unx     6381 b- defN 80-Jan-01 00:00 c7n_oci/actions/base.py
 -rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 c7n_oci/constants.py
 -rw-r--r--  2.0 unx      482 b- defN 80-Jan-01 00:00 c7n_oci/entry.py
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 c7n_oci/filters/__init__.py
 -rw-r--r--  2.0 unx     5282 b- defN 80-Jan-01 00:00 c7n_oci/log.py
 -rw-r--r--  2.0 unx     3372 b- defN 80-Jan-01 00:00 c7n_oci/output.py
@@ -13,11 +13,11 @@
 -rw-r--r--  2.0 unx     4642 b- defN 80-Jan-01 00:00 c7n_oci/resources/dns.py
 -rw-r--r--  2.0 unx    33036 b- defN 80-Jan-01 00:00 c7n_oci/resources/identity.py
 -rw-r--r--  2.0 unx     6441 b- defN 80-Jan-01 00:00 c7n_oci/resources/object_storage.py
 -rw-r--r--  2.0 unx      626 b- defN 80-Jan-01 00:00 c7n_oci/resources/resource_map.py
 -rw-r--r--  2.0 unx    12225 b- defN 80-Jan-01 00:00 c7n_oci/resources/virtual_network.py
 -rw-r--r--  2.0 unx     3084 b- defN 80-Jan-01 00:00 c7n_oci/session.py
 -rw-r--r--  2.0 unx      732 b- defN 80-Jan-01 00:00 c7n_oci/utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_oci-0.1.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4252 b- defN 16-Jan-01 00:00 c7n_oci-0.1.8.dist-info/METADATA
-?rw-------  2.0 unx     1653 b- defN 24-Jan-18 18:09 c7n_oci-0.1.8.dist-info/RECORD
-21 files, 107626 bytes uncompressed, 24082 bytes compressed:  77.6%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_oci-0.1.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4340 b- defN 16-Jan-01 00:00 c7n_oci-0.1.9.dist-info/METADATA
+?rw-------  2.0 unx     1653 b- defN 24-Mar-05 16:51 c7n_oci-0.1.9.dist-info/RECORD
+21 files, 107714 bytes uncompressed, 24104 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -48,17 +48,17 @@
 
 Filename: c7n_oci/session.py
 Comment: 
 
 Filename: c7n_oci/utils.py
 Comment: 
 
-Filename: c7n_oci-0.1.8.dist-info/WHEEL
+Filename: c7n_oci-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_oci-0.1.8.dist-info/METADATA
+Filename: c7n_oci-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_oci-0.1.8.dist-info/RECORD
+Filename: c7n_oci-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c7n_oci-0.1.8.dist-info/METADATA` & `c7n_oci-0.1.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: c7n-oci
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cloud Custodian - OCI Support
 Home-page: https://cloudcustodian.io
 License: Apache-2.0
 Author: Cloud Custodian Project
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: oci (==2.119.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: certifi (==2023.11.17) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: oci (==2.124.0) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: certifi (==2024.2.2) ; python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: circuitbreaker (==1.4.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: cryptography (==41.0.7) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: pyopenssl (==23.3.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: python-dateutil (==2.8.2) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: pytz (==2023.3.post1) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: cffi (==1.16.0) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: cryptography (==42.0.5) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: pyopenssl (==24.0.0) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: python-dateutil (==2.9.0.post0) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: pytz (==2024.1) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: cffi (==1.16.0) ; python_version >= "3.8" and python_version < "4.0" and platform_python_implementation != "PyPy"
 Requires-Dist: six (==1.16.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: pycparser (==2.21) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: pycparser (==2.21) ; python_version >= "3.8" and python_version < "4.0" and platform_python_implementation != "PyPy"
 Project-URL: Documentation, https://cloudcustodian.io/docs/
 Project-URL: Repository, https://github.com/cloud-custodian/cloud-custodian
 Description-Content-Type: text/markdown
 
 # Cloud Custodian - OCI Support
 
 This is a plugin to Cloud Custodian that adds OCI support.
```

## Comparing `c7n_oci-0.1.8.dist-info/RECORD` & `c7n_oci-0.1.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 c7n_oci/resources/dns.py,sha256=OZslm4rtkcUTMma3vKhtDfglBUR1HilqAuFc_mnDS-s,4642
 c7n_oci/resources/identity.py,sha256=Y62wDVs93SUhktTUnwptZ4RTrS4k1vU3vTfIUR39hWg,33036
 c7n_oci/resources/object_storage.py,sha256=jB7zA2j-e0WxwrJoeBx07OPPKrwzqBktJkBpfPWYyTs,6441
 c7n_oci/resources/resource_map.py,sha256=YJqd5DI-vpT3arof70BHt5X_evZe69sm1Gl-9qGxMLc,626
 c7n_oci/resources/virtual_network.py,sha256=YbQasuc3Dn8eOjhWG0bsR3ywU5D3kFgjc2kiHdNZEg8,12225
 c7n_oci/session.py,sha256=VNDgRQgMCrZjcDl4CeWG9GYcqtHv4knA0Z-W2GUlbtk,3084
 c7n_oci/utils.py,sha256=A2GLjgapOFwXF3AUich-HuqZVZ60DfecrJp9dNqQrHo,732
-c7n_oci-0.1.8.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-c7n_oci-0.1.8.dist-info/RECORD,,
-c7n_oci-0.1.8.dist-info/METADATA,sha256=wXtrqQuPVYECZwble9L_P5Ja7RYsG-dxb1lxTuoO-W0,4252
+c7n_oci-0.1.9.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+c7n_oci-0.1.9.dist-info/RECORD,,
+c7n_oci-0.1.9.dist-info/METADATA,sha256=Fe-9cC326DnrKPOshJc5eL1S71-jgMvBplgYJ879pLQ,4340
```

