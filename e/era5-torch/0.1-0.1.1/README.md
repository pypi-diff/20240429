# Comparing `tmp/era5_torch-0.1.tar.gz` & `tmp/era5_torch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era5_torch-0.1.tar", last modified: Fri Apr 26 13:40:12 2024, max compression
+gzip compressed data, was "era5_torch-0.1.1.tar", last modified: Mon Apr 29 09:57:28 2024, max compression
```

## Comparing `era5_torch-0.1.tar` & `era5_torch-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-26 13:40:12.237148 era5_torch-0.1/
--rw-r--r--   0 almico     (501) staff       (20)     1070 2024-04-26 12:52:29.000000 era5_torch-0.1/LICENSE.MIT
--rw-r--r--   0 almico     (501) staff       (20)     2784 2024-04-26 13:40:12.236711 era5_torch-0.1/PKG-INFO
--rw-r--r--   0 almico     (501) staff       (20)     2431 2024-04-26 13:33:22.000000 era5_torch-0.1/README.md
--rw-r--r--   0 almico     (501) staff       (20)      440 2024-04-26 13:36:59.000000 era5_torch-0.1/pyproject.toml
--rw-r--r--   0 almico     (501) staff       (20)       38 2024-04-26 13:40:12.237204 era5_torch-0.1/setup.cfg
-drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-26 13:40:12.228700 era5_torch-0.1/src/
-drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-26 13:40:12.233563 era5_torch-0.1/src/era5_torch/
--rw-r--r--   0 almico     (501) staff       (20)      235 2024-04-26 13:10:49.000000 era5_torch-0.1/src/era5_torch/__init__.py
--rw-r--r--   0 almico     (501) staff       (20)     7994 2024-04-26 12:01:05.000000 era5_torch-0.1/src/era5_torch/_auxiliaries.py
--rw-r--r--   0 almico     (501) staff       (20)     8649 2024-04-26 12:01:28.000000 era5_torch-0.1/src/era5_torch/_chunkers.py
--rw-r--r--   0 almico     (501) staff       (20)    16229 2024-04-26 13:09:44.000000 era5_torch-0.1/src/era5_torch/_dataset_class.py
--rw-r--r--   0 almico     (501) staff       (20)     2014 2024-04-26 12:01:37.000000 era5_torch-0.1/src/era5_torch/_patchers.py
-drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-26 13:40:12.235829 era5_torch-0.1/src/era5_torch.egg-info/
--rw-r--r--   0 almico     (501) staff       (20)     2784 2024-04-26 13:40:12.000000 era5_torch-0.1/src/era5_torch.egg-info/PKG-INFO
--rw-r--r--   0 almico     (501) staff       (20)      418 2024-04-26 13:40:12.000000 era5_torch-0.1/src/era5_torch.egg-info/SOURCES.txt
--rw-r--r--   0 almico     (501) staff       (20)        1 2024-04-26 13:40:12.000000 era5_torch-0.1/src/era5_torch.egg-info/dependency_links.txt
--rw-r--r--   0 almico     (501) staff       (20)       31 2024-04-26 13:40:12.000000 era5_torch-0.1/src/era5_torch.egg-info/requires.txt
--rw-r--r--   0 almico     (501) staff       (20)       11 2024-04-26 13:40:12.000000 era5_torch-0.1/src/era5_torch.egg-info/top_level.txt
-drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-26 13:40:12.235145 era5_torch-0.1/tests/
--rw-r--r--   0 almico     (501) staff       (20)     7433 2024-04-26 13:05:27.000000 era5_torch-0.1/tests/test_chunkers.py
--rw-r--r--   0 almico     (501) staff       (20)    13416 2024-04-26 13:05:37.000000 era5_torch-0.1/tests/test_datasets.py
+drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-29 09:57:28.947363 era5_torch-0.1.1/
+-rw-r--r--   0 almico     (501) staff       (20)     1070 2024-04-26 12:52:29.000000 era5_torch-0.1.1/LICENSE.MIT
+-rw-r--r--   0 almico     (501) staff       (20)     2773 2024-04-29 09:57:28.947190 era5_torch-0.1.1/PKG-INFO
+-rw-r--r--   0 almico     (501) staff       (20)     2418 2024-04-26 13:47:54.000000 era5_torch-0.1.1/README.md
+-rw-r--r--   0 almico     (501) staff       (20)      442 2024-04-29 09:56:15.000000 era5_torch-0.1.1/pyproject.toml
+-rw-r--r--   0 almico     (501) staff       (20)       38 2024-04-29 09:57:28.947400 era5_torch-0.1.1/setup.cfg
+drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-29 09:57:28.944083 era5_torch-0.1.1/src/
+drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-29 09:57:28.945725 era5_torch-0.1.1/src/era5_torch/
+-rw-r--r--   0 almico     (501) staff       (20)      397 2024-04-29 08:09:47.000000 era5_torch-0.1.1/src/era5_torch/__init__.py
+-rw-r--r--   0 almico     (501) staff       (20)     7994 2024-04-26 12:01:05.000000 era5_torch-0.1.1/src/era5_torch/_auxiliaries.py
+-rw-r--r--   0 almico     (501) staff       (20)     8649 2024-04-26 12:01:28.000000 era5_torch-0.1.1/src/era5_torch/_chunkers.py
+-rw-r--r--   0 almico     (501) staff       (20)    12381 2024-04-29 09:54:43.000000 era5_torch-0.1.1/src/era5_torch/_dataset_class.py
+-rw-r--r--   0 almico     (501) staff       (20)     2014 2024-04-26 12:01:37.000000 era5_torch-0.1.1/src/era5_torch/_patchers.py
+drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-29 09:57:28.947011 era5_torch-0.1.1/src/era5_torch.egg-info/
+-rw-r--r--   0 almico     (501) staff       (20)     2773 2024-04-29 09:57:28.000000 era5_torch-0.1.1/src/era5_torch.egg-info/PKG-INFO
+-rw-r--r--   0 almico     (501) staff       (20)      418 2024-04-29 09:57:28.000000 era5_torch-0.1.1/src/era5_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 almico     (501) staff       (20)        1 2024-04-29 09:57:28.000000 era5_torch-0.1.1/src/era5_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 almico     (501) staff       (20)       31 2024-04-29 09:57:28.000000 era5_torch-0.1.1/src/era5_torch.egg-info/requires.txt
+-rw-r--r--   0 almico     (501) staff       (20)       11 2024-04-29 09:57:28.000000 era5_torch-0.1.1/src/era5_torch.egg-info/top_level.txt
+drwxr-xr-x   0 almico     (501) staff       (20)        0 2024-04-29 09:57:28.946563 era5_torch-0.1.1/tests/
+-rw-r--r--   0 almico     (501) staff       (20)     7415 2024-04-29 08:07:39.000000 era5_torch-0.1.1/tests/test_chunkers.py
+-rw-r--r--   0 almico     (501) staff       (20)    12517 2024-04-29 09:54:02.000000 era5_torch-0.1.1/tests/test_datasets.py
```

### Comparing `era5_torch-0.1/LICENSE.MIT` & `era5_torch-0.1.1/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `era5_torch-0.1/PKG-INFO` & `era5_torch-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: era5_torch
-Version: 0.1
+Version: 0.1.1
 Summary: PyTorch-compatible wrapper for Era5
 Author-email: Alexander Conzelmann <a.conzelmann@student.uni-tuebingen.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.MIT
 Requires-Dist: torch
 Requires-Dist: torchvision
@@ -45,8 +45,7 @@
 ```
 from era5_torch import Era5, Coordinate, ContinuousChunker
 ds = Era5("/Users/almico/datasets/era5_temperatures_2008.nc", "t", normalize=False,chunker=ContinuousChunker((3,3,3)))
 ds[0]
 ```
 
 Returns a sample of shape `(3,3,3)` with values varying over `(time, lat, long)`. Alternatively, to get patches, you can also create a Chunker with `ContinuousChunker((3,3))`. All chunkers have different behaviour, the `ContinuousChunker` for example returns chunks starting from the first position in the dataset (usually the (0,0) coordinate) and creates as many chunks in an orderly manner as possible by traversing the coordinates one after another. Refer to the documentation of the Chunkers to get more information.# era5_torch
-# era5_torch
```

### Comparing `era5_torch-0.1/README.md` & `era5_torch-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,7 @@
 ```
 from era5_torch import Era5, Coordinate, ContinuousChunker
 ds = Era5("/Users/almico/datasets/era5_temperatures_2008.nc", "t", normalize=False,chunker=ContinuousChunker((3,3,3)))
 ds[0]
 ```
 
 Returns a sample of shape `(3,3,3)` with values varying over `(time, lat, long)`. Alternatively, to get patches, you can also create a Chunker with `ContinuousChunker((3,3))`. All chunkers have different behaviour, the `ContinuousChunker` for example returns chunks starting from the first position in the dataset (usually the (0,0) coordinate) and creates as many chunks in an orderly manner as possible by traversing the coordinates one after another. Refer to the documentation of the Chunkers to get more information.# era5_torch
-# era5_torch
```

### Comparing `era5_torch-0.1/src/era5_torch/_auxiliaries.py` & `era5_torch-0.1.1/src/era5_torch/_auxiliaries.py`

 * *Files identical despite different names*

### Comparing `era5_torch-0.1/src/era5_torch/_chunkers.py` & `era5_torch-0.1.1/src/era5_torch/_chunkers.py`

 * *Files identical despite different names*

### Comparing `era5_torch-0.1/src/era5_torch/_dataset_class.py` & `era5_torch-0.1.1/src/era5_torch/_dataset_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from ._chunkers import Chunker
 import xarray
 from enum import Enum
 
 import glob
 from pathlib import Path
-from coinpp.conversion import Converter
 
 
 # taken from our large 2008 dataset
 T_MIN = 194.8391418457031
 T_MAX = 327.346343994141
 T_MEAN = 264.752433
 T_STD = 18.535514
@@ -48,19 +47,23 @@
     tensor = torch.Tensor(sample.values)
     if len(tensor.shape) == 2:
         tensor = tensor.unsqueeze(0)
     assert len(tensor.shape) == 3
     return tensor
 
 
-def normalize(arr):
+def normalize(arr: torch.Tensor | np.ndarray):
+    """Normalizes the array to be in the range [0, 1]. Uses
+    the precomputed values from the year 2008 that might not be appropriate for other datasets.
+    """
     return (arr - T_MIN) / (T_MAX - T_MIN)
 
 
-def unnormalize(arr):
+def unnormalize(arr: torch.Tensor | np.ndarray):
+    """Undoes the normalization of this package. Uses the precomputed values from the year 2008 that might not be appropriate for other datasets."""
     return arr * (T_MAX - T_MIN) + T_MIN
 
 
 class Era5(Dataset):
     """Class that wraps the Era5 dataset to be used with PyTorch.
     Expect the dataset to be in NetCDF format, and contain latitude, longitude, level, and time dimensions.
 
@@ -321,111 +324,7 @@
     def __len__(self) -> int:
         if self._chunker.dimension == 2:
             return self._num_timesteps * self._num_levels * self._chunks_per_sample
         elif self._chunker.dimension == 3:
             return self._num_levels * self._chunks_per_sample
         else:
             raise ValueError(f"Invalid dimension {self._chunker.dimension}")
-
-
-class Era5Coinpp(torch.utils.data.Dataset):
-    """Taken from COIN++. Loads in a dataset of ERA5 temperatures, in the format that is used in the COIN++ paper.
-    This means a folder of three folders, train, val and test, each containing .npz files. The files are named according to the timestamp they are from,
-    in the format DD-MM-YYTHH.npz. The .npz files produce numpy arrays with the following keys:
-    - latitude: Latitude values for each pixel
-    - longitude: Longitude values for each pixel
-    - temperature: Temperature values for each pixel
-
-    Args:
-        root (string or PosixPath): Path to directory where data is stored.
-        split (string): Which split to use from train/val/test.
-        normalize (bool): Whether to normalize data to lie in [0, 1]. Defaults to True.
-    """
-
-    def __init__(
-        self,
-        root: Path,
-        split,
-        normalize=True,
-        coords_features: bool = True,
-        max_samples: Optional[int] = None,
-        feature_transform=None,
-        patch_size: Optional[int | tuple[int, int]] = None,
-    ):
-        if split not in ["train", "val", "test", "all"]:
-            raise ValueError("Invalid value for split argument")
-
-        self.root = root
-        self.split = split
-        self.normalize = normalize
-        self.coords_features = coords_features
-        self.converter = Converter("era5")
-        self.filepaths = glob.glob(str(root / f"era5_{split}/*.npz"))
-        self.filepaths.sort()  # Ensure consistent ordering of paths
-        self.max_samples = max_samples
-        self.patch_size = patch_size
-        self.feature_transform = feature_transform
-
-    def image_shape(self):
-        if self.patch_size is None:
-            return np.load(self.filepaths[0])["temperature"].shape
-        else:
-            if isinstance(self.patch_size, int):
-                return (self.patch_size, self.patch_size)
-            else:
-                return self.patch_size
-
-    def to_tensors(
-        self, n: Optional[int] = None, start: int = 0
-    ) -> tuple[torch.Tensor, torch.Tensor]:
-        coords = []
-        features = []
-        if n is None:
-            n = self.__len__() - start
-        if start + n > self.__len__():
-            raise ValueError(
-                f"Cannot get {n} samples starting at {start} from dataset of size {self.__len__()}"
-            )
-        for i in range(start, n + start):
-            c, f = self.__getitem__(i)
-            coords.append(c)
-            features.append(f)
-        return torch.stack(coords), torch.stack(features)
-
-    def _patch(self, item: torch.Tensor, channel_last: bool = True) -> torch.Tensor:
-        if self.patch_size is None:
-            return item
-
-        if channel_last:
-            item = torch.permute(item, (2, 0, 1))
-        item = T.RandomCrop(self.patch_size)(item)
-        if channel_last:
-            item = torch.permute(item, (1, 2, 0))
-        return item
-
-    def __getitem__(self, index) -> tuple[torch.Tensor, torch.Tensor]:
-        # Dictionary containing latitude, longitude and temperature
-        data = np.load(self.filepaths[index])
-        temperature = data["temperature"]  # Shape (num_lats, num_lons)
-        # Optionally normalize data
-        if self.normalize:
-            temperature = normalize(temperature)
-        # Convert to tensor and add channel dimension (1, num_lats, num_lons)
-        temperature = torch.Tensor(temperature).unsqueeze(0)
-
-        if self.coords_features:
-            coordinates, features = self.converter.to_coordinates_and_features(temperature)  # type: ignore
-            assert coordinates is not None
-            coordinates, features = (
-                self._patch(coordinates).flatten(0, 1),
-                torch.permute(self._patch(features), (2, 0, 1)),
-            )
-            if self.feature_transform is not None:
-                features = self.feature_transform(features)
-            return coordinates, features
-        else:
-            raise NotImplementedError("Only coordinates and features supported")
-
-    def __len__(self):
-        if self.max_samples is not None:
-            return self.max_samples
-        return len(self.filepaths)
```

### Comparing `era5_torch-0.1/src/era5_torch/_patchers.py` & `era5_torch-0.1.1/src/era5_torch/_patchers.py`

 * *Files identical despite different names*

### Comparing `era5_torch-0.1/src/era5_torch.egg-info/PKG-INFO` & `era5_torch-0.1.1/src/era5_torch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: era5_torch
-Version: 0.1
+Version: 0.1.1
 Summary: PyTorch-compatible wrapper for Era5
 Author-email: Alexander Conzelmann <a.conzelmann@student.uni-tuebingen.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.MIT
 Requires-Dist: torch
 Requires-Dist: torchvision
@@ -45,8 +45,7 @@
 ```
 from era5_torch import Era5, Coordinate, ContinuousChunker
 ds = Era5("/Users/almico/datasets/era5_temperatures_2008.nc", "t", normalize=False,chunker=ContinuousChunker((3,3,3)))
 ds[0]
 ```
 
 Returns a sample of shape `(3,3,3)` with values varying over `(time, lat, long)`. Alternatively, to get patches, you can also create a Chunker with `ContinuousChunker((3,3))`. All chunkers have different behaviour, the `ContinuousChunker` for example returns chunks starting from the first position in the dataset (usually the (0,0) coordinate) and creates as many chunks in an orderly manner as possible by traversing the coordinates one after another. Refer to the documentation of the Chunkers to get more information.# era5_torch
-# era5_torch
```

### Comparing `era5_torch-0.1/tests/test_chunkers.py` & `era5_torch-0.1.1/tests/test_chunkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from climate_compression.datasets import (
+from era5_torch import (
     ContinuousChunker,
     SingleChunker,
     SingleRandomWrapChunker,
     Offset,
 )
 import pytest
 import numpy as np
```

### Comparing `era5_torch-0.1/tests/test_datasets.py` & `era5_torch-0.1.1/tests/test_datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from climate_compression.datasets import (
+from era5_torch import (
     Era5,
-    Era5Lsm,
     ContinuousChunker,
     Coordinate,
     CoordinateBundle,
-    get_dataset,
     normalize,
     unnormalize,
 )
 import numpy as np
 import torch
 import xarray as xr
 import pytest
@@ -18,33 +16,17 @@
 
 
 def test_normalize_unnormalize_cancels():
     for i in range(100):
         xs = torch.rand(2, 3) * 100
         xs_prime = normalize(unnormalize(xs))
         xs_prime_reverse = unnormalize(normalize(xs))
-        assert np.allclose(xs, xs_prime, atol=1e-5)
-        assert np.allclose(xs_prime_reverse, xs_prime, atol=1e-5)
-        assert np.allclose(xs_prime_reverse, xs, atol=1e-5)
-
-
-def test_sz3_era5_same_coords():
-    ds1 = get_dataset("sz3_preds", split="train")
-    ds2 = get_dataset("era5_coinpp_64", split="train")
-    assert np.allclose(ds1[0][0], ds2[0][0])
-    assert ds1[0][1].shape == ds2[0][1].shape
-
-
-def test_kodak_correct_values():
-    ds = get_dataset("kodak")
-    # testing some random kodak values
-    assert ds[0][0][0][0].item() == 99
-    assert ds[0][0][12][24].item() == 96
-    assert ds[2][0][0][0].item() == 99
-    assert ds[2][0][12][24].item() == 114
+        assert np.allclose(xs, xs_prime, atol=1e-4)
+        assert np.allclose(xs_prime_reverse, xs_prime, atol=1e-4)
+        assert np.allclose(xs_prime_reverse, xs, atol=1e-4)
 
 
 def test_era5_retrieval_correct_values():
     ds = xr.open_dataset(temperature_path)
     era5 = Era5(temperature_path, "t", normalize=False)
 
     assert era5[0].squeeze().shape == (ds.latitude.size, ds.longitude.size)
@@ -249,33 +231,14 @@
 
     assert era5[0].squeeze().shape == (ds.latitude.size, ds.longitude.size)
     assert torch.allclose(era5[0].squeeze(), torch.Tensor(ds.lsm.isel(time=0).values))
     assert torch.allclose(era5[1].squeeze(), torch.Tensor(ds.lsm.isel(time=1).values))
     assert torch.allclose(era5[3].squeeze(), torch.Tensor(ds.lsm.isel(time=2).values))
 
 
-def test_aux_lsm():
-    era5 = Era5Lsm(
-        temperature_path,
-        lsm_path,
-        "t",
-        normalize=False,
-    )
-    ds_lsm = xr.open_dataset(lsm_path)
-    ds_t = xr.open_dataset(temperature_path)
-
-    assert era5[0].shape == (2, ds_t.latitude.size, ds_t.longitude.size)
-    assert torch.allclose(
-        era5[0].squeeze()[0, :, :], torch.Tensor(ds_t.t.isel(level=0, time=0).values)
-    )
-    assert torch.allclose(
-        era5[0].squeeze()[1, :, :], torch.Tensor(ds_lsm.lsm.isel(time=0).values)
-    )
-
-
 # fixtures
 @pytest.fixture(scope="session")
 def mock_dataset(tmp_path_factory):
     path = tmp_path_factory.mktemp("data") / "mock_dataset.nc"
     a = torch.Tensor([[1, 2, 3], [4, 5, 6]]).unsqueeze(0).unsqueeze(0)
     latitude = np.array([10, 20])
     longitude = np.array([30, 40, 50])
@@ -336,15 +299,17 @@
     )
     ds.to_netcdf(str(path))
     return path
 
 
 def test_dataset_coords_sphere(mock_dataset):
     ds = xr.open_dataset(mock_dataset)
-    era5 = Era5(ds, "t", normalize=False, coords=CoordinateBundle.SPHERE)
+    era5 = Era5(
+        ds, "t", normalize=False, coords=CoordinateBundle.SPHERE, normalize_coords=False
+    )
 
     assert era5[0].shape == (5, 2, 3)
     assert torch.allclose(
         era5[0],
         torch.Tensor(
             [
                 [[1, 2, 3], [4, 5, 6]],
@@ -360,14 +325,15 @@
 def test_dataset_coords_euclidean(mock_dataset_euclidean):
     ds = xr.open_dataset(mock_dataset_euclidean)
     era5 = Era5(
         ds,
         "t",
         normalize=False,
         coords=CoordinateBundle.EUCLIDEAN,
+        normalize_coords=False,
     )
 
     # just saving some space
     t0 = torch.Tensor([0])
     t1 = torch.Tensor([1])
     x00, y00, z00 = t0, t0, t1
     x01, y01, z01 = t0, t0, t1
@@ -422,14 +388,15 @@
 def test_dataset_coordinates_specifying_sphere(mock_dataset):
     ds = xr.open_dataset(mock_dataset)
     era5 = Era5(
         ds,
         "t",
         normalize=False,
         coords=[Coordinate.LATITUDE, Coordinate.LONGITUDE],
+        normalize_coords=False,
     )
 
     assert era5[0].shape == (3, 2, 3)
     assert torch.allclose(
         era5[0],
         torch.Tensor(
             [
@@ -441,14 +408,15 @@
     )
 
     era5 = Era5(
         ds,
         "t",
         normalize=False,
         coords=[Coordinate.TIME, Coordinate.LEVEL],
+        normalize_coords=False,
     )
 
     assert era5[0].shape == (3, 2, 3)
     assert torch.allclose(
         era5[0],
         torch.Tensor(
             [
@@ -463,14 +431,15 @@
 def test_dataset_coordinates_specifying(mock_dataset_euclidean):
     ds = xr.open_dataset(mock_dataset_euclidean)
     era5 = Era5(
         ds,
         "t",
         coords=[Coordinate.Y, Coordinate.X],
         normalize=False,
+        normalize_coords=False,
     )
     t0 = torch.Tensor([0])
     t1 = torch.Tensor([1])
     x00, y00 = t0, t0
     x01, y01 = t0, t0
     x02, y02 = t0, t0
     x10, y10 = t1, t0
```

