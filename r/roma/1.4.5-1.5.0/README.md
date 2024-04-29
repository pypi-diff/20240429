# Comparing `tmp/roma-1.4.5.tar.gz` & `tmp/roma-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roma-1.4.5.tar", last modified: Wed Apr 10 08:06:37 2024, max compression
+gzip compressed data, was "roma-1.5.0.tar", last modified: Mon Apr 29 06:57:25 2024, max compression
```

## Comparing `roma-1.4.5.tar` & `roma-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-10 08:06:37.597433 roma-1.4.5/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     1468 2024-04-08 09:35:19.000000 roma-1.4.5/LICENSE
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2276 2024-04-08 09:35:19.000000 roma-1.4.5/NOTICE
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4685 2024-04-10 08:06:37.597433 roma-1.4.5/PKG-INFO
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4207 2024-04-08 09:35:19.000000 roma-1.4.5/README.md
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      103 2023-02-08 15:17:32.000000 roma-1.4.5/pyproject.toml
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-10 08:06:37.597433 roma-1.4.5/roma/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      135 2024-04-08 09:35:19.000000 roma-1.4.5/roma/__init__.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3665 2024-04-08 09:35:19.000000 roma-1.4.5/roma/internal.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    19388 2024-04-08 09:35:19.000000 roma-1.4.5/roma/mappings.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    15139 2024-04-08 09:35:19.000000 roma-1.4.5/roma/transforms.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    21728 2024-04-08 09:35:19.000000 roma-1.4.5/roma/utils.py
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-10 08:06:37.597433 roma-1.4.5/roma.egg-info/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4685 2024-04-10 08:06:37.000000 roma-1.4.5/roma.egg-info/PKG-INFO
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      370 2024-04-10 08:06:37.000000 roma-1.4.5/roma.egg-info/SOURCES.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        1 2024-04-10 08:06:37.000000 roma-1.4.5/roma.egg-info/dependency_links.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        5 2024-04-10 08:06:37.000000 roma-1.4.5/roma.egg-info/top_level.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)       38 2024-04-10 08:06:37.597433 roma-1.4.5/setup.cfg
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      672 2024-04-08 09:35:19.000000 roma-1.4.5/setup.py
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-10 08:06:37.597433 roma-1.4.5/test/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      982 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_derivatives.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     8832 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_mappings.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3772 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_procrustes_derivatives.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    13180 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_transforms.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    15684 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_utils.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-29 06:57:25.556302 roma-1.5.0/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     1468 2024-04-08 09:35:19.000000 roma-1.5.0/LICENSE
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2276 2024-04-08 09:35:19.000000 roma-1.5.0/NOTICE
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4747 2024-04-29 06:57:25.556302 roma-1.5.0/PKG-INFO
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4269 2024-04-23 16:17:49.000000 roma-1.5.0/README.md
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      103 2023-02-08 15:17:32.000000 roma-1.5.0/pyproject.toml
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-29 06:57:25.552302 roma-1.5.0/roma/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      156 2024-04-19 12:26:44.000000 roma-1.5.0/roma/__init__.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     9863 2024-04-25 07:44:38.000000 roma-1.5.0/roma/euler.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3872 2024-04-19 16:12:23.000000 roma-1.5.0/roma/internal.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    19387 2024-04-19 11:18:29.000000 roma-1.5.0/roma/mappings.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    15139 2024-04-08 09:35:19.000000 roma-1.5.0/roma/transforms.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    21728 2024-04-08 09:35:19.000000 roma-1.5.0/roma/utils.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-29 06:57:25.556302 roma-1.5.0/roma.egg-info/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4747 2024-04-29 06:57:25.000000 roma-1.5.0/roma.egg-info/PKG-INFO
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      403 2024-04-29 06:57:25.000000 roma-1.5.0/roma.egg-info/SOURCES.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        1 2024-04-29 06:57:25.000000 roma-1.5.0/roma.egg-info/dependency_links.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        5 2024-04-29 06:57:25.000000 roma-1.5.0/roma.egg-info/top_level.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)       38 2024-04-29 06:57:25.556302 roma-1.5.0/setup.cfg
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      672 2024-04-19 15:06:45.000000 roma-1.5.0/setup.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-29 06:57:25.556302 roma-1.5.0/test/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      982 2024-04-08 09:35:19.000000 roma-1.5.0/test/test_derivatives.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     6276 2024-04-23 16:19:22.000000 roma-1.5.0/test/test_euler.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     8697 2024-04-19 12:24:47.000000 roma-1.5.0/test/test_mappings.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3772 2024-04-08 09:35:19.000000 roma-1.5.0/test/test_procrustes_derivatives.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    13180 2024-04-08 09:35:19.000000 roma-1.5.0/test/test_transforms.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    15684 2024-04-08 09:35:19.000000 roma-1.5.0/test/test_utils.py
```

### Comparing `roma-1.4.5/LICENSE` & `roma-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roma-1.4.5/NOTICE` & `roma-1.5.0/NOTICE`

 * *Files identical despite different names*

### Comparing `roma-1.4.5/PKG-INFO` & `roma-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roma
-Version: 1.4.5
+Version: 1.5.0
 Summary: A lightweight library to deal with 3D rotations in PyTorch.
 Home-page: https://github.com/naver/roma
 Author: Romain Brégier
 Author-email: romain.bregier@naverlabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,15 @@
 batch_shape = (2, 3)
 
 # Conversion between rotation representations
 rotvec = torch.randn(batch_shape + (3,))
 q = roma.rotvec_to_unitquat(rotvec)
 R = roma.unitquat_to_rotmat(q)
 Rbis = roma.rotvec_to_rotmat(rotvec)
+euler_angles = roma.unitquat_to_euler('xyz', q, degrees=True)
 
 # Regression of a rotation from an arbitrary input:
 # Special Procrustes orthonormalization of a 3x3 matrix
 R1 = roma.special_procrustes(torch.randn(batch_shape + (3, 3)))
 # Conversion from a 6D representation
 R2 = roma.special_gramschmidt(torch.randn(batch_shape + (3, 2)))
 # From the 10 coefficients of a 4x4 symmetric matrix
```

### Comparing `roma-1.4.5/README.md` & `roma-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 batch_shape = (2, 3)
 
 # Conversion between rotation representations
 rotvec = torch.randn(batch_shape + (3,))
 q = roma.rotvec_to_unitquat(rotvec)
 R = roma.unitquat_to_rotmat(q)
 Rbis = roma.rotvec_to_rotmat(rotvec)
+euler_angles = roma.unitquat_to_euler('xyz', q, degrees=True)
 
 # Regression of a rotation from an arbitrary input:
 # Special Procrustes orthonormalization of a 3x3 matrix
 R1 = roma.special_procrustes(torch.randn(batch_shape + (3, 3)))
 # Conversion from a 6D representation
 R2 = roma.special_gramschmidt(torch.randn(batch_shape + (3, 2)))
 # From the 10 coefficients of a 4x4 symmetric matrix
```

### Comparing `roma-1.4.5/roma/internal.py` & `roma-1.5.0/roma/internal.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,8 +100,16 @@
 try:
     torch.linalg.norm
     def norm(x, dim=None, keepdim=False):
         return torch.linalg.norm(x, dim=dim, keepdim=keepdim)
 except AttributeError:
     # torch.linalg.norm was introduced in PyTorch 1.7, and torch.norm is deprecated.
     def norm(x, dim=None, keepdim=False):
-        return torch.norm(x, dim=dim, keepdim=keepdim)
+        return torch.norm(x, dim=dim, keepdim=keepdim)
+    
+try:
+    torch.hypot
+    hypot = torch.hypot
+except AttributeError:
+    # torch.hypot is not available in PyTorch 1.6.
+    def hypot(x, y):
+        return torch.sqrt(torch.square(x) + torch.square(y))
```

### Comparing `roma-1.4.5/roma/mappings.py` & `roma-1.5.0/roma/mappings.py`

 * *Ordering differences only*

 * *Files identical despite different names*

```diff
@@ -446,8 +446,8 @@
 
     Args:
         wxyz (...x4 tensor, WXYZ convention): batch of quaternions.
     Returns:
         batch of quaternions (...x4 tensor, XYZW convention).
     """
     assert wxyz.shape[-1] == 4
-    return torch.cat((wxyz[...,1:], wxyz[...,0,None]), dim=-1)
+    return torch.cat((wxyz[...,1:], wxyz[...,0,None]), dim=-1)
```

### Comparing `roma-1.4.5/roma/transforms.py` & `roma-1.5.0/roma/transforms.py`

 * *Files identical despite different names*

### Comparing `roma-1.4.5/roma/utils.py` & `roma-1.5.0/roma/utils.py`

 * *Files identical despite different names*

### Comparing `roma-1.4.5/roma.egg-info/PKG-INFO` & `roma-1.5.0/roma.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roma
-Version: 1.4.5
+Version: 1.5.0
 Summary: A lightweight library to deal with 3D rotations in PyTorch.
 Home-page: https://github.com/naver/roma
 Author: Romain Brégier
 Author-email: romain.bregier@naverlabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,15 @@
 batch_shape = (2, 3)
 
 # Conversion between rotation representations
 rotvec = torch.randn(batch_shape + (3,))
 q = roma.rotvec_to_unitquat(rotvec)
 R = roma.unitquat_to_rotmat(q)
 Rbis = roma.rotvec_to_rotmat(rotvec)
+euler_angles = roma.unitquat_to_euler('xyz', q, degrees=True)
 
 # Regression of a rotation from an arbitrary input:
 # Special Procrustes orthonormalization of a 3x3 matrix
 R1 = roma.special_procrustes(torch.randn(batch_shape + (3, 3)))
 # Conversion from a 6D representation
 R2 = roma.special_gramschmidt(torch.randn(batch_shape + (3, 2)))
 # From the 10 coefficients of a 4x4 symmetric matrix
```

### Comparing `roma-1.4.5/setup.py` & `roma-1.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="roma",
-    version="1.4.5",
+    version="1.5.0",
     author="Romain Brégier",
     author_email="romain.bregier@naverlabs.com",
     description="A lightweight library to deal with 3D rotations in PyTorch.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/naver/roma",
     packages=["roma"],
```

### Comparing `roma-1.4.5/test/test_derivatives.py` & `roma-1.5.0/test/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `roma-1.4.5/test/test_mappings.py` & `roma-1.5.0/test/test_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 # 3-Clause BSD License.
 import unittest
 import torch
 import roma
 import numpy as np
 from test.utils import is_close
 
-def is_close(A, B, eps1 = 1e-5, eps2 = 1e-5):
-    return torch.norm(A - B) / (torch.norm(torch.abs(A) + torch.abs(B)) + eps1) < eps2
-
 device = torch.device(0) if torch.cuda.is_available() else torch.device('cpu')
 
 class TestMappings(unittest.TestCase):
     def test_orthonormal(self):
         for dtype in (torch.float32, torch.float64):
             M = torch.eye(3, dtype=dtype, device=device).expand(10, 3, 3).contiguous()
             self.assertTrue(roma.is_orthonormal_matrix(M))
@@ -187,10 +184,9 @@
         for batch_shape in [(), (10,), (23,5)]:
             quat_xyzw = torch.randn(batch_shape + (4,))
             quat_wxyz = roma.mappings.quat_xyzw_to_wxyz(quat_xyzw)
             self.assertTrue(quat_xyzw.shape == quat_wxyz.shape)
             quat_xyzw_bis = roma.mappings.quat_wxyz_to_xyzw(quat_wxyz)
             self.assertTrue(torch.all(quat_xyzw == quat_xyzw_bis))
 
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `roma-1.4.5/test/test_procrustes_derivatives.py` & `roma-1.5.0/test/test_procrustes_derivatives.py`

 * *Files identical despite different names*

### Comparing `roma-1.4.5/test/test_transforms.py` & `roma-1.5.0/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `roma-1.4.5/test/test_utils.py` & `roma-1.5.0/test/test_utils.py`

 * *Files identical despite different names*

