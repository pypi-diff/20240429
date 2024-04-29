# Comparing `tmp/dataset_iterator-0.4.1.tar.gz` & `tmp/dataset_iterator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_iterator-0.4.1.tar", last modified: Tue Apr 23 08:09:09 2024, max compression
+gzip compressed data, was "dataset_iterator-0.4.2.tar", last modified: Mon Apr 29 15:50:22 2024, max compression
```

## Comparing `dataset_iterator-0.4.1.tar` & `dataset_iterator-0.4.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:09:09.088481 dataset_iterator-0.4.1/dataset_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/concat_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/dataset_iterator/datasetIO/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/concatenate_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/group_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/h5pyIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/memoryIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/multiple_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/multiple_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/hard_sample_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/image_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/index_array_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57974 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/multichannel_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/ordered_enqueuer_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/tile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/tracking_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/dataset_iterator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/dataset_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/concat_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/dataset_iterator/datasetIO/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/concatenate_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/group_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/h5pyIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/memoryIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/multiple_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/multiple_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/hard_sample_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/image_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/index_array_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58005 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/multichannel_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/ordered_enqueuer_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/tile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/tracking_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/dataset_iterator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/setup.py
```

### Comparing `dataset_iterator-0.4.1/LICENSE.txt` & `dataset_iterator-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/PKG-INFO` & `dataset_iterator-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.1
+Version: 0.4.2
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.1/dataset_iterator-0.4.1.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.2/dataset_iterator-0.4.2.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.1/README.md` & `dataset_iterator-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/__init__.py` & `dataset_iterator-0.4.2/dataset_iterator/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/concat_iterator.py` & `dataset_iterator-0.4.2/dataset_iterator/concat_iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,24 +97,31 @@
         index_array -= self.it_off[it_idx] # remove ds offset to each index
         return it_idx
 
     def set_allowed_indexes(self, indexes):
         raise NotImplementedError("Not supported yet")
 
     def close(self):
-        self._close_datasetIO()
+        for it in self.iterators:
+            it.close()
 
     def _close_datasetIO(self):
         for it in self.iterators:
             it._close_datasetIO()
 
+
     def _open_datasetIO(self):
         for it in self.iterators:
             it._open_datasetIO()
 
+
+    def open(self):
+        for it in self.iterators:
+            it.open()
+
     def disable_random_transforms(self, data_augmentation:bool=True, channels_postprocessing:bool=False):
         return [it.disable_random_transforms(data_augmentation, channels_postprocessing) for it in self.iterators]
 
     def enable_random_transforms(self, parameters):
         for it, params in zip(self.iterators, parameters):
             it.enable_random_transforms(params)
```

### Comparing `dataset_iterator-0.4.1/dataset_iterator/datasetIO/concatenate_datasetIO.py` & `dataset_iterator-0.4.2/dataset_iterator/datasetIO/concatenate_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/datasetIO/datasetIO.py` & `dataset_iterator-0.4.2/dataset_iterator/datasetIO/datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/datasetIO/group_datasetIO.py` & `dataset_iterator-0.4.2/dataset_iterator/datasetIO/group_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/datasetIO/h5pyIO.py` & `dataset_iterator-0.4.2/dataset_iterator/datasetIO/h5pyIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/datasetIO/multiple_datasetIO.py` & `dataset_iterator-0.4.2/dataset_iterator/datasetIO/multiple_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/datasetIO/multiple_fileIO.py` & `dataset_iterator-0.4.2/dataset_iterator/datasetIO/multiple_fileIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/hard_sample_mining.py` & `dataset_iterator-0.4.2/dataset_iterator/hard_sample_mining.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,34 +36,39 @@
     def close(self):
         self.enq.stop()
         if self.data_aug_param is not None:
             self.iterator.enable_random_transforms(self.data_aug_param)
         self.iterator.close()
 
     def on_epoch_begin(self, epoch, logs=None):
-        self.wait_for_me.clear() # will block
+        if self.proba_per_metric is not None:
+            self.wait_for_me.clear() # will block
 
     def on_epoch_end(self, epoch, logs=None):
-        if self.period==1 or (epoch + 1 + self.start_epoch) % self.period == 0:
-            if (epoch > 0 or not self.skip_first) and epoch + self.start_epoch >= self.start_from_epoch:
+        if self.period == 1 or (epoch + 1 + self.start_epoch) % self.period == 0:
+            if (epoch > 0 or not self.skip_first) and epoch + 1 + self.start_epoch >= self.start_from_epoch:
+                self.target_iterator.close()
+                self.iterator.open()
                 metrics = self.compute_metrics()
+                self.iterator.close()
+                self.target_iterator.open()
                 first = self.proba_per_metric is None
                 self.proba_per_metric = get_index_probability(metrics, enrich_factor=self.enrich_factor, quantile_max=self.quantile_max, quantile_min=self.quantile_min, verbose=self.verbose)
                 self.n_metrics = self.proba_per_metric.shape[0] if len(self.proba_per_metric.shape) == 2 else 1
                 if first and self.n_metrics > self.period:
                     warnings.warn(f"Hard sample mining period = {self.period} should be greater than metric number = {self.n_metrics}")
         if self.proba_per_metric is not None:
             if len(self.proba_per_metric.shape) == 2:
                 self.metric_idx = (self.metric_idx + 1) % self.n_metrics
                 proba = self.proba_per_metric[self.metric_idx]
             else:
                 proba = self.proba_per_metric
             # set probability to iterator in case of multiprocessing iwth OrderedEnqueeur this will be taken into account only a next epoch has iterator has already been sent to processes at this stage
             self.target_iterator.set_index_probability(proba)
-        self.wait_for_me.set() # release block
+            self.wait_for_me.set() # release block
 
     def on_train_end(self, logs=None):
         self.close()
 
     def compute_metrics(self):
         workers = os.cpu_count() if self.workers is None else self.workers
         self.enq.start(workers=workers, max_queue_size=max(2, min(self.n_batches, workers)))
```

### Comparing `dataset_iterator-0.4.1/dataset_iterator/helpers.py` & `dataset_iterator-0.4.2/dataset_iterator/helpers.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/image_data_generator.py` & `dataset_iterator-0.4.2/dataset_iterator/image_data_generator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/index_array_iterator.py` & `dataset_iterator-0.4.2/dataset_iterator/index_array_iterator.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,23 @@
 
     def get_batch_size(self):
         return self.batch_size
 
     def set_index_probability(self, value):
         self.index_probability = value
 
+
+    def open(self):
+        pass
+
+
+    def close(self):
+        pass
+
+
     def __len__(self):
         if self.step_number > 0:
             return self.step_number
         if self.incomplete_last_batch_mode == 2:
             return max(1, self.n // self.batch_size)
         else:
             return (self.n + self.batch_size - 1) // self.batch_size  # round up
```

### Comparing `dataset_iterator-0.4.1/dataset_iterator/multichannel_iterator.py` & `dataset_iterator-0.4.2/dataset_iterator/multichannel_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,34 +224,34 @@
         self.channels_postprocessing_function=channels_postprocessing_function
         self.extract_tile_function=extract_tile_function
         self.paths=None
         self.group_map_paths=None
         self.return_image_index=return_image_index
         self._open_datasetIO()
         # check that all ds have compatible length between input and output
-        indexes = np.array([ds.shape[0] for ds in self.ds_array[0]])
+        indexes = np.array([len(ds) for ds in self.ds_array[0]])
         if len(channel_keywords)>1:
             for c, ds_l in enumerate(self.ds_array):
                 if self.channel_keywords[c] is not None:
                     singleton = c in self.singleton_channels
                     if len(self.ds_array[0])!=len(ds_l):
                         raise ValueError('Channels {}({}) has #{} datasets whereas first channel has #{} datasets'.format(c, channel_keywords[c], len(ds_l), len(self.ds_array[0])))
                     for ds_idx, ds in enumerate(ds_l):
                         if singleton:
-                            if ds.shape[0]!=1:
+                            if len(ds)!=1:
                                 raise ValueError("Channel {} is set as singleton but one dataset has more that one image".format(c))
-                        elif indexes[ds_idx] != ds.shape[0]:
+                        elif indexes[ds_idx] != len(ds):
                             raise ValueError('Channel {}({}) has at least one dataset with number of elements that differ from Channel 0'.format(c, channel_keywords[c]))
         if len(array_keywords)>1: # check that all array ds have compatible length
             for c, ds_l in enumerate(self.ads_array):
                 if self.array_keywords[c] is not None:
                     if len(self.ds_array[0])!=len(ds_l):
                         raise ValueError('Array {}({}) has #{} datasets whereas first channel has #{} datasets'.format(c, channel_keywords[c], len(ds_l), len(self.ds_array[0])))
                     for ds_idx, ds in enumerate(ds_l):
-                        if indexes[ds_idx] != ds.shape[0]:
+                        if indexes[ds_idx] != len(ds):
                             raise ValueError('Array {}({}) has at least one dataset with number of elements that differ from Channel 0'.format(c, channel_keywords[c]))
         # get offset for each dataset
         for i in range(1, len(indexes)):
             indexes[i]=indexes[i-1]+indexes[i]
         self.ds_len=indexes
         self.ds_off=np.insert(self.ds_len[:-1], 0, 0)
         # get offset for each group of dataset
@@ -277,15 +277,15 @@
         try:
             label_path = [replace_last(path, self.channel_keywords[0], '/labels') for path in self.paths]
             self.labels = [self.datasetIO.get_dataset(path) if path in self.datasetIO else None for path in label_path]
             for i, ds in enumerate(self.labels):
                 self.labels[i] = np.char.asarray(ds[()].astype('unicode')) # todo: check if necessary to convert to char array ? unicode is necessary
             if len(self.labels)!=len(self.ds_array[0]):
                 raise ValueError('Invalid input file: number of label array differ from dataset number')
-            if any(len(self.labels[i].shape)==0 or self.labels[i].shape[0]!=self.ds_array[0][i].shape[0] for i in range(len(self.labels))):
+            if any(len(self.labels[i].shape)==0 or len(self.labels[i]) != len(self.ds_array[0][i]) for i in range(len(self.labels))):
                 raise ValueError('Invalid input file: at least one dataset has element numbers that differ from corresponding label array')
         except:
             self.labels = None
 
         if not memory_persistant:
             self._close_datasetIO()
         self.void_mask_proportion = void_mask_proportion
@@ -317,14 +317,18 @@
         # get all matching dataset
         self.ds_array = [ [self.datasetIO.get_dataset(self._get_dataset_path(c, ds_idx)) for ds_idx in range(len(self.paths))] if self.channel_keywords[c] is not None else None for c in range(len(self.channel_keywords))]
         self.ads_array = [ [self.datasetIO.get_dataset(self._get_dataset_path(c, ds_idx, is_array=True)) for ds_idx in range(len(self.paths))] if self.array_keywords[c] is not None else None for c in range(len(self.array_keywords))]
         getAttribute = lambda a, def_val : def_val if a is None else (a[0] if isinstance(a, list) else a)
         self.ds_scaling_center = [[getAttribute(self.datasetIO.get_attribute(self._get_dataset_path(c, ds_idx), "scaling_center"), 0) for ds_idx in range(len(self.paths))]  if self.channel_keywords[c] is not None else None for c in range(len(self.channel_keywords))]
         self.ds_scaling_factor = [[getAttribute(self.datasetIO.get_attribute(self._get_dataset_path(c, ds_idx), "scaling_factor"), 1) for ds_idx in range(len(self.paths))]  if self.channel_keywords[c] is not None else None for c in range(len(self.channel_keywords))]
 
+    def open(self):
+        self._open_datasetIO()
+
+
     def _close_datasetIO(self):
         if self.datasetIO is not None:
             self.datasetIO.close()
             self.datasetIO = None
             self.ds_array = None
             self.ads_array = None
```

### Comparing `dataset_iterator-0.4.1/dataset_iterator/ordered_enqueuer_cf.py` & `dataset_iterator-0.4.2/dataset_iterator/ordered_enqueuer_cf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
+import traceback
 from concurrent.futures import ProcessPoolExecutor
 import multiprocessing
-import queue
 import random
-import numpy as np
 import threading
 import time
-from multiprocessing import managers, shared_memory
+from multiprocessing import managers
 from threading import BoundedSemaphore
+from .shared_memory import to_shm, from_shm
 
 # adapted from https://github.com/keras-team/keras/blob/v2.13.1/keras/utils/data_utils.py#L651-L776
 # uses concurrent.futures, solves a memory leak in case of hard sample mining run as callback with regular orderedEnqueur. Option to pass tensors through shared memory
 
 
 # Global variables to be shared across processes
 _SHARED_SEQUENCES = {}
@@ -93,26 +93,28 @@
         sequence = list(range(len(self.sequence)))
         self._send_sequence()  # Share the initial sequence
         while True:
             if self.shuffle:
                 random.shuffle(sequence)
             task = get_item_shm if self.use_shm else get_item
             executor = ProcessPoolExecutor(max_workers=self.workers, initializer=init_pool_generator, initargs=(self.sequence, self.uid, self.shm_manager))
+            #print(f"executor started", flush=True)
             for idx, i in enumerate(sequence):
                 if self.stop_signal.is_set():
                     return
                 self.semaphore.acquire()
                 future = executor.submit(task, self.uid, i)
                 self.queue.append((future, i))
+                #print(f"sumit task: {i} {idx+1}/{len(sequence)}")
             # Done with the current epoch, waiting for the final batches
             self._wait_queue(True) # safer to wait before calling shutdown than calling directly shutdown with wait=True
-            print("exiting from ProcessPoolExecutor...", flush=True)
+            #print("exiting from ProcessPoolExecutor...", flush=True)
             time.sleep(0.1)
             executor.shutdown(wait=False, cancel_futures=True)
-            print("exiting from ProcessPoolExecutor done", flush=True)
+            #print("exiting from ProcessPoolExecutor done", flush=True)
             if self.stop_signal.is_set() or self.single_epoch:
                 # We're done
                 return
             if self.wait_for_me is not None:
                 self.wait_for_me.wait()
             # Call the internal on epoch end.
             self.sequence.on_epoch_end()
@@ -136,40 +138,41 @@
             `(inputs, targets)` or
             `(inputs, targets, sample_weights)`.
         """
         while self.is_running():
             self._wait_queue(False)
             if len(self.queue) > 0:
                 future, i = self.queue[0]
-                try:
+                #print(f"processing task: {i}")
+                ex = future.exception()
+                if ex is None:
                     inputs = future.result()
-                    self.queue.pop(0)  # only remove after result() is called to avoid terminating pool while a process is still running
                     if self.use_shm:
                         inputs = from_shm(*inputs)
-                    self.semaphore.release() # release is done here and not as a future callback to limit effective number of samples in memory
-                except Exception as e:
-                    self.stop()
-                    print(f"Exception raised while getting future result from task: {i}", flush=True)
-                    raise e
-                finally:
-                    future.cancel()
-                    del future
+                else:
+                    traceback.print_exception(ex)
+                    print(f"Exception raised while getting future result from task: {i}. Task will be re-computed.", flush=True)
+                    inputs = get_item(self.uid, i)
+                self.queue.pop(0)  # only remove after result() is called to avoid terminating pool while a process is still running
+                self.semaphore.release()  # release is done here and not as a future callback to limit effective number of samples in memory
+                future.cancel()
+                del future
                 yield inputs
 
     def stop(self, timeout=None):
         """Stops running threads and wait for them to exit, if necessary.
 
         Should be called by the same thread which called `start()`.
 
         Args:
             timeout: maximum time to wait on `thread.join()`
         """
         self.stop_signal.set()
         self.run_thread.join(timeout)
-        if self.use_shm is not None:
+        if self.shm_manager is not None:
             self.shm_manager.shutdown()
             self.shm_manager.join()
         self.queue = None
         self.semaphore = None
         global _SHARED_SHM_MANAGER
         _SHARED_SHM_MANAGER[self.uid] = None
         global _SHARED_SEQUENCES
@@ -187,99 +190,7 @@
     tensors = _SHARED_SEQUENCES[uid][i]
     return to_shm(_SHARED_SHM_MANAGER[uid], tensors)
 
 
 def get_item(uid, i):
     return _SHARED_SEQUENCES[uid][i]
 
-
-def to_shm(shm_manager, tensors):
-    flatten_tensor_list, nested_structure = get_flatten_list(tensors)
-    size = np.sum([a.nbytes for a in flatten_tensor_list])
-    shm = shm_manager.SharedMemory(size=size)
-    shapes = []
-    dtypes = []
-    offset = 0
-    for a in flatten_tensor_list:
-        shm_a = np.ndarray(a.shape, dtype=a.dtype, buffer=shm.buf, offset=offset)
-        shm_a[:] = a[:]
-        shapes.append(a.shape)
-        dtypes.append(a.dtype)
-        offset += a.nbytes
-    tensor_ref = (shapes, dtypes, shm.name, nested_structure)
-    shm.close()
-    del shm
-    return tensor_ref
-
-
-def from_shm(shapes, dtypes, shm_name, nested_structure):
-    existing_shm = ErasingSharedMemory(shm_name)
-    offset = 0
-    tensor_list = []
-    for shape, dtype in zip(shapes, dtypes):
-        a = ShmArray(shape, dtype=dtype, buffer=existing_shm.buf, offset=offset, shm=existing_shm)
-        tensor_list.append(a)
-        offset += a.nbytes
-    return get_nested_structure(tensor_list, nested_structure)
-
-
-def multiple(item):
-    return isinstance(item, (list, tuple))
-
-
-def get_flatten_list(item):
-    flatten_list = []
-    nested_structure = []
-    _flatten(item, 0, flatten_list, nested_structure)
-    return flatten_list, nested_structure[0]
-
-
-def _flatten(item, offset, flatten_list, nested_structure):
-    if multiple(item):
-        nested_structure.append([])
-        for sub_item in item:
-            offset = _flatten(sub_item, offset, flatten_list, nested_structure[-1])
-        return offset
-    else:
-        nested_structure.append(offset)
-        flatten_list.append(item)
-        return offset + 1
-
-
-def get_nested_structure(flatten_list, nested_structure):
-    if multiple(nested_structure):
-        result = []
-        _get_nested(flatten_list, nested_structure, 0, result)
-        return result[0]
-    else:
-        return flatten_list[0]
-
-
-def _get_nested(flatten_list, nested_structure, offset, result):
-    if multiple(nested_structure):
-        result.append([])
-        for sub_nested in nested_structure:
-            offset = _get_nested(flatten_list, sub_nested, offset, result[-1])
-        return offset
-    else:
-        result.append(flatten_list[offset])
-        return offset + 1
-
-
-# code from: https://muditb.medium.com/speed-up-your-keras-sequence-pipeline-f5d158359f46
-class ShmArray(np.ndarray):
-    def __new__(cls, shape, dtype=float, buffer=None, offset=0, strides=None, order=None, shm=None):
-        obj = super(ShmArray, cls).__new__(cls, shape, dtype, buffer, offset, strides,  order)
-        obj.shm = shm
-        return obj
-
-    def __array_finalize__(self, obj):
-        if obj is None: return
-        self.shm = getattr(obj, 'shm', None)
-
-class ErasingSharedMemory(shared_memory.SharedMemory):
-    def __del__(self):
-        super(ErasingSharedMemory, self).__del__()
-        try:
-            self.unlink() # manager can delete the file before array is finalized
-        except FileNotFoundError:
-            pass
```

### Comparing `dataset_iterator-0.4.1/dataset_iterator/pre_processing.py` & `dataset_iterator-0.4.2/dataset_iterator/pre_processing.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/tile_utils.py` & `dataset_iterator-0.4.2/dataset_iterator/tile_utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/tracking_iterator.py` & `dataset_iterator-0.4.2/dataset_iterator/tracking_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator/utils.py` & `dataset_iterator-0.4.2/dataset_iterator/utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.1/dataset_iterator.egg-info/PKG-INFO` & `dataset_iterator-0.4.2/dataset_iterator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.1
+Version: 0.4.2
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.1/dataset_iterator-0.4.1.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.2/dataset_iterator-0.4.2.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.1/dataset_iterator.egg-info/SOURCES.txt` & `dataset_iterator-0.4.2/dataset_iterator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 dataset_iterator/hard_sample_mining.py
 dataset_iterator/helpers.py
 dataset_iterator/image_data_generator.py
 dataset_iterator/index_array_iterator.py
 dataset_iterator/multichannel_iterator.py
 dataset_iterator/ordered_enqueuer_cf.py
 dataset_iterator/pre_processing.py
+dataset_iterator/shared_memory.py
 dataset_iterator/tile_utils.py
 dataset_iterator/tracking_iterator.py
 dataset_iterator/utils.py
 dataset_iterator.egg-info/PKG-INFO
 dataset_iterator.egg-info/SOURCES.txt
 dataset_iterator.egg-info/dependency_links.txt
 dataset_iterator.egg-info/requires.txt
```

### Comparing `dataset_iterator-0.4.1/setup.py` & `dataset_iterator-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dataset_iterator",
-    version="0.4.1",
+    version="0.4.2",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/dataset_iterator.git",
-    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.1/dataset_iterator-0.4.1.tar.gz',
+    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.2/dataset_iterator-0.4.2.tar.gz',
     keywords=['Iterator', 'Dataset', 'Image', 'Numpy'],
     packages=setuptools.find_packages(),
     classifiers=[ #https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

