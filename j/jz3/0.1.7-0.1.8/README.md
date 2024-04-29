# Comparing `tmp/jz3-0.1.7.tar.gz` & `tmp/jz3-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jz3-0.1.7.tar", last modified: Sun Apr 28 16:34:50 2024, max compression
+gzip compressed data, was "jz3-0.1.8.tar", last modified: Mon Apr 29 05:36:08 2024, max compression
```

## Comparing `jz3-0.1.7.tar` & `jz3-0.1.8.tar`

### file list

```diff
@@ -1,45 +1,42 @@
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.436168 jz3-0.1.7/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.7/LICENSE-Z3.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.7/LICENSE.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:30:26.000000 jz3-0.1.7/MANIFEST.in
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-28 16:34:50.436027 jz3-0.1.7/PKG-INFO
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.7/README.md
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.393260 jz3-0.1.7/jz3/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       55 2024-04-26 16:59:15.000000 jz3-0.1.7/jz3/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.394636 jz3-0.1.7/jz3/analysis/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.7/jz3/analysis/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.394874 jz3-0.1.7/jz3/analysis/archive/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.7/jz3/analysis/archive/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.7/jz3/analysis/archive/export_to_excel.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.395770 jz3-0.1.7/jz3/analysis/scripts/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 04:00:01.000000 jz3-0.1.7/jz3/analysis/scripts/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7252 2024-04-19 16:25:42.000000 jz3-0.1.7/jz3/analysis/scripts/compare_whole_problems.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7955 2024-04-28 04:25:24.000000 jz3-0.1.7/jz3/analysis/scripts/plot_comparison.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.396035 jz3-0.1.7/jz3/solvers/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.7/jz3/solvers/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20) 20962472 2024-04-18 02:04:14.000000 jz3-0.1.7/jz3/solvers/cvc5-macOS-arm64
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.429858 jz3-0.1.7/jz3/src/
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.435214 jz3-0.1.7/jz3/src/SMTs/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.7/jz3/src/SMTs/SMTs.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.7/jz3/src/SMTs/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.435341 jz3-0.1.7/jz3/src/Sudokus/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.7/jz3/src/Sudokus/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.7/jz3/src/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       84 2024-04-18 02:04:15.000000 jz3-0.1.7/jz3/src/clean_up.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3542 2024-04-28 05:00:33.000000 jz3-0.1.7/jz3/src/run_solvers.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      282 2024-04-28 04:36:42.000000 jz3-0.1.7/jz3/src/z3_quick_start_guide.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    10939 2024-04-26 02:43:34.000000 jz3-0.1.7/jz3/src/z3_wrapper.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.435584 jz3-0.1.7/jz3/tests/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.7/jz3/tests/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.7/jz3/tests/test_solver.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.435806 jz3-0.1.7/jz3/utils/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 07:53:53.000000 jz3-0.1.7/jz3/utils/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1466 2024-04-28 16:33:47.000000 jz3-0.1.7/jz3/utils/helpers.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 16:34:50.394467 jz3-0.1.7/jz3.egg-info/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-28 16:34:50.000000 jz3-0.1.7/jz3.egg-info/PKG-INFO
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      759 2024-04-28 16:34:50.000000 jz3-0.1.7/jz3.egg-info/SOURCES.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-28 16:34:50.000000 jz3-0.1.7/jz3.egg-info/dependency_links.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-28 16:34:50.000000 jz3-0.1.7/jz3.egg-info/requires.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-28 16:34:50.000000 jz3-0.1.7/jz3.egg-info/top_level.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-28 16:34:50.436223 jz3-0.1.7/setup.cfg
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      894 2024-04-28 16:34:21.000000 jz3-0.1.7/setup.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.363923 jz3-0.1.8/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.8/LICENSE-Z3.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.8/LICENSE.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:30:26.000000 jz3-0.1.8/MANIFEST.in
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-29 05:36:08.363510 jz3-0.1.8/PKG-INFO
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.8/README.md
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.333994 jz3-0.1.8/jz3/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       76 2024-04-28 23:38:27.000000 jz3-0.1.8/jz3/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.334939 jz3-0.1.8/jz3/analysis/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.8/jz3/analysis/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.335129 jz3-0.1.8/jz3/analysis/archive/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.8/jz3/analysis/archive/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.8/jz3/analysis/archive/export_to_excel.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.336335 jz3-0.1.8/jz3/analysis/scripts/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 04:00:01.000000 jz3-0.1.8/jz3/analysis/scripts/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7204 2024-04-29 03:30:57.000000 jz3-0.1.8/jz3/analysis/scripts/compare_whole_problems.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7955 2024-04-28 04:25:24.000000 jz3-0.1.8/jz3/analysis/scripts/plot_comparison.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.336737 jz3-0.1.8/jz3/solvers/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.8/jz3/solvers/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20) 20962472 2024-04-18 02:04:14.000000 jz3-0.1.8/jz3/solvers/cvc5-macOS-arm64
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.358243 jz3-0.1.8/jz3/src/
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.360969 jz3-0.1.8/jz3/src/SMTs/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.8/jz3/src/SMTs/SMTs.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.8/jz3/src/SMTs/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.8/jz3/src/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4545 2024-04-28 23:56:27.000000 jz3-0.1.8/jz3/src/run_solvers.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      282 2024-04-28 04:36:42.000000 jz3-0.1.8/jz3/src/z3_quick_start_guide.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    11111 2024-04-29 03:24:04.000000 jz3-0.1.8/jz3/src/z3_wrapper.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.361525 jz3-0.1.8/jz3/tests/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.8/jz3/tests/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.8/jz3/tests/test_solver.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.362433 jz3-0.1.8/jz3/utils/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 07:53:53.000000 jz3-0.1.8/jz3/utils/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2900 2024-04-28 17:01:30.000000 jz3-0.1.8/jz3/utils/helpers.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.334819 jz3-0.1.8/jz3.egg-info/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/PKG-INFO
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      711 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/SOURCES.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/dependency_links.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/requires.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/top_level.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-29 05:36:08.364165 jz3-0.1.8/setup.cfg
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      894 2024-04-29 05:36:07.000000 jz3-0.1.8/setup.py
```

### Comparing `jz3-0.1.7/LICENSE-Z3.txt` & `jz3-0.1.8/LICENSE-Z3.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.7/LICENSE.txt` & `jz3-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.7/PKG-INFO` & `jz3-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jz3-0.1.7/README.md` & `jz3-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jz3-0.1.7/jz3/analysis/archive/export_to_excel.py` & `jz3-0.1.8/jz3/analysis/archive/export_to_excel.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.7/jz3/analysis/scripts/compare_whole_problems.py` & `jz3-0.1.8/jz3/analysis/scripts/compare_whole_problems.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     print(generate_latex(*timeout_count_lst, constraint_true, constraint_false))
     return timeout_only_true, timeout_both, timeout_only_false, timeout_both
 
 
 if __name__ == '__main__':
     TIME_OUT = 5
 
-    files_directory = '/Users/jiazhenghao/Desktop/CodingProjects/jz3/jz3/time-record/whole_problem_time_records'
+    files_directory = './time-record/whole_problem_time_records'
     # plot_comparison_for_constraint(files_directory, 'distinct', 'PbEq', time_cap=200)  # extended
     plot_name = "full_problem_no_num comparison"
     # plot_comparison_for_constraint(files_directory, 'is_num', 'is_bool',
     #                                time_cap=5,)
     constraint_true_false_lst = [
         ("classic","argyle"),
         ("distinct","PbEq"),
```

### Comparing `jz3-0.1.7/jz3/analysis/scripts/plot_comparison.py` & `jz3-0.1.8/jz3/analysis/scripts/plot_comparison.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.7/jz3/solvers/cvc5-macOS-arm64` & `jz3-0.1.8/jz3/solvers/cvc5-macOS-arm64`

 * *Files identical despite different names*

### Comparing `jz3-0.1.7/jz3/src/SMTs/SMTs.py` & `jz3-0.1.8/jz3/src/SMTs/SMTs.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.7/jz3/src/run_solvers.py` & `jz3-0.1.8/jz3/src/run_solvers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import subprocess
 import time
 import os
 from pathlib import Path
+import warnings
 
+class SMTFileErrorWarning(UserWarning):
+    pass
 
 def run_cvc5(smt2_file, time_out: int = 5):
     cvc_path = get_executable_path("cvc5-macOS-arm64")
     command = [cvc_path, smt2_file, "--lang", "smt2"]
     start_time = time.time()
     did_timeout = False
     try:
@@ -23,14 +26,18 @@
     end_time = time.time()
     total_time = end_time - start_time
     if not did_timeout:
         if "unsat" in combined_output:
             ans = "unsat"
         elif "sat" in combined_output:
             ans = "sat"
+        elif "error" in combined_output.lower() or "unsupported" in combined_output.lower():
+            ans = "error"
+            warning_message = f"CVC5 encountered an error while processing {smt2_file}:\n{combined_output}"
+            warnings.warn(warning_message, SMTFileErrorWarning)
         else:
             ans = "unknown"
     else:
         total_time = time_out
     return (total_time, did_timeout, ans)
 
 
@@ -43,30 +50,37 @@
     start_time = time.time()
     did_timeout = False
     try:
         result = subprocess.run(["z3", "-smt2", smt2_file],
                                 capture_output=True, text=True, timeout=time_out)
         combined_output = ((result.stdout if result.stdout is not None else "") +
                            (result.stderr if result.stderr is not None else ""))  # capture all output
+        print(f'z3 std output: {result.stdout}'
+              f'z3 stderr output: {result.stderr}')
     except subprocess.TimeoutExpired as exc:
         did_timeout = True
+        combined_output = ''
         result = exc
     ans = "timeout"
     end_time = time.time()
     total_time = end_time - start_time
     if not did_timeout:
         if "unsat" in combined_output:
             ans = "unsat"
         elif "sat" in combined_output:
             ans = "sat"
+        elif "error" in combined_output.lower() or "unsupported" in combined_output.lower():
+            ans = "error"
+            warning_message = f"Z3 encountered an error while processing {smt2_file}:\n{combined_output}"
+            warnings.warn(warning_message, SMTFileErrorWarning)
         else:
             ans = "unknown"
     else:
         total_time = time_out
-    return (total_time, did_timeout, ans)
+    return total_time, did_timeout, ans
 
 
 def run_yices(smt2_file):
     command = f"yices-smt2 {smt2_file}"
     try:
         result = subprocess.run(command, shell=True, capture_output=True, text=True, check=True)
         return result.stdout.strip()
@@ -78,19 +92,24 @@
 solvers = {
     "cvc5": run_cvc5,
     "z3": run_z3
     # "yices": run_yices
 }
 
 
-def run_solvers(smt2_file, verbose=False, time_out=5):
+def run_solvers(smt2_file:str='', smt2_str:str='', verbose=False, time_out=5):
     """
     time_out: in seconds
     """
     results = {}
+    if smt2_str and smt2_file=='':
+        smt2_file = os.path.join(os.path.dirname(__file__), 'smt_file.smt2')
+        with open(smt2_file, 'w') as f:
+            f.truncate()
+            f.write(smt2_str)
 
     for solver, run_function in solvers.items():
         if verbose:
             print(f"Running {solver}...")
         result = run_function(smt2_file,time_out=time_out)
         results[solver] = result
```

### Comparing `jz3-0.1.7/jz3/src/z3_wrapper.py` & `jz3-0.1.8/jz3/src/z3_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,32 +106,33 @@
                             if self.__start_recording:
                                 self.__history.append(("add", str(conditional_constraint.sexpr())))
                             solver_with_conditional_constraint.add(conditional_constraint)
 
                     # append the combination to the results
                     # solver_with_conditional_constraint.start_recording()
                     result = solver_with_conditional_constraint.check()
-                    self.__latest_solvers_results.append(run_solvers.run_solvers("conditional_constraints.smt2"))
+                    single_condition_smt_str = solver_with_conditional_constraint.to_smt2()
+                    print(single_condition_smt_str)
+                    self.__latest_solvers_results.append(run_solvers.run_solvers(smt2_str=single_condition_smt_str,verbose=True))
                     self.__condition_var_assignment_model.append(model)
                     min_hamdist = z3.Int("min_hamdist")
 
                     opt.add(min_hamdist <= z3.Sum(
                         tuple(z3.If((var == bool(model[var])), 0, 1) for var in self.__variables)))
-                    # opt.add(min_hamdist <= z3.Sum([0,1,0,1]))
 
                     opt.maximize(min_hamdist)
                     opt.check()
                     model = opt.model()
                     dist = model[min_hamdist].as_long()
                     count += 1
 
                 # store smt file/str
                 self.__smt_str = solver_with_conditional_constraint.generate_smtlib()
 
-                with open("conditional_constraints.smt2", "w") as file:
+                with open("conditional_constraints.smt2", "w") as file: # TODO
                     file.write(self.__smt_str)
 
                 # launch multiple solvers and store resutls
 
             # pop the temporarily added conditional constraints
             if args:
                 self.__assertions.pop()
@@ -204,27 +205,28 @@
     def get_condition_var_assignment_model(self):
         return self.__condition_var_assignment_model
 
     def get_latest_solvers_results(self):
         return self.__latest_solvers_results
 
 
-def simple_test():
+def solver_demo():
     solver = Solver(benchmark_mode=True)
 
     x = z3.Int('x')
     y = z3.Int('y')
 
     solver.add(x > 0)
     solver.add(y > 0)
 
     condition1 = z3.Bool('condition1')
     condition2 = z3.Bool('condition2')
 
     solver.add_global_constraints(z3.Or(condition1, condition2))
+    solver.add_global_constraints(z3.Distinct(condition1,condition2))
 
     solver.add_conditional_constraint(x < 5, condition=condition1)
     solver.add_conditional_constraint(x > 5, condition=condition2)
 
     solver.start_recording()
     result = solver.check_conditional_constraints()
     print(result)
@@ -279,11 +281,10 @@
 
     # Print the combinations
     print("Combination 1:")
     print(combination1)
     print("Combination 2:")
     print(combination2)
 
-
 if __name__ == '__main__':
-    # simple_test()
-    optimizer_test()
+    solver_demo()
+    # optimizer_test()
```

### Comparing `jz3-0.1.7/jz3.egg-info/PKG-INFO` & `jz3-0.1.8/jz3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jz3-0.1.7/jz3.egg-info/SOURCES.txt` & `jz3-0.1.8/jz3.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 jz3/analysis/archive/export_to_excel.py
 jz3/analysis/scripts/__init__.py
 jz3/analysis/scripts/compare_whole_problems.py
 jz3/analysis/scripts/plot_comparison.py
 jz3/solvers/__init__.py
 jz3/solvers/cvc5-macOS-arm64
 jz3/src/__init__.py
-jz3/src/clean_up.py
 jz3/src/run_solvers.py
 jz3/src/z3_quick_start_guide.py
 jz3/src/z3_wrapper.py
 jz3/src/SMTs/SMTs.py
 jz3/src/SMTs/__init__.py
-jz3/src/Sudokus/__init__.py
 jz3/tests/__init__.py
 jz3/tests/test_solver.py
 jz3/utils/__init__.py
 jz3/utils/helpers.py
```

