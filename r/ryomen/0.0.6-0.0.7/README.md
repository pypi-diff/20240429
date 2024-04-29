# Comparing `tmp/ryomen-0.0.6.tar.gz` & `tmp/ryomen-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryomen-0.0.6.tar", last modified: Thu Apr 25 17:32:22 2024, max compression
+gzip compressed data, was "ryomen-0.0.7.tar", last modified: Mon Apr 29 15:31:31 2024, max compression
```

## Comparing `ryomen-0.0.6.tar` & `ryomen-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-25 17:32:22.216184 ryomen-0.0.6/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1064 2024-04-16 15:51:46.000000 ryomen-0.0.6/LICENSE
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5929 2024-04-25 17:32:22.216283 ryomen-0.0.6/PKG-INFO
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-25 17:32:22.214443 ryomen-0.0.6/ryomen/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       31 2024-04-15 17:56:53.000000 ryomen-0.0.6/ryomen/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    23926 2024-04-25 17:32:01.000000 ryomen-0.0.6/ryomen/main.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-25 17:32:22.215658 ryomen-0.0.6/ryomen.egg-info/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5929 2024-04-25 17:32:22.000000 ryomen-0.0.6/ryomen.egg-info/PKG-INFO
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      226 2024-04-25 17:32:22.000000 ryomen-0.0.6/ryomen.egg-info/SOURCES.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-25 17:32:22.000000 ryomen-0.0.6/ryomen.egg-info/dependency_links.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        7 2024-04-25 17:32:22.000000 ryomen-0.0.6/ryomen.egg-info/top_level.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-16 13:55:45.000000 ryomen-0.0.6/ryomen.egg-info/zip-safe
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      260 2024-04-25 17:32:22.216585 ryomen-0.0.6/setup.cfg
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      396 2024-04-16 14:03:09.000000 ryomen-0.0.6/setup.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-25 17:32:22.215922 ryomen-0.0.6/tests/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    11642 2024-04-25 17:02:33.000000 ryomen-0.0.6/tests/test_ryomen.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-29 15:31:31.561542 ryomen-0.0.7/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1064 2024-04-16 15:51:46.000000 ryomen-0.0.7/LICENSE
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     6118 2024-04-29 15:31:31.561646 ryomen-0.0.7/PKG-INFO
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5810 2024-04-25 19:14:54.000000 ryomen-0.0.7/README.md
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-29 15:31:31.560246 ryomen-0.0.7/ryomen/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       68 2024-04-25 18:23:48.000000 ryomen-0.0.7/ryomen/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    24369 2024-04-29 15:30:00.000000 ryomen-0.0.7/ryomen/main.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-29 15:31:31.560947 ryomen-0.0.7/ryomen.egg-info/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     6118 2024-04-29 15:31:31.000000 ryomen-0.0.7/ryomen.egg-info/PKG-INFO
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      274 2024-04-29 15:31:31.000000 ryomen-0.0.7/ryomen.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-29 15:31:31.000000 ryomen-0.0.7/ryomen.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       13 2024-04-29 15:31:31.000000 ryomen-0.0.7/ryomen.egg-info/top_level.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-16 13:55:45.000000 ryomen-0.0.7/ryomen.egg-info/zip-safe
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      260 2024-04-29 15:31:31.561943 ryomen-0.0.7/setup.cfg
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      396 2024-04-16 14:03:09.000000 ryomen-0.0.7/setup.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-29 15:31:31.561402 ryomen-0.0.7/tests/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 17:55:35.000000 ryomen-0.0.7/tests/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      751 2024-04-29 15:29:43.000000 ryomen-0.0.7/tests/playground.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    11642 2024-04-25 17:02:33.000000 ryomen-0.0.7/tests/test_ryomen.py
```

### Comparing `ryomen-0.0.6/LICENSE` & `ryomen-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ryomen-0.0.6/PKG-INFO` & `ryomen-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryomen
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ryomen
 Home-page: https://github.com/buswinka/ryomen
 Author: Chris Buswinka
 Author-email: buswinka@g.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 
 
 ### Why do we need this?
 
 Modern microscopes can image cells, tissue, or whatever else, over huge spatial areas, resulting in images that can be
 quite large (hundreds of gigabytes). This can make applying image processing or deep learning algorithms difficult. 
 Ryomen makes this easy by automatically slicing up large images and providing an easy-to-use interface for working with the
-crops. Ryomen is powerful when paired with 
+crops. Check out the docs here: https://ryomen.readthedocs.io/
 
 ### What can it do? 
 
 Ryomen works with N dimensional, arbitrary array types, including numpy, zarr, pytorch, or anything else. It simplifies
 the process of slicing large images, with slices that may overlap, applying a function to the image, and extracting the
 non-overlapping subregions. First, install with pip: ```pip install ryomen```. The following example crops a large ```image``` into 512x512 crops overlapping by 64px, aplies a hard to run
 function ```expensive_fn```, and takes the result and puts it into a pre-allocated ```output``` array.
@@ -157,14 +157,19 @@
     # Slot the batched crop into an output array, excluding the overlap
     for b, (_source, _destination) in enumerate(zip(source, destination)):
         output[_destination] = crop[b, ...][_source]  
 ```
 
 ### Change Log
 
+#### 0.0.6
+    - fixed bug where leading dimensions break the slicer when padding is applied
+    - changed padding to be on by default
+    - refactored for code clarity
+
 
 #### 0.0.5
     - fixed bug with duplicate indices being shown, leading to redundant behaviro
     - added support for zarr arrays, as they do not implement a flip method or support negative indexing
     - refactored for readability
 
 #### 0.0.4
```

### Comparing `ryomen-0.0.6/ryomen/main.py` & `ryomen-0.0.7/ryomen/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,49 +5,55 @@
     Tuple,
     Callable,
     List,
     Any,
     Iterator,
     Generator,
     Union,
+    NewType
 )
 from copy import copy, deepcopy
 
 Shape = Sequence[int]
 Index = Tuple[Union[type(Ellipsis), slice], ...]
 SliceList = List[Union[type(Ellipsis), slice]]
 
 
 class TensorLike:
-    """ generic class for any tensor like object: zarr, numpy, pytorch, etc... """
+    """ Any array type that matches this signature will work with ryomen. Tested include: zarr, numpy, pytorch... """
 
     shape: Shape
 
     def __init__(self):
         ...
 
     def __getitem__(self, item: Any) -> TensorLike:
+        """ Required Method """
         ...
 
     def __setitem__(self, index: Any, item: Any) -> TensorLike:
+        """ Required Method """
         ...
 
     def __iter__(self) -> Iterator:
+        """ Required Method"""
         ...
 
     def __next__(self) -> TensorLike:
         ...
 
     def __mul__(self, other) -> TensorLike:
         ...
 
     def size(self) -> Shape:
+        """ Required Method """
         ...
 
     def flip(self, dim: int) -> TensorLike:
+        """ not necessary if tensor supports negative strides """
         ...
 
 
 def default_collate(x: Sequence[TensorLike]) -> TensorLike | Sequence[TensorLike]:
     return x
 
 
@@ -124,28 +130,29 @@
         >>> for crop, index = Slicer(image, crop_size, overlap, batch_size=8, collate=collate, output_transform=normalize)
         >>>     print(crop.shape)  # [8, 3, 10, 10, 10]
 
         :param image: N Dimensional Array of any type
         :param crop_size: Tuple ints for cropping dimensions
         :param overlap: Tuple of ints for the overlap between crops
         :param batch_size: batch size of crops. Allows for returning multiple crops in one iteration
-        :param pad: pads the image by overlap if true. Only supported if input tensor implements a flip method.
+        :param pad: pads the image by reflection if true. Only supported if input tensor implements a flip method.
         :param output_transform: function to apply to each crop before returning
         :param collate: function to collate images, the default behavior is to return a list of crops
         :param progress_bar: function which wraps the iteration and displays a progress bar. (e.g. tqdm)
         """
 
         self.__N = None
         self.__image: TensorLike = image
         self.__crop_size = list(crop_size)
         self.__overlap = list(overlap)
         self.__batch_size = batch_size
         self.__output_fn = output_transform
         self.__collate_fn = collate
         self.__progress_bar = progress_bar
+        self.__crop_cache = None
 
         # Default, is changed to value of pad after suitable checks
         self.__can_pad = False
 
         # Default, is changed to true after suitable checks
         self.__support_negative_strides = False
 
@@ -360,39 +367,39 @@
 
         # init a list of zeros as the "first" crop location
         x = [-o if pad else 0 for _, o in zip(crop, overlap)]
         assert len(shape) >= len(crop)
 
         # We cache all previous indices here, as the cost of looking this up
         # is presumably less than the cost of re-running the expensive fn
-        previously_yeilded = []
+        previously_yielded = set()
 
         # copy because lists are mutable -- we need to mutate it in this scope but not the higher one...
         shape = copy(list(shape))
 
         # Leading dimensions are allowed, therefore we pop off all leading dimensions until the shape
         # and crop shape are the same!
         while len(shape) > len(crop):
             shape.pop(0)
 
         ind, x = self._get_next_slice(x, crop, overlap, shape, pad)
         while not all((a + c) > b + (o * pad) for a, b, c, o in zip(x, shape, crop, overlap)):
-            if str(ind) not in previously_yeilded:
-                previously_yeilded.append(str(ind))
+            if str(ind) not in previously_yielded:
+                previously_yielded.add(str(ind))
                 yield ind, x
 
             ind, x = self._get_next_slice(x, crop, overlap, shape, pad)
 
-        if str(ind) not in previously_yeilded:
-            previously_yeilded.append(str(ind))
+        if str(ind) not in previously_yielded:
+            previously_yielded.add(str(ind))
             yield ind, x
 
         ind, x = self._get_next_slice(x, crop, overlap, shape, pad)
-        if str(ind) not in previously_yeilded:
-            previously_yeilded.append(str(ind))
+        if str(ind) not in previously_yielded:
+            previously_yielded.add(str(ind))
             yield ind, x
 
     def _flush_output(
             self, output_cache
     ) -> Tuple[
         TensorLike | Sequence[TensorLike],
         Index | Sequence[Index],
@@ -415,15 +422,14 @@
 
         if is_list and all_same_size:
             return images[0], sources[0], destinations[0]
 
         else:
             return images, sources, destinations
 
-
     @staticmethod
     def _minmax(a: slice, m: int) -> slice:
         """ utility function to clamp a slice between 0 and m """
 
         if a.start < 0:
             delta = abs(a.start)
             a = slice(a.start + delta, a.stop + delta, a.step)
@@ -477,22 +483,27 @@
                 padding_necessary = True
 
         if not padding_necessary:
             return self.__image[index]
 
         # We have a problem! We need a library agnostic way to create a tensor
         # We can do this by indexing another part of the tensor, and doing a deepcopy.
-        _output_index, _ = self._get_next_slice(
-            [0 for _ in self.__crop_size],
-            c=self.__crop_size,
-            o=self.__overlap,
-            shape=shape,
-            pad=False,
-        )
-        output_array = self.__image[_output_index] * 0  # zeros the array
+        if self.__crop_cache is None:
+            _output_index, _ = self._get_next_slice(
+                [0 for _ in self.__crop_size],
+                c=self.__crop_size,
+                o=self.__overlap,
+                shape=shape,
+                pad=False,
+            )
+            output_array = self.__image[_output_index] * 0  # zeros the array
+            self.__crop_cache = output_array
+        else:
+            output_array = self.__crop_cache
+
         first_access = False
 
         n_leading_dimensions = len(shape) - len(self.__crop_size)
         for i, (ind, s, o) in enumerate(zip(modified_index, shape, self.__overlap)):
 
             padding_source: SliceList = [Ellipsis]
             other_source: SliceList = [Ellipsis]
@@ -591,8 +602,7 @@
 
             # If we've added more to the output cache than the batch size, we flush the batch away
             if len(output_cache) == self.__batch_size:
                 yield self._flush_output(output_cache)
 
         if len(output_cache) > 0:
             yield self._flush_output(output_cache)
-
```

### Comparing `ryomen-0.0.6/ryomen.egg-info/PKG-INFO` & `ryomen-0.0.7/ryomen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryomen
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ryomen
 Home-page: https://github.com/buswinka/ryomen
 Author: Chris Buswinka
 Author-email: buswinka@g.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 
 
 ### Why do we need this?
 
 Modern microscopes can image cells, tissue, or whatever else, over huge spatial areas, resulting in images that can be
 quite large (hundreds of gigabytes). This can make applying image processing or deep learning algorithms difficult. 
 Ryomen makes this easy by automatically slicing up large images and providing an easy-to-use interface for working with the
-crops. Ryomen is powerful when paired with 
+crops. Check out the docs here: https://ryomen.readthedocs.io/
 
 ### What can it do? 
 
 Ryomen works with N dimensional, arbitrary array types, including numpy, zarr, pytorch, or anything else. It simplifies
 the process of slicing large images, with slices that may overlap, applying a function to the image, and extracting the
 non-overlapping subregions. First, install with pip: ```pip install ryomen```. The following example crops a large ```image``` into 512x512 crops overlapping by 64px, aplies a hard to run
 function ```expensive_fn```, and takes the result and puts it into a pre-allocated ```output``` array.
@@ -157,14 +157,19 @@
     # Slot the batched crop into an output array, excluding the overlap
     for b, (_source, _destination) in enumerate(zip(source, destination)):
         output[_destination] = crop[b, ...][_source]  
 ```
 
 ### Change Log
 
+#### 0.0.6
+    - fixed bug where leading dimensions break the slicer when padding is applied
+    - changed padding to be on by default
+    - refactored for code clarity
+
 
 #### 0.0.5
     - fixed bug with duplicate indices being shown, leading to redundant behaviro
     - added support for zarr arrays, as they do not implement a flip method or support negative indexing
     - refactored for readability
 
 #### 0.0.4
```

### Comparing `ryomen-0.0.6/tests/test_ryomen.py` & `ryomen-0.0.7/tests/test_ryomen.py`

 * *Files identical despite different names*

