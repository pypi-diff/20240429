# Comparing `tmp/osesd-1.0.0.tar.gz` & `tmp/osesd-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osesd-1.0.0.tar", last modified: Wed Apr 17 06:47:49 2024, max compression
+gzip compressed data, was "osesd-1.1.0.tar", last modified: Mon Apr 29 07:44:07 2024, max compression
```

## Comparing `osesd-1.0.0.tar` & `osesd-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:47:49.201265 osesd-1.0.0/
--rw-rw-rw-   0        0        0     1089 2024-04-17 06:02:33.000000 osesd-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3186 2024-04-17 06:47:49.200268 osesd-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2706 2024-04-17 01:34:03.000000 osesd-1.0.0/README.md
--rw-rw-rw-   0        0        0      391 2024-04-17 06:06:17.000000 osesd-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 06:47:49.201265 osesd-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 06:47:49.114596 osesd-1.0.0/src/
--rw-rw-rw-   0        0        0        0 2024-04-17 06:27:12.000000 osesd-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     8619 2023-09-19 07:15:12.000000 osesd-1.0.0/src/auto_osESD.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:47:49.177882 osesd-1.0.0/src/models/
--rw-rw-rw-   0        0        0        0 2024-04-17 06:27:12.000000 osesd-1.0.0/src/models/__init__.py
--rw-rw-rw-   0        0        0    10153 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/auto_osESD_Detector.py
--rw-rw-rw-   0        0        0     3859 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/norep_Test.py
--rw-rw-rw-   0        0        0      973 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/norep_osESD_Detector.py
--rw-rw-rw-   0        0        0     3259 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/norep_osESD_Transform.py
--rw-rw-rw-   0        0        0     1503 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/oGESD_Detector.py
--rw-rw-rw-   0        0        0     2498 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/oGESD_Test.py
--rw-rw-rw-   0        0        0     3296 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/oGESD_Transform.py
--rw-rw-rw-   0        0        0     1553 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/osESD_Detector.py
--rw-rw-rw-   0        0        0     3867 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/osESD_Test.py
--rw-rw-rw-   0        0        0     3259 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/osESD_Transform.py
--rw-rw-rw-   0        0        0      352 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/sosESD_Detector.py
--rw-rw-rw-   0        0        0     1984 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/sosESD_Test.py
--rw-rw-rw-   0        0        0      961 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/ts_AE.py
--rw-rw-rw-   0        0        0      953 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/ts_LSTMED.py
--rw-rw-rw-   0        0        0      925 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/ts_VAE.py
--rw-rw-rw-   0        0        0      999 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/ts_isolation_forest.py
--rw-rw-rw-   0        0        0     1382 2023-09-19 07:15:12.000000 osesd-1.0.0/src/models/ts_random_robust_cut_classifier.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:47:49.198274 osesd-1.0.0/src/osESD.egg-info/
--rw-rw-rw-   0        0        0     3186 2024-04-17 06:47:49.000000 osesd-1.0.0/src/osESD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2024-04-17 06:47:49.000000 osesd-1.0.0/src/osESD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:47:49.000000 osesd-1.0.0/src/osESD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2024-04-17 06:47:49.000000 osesd-1.0.0/src/osESD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5892 2024-04-17 06:28:37.000000 osesd-1.0.0/src/osESD.py
--rw-rw-rw-   0        0        0     5319 2023-09-19 07:15:12.000000 osesd-1.0.0/src/parameters.py
--rw-rw-rw-   0        0        0     9750 2023-09-19 07:15:12.000000 osesd-1.0.0/src/run_ablation_tests.py
--rw-rw-rw-   0        0        0     6856 2023-09-19 07:15:12.000000 osesd-1.0.0/src/run_auto_osESD_tests.py
--rw-rw-rw-   0        0        0    10738 2023-09-19 07:15:12.000000 osesd-1.0.0/src/run_comparison_tests.py
--rw-rw-rw-   0        0        0    17495 2023-09-19 07:15:12.000000 osesd-1.0.0/src/run_single_test.py
--rw-rw-rw-   0        0        0      803 2023-09-19 07:15:12.000000 osesd-1.0.0/src/run_tests.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:47:49.196280 osesd-1.0.0/src/utils/
--rw-rw-rw-   0        0        0        0 2024-04-17 06:27:12.000000 osesd-1.0.0/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3887 2023-09-19 07:15:12.000000 osesd-1.0.0/src/utils/data_aug.py
--rw-rw-rw-   0        0        0      460 2023-09-19 07:15:12.000000 osesd-1.0.0/src/utils/plotting_modules.py
--rw-rw-rw-   0        0        0      897 2023-09-19 07:15:12.000000 osesd-1.0.0/src/utils/scores_module.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:44:07.340693 osesd-1.1.0/
+-rw-rw-rw-   0        0        0     1089 2024-04-17 06:02:33.000000 osesd-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3444 2024-04-29 07:44:07.339697 osesd-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2946 2024-04-22 05:56:03.000000 osesd-1.1.0/README.md
+-rw-rw-rw-   0        0        0      391 2024-04-29 07:43:38.000000 osesd-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:44:07.340693 osesd-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 07:44:07.249147 osesd-1.1.0/src/
+-rw-rw-rw-   0        0        0        0 2024-04-17 06:27:12.000000 osesd-1.1.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:44:07.288846 osesd-1.1.0/src/models/
+-rw-rw-rw-   0        0        0        0 2024-04-17 06:27:12.000000 osesd-1.1.0/src/models/__init__.py
+-rw-rw-rw-   0        0        0    10153 2024-04-29 04:40:11.000000 osesd-1.1.0/src/models/auto_osESD_Detector.py
+-rw-rw-rw-   0        0        0     1553 2023-09-19 07:15:12.000000 osesd-1.1.0/src/models/osESD_Detector.py
+-rw-rw-rw-   0        0        0     3867 2023-09-19 07:15:12.000000 osesd-1.1.0/src/models/osESD_Test.py
+-rw-rw-rw-   0        0        0     3259 2023-09-19 07:15:12.000000 osesd-1.1.0/src/models/osESD_Transform.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:44:07.337703 osesd-1.1.0/src/osESD.egg-info/
+-rw-rw-rw-   0        0        0     3444 2024-04-29 07:44:07.000000 osesd-1.1.0/src/osESD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-04-29 07:44:07.000000 osesd-1.1.0/src/osESD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:44:07.000000 osesd-1.1.0/src/osESD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-29 07:44:07.000000 osesd-1.1.0/src/osESD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8810 2024-04-29 04:44:46.000000 osesd-1.1.0/src/osESD.py
+-rw-rw-rw-   0        0        0     5319 2023-09-19 07:15:12.000000 osesd-1.1.0/src/parameters.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:44:07.335737 osesd-1.1.0/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-17 06:27:12.000000 osesd-1.1.0/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3887 2023-09-19 07:15:12.000000 osesd-1.1.0/src/utils/data_aug.py
+-rw-rw-rw-   0        0        0      460 2023-09-19 07:15:12.000000 osesd-1.1.0/src/utils/plotting_modules.py
+-rw-rw-rw-   0        0        0      897 2023-09-19 07:15:12.000000 osesd-1.1.0/src/utils/scores_module.py
```

### Comparing `osesd-1.0.0/LICENSE` & `osesd-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osesd-1.0.0/src/models/auto_osESD_Detector.py` & `osesd-1.1.0/src/models/auto_osESD_Detector.py`

 * *Files identical despite different names*

### Comparing `osesd-1.0.0/src/models/norep_Test.py` & `osesd-1.1.0/src/models/osESD_Test.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
         self.alpha = alpha
         self.maxr = maxr
         self.data = data
         self.size = len(data)
         self.mean = np.mean(data)
         self.sqsum = np.sum(np.square(data))
 
-    def test(self, f, on):
-        out = f
+    def test(self, on):
+        out = self.data[0]
         self.data = np.append(self.data[1:], on)
         self.mean += -(out - on) / self.size
         self.sqsum += (-out ** 2) + (on ** 2)
         mean_ = self.mean
         sqsum_ = self.sqsum
         size_ = self.size
         data_ = self.data
```

### Comparing `osesd-1.0.0/src/models/norep_osESD_Detector.py` & `osesd-1.1.0/src/models/osESD_Detector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 
 from . import osESD_Test
 from . import osESD_Transform
 
-def norep_osESD(data, dwins, rwins, train_size, alpha, maxr, time=None):
+def osESD(data, dwins, rwins, train_size, alpha, maxr, condition, time=None):
     offline_data = data[:train_size]
     online_data = data[train_size:len(data)]
     offline_time = time[:train_size]
     online_time = time[train_size:len(data)]
-    r_ins = osESD_Transform.TRES(data = offline_data, time = offline_time, wins = rwins)
     c_ins = osESD_Transform.TCHA(data = offline_data, time = offline_time, wins = dwins)
-    SESD_TRES = osESD_Test.SESD_tres(data = r_ins.tres.copy(), alpha = alpha, maxr = maxr)
+    r_ins = osESD_Transform.TRES(data = offline_data, time = offline_time, wins = rwins)
     SESD_TCHA = osESD_Test.SESD_tcha(data = c_ins.tcha.copy(), alpha = alpha, maxr = maxr)
+    SESD_TRES = osESD_Test.SESD_tres(data = r_ins.tres.copy(), alpha = alpha, maxr = maxr)
     anomaly_index = []
     for i in range(len(online_data)):
-        ranom = SESD_TRES.test(r_ins.update(online_data[i], online_time[i]))
         canom = SESD_TCHA.test(c_ins.update(online_data[i], online_time[i]))
-        if (canom or ranom):
+        ranom = SESD_TRES.test(r_ins.update(online_data[i], online_time[i]))
+        if condition: function_ = (canom and ranom)
+        else: function_ = (canom or ranom)
+        if function_ :
             anomaly_index.append(i+train_size)
-
+            D = r_ins.data.copy()
+            T = r_ins.time.copy()
+            del D[rwins-1]
+            del T[rwins-1]
+            x_bar = ((rwins*r_ins.x_bar) - r_ins.time[rwins-1]) / (rwins-1)
+            y_bar = ((rwins*r_ins.y_bar) - r_ins.data[rwins-1]) / (rwins-1)
+            beta_ = sum((T-x_bar)*(D-y_bar))/sum((T-x_bar)**2)
+            alpha_ = y_bar - beta_*x_bar
+            rep = alpha_ + beta_*T[rwins-2]
+            c_ins.replace(rep)
+            r_ins.replace(rep)
     return (anomaly_index)
+
+
+
```

### Comparing `osesd-1.0.0/src/models/norep_osESD_Transform.py` & `osesd-1.1.0/src/models/osESD_Transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         self.data.append(ond)
         self.time.append(self.time[-1]+1 if ont is None else ont)
         self.x_bar -= (first_time - self.time[-1]) / self.wins
         self.y_bar -= (first_data - ond) / self.wins
         beta = sum([(self.time[i]-self.x_bar)*(self.data[i]-self.y_bar) for i in range(self.wins)]) / sum([(t-self.x_bar)**2 for t in self.time])
         alpha = self.y_bar - beta * self.x_bar
         tres_ = ond - (alpha + beta * self.time[-1])
-        F = self.tres.pop(0)
+        # F = self.tres.pop(0)
         self.tres.append(tres_)
-        return F,tres_
+        return tres_
     
     def replace(self,rep):
         prev = self.data[self.wins-1]
         self.data[self.wins-1] = rep
         self.y_bar -= (prev-rep)/self.wins
```

### Comparing `osesd-1.0.0/src/parameters.py` & `osesd-1.1.0/src/parameters.py`

 * *Files identical despite different names*

### Comparing `osesd-1.0.0/src/utils/data_aug.py` & `osesd-1.1.0/src/utils/data_aug.py`

 * *Files identical despite different names*

### Comparing `osesd-1.0.0/src/utils/scores_module.py` & `osesd-1.1.0/src/utils/scores_module.py`

 * *Files identical despite different names*

