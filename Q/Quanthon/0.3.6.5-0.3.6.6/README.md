# Comparing `tmp/quanthon-0.3.6.5.tar.gz` & `tmp/quanthon-0.3.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanthon-0.3.6.5.tar", last modified: Fri Apr 26 13:41:46 2024, max compression
+gzip compressed data, was "quanthon-0.3.6.6.tar", last modified: Mon Apr 29 06:18:42 2024, max compression
```

## Comparing `quanthon-0.3.6.5.tar` & `quanthon-0.3.6.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-26 13:41:46.422444 quanthon-0.3.6.5/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 quanthon-0.3.6.5/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-04-26 13:41:46.422211 quanthon-0.3.6.5/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-26 13:41:46.419692 quanthon-0.3.6.5/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 quanthon-0.3.6.5/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      340 2024-04-25 10:06:17.000000 quanthon-0.3.6.5/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     7161 2024-04-26 13:39:58.000000 quanthon-0.3.6.5/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     4727 2024-04-25 10:06:05.000000 quanthon-0.3.6.5/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-10 00:38:34.000000 quanthon-0.3.6.5/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 quanthon-0.3.6.5/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     4775 2024-04-24 11:29:34.000000 quanthon-0.3.6.5/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)     6791 2024-04-25 10:03:08.000000 quanthon-0.3.6.5/Quanthon/mappers_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 quanthon-0.3.6.5/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 quanthon-0.3.6.5/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 quanthon-0.3.6.5/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 quanthon-0.3.6.5/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     6569 2024-04-18 11:08:36.000000 quanthon-0.3.6.5/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-26 13:41:46.421994 quanthon-0.3.6.5/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-04-26 13:41:46.000000 quanthon-0.3.6.5/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      557 2024-04-26 13:41:46.000000 quanthon-0.3.6.5/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-26 13:41:46.000000 quanthon-0.3.6.5/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-26 13:41:46.000000 quanthon-0.3.6.5/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-26 13:41:46.000000 quanthon-0.3.6.5/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 quanthon-0.3.6.5/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-26 13:41:46.422489 quanthon-0.3.6.5/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-26 13:41:43.000000 quanthon-0.3.6.5/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-26 13:41:46.421523 quanthon-0.3.6.5/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 quanthon-0.3.6.5/tests/test_cmp_qk.py
--rw-r--r--   0 bukser     (501) staff       (20)     1472 2024-04-25 10:07:26.000000 quanthon-0.3.6.5/tests/test_mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 quanthon-0.3.6.5/tests/test_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-25 10:07:37.000000 quanthon-0.3.6.5/tests/test_vqes.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-29 06:18:42.495130 quanthon-0.3.6.6/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 quanthon-0.3.6.6/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-04-29 06:18:42.494908 quanthon-0.3.6.6/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-29 06:18:42.492718 quanthon-0.3.6.6/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 quanthon-0.3.6.6/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      340 2024-04-25 10:06:17.000000 quanthon-0.3.6.6/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     7244 2024-04-29 06:12:42.000000 quanthon-0.3.6.6/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4727 2024-04-25 10:06:05.000000 quanthon-0.3.6.6/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-10 00:38:34.000000 quanthon-0.3.6.6/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 quanthon-0.3.6.6/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4775 2024-04-24 11:29:34.000000 quanthon-0.3.6.6/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6791 2024-04-25 10:03:08.000000 quanthon-0.3.6.6/Quanthon/mappers_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 quanthon-0.3.6.6/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 quanthon-0.3.6.6/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 quanthon-0.3.6.6/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 quanthon-0.3.6.6/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6569 2024-04-18 11:08:36.000000 quanthon-0.3.6.6/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-29 06:18:42.494673 quanthon-0.3.6.6/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      557 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 quanthon-0.3.6.6/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-29 06:18:42.495174 quanthon-0.3.6.6/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-29 06:16:24.000000 quanthon-0.3.6.6/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-29 06:18:42.494378 quanthon-0.3.6.6/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 quanthon-0.3.6.6/tests/test_cmp_qk.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1472 2024-04-25 10:07:26.000000 quanthon-0.3.6.6/tests/test_mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 quanthon-0.3.6.6/tests/test_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-25 10:07:37.000000 quanthon-0.3.6.6/tests/test_vqes.py
```

### Comparing `quanthon-0.3.6.5/PKG-INFO` & `quanthon-0.3.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.6.5
+Version: 0.3.6.6
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quanthon-0.3.6.5/Quanthon/Models.py` & `quanthon-0.3.6.6/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/algorithms.py` & `quanthon-0.3.6.6/Quanthon/algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,15 @@
                 op_cand = op
                 max_abs_grad = abs_grad
         
         print("max_abs_grad: ", max_abs_grad)
         
         if max_abs_grad < eps:
             print(f"end of adapt, grad = {max_abs_grad}")
-            return False # gradient = 0, end of adapt 
-        
+            return False # gradient = 0, end of adapt  
         # print(f"appending, op: {op_cand}, grad: {max_abs_grad}")
         # grow the ansatz
         # self.old_gates.append(op_cand) # type(op_cand) == str
         self.params = np.append(self.params, 0)
         self.ansatz.append_op(op_cand)
 
         return True
@@ -180,14 +179,16 @@
             self.params = old_params
             print(f"i: {i}, min_energy = {energy}")
             
 
             if not self._append_operator(eps=grad_eps): # new parameter is added here 
                 break
             
+        if i == max_iter - 1:
+            warnings.warn('Adapt circuit did not converge.')
         self.ansatz.run(self.params) # update the state with the final parameters
         return self.ansatz, energy
     
 
     def minimise_eigenvalue(self, num_shots=10000):
 
         self.num_shots = num_shots
```

### Comparing `quanthon-0.3.6.5/Quanthon/ansatzs.py` & `quanthon-0.3.6.6/Quanthon/ansatzs.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/base.py` & `quanthon-0.3.6.6/Quanthon/base.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/expectation.py` & `quanthon-0.3.6.6/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/mappers.py` & `quanthon-0.3.6.6/Quanthon/mappers.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/mappers_utils.py` & `quanthon-0.3.6.6/Quanthon/mappers_utils.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/ut_pyscf_mel.py` & `quanthon-0.3.6.6/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/ut_qiskit_hamiltonian.py` & `quanthon-0.3.6.6/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/ut_test_jw.py` & `quanthon-0.3.6.6/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon/utils.py` & `quanthon-0.3.6.6/Quanthon/utils.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/Quanthon.egg-info/PKG-INFO` & `quanthon-0.3.6.6/Quanthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.6.5
+Version: 0.3.6.6
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quanthon-0.3.6.5/Quanthon.egg-info/SOURCES.txt` & `quanthon-0.3.6.6/Quanthon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/README.md` & `quanthon-0.3.6.6/README.md`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/setup.py` & `quanthon-0.3.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.6.5" #####
+version = "0.3.6.6" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `quanthon-0.3.6.5/tests/test_cmp_qk.py` & `quanthon-0.3.6.6/tests/test_cmp_qk.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/tests/test_mappers.py` & `quanthon-0.3.6.6/tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.5/tests/test_vqes.py` & `quanthon-0.3.6.6/tests/test_vqes.py`

 * *Files identical despite different names*

