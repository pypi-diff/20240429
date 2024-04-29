# Comparing `tmp/step_machine-0.0.1.tar.gz` & `tmp/step_machine-0.0.2.tar.gz`

## Comparing `step_machine-0.0.1.tar` & `step_machine-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,29 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 step_machine-0.0.1/Makefile
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 step_machine-0.0.1/readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/__init__.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/backend.py
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/cli.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/config.py
--rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/progress.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/target.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/backends/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/backends/core.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/backends/file.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/backends/pg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/templates/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/templates/post_validate.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/templates/pre_check.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 step_machine-0.0.1/src/step_machine/templates/up.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 step_machine-0.0.1/.gitignore
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 step_machine-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 step_machine-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 step_machine-0.0.2/Makefile
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 step_machine-0.0.2/readme.md
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 step_machine-0.0.2/_stepm_history/34f613f7-1cce-418b-86bf-018d8c1b95ae/run_history/00001_s1_20240425024519/status.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 step_machine-0.0.2/_stepm_history/4bf1dd1d-87c5-40b4-8dc0-75c923a112c6/run_history/00001_s1_20240425024537/status.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 step_machine-0.0.2/_stepm_history/bd5cfb31-06bb-47df-9844-2ca726dfccd3/run_history/00001_s1_20240425024548/status.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/__init__.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/backend.py
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/cli.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/config.py
+-rw-r--r--   0        0        0    10897 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/progress.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/target.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/backends/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/backends/core.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/backends/file.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/backends/pg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/templates/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/templates/post_validate.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/templates/pre_check.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/templates/up.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/utils/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/utils/jinja2.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/utils/peewee.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 step_machine-0.0.2/src/step_machine/utils/userdata.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 step_machine-0.0.2/.gitignore
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 step_machine-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 step_machine-0.0.2/PKG-INFO
```

### Comparing `step_machine-0.0.1/src/step_machine/backend.py` & `step_machine-0.0.2/src/step_machine/backend.py`

 * *Files identical despite different names*

### Comparing `step_machine-0.0.1/src/step_machine/cli.py` & `step_machine-0.0.2/src/step_machine/cli.py`

 * *Files identical despite different names*

### Comparing `step_machine-0.0.1/src/step_machine/core.py` & `step_machine-0.0.2/src/step_machine/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     current_time = datetime.now()
     formatted_time = current_time.strftime('%Y%m%d%H%M%S')
     return int(formatted_time)
 
 
 class StepMachineProject:
     STEP_FOLDER_NAME = '_steps'
+    ASSET_FOLDER_NAME = 'assets'
     STEP_CFG_FILE_NAME = 'step_machine_config.json'
 
     project_base: str
     config: SMConfig
 
     steps: list[Step]
     pre_check: str
@@ -175,15 +176,15 @@
         new_meta = step.meta.rename(step.meta.name, new_index=new_index)
         dest = os.path.join(self.steps_base, new_meta.filename())
 
         shutil.move(step_base, dest)
 
     def reorder_all_steps(self):
         steps = self.get_steps(ensure_order=False)
-        sorted_steps = sorted(steps, key=lambda x: x.meta.timestr)
+        sorted_steps = sorted(steps, key=lambda x: x.meta.time_str)
         for idx, step in enumerate(sorted_steps):
             if idx + 1 != step.meta.index:
                 self.reorder_step(step, idx + 1)
 
     def create_new_step(
             self,
             step_name,
@@ -195,45 +196,50 @@
         )
 
         out_file_base = os.path.join(self.steps_base, step.filename())
         os.makedirs(os.path.dirname(out_file_base), exist_ok=True)
         copy_to_target(f'up.py', out_file_base)
         return Step.load_from_file_or_none(out_file_base)
 
+    def get_env(self):
+        return {
+            'SM_ASSET_HOME': os.path.join(self.steps_base, self.ASSET_FOLDER_NAME)
+        }
+
     def execute_single_step(
             self,
             step: Step,
             record_output=True
     ) -> StepStatus:
-        output = run_script('python', step.location)
+        output = run_script('python', step.location, env=self.get_env())
         if output.exit_code == 0:
             status_state = StepStatusState.FINISHED
         else:
             status_state = StepStatusState.FAILED
         new_status = StepStatus(state=status_state, timestamp=output.timestamp, output=output)
 
         if record_output:
             self.get_backend().set_status(self.config.project_name, step.meta, new_status)
         return new_status
 
     def execute_pre_check(self) -> StepStatus:
         p = os.path.join(self.steps_base, 'pre_check.py')
         if os.path.exists(p):
-            output = run_script('python', p)
+            output = run_script('python', p, env=self.get_env())
             if output.exit_code == 0:
                 status_state = StepStatusState.FINISHED
             else:
                 status_state = StepStatusState.FAILED
             new_status = StepStatus(state=status_state, timestamp=output.timestamp, output=output)
             return new_status
 
     def execute_post_validate(self) -> StepStatus:
         p = os.path.join(self.steps_base, 'post_validate.py')
         if os.path.exists(p):
-            output = run_script('python', p)
+            output = run_script('python', p, env=self.get_env())
             if output.exit_code == 0:
                 status_state = StepStatusState.FINISHED
             else:
                 status_state = StepStatusState.FAILED
             new_status = StepStatus(state=status_state, timestamp=output.timestamp, output=output)
             return new_status
```

### Comparing `step_machine-0.0.1/src/step_machine/script.py` & `step_machine-0.0.2/src/step_machine/script.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import hashlib
+import os
 import subprocess
 import sys
 
 import time
 
 from step_machine.types import StepExecutionOutput
 
@@ -23,22 +24,27 @@
         for byte_block in iter(lambda: f.read(4096), b""):
             sha256_hash.update(byte_block)
 
     # Return the hexadecimal representation of the digest
     return sha256_hash.hexdigest()
 
 
-def run_script(entry_point, script_path) -> StepExecutionOutput:
+def run_script(entry_point, script_path, env=None) -> StepExecutionOutput:
+    if env is None:
+        env = {}
+
+    env.update(os.environ)
     # Start the subprocess and specify stdout and stderr to be piped
     with subprocess.Popen(
             [entry_point, script_path],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
             bufsize=1,  # Line-buffered
+            env=env,
     ) as proc:
         # Variables to store captured outputs
         stdout_capture = []
         stderr_capture = []
 
         # Stream stdout and stderr line by line
         while True:
```

### Comparing `step_machine-0.0.1/src/step_machine/types.py` & `step_machine-0.0.2/src/step_machine/types.py`

 * *Files identical despite different names*

### Comparing `step_machine-0.0.1/src/step_machine/backends/file.py` & `step_machine-0.0.2/src/step_machine/backends/file.py`

 * *Files identical despite different names*

### Comparing `step_machine-0.0.1/src/step_machine/backends/pg.py` & `step_machine-0.0.2/src/step_machine/backends/pg.py`

 * *Files identical despite different names*

### Comparing `step_machine-0.0.1/.gitignore` & `step_machine-0.0.2/.gitignore`

 * *Files identical despite different names*

