# Comparing `tmp/hep_ml_lab-0.4.1.tar.gz` & `tmp/hep_ml_lab-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hep_ml_lab-0.4.1.tar", max compression
+gzip compressed data, was "hep_ml_lab-0.4.2.tar", max compression
```

## Comparing `hep_ml_lab-0.4.1.tar` & `hep_ml_lab-0.4.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1064 2023-12-23 08:40:53.016508 hep_ml_lab-0.4.1/LICENSE
--rw-r--r--   0        0        0     3350 2024-04-24 09:31:52.071094 hep_ml_lab-0.4.1/README.md
--rw-r--r--   0        0        0      193 2024-04-24 09:31:52.075094 hep_ml_lab-0.4.1/hml/__init__.py
--rw-r--r--   0        0        0      530 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/__init__.py
--rw-r--r--   0        0        0       92 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/cuts/__init__.py
--rw-r--r--   0        0        0     2851 2024-04-24 08:39:13.795076 hep_ml_lab-0.4.1/hml/approaches/cuts/cut.py
--rw-r--r--   0        0        0     7318 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/approaches/cuts/cut_and_count.py
--rw-r--r--   0        0        0     4244 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/cuts/cut_layer.py
--rw-r--r--   0        0        0       84 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/__init__.py
--rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/cnns/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/cnns/simple_cnn.py
--rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/gnns/__init__.py
--rw-r--r--   0        0        0       25 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/gnns/simple_gnn.py
--rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/mlps/__init__.py
--rw-r--r--   0        0        0      904 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/mlps/simple_mlp.py
--rw-r--r--   0        0        0       72 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/approaches/trees/__init__.py
--rw-r--r--   0        0        0     9251 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/approaches/trees/gradient_boosted_decision_tree.py
--rw-r--r--   0        0        0      552 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/datasets/__init__.py
--rw-r--r--   0        0        0       25 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/datasets/demo_z_tagging.py
--rw-r--r--   0        0        0       28 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/datasets/graph_dataset.py
--rw-r--r--   0        0        0    10756 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/datasets/image_dataset.py
--rw-r--r--   0        0        0     8472 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/datasets/set_dataset.py
--rw-r--r--   0        0        0       47 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/generators/__init__.py
--rw-r--r--   0        0        0    17799 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/generators/madgraph5.py
--rw-r--r--   0        0        0      148 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/metrics/__init__.py
--rw-r--r--   0        0        0     1193 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/metrics/max_significance.py
--rw-r--r--   0        0        0     1205 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/metrics/rejection_at_efficiency.py
--rw-r--r--   0        0        0     2774 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/observables/__init__.py
--rw-r--r--   0        0        0     1699 2024-04-23 12:46:29.442671 hep_ml_lab-0.4.1/hml/observables/angular_distance.py
--rw-r--r--   0        0        0      399 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/charge.py
--rw-r--r--   0        0        0     1043 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/observables/invariant_mass.py
--rw-r--r--   0        0        0     2435 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/kinematics.py
--rw-r--r--   0        0        0     3647 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/n_subjettiness.py
--rw-r--r--   0        0        0     6130 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/observables/observable.py
--rw-r--r--   0        0        0      732 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/size.py
--rw-r--r--   0        0        0      681 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/tag.py
--rw-r--r--   0        0        0      235 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/__init__.py
--rw-r--r--   0        0        0      637 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/fastjet_ops.py
--rw-r--r--   0        0        0     1305 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/keras_ops.py
--rw-r--r--   0        0        0        0 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/repr_ops.py
--rw-r--r--   0        0        0     5529 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/uproot_ops.py
--rw-r--r--   0        0        0     1056 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/physics_objects/__init__.py
--rw-r--r--   0        0        0     1969 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/collective.py
--rw-r--r--   0        0        0     2227 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/multiple.py
--rw-r--r--   0        0        0     1800 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/nested.py
--rw-r--r--   0        0        0     1228 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/physics_object.py
--rw-r--r--   0        0        0     1256 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/single.py
--rw-r--r--   0        0        0       71 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/representations/__init__.py
--rw-r--r--   0        0        0       21 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/representations/graph.py
--rw-r--r--   0        0        0    17647 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/representations/image.py
--rw-r--r--   0        0        0     2472 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/representations/set.py
--rw-r--r--   0        0        0     1872 2024-04-24 09:31:52.075094 hep_ml_lab-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 hep_ml_lab-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-12-23 08:40:53.016508 hep_ml_lab-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3694 2024-04-29 08:02:51.513509 hep_ml_lab-0.4.2/README.md
+-rw-r--r--   0        0        0      193 2024-04-29 07:58:59.817508 hep_ml_lab-0.4.2/hml/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/cuts/__init__.py
+-rw-r--r--   0        0        0     3410 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/approaches/cuts/cut.py
+-rw-r--r--   0        0        0     7318 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.2/hml/approaches/cuts/cut_and_count.py
+-rw-r--r--   0        0        0     4244 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/cuts/cut_layer.py
+-rw-r--r--   0        0        0       84 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/cnns/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/approaches/networks/cnns/simple_cnn.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/gnns/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/gnns/simple_gnn.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/mlps/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/mlps/simple_mlp.py
+-rw-r--r--   0        0        0       72 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/approaches/trees/__init__.py
+-rw-r--r--   0        0        0     9251 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.2/hml/approaches/trees/gradient_boosted_decision_tree.py
+-rw-r--r--   0        0        0      552 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/datasets/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/datasets/demo_z_tagging.py
+-rw-r--r--   0        0        0       28 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/datasets/graph_dataset.py
+-rw-r--r--   0        0        0    10756 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/datasets/image_dataset.py
+-rw-r--r--   0        0        0     8442 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/datasets/set_dataset.py
+-rw-r--r--   0        0        0       47 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/generators/__init__.py
+-rw-r--r--   0        0        0    17799 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.2/hml/generators/madgraph5.py
+-rw-r--r--   0        0        0      148 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/metrics/__init__.py
+-rw-r--r--   0        0        0     2463 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/metrics/max_significance.py
+-rw-r--r--   0        0        0     1205 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/metrics/rejection_at_efficiency.py
+-rw-r--r--   0        0        0     1384 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/__init__.py
+-rw-r--r--   0        0        0     1771 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/angular_distance.py
+-rw-r--r--   0        0        0      431 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/charge.py
+-rw-r--r--   0        0        0     1174 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/invariant_mass.py
+-rw-r--r--   0        0        0     2874 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/kinematics.py
+-rw-r--r--   0        0        0     3812 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/n_subjettiness.py
+-rw-r--r--   0        0        0     6437 2024-04-29 09:02:20.361529 hep_ml_lab-0.4.2/hml/observables/observable.py
+-rw-r--r--   0        0        0      848 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/size.py
+-rw-r--r--   0        0        0      743 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/tag.py
+-rw-r--r--   0        0        0      235 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/__init__.py
+-rw-r--r--   0        0        0      637 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/fastjet_ops.py
+-rw-r--r--   0        0        0     1305 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/keras_ops.py
+-rw-r--r--   0        0        0        0 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/repr_ops.py
+-rw-r--r--   0        0        0     5529 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/uproot_ops.py
+-rw-r--r--   0        0        0     1056 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.2/hml/physics_objects/__init__.py
+-rw-r--r--   0        0        0     1969 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/collective.py
+-rw-r--r--   0        0        0     2227 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/multiple.py
+-rw-r--r--   0        0        0     1800 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/nested.py
+-rw-r--r--   0        0        0     1228 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/physics_object.py
+-rw-r--r--   0        0        0     1256 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/single.py
+-rw-r--r--   0        0        0       71 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/representations/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/representations/graph.py
+-rw-r--r--   0        0        0    17647 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.2/hml/representations/image.py
+-rw-r--r--   0        0        0     2545 2024-04-29 09:02:20.361529 hep_ml_lab-0.4.2/hml/representations/set.py
+-rw-r--r--   0        0        0     1872 2024-04-29 07:58:52.317508 hep_ml_lab-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4948 1970-01-01 00:00:00.000000 hep_ml_lab-0.4.2/PKG-INFO
```

### Comparing `hep_ml_lab-0.4.1/LICENSE` & `hep_ml_lab-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/README.md` & `hep_ml_lab-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,21 @@
 - `hml.representations`: Different data structure used to represent an event;
 - `hml.datasets`: Existing datasets and helper classes for creating new datasets;
 - `hml.approaches`: Cuts, trees and networks for classification;
 - `hml.metrics`: Metrics used in classical signal vs background analysis;
 
 ## Updates
 
+### v0.4.2
+- Fix parsing cuts like "muon0.charge != muon1.charge".
+- Fix inconsistent model layers in `hml.approaches.networks.SimpleCNN`.
+- Fix registering and saving custom observables.
+- Add cross sections, luminosity and weights as parameters in `hml.metrics.MaxSignificance`.
+- Improve the figure ratio in `hml.datasets.SetDataset.show`.
+
 ### v0.4.1
 - Fix module overview image in README.
 - Fix `GradientBoostedDecisionTree` to be compatible with different `sklearn` versions.
 - Fix `hml.datasets.SetDataset.show` to display the correct rows and columns.
 - Rename the `parse` and `register` functions to `parse_physics_object`, `parse_observable`, and `register_observable`.
 - Update the installation document.
```

### Comparing `hep_ml_lab-0.4.1/hml/approaches/__init__.py` & `hep_ml_lab-0.4.2/hml/approaches/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/approaches/cuts/cut.py` & `hep_ml_lab-0.4.2/hml/approaches/cuts/cut.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,47 +32,59 @@
         cuts = [cut.strip().split("|") for cut in cuts]
         cuts = [c.strip() for cut in cuts for c in cut]
         cuts = [cut.replace("(", "").replace(")", "") for cut in cuts]
 
         obs_pattern = r"\b(?!\d+\b)(?!\d*\.\d+\b)\S+\b"
         cuts_dict = {}
         for cut in cuts:
-            obs = re.findall(obs_pattern, cut)[0]
-            if "" not in cut.split(obs):
+            all_obs = re.findall(obs_pattern, cut)
+            # for the case value1 < obs < value2
+            if len(all_obs) == 1 and "" not in cut.split(all_obs[0]):
+                obs = all_obs[0]
                 new_cut = [cut.split(obs)[0] + obs, obs + cut.split(obs)[1]]
-                cuts_dict[new_cut[0]] = obs
-                cuts_dict[new_cut[1]] = obs
-                expr = expr.replace(cut, f"({new_cut[0]} & {new_cut[1]})")
+                cuts_dict[new_cut[0]] = [obs]
+                cuts_dict[new_cut[1]] = [obs]
+                expr = expr.replace(cut, f"( {new_cut[0]} & {new_cut[1]} )")
             else:
-                cuts_dict[cut] = obs
+                cuts_dict[cut] = all_obs
 
-        self._cuts_dict = cuts_dict
-        self._observables_dict = {
-            obs: parse_observable(obs) for obs in cuts_dict.values()
-        }
+        self._cuts_dict = cuts_dict  # single expression and its obs name
+        self._observables_dict = {}
+        for all_obs in cuts_dict.values():
+            for obs in all_obs:
+                self._observables_dict[obs] = parse_observable(obs)
         self._expr = expr
 
     def read(self, events):
         for obs in self._observables_dict.values():
             obs.read(events)
         observables_dict = self._observables_dict
 
         cuts_results = {}
-        for cut, obs in self._cuts_dict.items():
-            result = eval(cut.replace(obs, f"observables_dict['{obs}'].value"))
+        for cut, all_obs in self._cuts_dict.items():
+            temp_cut = cut
+            for obs in all_obs:
+                temp_cut = temp_cut.replace(obs, f"observables_dict['{obs}'].value")
+            result = eval(temp_cut)
             cuts_results[cut] = result
 
         # Validate the type
         shapes = set([obs.shape for obs in observables_dict.values()])
         if len(shapes) != 1:
             raise ValueError
 
         expression = self._expr
         for cut in cuts_results:
-            cut_pattern = r"\b" + cut.replace(".", "\\.") + r"\b"
+            if (
+                len(re.findall(r"\b" + cut.replace(".", "\\.") + r"\b", expression))
+                != 0
+            ):
+                cut_pattern = r"\b" + cut.replace(".", "\\.") + r"\b"
+            else:
+                cut_pattern = r"\s" + cut.replace(".", "\\.") + r"\s"
             expression = re.sub(cut_pattern, f"cuts_results['{cut}']", expression)
 
         self._value = ak.fill_none(eval(expression), False)
 
         if self._value.ndim > 1:
             if self._is_any:
                 self._value = ak.any(self._value, axis=1)
```

### Comparing `hep_ml_lab-0.4.1/hml/approaches/cuts/cut_and_count.py` & `hep_ml_lab-0.4.2/hml/approaches/cuts/cut_and_count.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/approaches/cuts/cut_layer.py` & `hep_ml_lab-0.4.2/hml/approaches/cuts/cut_layer.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/approaches/networks/cnns/simple_cnn.py` & `hep_ml_lab-0.4.2/hml/approaches/networks/cnns/simple_cnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,25 @@
         self.input_shape = input_shape
         self.conv1 = Conv2D(8, 3, padding="same", activation="relu")
         self.conv2 = Conv2D(16, 3, padding="same", activation="relu")
         self.conv3 = Conv2D(32, 3, padding="same", activation="relu")
         self.max_pool = MaxPooling2D()
         self.global_avg_pool = GlobalAveragePooling2D()
         self.dropout = Dropout(0.5)
-        self.dense1 = Dense(2, activation="relu")
-        self.dense2 = Dense(2, activation="softmax")
+        self.dense1 = Dense(2, activation="softmax")
 
         self.call(Input(shape=input_shape))
 
     def call(self, x):
         x = self.conv1(x)
         x = self.max_pool(x)
         x = self.conv2(x)
         x = self.max_pool(x)
         x = self.conv3(x)
         x = self.max_pool(x)
         x = self.global_avg_pool(x)
-        x = self.dense1(x)
-        return self.dense2(x)
+        return self.dense1(x)
 
     def get_config(self):
         base_config = super().get_config()
         config = {"input_shape": self.input_shape}
         return {**base_config, **config}
```

### Comparing `hep_ml_lab-0.4.1/hml/approaches/networks/mlps/simple_mlp.py` & `hep_ml_lab-0.4.2/hml/approaches/networks/mlps/simple_mlp.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/approaches/trees/gradient_boosted_decision_tree.py` & `hep_ml_lab-0.4.2/hml/approaches/trees/gradient_boosted_decision_tree.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/datasets/__init__.py` & `hep_ml_lab-0.4.2/hml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/datasets/image_dataset.py` & `hep_ml_lab-0.4.2/hml/datasets/image_dataset.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/datasets/set_dataset.py` & `hep_ml_lab-0.4.2/hml/datasets/set_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,21 +232,18 @@
     def show(self, n_feature_per_line=3, n_samples=-1, target=None):
         if n_samples != -1:
             samples = self.samples[:n_samples]
         else:
             samples = self.samples
 
         n_features = len(self.feature_names)
-        plt.figure(figsize=(3 * n_feature_per_line, 3))
+        n_rows = (n_features + n_feature_per_line - 1) // n_feature_per_line
+        plt.figure(figsize=(4 * n_feature_per_line, 3 * n_rows))
         for i, name in enumerate(self.feature_names):
-            ax = plt.subplot(
-                (n_features + n_feature_per_line - 1) // n_feature_per_line,
-                n_feature_per_line,
-                i + 1,
-            )
+            ax = plt.subplot(n_rows, n_feature_per_line, i + 1)
 
             if target is None:
                 for i_target in np.unique(self.targets):
                     ax.hist(
                         samples[np.squeeze(self.targets == i_target)][:, i],
                         bins=50,
                         histtype="step",
```

### Comparing `hep_ml_lab-0.4.1/hml/generators/madgraph5.py` & `hep_ml_lab-0.4.2/hml/generators/madgraph5.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/metrics/rejection_at_efficiency.py` & `hep_ml_lab-0.4.2/hml/metrics/rejection_at_efficiency.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/observables/angular_distance.py` & `hep_ml_lab-0.4.2/hml/observables/angular_distance.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,7 +44,10 @@
 
     @classmethod
     def from_name(cls, name: str, **kwargs) -> AngularDistance:
         *parts, class_name = name.split(".")
         physics_object = ".".join(parts) if len(parts) > 0 else None
 
         return cls(physics_object, class_name)
+
+
+AngularDistance.with_aliases("angular_distance", "DeltaR", "delta_r")
```

### Comparing `hep_ml_lab-0.4.1/hml/observables/invariant_mass.py` & `hep_ml_lab-0.4.2/hml/observables/invariant_mass.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,7 +31,17 @@
             padded_momentum4d = ak.pad_none(momentum4d[:, obj.slices[0]], 1)
             momenta.append(padded_momentum4d)
 
         total = reduce(lambda x, y: x + y, momenta)
         self._value = total.mass
 
         return self
+
+
+InvariantMass.with_aliases(
+    "InvariantMass",
+    "invariant_mass",
+    "InvMass",
+    "inv_mass",
+    "InvM",
+    "inv_m",
+)
```

### Comparing `hep_ml_lab-0.4.1/hml/observables/kinematics.py` & `hep_ml_lab-0.4.2/hml/observables/kinematics.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,75 +10,99 @@
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective", "nested"]
         super().__init__(physics_object, class_name, supported_objects)
 
 
+Px.with_aliases("MomentumX", "momentum_x", "px")
+
+
 class Py(Observable):
     def __init__(
         self,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective", "nested"]
         super().__init__(physics_object, class_name, supported_objects)
 
 
+Py.with_aliases("MomentumY", "momentum_y", "py")
+
+
 class Pz(Observable):
     def __init__(
         self,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective", "nested"]
         super().__init__(physics_object, class_name, supported_objects)
 
 
+Pz.with_aliases("MomentumZ", "momentum_z", "pz")
+
+
 class E(Observable):
     def __init__(
         self,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective", "nested"]
         super().__init__(physics_object, class_name, supported_objects)
 
 
+E.with_aliases("Energy", "energy", "e")
+
+
 class Pt(Observable):
     def __init__(
         self,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective", "nested"]
         super().__init__(physics_object, class_name, supported_objects)
 
 
+Pt.with_aliases("TransverseMomentum", "transverse_momentum", "pt", "PT", "pT")
+
+
 class Eta(Observable):
     def __init__(
         self,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective", "nested"]
         super().__init__(physics_object, class_name, supported_objects)
 
 
+Eta.with_aliases("Pseudorapidity", "pseudorapidity", "eta")
+
+
 class Phi(Observable):
     def __init__(
         self,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective", "nested"]
         super().__init__(physics_object, class_name, supported_objects)
 
 
+Phi.with_aliases("AzimuthalAngle", "azimuthal_angle", "phi")
+
+
 class M(Observable):
     def __init__(
         self,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective", "nested"]
         super().__init__(physics_object, class_name, supported_objects)
+
+
+M.with_aliases("Mass", "mass", "m")
```

### Comparing `hep_ml_lab-0.4.1/hml/observables/n_subjettiness.py` & `hep_ml_lab-0.4.2/hml/observables/n_subjettiness.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     @property
     def config(self):
         config = super().config
         config.update({"n": self.n})
         return config
 
 
+NSubjettiness.with_aliases("n_subjettiness")
+
+
 class TauN(NSubjettiness):
     @classmethod
     def from_name(cls, name: str, **kwargs) -> TauN:
         *parts, class_name = name.split(".")
         physics_object = ".".join(parts) if len(parts) > 0 else None
 
         if class_name.lower().startswith("tau"):
@@ -71,14 +74,17 @@
                 n = int(class_name[-1])
             else:
                 n = kwargs["n"]
 
         return cls(n, physics_object, class_name)
 
 
+TauN.with_aliases("tau_n")
+
+
 class NSubjettinessRatio(Observable):
     def __init__(
         self,
         m: int,
         n: int,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
@@ -102,14 +108,17 @@
     @property
     def config(self):
         config = super().config
         config.update({"m": self.m, "n": self.n})
         return config
 
 
+NSubjettinessRatio.with_aliases("n_subjettiness_ratio")
+
+
 class TauMN(NSubjettinessRatio):
     @classmethod
     def from_name(cls, name: str, **kwargs) -> TauMN:
         *parts, class_name = name.split(".")
         physics_object = ".".join(parts) if len(parts) > 0 else None
 
         if class_name.lower().startswith("tau"):
@@ -120,7 +129,10 @@
 
             if "n" not in kwargs:
                 n = int(class_name[-1])
             else:
                 n = kwargs["n"]
 
         return cls(m, n, physics_object, class_name)
+
+
+TauMN.with_aliases("tau_mn")
```

### Comparing `hep_ml_lab-0.4.1/hml/observables/observable.py` & `hep_ml_lab-0.4.2/hml/observables/observable.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,35 @@
 
 from ..operations import branch_to_momentum4d, constituents_to_momentum4d
 from ..physics_objects import PhysicsObject, is_collective, is_multiple, is_single
 from ..physics_objects import parse_physics_object as parse_object
 
 
 class Observable:
+    aliases = {}
+
     def __init__(
         self,
         physics_object: str | PhysicsObject | None = None,
         class_name: str | None = None,
         supported_objects: list[str | PhysicsObject] | None = None,
     ) -> None:
         self._physics_object = self._init_object(physics_object)
         self._class_name = self._init_class_name(class_name)
         self._supported_objects = self._init_supported_objects(supported_objects)
         self._validate_physics_object()
 
+    def __init_subclass__(cls, **kwargs):
+        cls.aliases[cls.__name__] = cls
+
+    @classmethod
+    def with_aliases(cls, *aliases: str) -> Observable:
+        for alias in aliases:
+            cls.aliases[alias] = cls
+
     def _init_object(self, object_: str | PhysicsObject | None) -> PhysicsObject | None:
         if isinstance(object_, PhysicsObject):
             return object_
 
         elif isinstance(object_, str):
             return parse_object(object_)
 
@@ -105,15 +115,15 @@
             return f"{self.physics_object.name}.{self.class_name}"
         else:
             return self.class_name
 
     @property
     def config(self) -> dict:
         return {
-            "physics_object": self.physics_object.name,
+            "physics_object": self.physics_object.name if self.physics_object else None,
             "class_name": self.class_name,
         }
 
     def read(self, events) -> Observable:
         if "multiple" in self.supported_objects:
             raise NotImplementedError
 
@@ -121,25 +131,25 @@
         branch = self.physics_object.branch.lower()
         slices = self.physics_object.slices
 
         if branch is None:
             raise ValueError(f"Branch {self.physics_object.branch} not found")
 
         if is_single(self.physics_object) or is_collective(self.physics_object):
-            if f"{branch}.{self.class_name.lower()}" in all_keys:
-                key = all_keys[f"{branch}.{self.class_name.lower()}"]
+            if f"{branch}.{self.__class__.__name__.lower()}" in all_keys:
+                key = all_keys[f"{branch}.{self.__class__.__name__.lower()}"]
                 value = events[key].array()
 
             else:
                 array = branch_to_momentum4d(events, all_keys[branch])
-                value = getattr(array, self.class_name.lower())
+                value = getattr(array, self.__class__.__name__.lower())
 
         else:
             array = constituents_to_momentum4d(events, all_keys[branch])
-            value = getattr(array, self.class_name.lower())
+            value = getattr(array, self.__class__.__name__.lower())
 
         if len(slices) == 1:
             value = value[:, slices[0]]
         else:
             value = value[:, slices[0], slices[1]]
 
         for i, slice_ in enumerate(slices):
```

### Comparing `hep_ml_lab-0.4.1/hml/observables/size.py` & `hep_ml_lab-0.4.2/hml/observables/size.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,11 +16,16 @@
     def read(self, events) -> Observable:
         all_keys = {i.lower(): i for i in events.keys(full_paths=False)}
         branch = self.physics_object.branch.lower()
 
         if f"{branch}_size" in all_keys:
             key = all_keys[f"{branch}_size"]
             value = events[key].array()
+        else:
+            raise KeyError(f"Key {branch}_size not found in the events.")
 
         self._value = value
 
         return self
+
+
+Size.with_aliases("size")
```

### Comparing `hep_ml_lab-0.4.1/hml/observables/tag.py` & `hep_ml_lab-0.4.2/hml/observables/tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,21 @@
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective"]
         super().__init__(physics_object, class_name, supported_objects)
 
 
+BTag.with_aliases("b_tag")
+
+
 class TauTag(Observable):
     def __init__(
         self,
         physics_object: str | PhysicsObject,
         class_name: str | None = None,
     ) -> None:
         supported_objects = ["single", "collective"]
         super().__init__(physics_object, class_name, supported_objects)
+
+
+TauTag.with_aliases("tau_tag")
```

### Comparing `hep_ml_lab-0.4.1/hml/operations/fastjet_ops.py` & `hep_ml_lab-0.4.2/hml/operations/fastjet_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/operations/keras_ops.py` & `hep_ml_lab-0.4.2/hml/operations/keras_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/operations/uproot_ops.py` & `hep_ml_lab-0.4.2/hml/operations/uproot_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/physics_objects/__init__.py` & `hep_ml_lab-0.4.2/hml/physics_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/physics_objects/collective.py` & `hep_ml_lab-0.4.2/hml/physics_objects/collective.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/physics_objects/multiple.py` & `hep_ml_lab-0.4.2/hml/physics_objects/multiple.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/physics_objects/nested.py` & `hep_ml_lab-0.4.2/hml/physics_objects/nested.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/physics_objects/physics_object.py` & `hep_ml_lab-0.4.2/hml/physics_objects/physics_object.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/physics_objects/single.py` & `hep_ml_lab-0.4.2/hml/physics_objects/single.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/representations/image.py` & `hep_ml_lab-0.4.2/hml/representations/image.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.1/hml/representations/set.py` & `hep_ml_lab-0.4.2/hml/representations/set.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,16 +76,17 @@
                 for i, obs in enumerate(self.observables)
             },
         }
 
     @classmethod
     def from_config(cls, config):
         observables = []
-        module = import_module("hml.observables")
 
         for i_config in config["observable_configs"].values():
-            class_name = i_config["class_name"]
-            class_config = i_config["config"]
+            class_type = Observable.aliases[i_config["class_name"]]
+            class_name = class_type.__name__
+            module = import_module(class_type.__module__)
             class_ = getattr(module, class_name)
+            class_config = i_config["config"]
             observables.append(class_.from_config(class_config))
 
         return cls(observables)
```

### Comparing `hep_ml_lab-0.4.1/pyproject.toml` & `hep_ml_lab-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hep-ml-lab"
-version = "0.4.1"
+version = "0.4.2"
 description = "An end-to-end framework used for research combining high-energy physics phenomenology with machine learning."
 license = "MIT"
 authors = ["Star9daisy <star9daisy@outlook.com>"]
 readme = "README.md"
 homepage = "https://github.com/Star9daisy/hep-ml-lab"
 documentation = "https://star9daisy.github.io/hep-ml-lab/"
 keywords = ["high energy physics", "machine learning", "framework"]
```

### Comparing `hep_ml_lab-0.4.1/PKG-INFO` & `hep_ml_lab-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hep-ml-lab
-Version: 0.4.1
+Version: 0.4.2
 Summary: An end-to-end framework used for research combining high-energy physics phenomenology with machine learning.
 Home-page: https://github.com/Star9daisy/hep-ml-lab
 License: MIT
 Keywords: high energy physics,machine learning,framework
 Author: Star9daisy
 Author-email: star9daisy@outlook.com
 Requires-Python: >=3.9,<3.12
@@ -64,14 +64,21 @@
 - `hml.representations`: Different data structure used to represent an event;
 - `hml.datasets`: Existing datasets and helper classes for creating new datasets;
 - `hml.approaches`: Cuts, trees and networks for classification;
 - `hml.metrics`: Metrics used in classical signal vs background analysis;
 
 ## Updates
 
+### v0.4.2
+- Fix parsing cuts like "muon0.charge != muon1.charge".
+- Fix inconsistent model layers in `hml.approaches.networks.SimpleCNN`.
+- Fix registering and saving custom observables.
+- Add cross sections, luminosity and weights as parameters in `hml.metrics.MaxSignificance`.
+- Improve the figure ratio in `hml.datasets.SetDataset.show`.
+
 ### v0.4.1
 - Fix module overview image in README.
 - Fix `GradientBoostedDecisionTree` to be compatible with different `sklearn` versions.
 - Fix `hml.datasets.SetDataset.show` to display the correct rows and columns.
 - Rename the `parse` and `register` functions to `parse_physics_object`, `parse_observable`, and `register_observable`.
 - Update the installation document.
```

