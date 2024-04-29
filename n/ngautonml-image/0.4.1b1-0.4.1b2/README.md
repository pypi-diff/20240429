# Comparing `tmp/ngautonml_image-0.4.1b1.tar.gz` & `tmp/ngautonml_image-0.4.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngautonml_image-0.4.1b1.tar", last modified: Thu Jan  4 16:49:49 2024, max compression
+gzip compressed data, was "ngautonml_image-0.4.1b2.tar", last modified: Mon Apr 29 18:58:15 2024, max compression
```

## Comparing `ngautonml_image-0.4.1b1.tar` & `ngautonml_image-0.4.1b2.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:49:49.389697 ngautonml_image-0.4.1b1/
--rw-r--r--   0 root         (0) root         (0)     4283 2024-01-04 16:49:49.389697 ngautonml_image-0.4.1b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3706 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:49:49.384698 ngautonml_image-0.4.1b1/ngautonml_image/
--rw-rw-rw-   0 root         (0) root         (0)     1055 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:49:49.387698 ngautonml_image-0.4.1b1/ngautonml_image/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/algorithms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4944 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/algorithms/sequential.py
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/algorithms/sequential_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:49:49.387698 ngautonml_image-0.4.1b1/ngautonml_image/dataset_formats/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/dataset_formats/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4064 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/dataset_formats/image_dir.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/dataset_formats/image_dir_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2382 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/examples_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:49:49.388697 ngautonml_image-0.4.1b1/ngautonml_image/splitters/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/splitters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1937 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/splitters/nop_splitter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:49:49.388697 ngautonml_image-0.4.1b1/ngautonml_image/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/ngautonml_image/templates/image_clf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:49:49.388697 ngautonml_image-0.4.1b1/ngautonml_image.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4283 2024-01-04 16:49:49.000000 ngautonml_image-0.4.1b1/ngautonml_image.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      715 2024-01-04 16:49:49.000000 ngautonml_image-0.4.1b1/ngautonml_image.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-04 16:49:49.000000 ngautonml_image-0.4.1b1/ngautonml_image.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      243 2024-01-04 16:49:49.000000 ngautonml_image-0.4.1b1/ngautonml_image.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-01-04 16:49:49.000000 ngautonml_image-0.4.1b1/ngautonml_image.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      933 2024-01-04 16:46:44.000000 ngautonml_image-0.4.1b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-01-04 16:49:49.389697 ngautonml_image-0.4.1b1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:15.098370 ngautonml_image-0.4.1b2/
+-rw-r--r--   0 root         (0) root         (0)     4283 2024-04-29 18:58:15.098370 ngautonml_image-0.4.1b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3706 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:15.094370 ngautonml_image-0.4.1b2/ngautonml_image/
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:15.095370 ngautonml_image-0.4.1b2/ngautonml_image/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/algorithms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5069 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/algorithms/sequential.py
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/algorithms/sequential_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:15.096370 ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4201 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/image_tensor_data_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/image_tensor_data_loader_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:15.097370 ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/impl/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/impl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/impl/image_tensor_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/impl/image_tensor_params_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/examples_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:15.097370 ngautonml_image-0.4.1b2/ngautonml_image/splitters/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/splitters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/splitters/nop_splitter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:15.098370 ngautonml_image-0.4.1b2/ngautonml_image/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/ngautonml_image/templates/image_clf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:15.098370 ngautonml_image-0.4.1b2/ngautonml_image.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4283 2024-04-29 18:58:15.000000 ngautonml_image-0.4.1b2/ngautonml_image.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-29 18:58:15.000000 ngautonml_image-0.4.1b2/ngautonml_image.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 18:58:15.000000 ngautonml_image-0.4.1b2/ngautonml_image.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2024-04-29 18:58:15.000000 ngautonml_image-0.4.1b2/ngautonml_image.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-29 18:58:15.000000 ngautonml_image-0.4.1b2/ngautonml_image.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-29 18:54:58.000000 ngautonml_image-0.4.1b2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-29 18:58:15.098370 ngautonml_image-0.4.1b2/setup.cfg
```

### Comparing `ngautonml_image-0.4.1b1/PKG-INFO` & `ngautonml_image-0.4.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngautonml_image
-Version: 0.4.1b1
+Version: 0.4.1b2
 Summary: a plugin that installs image processing tools for ngAutonML
 Author-email: "L.H. Piggy Yarroll" <piggy@cmu.edu>, Merritt Kowaleski <merrittk@cmu.edu>, Andrew Williams <awillia2@andrew.cmu.edu>, Jieshi Chen <jieshic@andrew.cmu.edu>
 Keywords: machine learning,image processing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
```

### Comparing `ngautonml_image-0.4.1b1/README.md` & `ngautonml_image-0.4.1b2/README.md`

 * *Files identical despite different names*

### Comparing `ngautonml_image-0.4.1b1/ngautonml_image/__init__.py` & `ngautonml_image-0.4.1b2/ngautonml_image/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def algorithms_make_catalog(**kwargs) -> Catalog:
     '''Make the plugin algorithms catalog.'''
     return PathedCatalog([Path(__file__).parent / 'algorithms'], **kwargs)
 
 
-def dataset_formats_make_catalog(**kwargs) -> Catalog:
-    '''Make the plugin dataset formats catalog.'''
-    return PathedCatalog([Path(__file__).parent / 'dataset_formats'], **kwargs)
+def data_loaders_make_catalog(**kwargs) -> Catalog:
+    '''Make the plugin data_loaders catalog.'''
+    return PathedCatalog([Path(__file__).parent / 'data_loaders'], **kwargs)
 
 
 def splitters_make_catalog(**kwargs) -> Catalog:
     '''Make the plugin splitters catalog.'''
     return PathedCatalog([Path(__file__).parent / 'splitters'], **kwargs)
```

### Comparing `ngautonml_image-0.4.1b1/ngautonml_image/algorithms/sequential.py` & `ngautonml_image-0.4.1b2/ngautonml_image/algorithms/sequential.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,41 +28,43 @@
     _class_names: List[str]
     _impl: Optional[tf.keras.Sequential]
 
     def __init__(self, **overrides: Any):
         parent = overrides.pop('parent')
         self._constructor = tf.keras.Sequential
         super().__init__(parent=parent)
-        self._hyperparams = self._algorithm.hyperparams(**overrides)
+        self._hyperparams = self.algorithm.hyperparams(**overrides)
         self._impl = None
 
     def hyperparams(self, **overrides) -> Dict[str, Any]:
         '''Report hyperparams with the ability to override them.'''
         retval = self._hyperparams.copy()
         retval.update(overrides)
         return retval
 
     def _mk_model(self, **overrides) -> tf.keras.Sequential:
-        params = self._algorithm.hyperparams(**overrides)
+        params = self.algorithm.hyperparams(**overrides)
         print(params)
         return tf.keras.Sequential([
             layers.Rescaling(1. / 255, input_shape=(params['img_height'], params['img_width'], 3)),
             layers.Conv2D(16, 3, padding='same', activation='relu'),
             layers.MaxPooling2D(),
             layers.Conv2D(32, 3, padding='same', activation='relu'),
             layers.MaxPooling2D(),
             layers.Conv2D(64, 3, padding='same', activation='relu'),
             layers.MaxPooling2D(),
             layers.Flatten(),
             layers.Dense(128, activation='relu'),
             layers.Dense(params['num_classes'])
         ])
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         '''Fit the model.'''
+        if dataset is None:
+            return
         params = self.hyperparams()
         train_ds = dataset[DatasetKeys.KERAS_DS.value]
         assert isinstance(train_ds, tf.data.Dataset)
         val_ds = dataset[DatasetKeys.KERAS_VALIDATE.value]
         assert isinstance(val_ds, tf.data.Dataset)
 
         self._class_names = train_ds.class_names
@@ -79,18 +81,21 @@
 
         # unsure why this was in a try/except
         self._impl.fit(train_ds,
                        validation_data=val_ds,
                        epochs=epochs)
         self._trained = True
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         # TODO(Merritt): we should get train predictions somehow
         if not self._trained:
-            raise UntrainedError(f'attempt to predict before fit for {self._algorithm.name}')
+            raise UntrainedError(f'attempt to predict before fit for {self.catalog_name}')
+
+        if dataset is None:
+            return None
 
         assert self._impl is not None
 
         predictions = self._impl.predict(dataset[DatasetKeys.KERAS_DS.value])
         assert isinstance(predictions, np.ndarray)
         scores: Iterable[tf.Tensor] = tf.nn.softmax(predictions)
         prediction_result: List[str] = [self._class_names[np.argmax(score)] for score in scores]
```

### Comparing `ngautonml_image-0.4.1b1/ngautonml_image/algorithms/sequential_test.py` & `ngautonml_image-0.4.1b2/ngautonml_image/algorithms/sequential_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml_image-0.4.1b1/ngautonml_image/dataset_formats/image_dir_test.py` & `ngautonml_image-0.4.1b2/ngautonml_image/data_loaders/image_tensor_data_loader_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,55 +2,67 @@
 
 import math
 from pathlib import Path
 
 # pylint: disable=no-name-in-module
 from tensorflow.python.data.ops.dataset_ops import BatchDataset  # type: ignore[import]
 
-from .image_dir import ImageDirDatasetFormat
+from ngautonml.config_components.dataset_config import DatasetConfig
+
+from .image_tensor_data_loader import ImageTensorDataLoader
 
 
 NUM_IMAGES = 3665
 
 MINIMAL_CLAUSE = {
     'config': 'image_dir',
-    'train_dir': str(Path(__file__).parents[4] / 'examples' / 'flowers' / 'train')
+    'params': {
+        'train_dir': str(Path(__file__).parents[4] / 'examples' / 'flowers' / 'train')
+    }
 }
 
 
 def test_defaults() -> None:
     '''Test that default parameters get applied when not specified.'''
-    dut = ImageDirDatasetFormat().build(MINIMAL_CLAUSE)
-    got = dut.load_train()['keras_ds']
+    config = DatasetConfig(MINIMAL_CLAUSE)
+    dut = ImageTensorDataLoader(config)
+    dataset = dut.load_train()
+    assert dataset is not None
+    got = dataset['keras_ds']
     assert isinstance(got, BatchDataset)
     assert got.class_names == ['daisy', 'dandelion', 'roses', 'sunflowers', 'tulips']
     for image_batch, _ in got:
         # shape tuple is (batch_size, img_height, img_width, _)
         assert image_batch.shape == (32, 128, 128, 3)
         break
     want_val_split = 1 - 0.2
     num_images_got = len([1 for _ in got.unbatch()])
     num_images_want = math.floor(NUM_IMAGES * want_val_split)
     assert num_images_got == num_images_want
 
 
 OVERRIDE_CLAUSE = {
     'config': 'image_dir',
-    'train_dir': str(Path(__file__).parents[4] / 'examples' / 'flowers' / 'train'),
-    'validation_split': 0.6,
-    'img_height': 2,
-    'img_width': 8,
-    'batch_size': 10
+    'params': {
+        'train_dir': str(Path(__file__).parents[4] / 'examples' / 'flowers' / 'train'),
+        'validation_split': 0.6,
+        'img_height': 2,
+        'img_width': 8,
+        'batch_size': 10
+    }
 }
 
 
 def test_overrides() -> None:
     '''Test that overridden parameters get properly applied.'''
-    dut = ImageDirDatasetFormat().build(OVERRIDE_CLAUSE)
-    got = dut.load_train()['keras_ds']
+    config = DatasetConfig(OVERRIDE_CLAUSE)
+    dut = ImageTensorDataLoader(config=config)
+    dataset = dut.load_train()
+    assert dataset is not None
+    got = dataset['keras_ds']
     assert isinstance(got, BatchDataset)
     for image_batch, _ in got:
         # shape tuple is (batch_size, img_height, img_width, _)
         assert image_batch.shape == (10, 2, 8, 3)
         break
     want_val_split = 1 - 0.6
     num_images_got = len([1 for _ in got.unbatch()])
```

### Comparing `ngautonml_image-0.4.1b1/ngautonml_image/examples_test.py` & `ngautonml_image-0.4.1b2/ngautonml_image/examples_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def flowers_config():
     train_dir = module_path() / 'examples' / 'flowers' / 'train'
     test_dir = module_path() / 'examples' / 'flowers' / 'test'
     pdef = {
         "dataset": {
-            "config": "image_dir",
+            "config": "image_tensor",
             "train_dir": train_dir,
             "test_dir": test_dir
         },
         "problem_type": {
             "data_type": "IMAGE",
             "task": "MULTICLASS_CLASSIFICATION"
         },
```

### Comparing `ngautonml_image-0.4.1b1/ngautonml_image/splitters/nop_splitter.py` & `ngautonml_image-0.4.1b2/ngautonml_image/splitters/nop_splitter.py`

 * *Files identical despite different names*

### Comparing `ngautonml_image-0.4.1b1/ngautonml_image/templates/image_clf.py` & `ngautonml_image-0.4.1b2/ngautonml_image/templates/image_clf.py`

 * *Files identical despite different names*

### Comparing `ngautonml_image-0.4.1b1/ngautonml_image.egg-info/PKG-INFO` & `ngautonml_image-0.4.1b2/ngautonml_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngautonml_image
-Version: 0.4.1b1
+Version: 0.4.1b2
 Summary: a plugin that installs image processing tools for ngAutonML
 Author-email: "L.H. Piggy Yarroll" <piggy@cmu.edu>, Merritt Kowaleski <merrittk@cmu.edu>, Andrew Williams <awillia2@andrew.cmu.edu>, Jieshi Chen <jieshic@andrew.cmu.edu>
 Keywords: machine learning,image processing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
```

### Comparing `ngautonml_image-0.4.1b1/pyproject.toml` & `ngautonml_image-0.4.1b2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngautonml_image"
-version = "0.4.1b01"
+version = "0.4.1b02"
 description = "a plugin that installs image processing tools for ngAutonML"
 authors = [
     {name = "L.H. Piggy Yarroll", email = "piggy@cmu.edu"},
     {name = "Merritt Kowaleski", email = "merrittk@cmu.edu"},
     {name = "Andrew Williams", email = "awillia2@andrew.cmu.edu"},
     {name = "Jieshi Chen", email = "jieshic@andrew.cmu.edu"},
 ]
@@ -16,9 +16,9 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Typing :: Typed"
 ]
 
 [project.entry-points."ngautonml.make_catalog"]
 templates = "ngautonml_image:templates_make_catalog"
 algorithms = "ngautonml_image:algorithms_make_catalog"
-dataset_formats = "ngautonml_image:dataset_formats_make_catalog"
-splitters = "ngautonml_image:splitters_make_catalog"
+splitters = "ngautonml_image:splitters_make_catalog"
+data_loaders = "ngautonml_image:data_loaders_make_catalog"
```

