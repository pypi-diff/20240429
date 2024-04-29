# Comparing `tmp/rcwa_tlv-0.0.1.tar.gz` & `tmp/rcwa_tlv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcwa_tlv-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rcwa_tlv-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rcwa_tlv-0.0.1.tar` & `rcwa_tlv-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1109 2024-04-24 14:03:13.173831 rcwa_tlv-0.0.1/README.md
--rw-r--r--   0        0        0      776 2024-04-24 14:16:03.310502 rcwa_tlv-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      141 2024-04-24 14:01:05.412424 rcwa_tlv-0.0.1/src/rcwa_tlv/__init__.py
--rw-r--r--   0        0        0      308 2024-04-24 11:08:07.976197 rcwa_tlv-0.0.1/src/rcwa_tlv/devices/device.py
--rw-r--r--   0        0        0       38 2024-04-19 11:41:39.425074 rcwa_tlv-0.0.1/src/rcwa_tlv/devices/normal_fields.py
--rw-r--r--   0        0        0     1752 2024-04-24 11:16:37.097162 rcwa_tlv-0.0.1/src/rcwa_tlv/devices/shapes.py
--rw-r--r--   0        0        0      693 2024-04-24 11:10:05.357323 rcwa_tlv-0.0.1/src/rcwa_tlv/devices/source.py
--rw-r--r--   0        0        0     4650 2023-11-21 15:43:58.000000 rcwa_tlv-0.0.1/src/rcwa_tlv/materials/Si.txt
--rw-r--r--   0        0        0      307 2023-11-21 15:43:58.000000 rcwa_tlv-0.0.1/src/rcwa_tlv/materials/SiO2.txt
--rw-r--r--   0        0        0      370 2023-11-21 15:43:58.000000 rcwa_tlv-0.0.1/src/rcwa_tlv/materials/TiO2.txt
--rw-r--r--   0        0        0    12891 2024-04-24 11:42:43.657035 rcwa_tlv-0.0.1/src/rcwa_tlv/rcwa.py
--rw-r--r--   0        0        0     1431 2024-04-24 07:00:20.140807 rcwa_tlv-0.0.1/src/rcwa_tlv/utils/convmat.py
--rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 rcwa_tlv-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-04-24 14:03:13.173831 rcwa_tlv-0.0.2/README.md
+-rw-r--r--   0        0        0      776 2024-04-24 14:16:03.310502 rcwa_tlv-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      141 2024-04-29 13:22:45.879796 rcwa_tlv-0.0.2/src/rcwa_tlv/__init__.py
+-rw-r--r--   0        0        0      308 2024-04-24 11:08:07.976197 rcwa_tlv-0.0.2/src/rcwa_tlv/devices/device.py
+-rw-r--r--   0        0        0       38 2024-04-19 11:41:39.425074 rcwa_tlv-0.0.2/src/rcwa_tlv/devices/normal_fields.py
+-rw-r--r--   0        0        0     1762 2024-04-27 15:37:18.813112 rcwa_tlv-0.0.2/src/rcwa_tlv/devices/shapes.py
+-rw-r--r--   0        0        0      693 2024-04-24 11:10:05.357323 rcwa_tlv-0.0.2/src/rcwa_tlv/devices/source.py
+-rw-r--r--   0        0        0     4146 2024-04-27 04:47:19.202885 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/Si.txt
+-rw-r--r--   0        0        0      279 2024-04-27 04:38:11.772145 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/SiO2.txt
+-rw-r--r--   0        0        0      370 2023-11-21 15:43:58.000000 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/TiO2.txt
+-rw-r--r--   0        0        0       57 2024-04-27 05:06:13.312988 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-27 10:24:36.008784 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/materials.py
+-rw-r--r--   0        0        0    13637 2024-04-29 13:22:22.967728 rcwa_tlv-0.0.2/src/rcwa_tlv/rcwa.py
+-rw-r--r--   0        0        0     1431 2024-04-24 07:00:20.140807 rcwa_tlv-0.0.2/src/rcwa_tlv/utils/convmat.py
+-rw-r--r--   0        0        0      598 2024-04-27 16:10:11.507347 rcwa_tlv-0.0.2/src/rcwa_tlv/utils/normal_vector.py
+-rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 rcwa_tlv-0.0.2/PKG-INFO
```

### Comparing `rcwa_tlv-0.0.1/README.md` & `rcwa_tlv-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.1/pyproject.toml` & `rcwa_tlv-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.1/src/rcwa_tlv/devices/shapes.py` & `rcwa_tlv-0.0.2/src/rcwa_tlv/devices/shapes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import numpy as np
 
 
-def add_circle(array: np.ndarray, center: tuple, radius: float, val: float) -> np.ndarray:
+def add_circle(array: np.ndarray, center: tuple, radius: float, val: float | complex) -> np.ndarray:
     """
     Add a circle with a given value to a 2D array.
 
     Parameters:
         array (numpy.ndarray): The 2D array.
         center (tuple): Coordinates of the center of the circle (row, column).
         radius (int): Radius of the circle.
```

### Comparing `rcwa_tlv-0.0.1/src/rcwa_tlv/devices/source.py` & `rcwa_tlv-0.0.2/src/rcwa_tlv/devices/source.py`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.1/src/rcwa_tlv/rcwa.py` & `rcwa_tlv-0.0.2/src/rcwa_tlv/rcwa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 import numpy as np
 from scipy.linalg import expm
 from typing import Literal
 
 from rcwa_tlv.utils.convmat import convmat
+from rcwa_tlv.utils.normal_vector import calc_nv_fields
 from rcwa_tlv import Device, Source
 
 
 class RCWA:
     def __init__(
             self,
             device: Device,
@@ -24,24 +25,29 @@
         self.renormalize = renormalize
         self.result = None
 
         self.dtype = dtype
         self.cdtype = np.complex128 if dtype == np.float64 else np.complex64
         self.idtype = np.int64 if dtype == np.float64 else np.int32
 
-        if apply_nv:
-            raise NotImplementedError("NV is not yet implemented.")
+        # if apply_nv:
+        #     raise NotImplementedError("NV is not yet implemented.")
 
-    def __call__(self, *args, **kwargs) -> dict:
+    def __call__(self, *args, apply_nv=None, **kwargs) -> dict:
         ur1 = self.device.ur1
         er1 = self.device.er1
         ur2 = self.device.ur2
         er2 = self.device.er2
         gamma = self.gamma
         polarization_vec = self.source.polarization_vec
+        self.apply_nv = apply_nv if apply_nv is not None else self.apply_nv
+
+        if self.apply_nv:
+            for layer in self.device.layers:
+                layer['nv_x'], layer['nv_y'] = calc_nv_fields(layer['er'])
 
         n_layers = len(self.device.layers)
         num_of_m = 1 + 2 * self.device.p  # x/width axis
         num_of_n = 1 + 2 * self.device.q  # y/height axis
 
         # Compute k0 and incident wavevector
         k0 = 2 * np.pi / self.source.lam0
@@ -52,69 +58,70 @@
         ])
 
         # Compute kx and ky
         m = np.arange(-self.device.p, self.device.p + 1)  # x/width axis
         n = np.arange(-self.device.q, self.device.q + 1)  # y/height axis
         kx = k_inc[0] - 2 * np.pi * m / (k0 * self.device.period_x)
         ky = k_inc[1] - 2 * np.pi * n / (k0 * self.device.period_y)
-        kx, ky = np.meshgrid(kx.astype(self.cdtype), ky.astype(self.cdtype))
+        # kx, ky = np.meshgrid(kx.astype(self.cdtype), ky.astype(self.cdtype))
+        ky, kx = np.meshgrid(ky.astype(self.cdtype), kx.astype(self.cdtype))
 
         # Compute kz in reflection and transmission regions
         kz_ref = np.conj((ur1 * er1 - kx ** 2 - ky ** 2).astype(self.cdtype) ** 0.5)
         kz_trn = np.conj((ur2 * er2 - kx ** 2 - ky ** 2).astype(self.cdtype) ** 0.5)
-        maxk = ky[0, 0] * kx[0, 0] * 4
 
-        m_vec, n_vec = np.meshgrid(m.astype(self.idtype), n.astype(self.idtype))
+        # m_vec, n_vec = np.meshgrid(m.astype(self.idtype), n.astype(self.idtype))
+        n_vec, m_vec = np.meshgrid(n.astype(self.idtype), m.astype(self.idtype))
 
         # Truncate k vectors
         shape = (np.abs(m_vec / self.device.p) ** (2 * gamma) + np.abs(n_vec / self.device.q) ** (2 * gamma)) <= 1
         non_zero_rows, non_zero_cols = np.nonzero(shape)
         inxs = np.ravel_multi_index((non_zero_rows, non_zero_cols), shape.shape)
         n_nonzero = np.count_nonzero(shape)
 
-        kx = (kx + maxk) * shape
-        ky = (ky + maxk) * shape
-        kz_ref = (kz_ref + maxk) * shape
-        kz_trn = (kz_trn + maxk) * shape
+        kx[np.logical_not(shape)] = 0
+        ky[np.logical_not(shape)] = 0
+        kz_ref[np.logical_not(shape)] = 0
+        kz_trn[np.logical_not(shape)] = 0
 
         # Compute convolution matrices and truncate
         er_c_mat = np.zeros((n_layers, n_nonzero, n_nonzero), dtype=self.cdtype)
         er_inv_mat = np.zeros((n_layers, n_nonzero, n_nonzero), dtype=self.cdtype)
         delta_mat = np.zeros((n_layers, n_nonzero, n_nonzero), dtype=self.cdtype)
 
-        if self.apply_nv:
-            ...
-            # NVx_C = np.zeros((n_layers, np.count_nonzero(shape), np.count_nonzero(shape)))
-            # NVy_C = np.zeros((n_layers, np.count_nonzero(shape), np.count_nonzero(shape)))
-            # NVxy_C = np.zeros((n_layers, np.count_nonzero(shape), np.count_nonzero(shape)))
+        nvx_c = np.zeros((n_layers, n_nonzero, n_nonzero), dtype=self.cdtype) if self.apply_nv else None
+        nvy_c = np.zeros((n_layers, n_nonzero, n_nonzero), dtype=self.cdtype) if self.apply_nv else None
+        nvxy_c = np.zeros((n_layers, n_nonzero, n_nonzero), dtype=self.cdtype) if self.apply_nv else None
 
         for i_layer in range(n_layers):
             er_temp = convmat(
                 self.device.layers[i_layer]['er'].astype(self.cdtype), num_of_m, num_of_n, dtype=self.cdtype
             )
             er_c_mat[i_layer, :, :] = er_temp[inxs, :][:, inxs]
 
             er_inv = convmat(1 / self.device.layers[i_layer]['er'], num_of_m, num_of_n, dtype=self.cdtype)
             er_inv_mat[i_layer, :, :] = np.linalg.inv(er_inv[inxs, :][:, inxs])
 
             delta_mat[i_layer, :, :] = er_c_mat[i_layer, :, :] - er_inv_mat[i_layer, :, :]
 
             if self.apply_nv:
-                ...
-                # NVxtemp = convmat(DEV['NVx'] ** 2, M, N)
-                # NVytemp = convmat(DEV['NVy'] ** 2, M, N)
-                # NVxytemp = convmat(DEV['NVx'] * DEV['NVy'], M, N)
-                # NVx_C[i_layer, :, :] = NVxtemp[shape, :][:, shape]
-                # NVy_C[i_layer, :, :] = NVytemp[shape, :][:, shape]
-                # NVxy_C[i_layer, :, :] = NVxytemp[shape, :][:, shape]
-
-        kx_mat = np.diag(kx[non_zero_rows, non_zero_cols] - maxk).astype(self.cdtype)
-        ky_mat = np.diag(ky[non_zero_rows, non_zero_cols] - maxk).astype(self.cdtype)
-        kz_ref_mat = np.diag(kz_ref[non_zero_rows, non_zero_cols] - maxk)
-        kz_trn_mat = np.diag(kz_trn[non_zero_rows, non_zero_cols] - maxk)
+                nvxtemp = convmat(self.device.layers[i_layer]['nv_x'] ** 2, num_of_m, num_of_n)
+                nvytemp = convmat(self.device.layers[i_layer]['nv_y'] ** 2, num_of_m, num_of_n)
+                nvxytemp = convmat(
+                    self.device.layers[i_layer]['nv_x'] * self.device.layers[i_layer]['nv_y'], num_of_m, num_of_n
+                )
+
+                nvx_c[i_layer, :, :] = nvxtemp[inxs, :][:, inxs]
+                nvy_c[i_layer, :, :] = nvytemp[inxs, :][:, inxs]
+                nvxy_c[i_layer, :, :] = nvxytemp[inxs, :][:, inxs]
+
+        kx_mat = np.diag(kx[non_zero_rows, non_zero_cols]).astype(self.cdtype)
+        ky_mat = np.diag(ky[non_zero_rows, non_zero_cols]).astype(self.cdtype)
+        kz_ref_mat = np.diag(kz_ref[non_zero_rows, non_zero_cols])
+        kz_trn_mat = np.diag(kz_trn[non_zero_rows, non_zero_cols])
 
         # EMT RCWA
         delta = np.zeros(n_nonzero)
         delta[len(delta) // 2] = 1
         s_mat = np.concatenate([
             polarization_vec[0] * delta,
             polarization_vec[1] * delta,
@@ -162,24 +169,29 @@
                 erkx = np.linalg.solve(er_c_mat[i_layer], kx_mat)
 
                 p_mat[:, :, i_layer] = np.block([  # type:ignore
                     [kx_mat @ erky, i_mat - kx_mat @ erkx],
                     [ky_mat @ erky - i_mat, -ky_mat @ erkx]
                 ])
                 if self.apply_nv:
-                    ...
-                    # DeltaNxy = DELTA[i_layer] @ NVxy_C[i_layer]
-                    # Q[:, :, i_layer] = np.block([
-                    #     [Kx @ Ky - DeltaNxy, ER_C[i_layer] - DELTA[i_layer] @ NVy_C[i_layer] - Kx @ Kx],
-                    #     [Ky @ Ky - ER_C[i_layer] + DELTA[i_layer] @ NVx_C[i_layer], -Ky @ Kx + DeltaNxy]
-                    # ])
+                    delta_nxy = delta_mat[i_layer] @ nvxy_c[i_layer]
+                    q_mat[:, :, i_layer] = np.block([  # type:ignore
+                        [
+                            kx_mat @ ky_mat - delta_nxy,
+                            er_c_mat[i_layer] - delta_mat[i_layer] @ nvy_c[i_layer] - kx_mat @ kx_mat
+                        ],
+                        [
+                            ky_mat @ ky_mat - er_c_mat[i_layer] + delta_mat[i_layer] @ nvx_c[i_layer],
+                            -ky_mat @ kx_mat + delta_nxy
+                        ]
+                    ])
                 else:
                     q_mat[:, :, i_layer] = np.block([  # type:ignore
                         [kx_mat @ ky_mat, er_c_mat[i_layer] - kx_mat @ kx_mat],
-                        [ky_mat @ ky_mat - er_c_mat[i_layer], -kx_mat @ kx_mat]
+                        [ky_mat @ ky_mat - er_c_mat[i_layer], -ky_mat @ kx_mat]
                     ])
                 omega_2 = p_mat[:, :, i_layer] @ q_mat[:, :, i_layer]
                 lam, w_mat = np.linalg.eig(omega_2)
                 lam = np.diag(np.sqrt(lam))
                 x_mat[:, :, i_layer] = expm(-lam * k0 * self.device.layers[i_layer]['length_z'])
                 v_mat = q_mat[:, :, i_layer] @ w_mat @ np.linalg.inv(lam)
                 f_mat[:, :, i_layer] = np.block([  # type:ignore
```

### Comparing `rcwa_tlv-0.0.1/src/rcwa_tlv/utils/convmat.py` & `rcwa_tlv-0.0.2/src/rcwa_tlv/utils/convmat.py`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.1/PKG-INFO` & `rcwa_tlv-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcwa_tlv
-Version: 0.0.1
+Version: 0.0.2
 Summary: RCWA solver for photonic devices
 Author-email: Victor Egorov <victoregorov23@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

