# Comparing `tmp/magnum_opus-2.3.tar.gz` & `tmp/magnum_opus-3.0.tar.gz`

## Comparing `magnum_opus-2.3.tar` & `magnum_opus-3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magnum_opus-2.3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magnum_opus-2.3/MANIFEST.in
--rwxr-xr-x   0        0        0      877 2020-02-02 00:00:00.000000 magnum_opus-2.3/run_tests.sh
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 magnum_opus-2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 magnum_opus-2.3/.vscode/settings.json
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 magnum_opus-2.3/doc/coverage/README.md
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 magnum_opus-2.3/examples/hello_world.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magnum_opus-2.3/src/magnum_opus/__init__.py
--rw-r--r--   0        0        0   156552 2020-02-02 00:00:00.000000 magnum_opus-2.3/src/magnum_opus/operarius.py
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 magnum_opus-2.3/tests/test_hello_world.py
--rw-r--r--   0        0        0   129609 2020-02-02 00:00:00.000000 magnum_opus-2.3/tests/test_models_task.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magnum_opus-2.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 magnum_opus-2.3/LICENSE
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 magnum_opus-2.3/README.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 magnum_opus-2.3/pyproject.toml
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 magnum_opus-2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magnum_opus-3.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magnum_opus-3.0/MANIFEST.in
+-rwxr-xr-x   0        0        0      875 2020-02-02 00:00:00.000000 magnum_opus-3.0/run_tests.sh
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 magnum_opus-3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 magnum_opus-3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 magnum_opus-3.0/doc/coverage/README.md
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 magnum_opus-3.0/examples/hello_world.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magnum_opus-3.0/src/magnum_opus/__init__.py
+-rw-r--r--   0        0        0   113519 2020-02-02 00:00:00.000000 magnum_opus-3.0/src/magnum_opus/operarius.py
+-rw-r--r--   0        0        0    35665 2020-02-02 00:00:00.000000 magnum_opus-3.0/tests/test_hello_world.py
+-rw-r--r--   0        0        0   121445 2020-02-02 00:00:00.000000 magnum_opus-3.0/tests/test_operarius.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magnum_opus-3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 magnum_opus-3.0/LICENSE
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 magnum_opus-3.0/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 magnum_opus-3.0/pyproject.toml
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 magnum_opus-3.0/PKG-INFO
```

### Comparing `magnum_opus-2.3/run_tests.sh` & `magnum_opus-3.0/run_tests.sh`

 * *Files 15% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 export DEBUG=1
 
 rm -frR reports
 mkdir reports
 
 echo ; echo ; echo "########################################################################################################################"
 
-coverage run -a tests/test_models_task.py
+coverage run -a tests/test_hello_world.py
 
 echo ; echo ; echo "########################################################################################################################"
 
-coverage run -a tests/test_hello_world.py
+coverage run -a tests/test_operarius.py
 
 
 echo ; echo ; echo "########################################################################################################################"
 coverage report --omit="tests/test*" -m
 coverage html -d reports --omit="tests/test*","/tmp/test_manifest_classes/*"
 coverage report --format=markdown --omit="tests/test*","/tmp/test_manifest_classes/*" > doc/coverage/README.md
 echo "Report available in file://$PWD/reports/index.html"
```

### Comparing `magnum_opus-2.3/.github/workflows/python-publish.yml` & `magnum_opus-3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `magnum_opus-2.3/examples/hello_world.py` & `magnum_opus-3.0/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `magnum_opus-2.3/tests/test_models_task.py` & `magnum_opus-3.0/tests/test_operarius.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import sys
 import os
-from itertools import permutations
 import hashlib
-from datetime import datetime
+from inspect import stack
 
 sys.path.append(os.path.dirname(os.path.realpath(__file__)) + "/../src")
 print('sys.path={}'.format(sys.path))
 
 import unittest
 
 from magnum_opus.operarius import *
 
 running_path = os.getcwd()
 print('Current Working Path: {}'.format(running_path))
 
 
-class TestLogger(LoggerWrapper):
+class TestLogger:   # pragma: no cover
 
     def __init__(self):
         super().__init__()
         self.info_lines = list()
         self.warn_lines = list()
         self.debug_lines = list()
         self.critical_lines = list()
@@ -59,3121 +58,2947 @@
     def error(self, message: str):
         self.error_lines.append('[LOG] ERROR: {}'.format(message))
         self.all_lines_in_sequence.append(
             copy.deepcopy(self.error_lines[-1])
         )
 
     def reset(self):
+        self.info_lines = None
+        self.warn_lines = None
+        self.debug_lines = None
+        self.critical_lines = None
+        self.error_lines = None
+        self.all_lines_in_sequence = None
         self.info_lines = list()
         self.warn_lines = list()
         self.debug_lines = list()
         self.critical_lines = list()
         self.error_lines = list()
+        self.all_lines_in_sequence = list()
+        print('*** LOGGER RESET DONE ***')
 
 
-def print_logger_lines(logger:LoggerWrapper):
+def print_logger_lines(logger:TestLogger):  # pragma: no cover
+    print('\n\n-------------------------------------------------------------------------------')
+    print('\t\tLOG DUMP')
+    print('\t\t-------------------')
     for line in logger.all_lines_in_sequence:
         print(line)
+    print('\n_______________________________________________________________________________')
 
 
-class TestFunctionKeysToLower(unittest.TestCase):    # pragma: no cover
+def dump_variable_store(test_class_name: str, test_method_name: str, variable_store: VariableStore):
+    try:
+        print('\n\n-------------------------------------------------------------------------------')
+        print('\t\tVARIABLE STORE DUMP')
+        print('\t\t-------------------')
+        print('\t\tTest Class  : {}'.format(test_class_name))
+        print('\t\tTest Method : {}'.format(test_method_name))
+        print()
+
+        # First get the max key length:
+        max_key_len = 0
+        for key,val in variable_store.variable_store.items():
+            if len(key) > max_key_len:
+                max_key_len = len(key)
+
+        for key,val in variable_store.variable_store.items():
+            final_key = '{}'.format(key)
+            spaces_qty = max_key_len - len(final_key) + 1
+            spaces = ' '*spaces_qty
+            final_key = '{}{}: '.format(final_key, spaces)
+            print('{}{}\n'.format(final_key, val))
+
+        print('\n_______________________________________________________________________________')
+    except:
+        pass
+
+
+def dump_events(task_id: str, variable_store: VariableStore):   # pragma: no cover
+    print('\n\n-------------------------------------------------------------------------------')
+    print('\t\tEVENTS for task  : {}'.format(task_id))
+    print()
+    event_key = '{}:PROCESSING_EVENTS'.format(task_id)
+    if event_key in variable_store.variable_store:
+        if variable_store.variable_store[event_key] is not None:
+            if isinstance(variable_store.variable_store[event_key], list):
+                for event in variable_store.variable_store[event_key]:
+                    print(json.dumps(event, default=str))
+    print('\n_______________________________________________________________________________')
+
+
+def dump_state(task: Task, persistence: StatePersistence):   # pragma: no cover
+    print('\n\n-------------------------------------------------------------------------------')
+    print('\t\tSTATE for task  : {}'.format(task.task_id))
+    print()
+    try:
+        current_state = persistence.get(object_identifier='{}:TASK_STATE'.format(task.task_id))
+        print('{}'.format(json.dumps(current_state, default=str, indent=4)))
+    except:
+        print('No state available.')
+    print('\n_______________________________________________________________________________')
+
+
+test_logger = TestLogger()
+logger = test_logger
+override_logger(logger_class=test_logger)
+
+
+class DummyTaskProcessor1(TaskProcessor):
+
+    def __init__(self, api_version: str='DummyTaskProcessor1/v1') -> None:
+        super().__init__(api_version)
+
+    def create_action(
+        self,
+        task: Task,
+        persistence: StatePersistence=StatePersistence(),
+        variable_store: VariableStore=VariableStore(),
+        task_resolved_spec: dict=dict()
+    )->VariableStore:
+        updated_variable_store = VariableStore()
+        updated_variable_store.variable_store = copy.deepcopy(variable_store.variable_store)
+
+        if self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION') in updated_variable_store.variable_store:
+            if updated_variable_store.get_variable(variable_name=self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION')) is True:
+                raise Exception('CreateAction Failed!')
+
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='TASK_ORIGINAL_SPEC_CHECKSUM'),
+            value=hashlib.sha256(json.dumps(task.spec, default=str).encode('utf-8')).hexdigest()
+        )
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='TASK_RESOLVED_SPEC_CHECKSUM'),
+            value=hashlib.sha256(json.dumps(task_resolved_spec, default=str).encode('utf-8')).hexdigest()
+        )
+
+        if self.create_identifier(task=task, variable_name='PROCESSING_EVENTS') not in variable_store.variable_store:
+            updated_variable_store.add_variable(
+                variable_name=self.create_identifier(task=task, variable_name='PROCESSING_EVENTS'),
+                value=list()
+            )
+
+        if self.create_identifier(task=task, variable_name='UNITTEST_FORCE_PROCESSING_EXCEPTION') in variable_store.variable_store:
+            if variable_store.variable_store[self.create_identifier(task=task, variable_name='UNITTEST_FORCE_PROCESSING_EXCEPTION')] is not None:
+                if isinstance(variable_store.variable_store[self.create_identifier(task=task, variable_name='UNITTEST_FORCE_PROCESSING_EXCEPTION')], bool):
+                    if variable_store.variable_store[self.create_identifier(task=task, variable_name='UNITTEST_FORCE_PROCESSING_EXCEPTION')] is True:
+                        raise Exception('Exception Forced By Unit Test Configuration')
+        
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='TASK_STATE_UPDATES'),
+            value={
+                'resource_checksum': hashlib.sha256('CreateAction for UnitTest Completed'.encode('utf-8')).hexdigest(),
+                'resolved_spec_applied': copy.deepcopy(task_resolved_spec),
+                'state_changed': True,
+                'is_created': True,
+                'create_timestamp': int(datetime.now(timezone.utc).timestamp()),
+                'raw_spec': copy.deepcopy(task.spec),
+                'metadata': copy.deepcopy(task.metadata),
+            }
+        )
 
-    def setUp(self):
-        print()
-        print('-'*80)
+        return updated_variable_store
+    
+    def rollback_action(
+        self,
+        task: Task,
+        persistence: StatePersistence=StatePersistence(),
+        variable_store: VariableStore=VariableStore(),
+        task_resolved_spec: dict=dict()
+    )->VariableStore:
+        updated_variable_store = VariableStore()
+        updated_variable_store.variable_store = copy.deepcopy(variable_store.variable_store)
+        if self.create_identifier(task=task, variable_name='TASK_ORIGINAL_SPEC_CHECKSUM') in updated_variable_store.variable_store:
+            updated_variable_store = self.delete_action(
+                task=task,
+                persistence=persistence,
+                variable_store=copy.deepcopy(updated_variable_store),
+                task_resolved_spec=task_resolved_spec
+            )
+        else:
+            if '__GLOBAL__:PROCESS_TASK_EXCEPTION_RAISED_FOR_ACTION' in updated_variable_store.variable_store:
+                if updated_variable_store.get_variable(variable_name='__GLOBAL__:PROCESS_TASK_EXCEPTION_RAISED_FOR_ACTION') == 'CreateAction':
+                    return updated_variable_store 
+            updated_variable_store = self.create_action(
+                task=task,
+                persistence=persistence,
+                variable_store=copy.deepcopy(updated_variable_store),
+                task_resolved_spec=task_resolved_spec
+            )
+        return updated_variable_store
+    
+    def delete_action(
+        self,
+        task: Task,
+        persistence: StatePersistence=StatePersistence(),
+        variable_store: VariableStore=VariableStore(),
+        task_resolved_spec: dict=dict()
+    )->VariableStore:
+        updated_variable_store = VariableStore()
+        updated_variable_store.variable_store = copy.deepcopy(variable_store.variable_store)
+
+        if self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION') in updated_variable_store.variable_store:
+            if updated_variable_store.get_variable(variable_name=self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION')) is True:
+                raise Exception('DeleteAction Failed!')
+        
+        if self.create_identifier(task=task, variable_name='TASK_ORIGINAL_SPEC_CHECKSUM') in updated_variable_store.variable_store:
+            updated_variable_store.variable_store.pop(self.create_identifier(task=task, variable_name='TASK_ORIGINAL_SPEC_CHECKSUM'))
+        if self.create_identifier(task=task, variable_name='TASK_RESOLVED_SPEC_CHECKSUM') in updated_variable_store.variable_store:
+            updated_variable_store.variable_store.pop(self.create_identifier(task=task, variable_name='TASK_RESOLVED_SPEC_CHECKSUM'))
+        
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='TASK_STATE_UPDATES'),
+            value={
+                'resource_checksum': None,
+                'resolved_spec_applied': copy.deepcopy(task_resolved_spec),
+                'state_changed': True,
+                'is_created': False,
+                'create_timestamp': 0,
+                'raw_spec': copy.deepcopy(task.spec),
+                'metadata': copy.deepcopy(task.metadata),
+            }
+        )
 
-    def test_keys_to_lower_1(self):
-        d = {
-            'a': 'AA',
-            'Bb': {
-                'c': 123,
-                'dD': True
-            },
-            'ccC': [ 1,2,3, ]
-        }
-        df = keys_to_lower(data=d)
-        print('df={}'.format(df))
-        self.assertIsNotNone(df)
-        self.assertIsInstance(df, dict)
-        self.assertEqual(len(df), len(d))
-        self.assertTrue('a' in df)
-        self.assertTrue('bb' in df)
-        self.assertTrue('ccc' in df)
-        bb = df['bb']
-        self.assertTrue('c' in bb)
-        self.assertTrue('dd' in bb)
+        return updated_variable_store
+    
+    def update_action(
+        self,
+        task: Task,
+        persistence: StatePersistence=StatePersistence(),
+        variable_store: VariableStore=VariableStore(),
+        task_resolved_spec: dict=dict()
+    )->VariableStore:
+        updated_variable_store = VariableStore()
+        updated_variable_store.variable_store = copy.deepcopy(variable_store.variable_store)
+
+        if self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION') in updated_variable_store.variable_store:
+            if updated_variable_store.get_variable(variable_name=self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION')) is True:
+                raise Exception('DeleteAction Failed!')
+        
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='TASK_STATE_UPDATES'),
+            value={
+                'resource_checksum': hashlib.sha256('UpdateAction for UnitTest Completed'.encode('utf-8')).hexdigest(),
+                'resolved_spec_applied': copy.deepcopy(task_resolved_spec),
+                'state_changed': True,
+                'is_created': True,
+                'create_timestamp': int(datetime.now(timezone.utc).timestamp()),
+                'raw_spec': copy.deepcopy(task.spec),
+                'metadata': copy.deepcopy(task.metadata),
+            }
+        )
 
+        return updated_variable_store
+    
+    def describe_action(
+        self,
+        task: Task,
+        persistence: StatePersistence=StatePersistence(),
+        variable_store: VariableStore=VariableStore(),
+        task_resolved_spec: dict=dict()
+    )->VariableStore:
+        updated_variable_store = VariableStore()
+        updated_variable_store.variable_store = copy.deepcopy(variable_store.variable_store)
+
+        if self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION') in updated_variable_store.variable_store:
+            if updated_variable_store.get_variable(variable_name=self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION')) is True:
+                raise Exception('UpdateAction Failed!')
+        
+        resource_checksum = hashlib.sha256('test_resource'.encode('utf-8')).hexdigest()
+        if 'ResourceData:{}'.format(task.task_id) in variable_store.variable_store:
+            resource_checksum = hashlib.sha256(
+                variable_store.variable_store['ResourceData:{}'.format(task.task_id)].encode('utf-8')
+            ).hexdigest()
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='TASK_DESCRIPTION_RAW'),
+            value=copy.deepcopy(
+                task.state.to_dict(
+                    human_readable=False,
+                    current_resolved_spec=task_resolved_spec,
+                    current_resource_checksum=resource_checksum,
+                    with_checksums=True,
+                    include_applied_spec=True
+                )
+            )
+        )
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='TASK_DESCRIPTION_HUMAN_READABLE_SUMMARY'),
+            value=copy.deepcopy(
+                task.state.to_dict(
+                    human_readable=True,
+                    current_resolved_spec=task_resolved_spec,
+                    current_resource_checksum=resource_checksum,
+                    with_checksums=False,
+                    include_applied_spec=False
+                )
+            )
+        )
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='TASK_DESCRIPTION_HUMAN_READABLE_EXTENDED'),
+            value=copy.deepcopy(
+                task.state.to_dict(
+                    human_readable=True,
+                    current_resolved_spec=task_resolved_spec,
+                    current_resource_checksum=resource_checksum,
+                    with_checksums=True,
+                    include_applied_spec=False
+                )
+            )
+        )
+        return updated_variable_store
+    
+    def detect_drift_action(
+        self,
+        task: Task,
+        persistence: StatePersistence=StatePersistence(),
+        variable_store: VariableStore=VariableStore(),
+        task_resolved_spec: dict=dict()
+    )->VariableStore:
+        updated_variable_store = VariableStore()
+        updated_variable_store.variable_store = copy.deepcopy(variable_store.variable_store)
+
+        if self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION') in updated_variable_store.variable_store:
+            if updated_variable_store.get_variable(variable_name=self.create_identifier(task=task, variable_name='UNITTEST_TROW_EXCEPTION')) is True:
+                raise Exception('DetectDriftAction Failed!')
+        
+        resource_checksum = hashlib.sha256('test_resource'.encode('utf-8')).hexdigest()
+        if 'ResourceData:{}'.format(task.task_id) in variable_store.variable_store:
+            resource_checksum = hashlib.sha256(
+                variable_store.variable_store['ResourceData:{}'.format(task.task_id)].encode('utf-8')
+            ).hexdigest()
 
-class TestObjectInstanceGlobalKeyValueStore(unittest.TestCase):    # pragma: no cover
+        current_task_state = task.state.to_dict(
+            human_readable=False,
+            current_resolved_spec=task_resolved_spec,
+            current_resource_checksum=resource_checksum,
+            with_checksums=True,
+            include_applied_spec=True
+        )
+        spec_drifted = False
+        resource_drifted = False
+        if 'IsCreated' in current_task_state:
+            if isinstance(current_task_state['IsCreated'], bool):
+                if current_task_state['IsCreated'] is True:
+                    if 'SpecDrifted' in current_task_state and 'ResourceDrifted' in current_task_state:
+                        if isinstance(current_task_state['SpecDrifted'], bool):
+                            spec_drifted = current_task_state['SpecDrifted']
+                        if isinstance(current_task_state['ResourceDrifted'], bool):
+                            resource_drifted = current_task_state['ResourceDrifted']
 
-    def setUp(self):
-        print()
-        print('-'*80)
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='SPEC_DRIFTED'),
+            value=spec_drifted
+        )
+        updated_variable_store.add_variable(
+            variable_name=self.create_identifier(task=task, variable_name='RESOURCE_DRIFTED'),
+            value=resource_drifted
+        )
 
-    def test_global_key_value_store_basic(self):
-        global_key_value_store = KeyValueStore()
-        self.assertIsInstance(global_key_value_store, KeyValueStore)
-        global_key_value_store.save(key='test_key_1', value='test_value')
-        global_key_value_store.save(key='test_key_2', value=123)
-        global_key_value_store.save(key='test_key_3', value=True)
-        self.assertEqual(len(global_key_value_store.store), 3)
-        self.assertTrue('test_key_1' in global_key_value_store.store)
-        self.assertTrue('test_key_2' in global_key_value_store.store)
-        self.assertTrue('test_key_3' in global_key_value_store.store)
-        self.assertIsInstance(global_key_value_store.store['test_key_1'], str)
-        self.assertIsInstance(global_key_value_store.store['test_key_2'], int)
-        self.assertIsInstance(global_key_value_store.store['test_key_3'], bool)
+        return updated_variable_store
 
 
-class TestClassTask(unittest.TestCase):    # pragma: no cover
+class TestDummyTaskProcessor1(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
-        self.logger = TestLogger()
+        self.task = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task'},
+            spec={'testField': 'testValue'}
+        )
 
-    def tearDown(self):
-        for line in self.logger.info_lines:
-            print(line)
-        for line in self.logger.warn_lines:
-            print(line)
-        for line in self.logger.debug_lines:
-            print(line)
-        for line in self.logger.critical_lines:
-            print(line)
-        for line in self.logger.error_lines:
-            print(line)
-
-    def test_task_basic_init_minimal_1(self):
-        spec_test_field_name = 'TestField1'
-        t = Task(kind='TestKind', version='v1', spec={spec_test_field_name: 'value1'}, metadata=dict(), logger=self.logger)
-        self.assertIsNotNone(t)
-        self.assertIsInstance(t, Task)
-        self.assertEqual(t.kind, 'TestKind')
+    def test_create_action_01(self):
+        p = DummyTaskProcessor1()
+        t = copy.deepcopy(self.task)
+        variable_store = p.process_task(
+            task=t,
+            variable_store=VariableStore(),
+            action='CreateAction',
+            task_resolved_spec=copy.deepcopy(t.spec)
+        )
 
-        match_found = False
-        for line in self.logger.info_lines:
-            if 'initialized. Task checksum:' in line:
-                match_found = True
-        self.assertTrue(match_found)
-
-        task_metadata = t.metadata
-        self.assertIsNotNone(task_metadata)
-        self.assertIsInstance(task_metadata, dict)
-        self.assertEqual(len(task_metadata), 0)
-
-        task_spec = t.spec
-        self.assertIsNotNone(task_spec)
-        self.assertIsInstance(task_spec, dict)
-        self.assertEqual(len(task_spec), 1)
-        self.assertTrue(spec_test_field_name.lower() in task_spec)
-
-        task_annotations = t.annotations
-        self.assertIsNotNone(task_annotations)
-        self.assertIsInstance(task_annotations, dict)
-        self.assertEqual(len(task_annotations), 0)
-
-        task_dependencies = t.task_dependencies
-        self.assertIsNotNone(task_dependencies)
-        self.assertIsInstance(task_dependencies, list)
-        self.assertEqual(len(task_dependencies), 0)
-        
-        data = dict(t)
-        self.assertIsNotNone(data)
-        self.assertIsInstance(data, dict)
-        self.assertEqual(len(data), 3)
-        self.assertTrue('kind' in data)
-        self.assertTrue('version' in data)
-        self.assertTrue('spec' in data)
-
-    def test_task_basic_init_minimal_with_name_1(self):
-        metadata = {
-            "identifiers": [
-                {
-                    "type": "ManifestName",
-                    "key": "test1"
-                }
-            ]
-        }
-        t = Task(kind='TestKind', version='v1', spec={'field1': 'value1'}, metadata=metadata, logger=self.logger)
-        self.assertIsNotNone(t)
-        self.assertIsInstance(t, Task)
-        self.assertEqual(t.kind, 'TestKind')
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
+        )
+        dump_events(
+            task_id=t.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertTrue('test-task:TASK_ORIGINAL_SPEC_CHECKSUM' in variable_store.variable_store)
+        self.assertTrue('test-task:TASK_RESOLVED_SPEC_CHECKSUM' in variable_store.variable_store)
+        self.assertEqual(
+            variable_store.variable_store['test-task:TASK_ORIGINAL_SPEC_CHECKSUM'],
+            variable_store.variable_store['test-task:TASK_RESOLVED_SPEC_CHECKSUM']
+        )
+
+    def test_describe_action_01(self):
+        p = DummyTaskProcessor1()
+        t = copy.deepcopy(self.task)
+        variable_store = VariableStore()
+        resolved_spec = copy.deepcopy(self.task.spec)
+        if 'ResolvedSpec:{}'.format(self.task.task_id) in variable_store.variable_store:
+            resolved_spec = copy.deepcopy(variable_store.variable_store['ResolvedSpec:{}'.format(self.task.task_id)])
+        variable_store = p.process_task(
+            task=t,
+            variable_store=copy.deepcopy(variable_store),
+            action='DescribeAction',
+            task_resolved_spec=resolved_spec
+        )
 
-        match_found = False
-        for line in self.logger.info_lines:
-            if 'initialized. Task checksum:' in line:
-                match_found = True
-        self.assertTrue(match_found)
-
-        match_1 = t.task_match_name(name='test1')
-        match_2 = t.task_match_name(name='test2')
-
-        self.assertTrue(match_1)
-        self.assertFalse(match_2)
-
-    def test_task_basic_init_minimal_with_name_and_value_1(self):
-        identifier_type = 'Label'
-        identifier_key = 'test1'
-        identifier_val = 'val2'
-        metadata = {
-            "identifiers": [
-                {
-                    "type": identifier_type,
-                    "key": identifier_key,
-                    "val": identifier_val,
-                }
-            ]
-        }
-        t = Task(kind='TestKind', version='v1', spec={'field1': 'value1'}, metadata=metadata, logger=self.logger)
-        self.assertIsNotNone(t)
-        self.assertIsInstance(t, Task)
-        self.assertEqual(t.kind, 'TestKind')
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=variable_store
+        )
+        dump_events(
+            task_id=t.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertTrue('test-task:TASK_DESCRIPTION_RAW' in variable_store.variable_store)
+        self.assertTrue('test-task:TASK_DESCRIPTION_HUMAN_READABLE_SUMMARY' in variable_store.variable_store)
+        self.assertTrue('test-task:TASK_DESCRIPTION_HUMAN_READABLE_EXTENDED' in variable_store.variable_store)
 
-        matching_identifier = Identifier(identifier_type=identifier_type, key=identifier_key, val=identifier_val)
-        none_matching_identifier_1 = Identifier(identifier_type=identifier_type, key=identifier_key, val='wrong')
-        none_matching_identifier_2 = Identifier(identifier_type=identifier_type, key='wrong', val=identifier_val)
-        none_matching_identifier_3 = Identifier(identifier_type='wrong', key=identifier_key, val=identifier_val)
-        self.assertTrue(t.match_name_or_label_identifier(identifier=matching_identifier))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_1))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_2))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_3))
-
-    def test_task_basic_init_minimal_with_name_and_value_2(self):
-        identifier_type = 'Label'
-        identifier_key = 'test1'
-        identifier_val = 'val2'
-        metadata = {
-            "identifiers": [
-                {
-                    "type": identifier_type,
-                    "key": identifier_key,
-                    "value": identifier_val,
-                }
-            ]
-        }
-        t = Task(kind='TestKind', version='v1', spec={'field1': 'value1'}, metadata=metadata, logger=self.logger)
-        self.assertIsNotNone(t)
-        self.assertIsInstance(t, Task)
-        self.assertEqual(t.kind, 'TestKind')
+    def test_drift_action_no_drift_detected_01(self):
+        
+        p = DummyTaskProcessor1()
+        t = copy.deepcopy(self.task)
+        t.state = TaskState(
+            report_label=copy.deepcopy(t.task_id),
+            manifest_spec=copy.deepcopy(t.spec),
+            manifest_metadata=copy.deepcopy(t.metadata),
+            applied_spec=copy.deepcopy(t.spec),
+            resolved_spec=copy.deepcopy(t.spec),
+            created_timestamp=1000, 
+            applied_resources_checksum=hashlib.sha256('test_resource'.encode('utf-8')).hexdigest()
+        )
+        variable_store = VariableStore()
+        variable_store.add_variable(
+            variable_name='ResourceData:{}'.format(t.task_id),
+            value='test_resource'
+        )
+        resolved_spec = copy.deepcopy(self.task.spec)
+        if 'ResolvedSpec:{}'.format(self.task.task_id) in variable_store.variable_store:
+            resolved_spec = copy.deepcopy(variable_store.variable_store['ResolvedSpec:{}'.format(self.task.task_id)])
+        variable_store = p.process_task(
+            task=t,
+            variable_store=copy.deepcopy(variable_store),
+            action='DetectDriftAction',
+            task_resolved_spec=resolved_spec
+        )
 
-        matching_identifier = Identifier(identifier_type=identifier_type, key=identifier_key, val=identifier_val)
-        none_matching_identifier_1 = Identifier(identifier_type=identifier_type, key=identifier_key, val='wrong')
-        none_matching_identifier_2 = Identifier(identifier_type=identifier_type, key='wrong', val=identifier_val)
-        none_matching_identifier_3 = Identifier(identifier_type='wrong', key=identifier_key, val=identifier_val)
-        self.assertTrue(t.match_name_or_label_identifier(identifier=matching_identifier))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_1))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_2))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_3))
-
-    def test_task_basic_init_minimal_with_name_and_value_3(self):
-        identifier_type = 'Label'
-        identifier_key = 'test1'
-        metadata = {
-            "contextualIdentifiers": [
-                {
-                    "type": identifier_type,
-                    "key": identifier_key,
-                    "contexts": [
-                        {
-                            "type": "Environment",
-                            "names": [
-                                "c1",
-                                "c2"
-                            ]
-                        }
-                    ]
-                }
-            ]
-        }
-        t = Task(kind='TestKind', version='v1', spec={'field1': 'value1'}, metadata=metadata, logger=self.logger)
-        self.assertIsNotNone(t)
-        self.assertIsInstance(t, Task)
-        self.assertEqual(t.kind, 'TestKind')
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=variable_store
+        )
+        dump_events(
+            task_id=t.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertTrue('test-task:SPEC_DRIFTED' in variable_store.variable_store)
+        self.assertTrue('test-task:RESOURCE_DRIFTED' in variable_store.variable_store)
+        self.assertIsInstance(variable_store.variable_store['test-task:SPEC_DRIFTED'], bool)
+        self.assertIsInstance(variable_store.variable_store['test-task:RESOURCE_DRIFTED'], bool)
+        self.assertFalse(variable_store.variable_store['test-task:SPEC_DRIFTED'])
+        self.assertFalse(variable_store.variable_store['test-task:RESOURCE_DRIFTED'])
 
-        matching_contexts_1 = IdentifierContexts()
-        matching_contexts_1.add_identifier_context(
-            identifier_context=IdentifierContext(context_type='Environment', context_name='c1')
-        )
-        matching_contexts_1.add_identifier_context(
-            identifier_context=IdentifierContext(context_type='Environment', context_name='c2')
-        )
-        matching_contexts_2 = IdentifierContexts()
-        matching_contexts_2.add_identifier_context(
-            identifier_context=IdentifierContext(context_type='Environment', context_name='c1')
-        )
-        matching_contexts_3 = IdentifierContexts()
-        matching_contexts_3.add_identifier_context(
-            identifier_context=IdentifierContext(context_type='Environment', context_name='c2')
-        )
-
-        none_matching_contexts_1 = IdentifierContexts()
-        none_matching_contexts_1.add_identifier_context(
-            identifier_context=IdentifierContext(context_type='Environment', context_name='c3')
-        )
-
-        matching_identifier_1 = Identifier(identifier_type=identifier_type, key=identifier_key, identifier_contexts=matching_contexts_1)
-        matching_identifier_2 = Identifier(identifier_type=identifier_type, key=identifier_key, identifier_contexts=matching_contexts_2)
-        matching_identifier_3 = Identifier(identifier_type=identifier_type, key=identifier_key, identifier_contexts=matching_contexts_3)
-        none_matching_identifier_1 = Identifier(identifier_type=identifier_type, key=identifier_key, val='wrong')
-        none_matching_identifier_2 = Identifier(identifier_type=identifier_type, key='wrong')
-        none_matching_identifier_3 = Identifier(identifier_type='wrong', key=identifier_key)
-        none_matching_identifier_4 = Identifier(identifier_type=identifier_type, key=identifier_key, identifier_contexts=none_matching_contexts_1)
-        self.assertTrue(t.match_name_or_label_identifier(identifier=matching_identifier_1))
-        self.assertTrue(t.match_name_or_label_identifier(identifier=matching_identifier_2))
-        self.assertTrue(t.match_name_or_label_identifier(identifier=matching_identifier_3))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_1))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_2))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_3))
-        self.assertFalse(t.match_name_or_label_identifier(identifier=none_matching_identifier_4))
-
-    def test_task_basic_init_minimal_with_no_name_produces_debug_message_when_lookup_by_name_is_done(self):
-        t = Task(kind='TestKind', version='v1', spec={'field1': 'value1'}, metadata=dict(), logger=self.logger)
-        match_1 = t.task_match_name(name='test1')
-        self.assertFalse(match_1)
-
-    def test_task_basic_init_minimal_with_name_and_labels_1(self):
-        metadata = {
-            "identifiers": [
-                {
-                    "type": "ManifestName",
-                    "key": "test1"
-                },
-                {
-                    "type": "Label",
-                    "key": "label1",
-                    "value": "labelvalue1"
-                },
-                {
-                    "type": "Label",
-                    "key": "label2",
-                    "value": "labelvalue2"
-                },
-            ]
-        }
-        t = Task(kind='TestKind', version='v1', spec={'field1': 'value1'}, metadata=metadata, logger=self.logger)
-        self.assertIsNotNone(t)
-        self.assertIsInstance(t, Task)
-        self.assertEqual(t.kind, 'TestKind')
 
-        match_1a = t.task_match_name(name='test1')
-        match_1b = t.task_match_label(key='label1', value='labelvalue1')
-        match_1c = t.task_match_label(key='label2', value='labelvalue2')
-        match_2a = t.task_match_name(name='test2')
-        match_2b = t.task_match_label(key='label1', value='labelvalue2')
-        match_2c = t.task_match_label(key='label2', value='labelvalue1')
-        match_2d = t.task_match_label(key='label3', value='labelvalue3')
-        
-        self.assertTrue(match_1a)
-        self.assertTrue(match_1b)
-        self.assertTrue(match_1c)
-        self.assertFalse(match_2a)
-        self.assertFalse(match_2b)
-        self.assertFalse(match_2c)
-        self.assertFalse(match_2d)
-
-    def test_task_basic_init_minimal_with_annotations_1(self):
-        custom_annotation_value = 'customvalue1'
-        custom_annotation_name = 'thirdparty/annotation/name1'
-        t = Task(
-            kind='TestKind',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "name1" },
-                            { "key": "name2" },
-                        ]
-                    },
-                    {
-                        "identifierType": "Label",
-                        "identifiers": [
-                            { "key": "labelname1", "value": "labelvalue1" },
-                        ]
-                    }
-                ],
-                "annotations": {
-                    custom_annotation_name: custom_annotation_value,
-                }
-            },
-            logger=self.logger
+    def test_drift_action_only_resource_drift_detected_01(self):
+        
+        p = DummyTaskProcessor1()
+        t = copy.deepcopy(self.task)
+        t.state = TaskState(
+            report_label=copy.deepcopy(t.task_id),
+            manifest_spec=copy.deepcopy(t.spec),
+            manifest_metadata=copy.deepcopy(t.metadata),
+            applied_spec=copy.deepcopy(t.spec),
+            resolved_spec=copy.deepcopy(t.spec),
+            created_timestamp=1000, 
+            applied_resources_checksum=hashlib.sha256('test_resource_original'.encode('utf-8')).hexdigest()
+        )
+        variable_store = VariableStore()
+        variable_store.add_variable(
+            variable_name='ResourceData:{}'.format(t.task_id),
+            value='test_resource'
+        )
+        resolved_spec = copy.deepcopy(self.task.spec)
+        if 'ResolvedSpec:{}'.format(self.task.task_id) in variable_store.variable_store:
+            resolved_spec = copy.deepcopy(variable_store.variable_store['ResolvedSpec:{}'.format(self.task.task_id)])
+        variable_store = p.process_task(
+            task=t,
+            variable_store=copy.deepcopy(variable_store),
+            action='DetectDriftAction',
+            task_resolved_spec=resolved_spec
         )
 
-        custom_annotations = t.annotations
-        self.assertIsNotNone(custom_annotations)
-        self.assertIsInstance(custom_annotations, dict)
-        self.assertEqual(len(custom_annotations), 1, 'custom_annotations: {}'.format(custom_annotations))
-        self.assertTrue(custom_annotation_name in custom_annotations)
-        self.assertEqual(custom_annotations[custom_annotation_name], custom_annotation_value)
-
-        dependencies = t.task_dependencies
-        self.assertIsNotNone(dependencies)
-        self.assertIsInstance(dependencies, list)
-        self.assertEqual(len(dependencies), 3, 'dependencies: {}'.format(dependencies))
-        for dependency in dependencies:
-            self.assertIsInstance(dependency, Identifier)
-
-
-class Processor1(TaskProcessor):
-
-    def __init__(self, logger: LoggerWrapper=TestLogger()):
-        super().__init__(kind='Processor1', kind_versions=['v1'], supported_commands=['command1', 'command2'], logger=logger)
-
-    def process_task(self, task: Task, command: str, context: str='default', key_value_store: KeyValueStore=KeyValueStore(), state_persistence: StatePersistence=StatePersistence())->KeyValueStore:
-        self.logger.info('[Processor1]: {}'.format('-'*80))
-        self.logger.info('[Processor1]: Processing task_id : "{}"'.format(task.task_id))
-        self.logger.info('[Processor1]: command            : "{}"'.format(command))
-        self.logger.info('[Processor1]: context            : "{}"'.format(context))
-        self.logger.info('[Processor1]: Processing Method  : "process_task()"')
-        new_key_value_store = KeyValueStore()
-        new_key_value_store.store = copy.deepcopy(key_value_store.store)
-        current_state = self.state_persistence.get_object_state(object_identifier=task.task_id)
-        can_process = True
-        if task.kind != 'Processor1':
-            self.logger.error('[Processor1]: Task kind "{}" mismatched and the task will NOT be processed'.format(task.kind))
-            can_process = False
-            current_state = {'ResourcesCreated': False}
-        if task.version not in self.versions:
-            self.logger.error('[Processor1]: Task version "{}" is not supported and the task will NOT be processed'.format(task.version))
-            can_process = False
-            current_state = {'ResourcesCreated': False}
-        if len(current_state) > 0:
-            self.logger.error('[Processor1]: Task version "{}" is already in the correct state'.format(task.version))
-            can_process = False
-        else:
-            current_state = {'ResourcesCreated': False}
-        self.logger.info('[Processor1]: can_process={}'.format(can_process))
-        if can_process is True:
-            # Emulate processing....
-            current_state = {'ResourcesCreated': True}
-            self.state_persistence.save_object_state(object_identifier=task.task_id, data={'ResourcesCreated': True})
-        new_key_value_store.save(key='Processor1:Processed:{}:Success'.format(task.task_id), value=current_state['ResourcesCreated'])
-        self.logger.info('[Processor1]: {}'.format('='*80))
-        return new_key_value_store
-    
-    def process_task_alternate_method(self, task: Task, command: str, context: str='default', key_value_store: KeyValueStore=KeyValueStore(), state_persistence: StatePersistence=StatePersistence())->KeyValueStore:
-        self.logger.info('[Processor1]: {}'.format('-'*80))
-        self.logger.info('[Processor1]: Processing task_id : "{}"'.format(task.task_id))
-        self.logger.info('[Processor1]: command            : "{}"'.format(command))
-        self.logger.info('[Processor1]: context            : "{}"'.format(context))
-        self.logger.info('[Processor1]: Processing Method  : "process_task_alternate_method()"')
-        new_key_value_store = KeyValueStore()
-        new_key_value_store.store = copy.deepcopy(key_value_store.store)
-        current_state = self.state_persistence.get_object_state(object_identifier=task.task_id)
-        can_process = True
-        if task.kind != 'Processor1':
-            self.logger.error('[Processor1]: Task kind "{}" mismatched and the task will NOT be processed'.format(task.kind))
-            can_process = False
-            current_state = {'ResourcesCreated': False}
-        if task.version not in self.versions:
-            self.logger.error('[Processor1]: Task version "{}" is not supported and the task will NOT be processed'.format(task.version))
-            can_process = False
-            current_state = {'ResourcesCreated': False}
-        if len(current_state) > 0:
-            self.logger.error('[Processor1]: Task version "{}" is already in the correct state'.format(task.version))
-            can_process = False
-        else:
-            current_state = {'ResourcesCreated': False}
-        self.logger.info('[Processor1]: can_process={}'.format(can_process))
-        if can_process is True:
-            # Emulate processing....
-            current_state = {'ResourcesCreated': True}
-            self.state_persistence.save_object_state(object_identifier=task.task_id, data={'ResourcesCreated': True})
-        new_key_value_store.save(key='Processor1:Processed:{}:Success'.format(task.task_id), value=current_state['ResourcesCreated'])
-        self.logger.info('[Processor1]: {}'.format('='*80))
-        return new_key_value_store
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=variable_store
+        )
+        dump_events(
+            task_id=t.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertTrue('test-task:SPEC_DRIFTED' in variable_store.variable_store)
+        self.assertTrue('test-task:RESOURCE_DRIFTED' in variable_store.variable_store)
+        self.assertIsInstance(variable_store.variable_store['test-task:SPEC_DRIFTED'], bool)
+        self.assertIsInstance(variable_store.variable_store['test-task:RESOURCE_DRIFTED'], bool)
+        self.assertFalse(variable_store.variable_store['test-task:SPEC_DRIFTED'])
+        self.assertTrue(variable_store.variable_store['test-task:RESOURCE_DRIFTED'])
 
+    def test_drift_action_only_spec_drift_detected_01(self):
+        
+        p = DummyTaskProcessor1()
+        t = copy.deepcopy(self.task)
+        t.state = TaskState(
+            report_label=copy.deepcopy(t.task_id),
+            manifest_spec=copy.deepcopy(t.spec),
+            manifest_metadata=copy.deepcopy(t.metadata),
+            applied_spec={'originalField': 'originalValue'},
+            resolved_spec=copy.deepcopy(t.spec),
+            created_timestamp=1000, 
+            applied_resources_checksum=hashlib.sha256('test_resource'.encode('utf-8')).hexdigest()
+        )
+        variable_store = VariableStore()
+        variable_store.add_variable(
+            variable_name='ResourceData:{}'.format(t.task_id),
+            value='test_resource'
+        )
+        resolved_spec = copy.deepcopy(self.task.spec)
+        if 'ResolvedSpec:{}'.format(self.task.task_id) in variable_store.variable_store:
+            resolved_spec = copy.deepcopy(variable_store.variable_store['ResolvedSpec:{}'.format(self.task.task_id)])
+        variable_store = p.process_task(
+            task=t,
+            variable_store=copy.deepcopy(variable_store),
+            action='DetectDriftAction',
+            task_resolved_spec=resolved_spec
+        )
 
-class Processor2(TaskProcessor):
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=variable_store
+        )
+        dump_events(
+            task_id=t.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertTrue('test-task:SPEC_DRIFTED' in variable_store.variable_store)
+        self.assertTrue('test-task:RESOURCE_DRIFTED' in variable_store.variable_store)
+        self.assertIsInstance(variable_store.variable_store['test-task:SPEC_DRIFTED'], bool)
+        self.assertIsInstance(variable_store.variable_store['test-task:RESOURCE_DRIFTED'], bool)
+        self.assertTrue(variable_store.variable_store['test-task:SPEC_DRIFTED'])
+        self.assertFalse(variable_store.variable_store['test-task:RESOURCE_DRIFTED'])
 
-    def __init__(self, logger: LoggerWrapper=TestLogger()):
-        super().__init__(kind='Processor2', kind_versions=['v1'], supported_commands=['command2'], logger=logger)
-    
-    def process_task(self, task: Task, command: str, context: str='default', key_value_store: KeyValueStore=KeyValueStore(), state_persistence: StatePersistence=StatePersistence())->KeyValueStore:
-        self.logger.info('[Processor2]: {}'.format('-'*80))
-        self.logger.info('[Processor2]: Processing task_id "{}"'.format(task.task_id))
-        self.logger.info('[Processor2]: command="{}"'.format(command))
-        self.logger.info('[Processor2]: context="{}"'.format(context))
-        new_key_value_store = KeyValueStore()
-        new_key_value_store.store = copy.deepcopy(key_value_store.store)
-        current_state = self.state_persistence.get_object_state(object_identifier=task.task_id)
-        can_process = True
-        if task.kind != 'Processor2':
-            self.logger.error('[Processor2]: Task kind "{}" mismatched and the task will NOT be processed'.format(task.kind))
-            can_process = False
-            current_state = {'ResourcesCreated': False}
-        if task.version not in self.versions:
-            self.logger.error('[Processor2]: Task version "{}" is not supported and the task will NOT be processed'.format(task.version))
-            can_process = False
-            current_state = {'ResourcesCreated': False}
-        if len(current_state) > 0:
-            self.logger.error('[Processor2]: Task version "{}" is already in the correct state'.format(task.version))
-            can_process = False
-        else:
-            current_state = {'ResourcesCreated': False}
-        self.logger.info('[Processor2]: can_process={}'.format(can_process))
-        if can_process is True:
-            # Emulate processing....
-            current_state = {'ResourcesCreated': True}
-            self.state_persistence.save_object_state(object_identifier=task.task_id, data={'ResourcesCreated': True})
-        new_key_value_store.save(key='Processor2:Processed:{}:Success'.format(task.task_id), value=current_state['ResourcesCreated'])
-        self.logger.info('[Processor2]: {}'.format('='*80))
-        return new_key_value_store
-    
-    def process_task_alternate_method(self, task: Task, command: str, context: str='default', key_value_store: KeyValueStore=KeyValueStore(), state_persistence: StatePersistence=StatePersistence())->KeyValueStore:
-        self.logger.info('[Processor1]: {}'.format('-'*80))
-        self.logger.info('[Processor1]: Processing task_id : "{}"'.format(task.task_id))
-        self.logger.info('[Processor1]: command            : "{}"'.format(command))
-        self.logger.info('[Processor1]: context            : "{}"'.format(context))
-        self.logger.info('[Processor1]: Processing Method  : "process_task_alternate_method()"')
-        new_key_value_store = KeyValueStore()
-        new_key_value_store.store = copy.deepcopy(key_value_store.store)
-        current_state = self.state_persistence.get_object_state(object_identifier=task.task_id)
-        can_process = True
-        if task.kind != 'Processor2':
-            self.logger.error('[Processor2]: Task kind "{}" mismatched and the task will NOT be processed'.format(task.kind))
-            can_process = False
-            current_state = {'ResourcesCreated': False}
-        if task.version not in self.versions:
-            self.logger.error('[Processor2]: Task version "{}" is not supported and the task will NOT be processed'.format(task.version))
-            can_process = False
-            current_state = {'ResourcesCreated': False}
-        if len(current_state) > 0:
-            self.logger.error('[Processor2]: Task version "{}" is already in the correct state'.format(task.version))
-            can_process = False
-        else:
-            current_state = {'ResourcesCreated': False}
-        self.logger.info('[Processor2]: can_process={}'.format(can_process))
-        if can_process is True:
-            # Emulate processing....
-            current_state = {'ResourcesCreated': True} 
-            self.state_persistence.save_object_state(object_identifier=task.task_id, data={'ResourcesCreated': True})
-        new_key_value_store.save(key='Processor2:Processed:{}:Success'.format(task.task_id), value=current_state['ResourcesCreated'])
-        self.logger.info('[Processor2]: {}'.format('='*80))
-        return new_key_value_store
+    def test_drift_action_resource_and_spec_drift_detected_01(self):
+        
+        p = DummyTaskProcessor1()
+        t = copy.deepcopy(self.task)
+        t.state = TaskState(
+            report_label=copy.deepcopy(t.task_id),
+            manifest_spec=copy.deepcopy(t.spec),
+            manifest_metadata=copy.deepcopy(t.metadata),
+            applied_spec={'originalField': 'originalValue'},
+            resolved_spec=copy.deepcopy(t.spec),
+            created_timestamp=1000, 
+            applied_resources_checksum=hashlib.sha256('test_resource_original'.encode('utf-8')).hexdigest()
+        )
+        variable_store = VariableStore()
+        variable_store.add_variable(
+            variable_name='ResourceData:{}'.format(t.task_id),
+            value='test_resource'
+        )
+        resolved_spec = copy.deepcopy(self.task.spec)
+        if 'ResolvedSpec:{}'.format(self.task.task_id) in variable_store.variable_store:
+            resolved_spec = copy.deepcopy(variable_store.variable_store['ResolvedSpec:{}'.format(self.task.task_id)])
+        variable_store = p.process_task(
+            task=t,
+            variable_store=copy.deepcopy(variable_store),
+            action='DetectDriftAction',
+            task_resolved_spec=resolved_spec
+        )
 
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=variable_store
+        )
+        dump_events(
+            task_id=t.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertTrue('test-task:SPEC_DRIFTED' in variable_store.variable_store)
+        self.assertTrue('test-task:RESOURCE_DRIFTED' in variable_store.variable_store)
+        self.assertIsInstance(variable_store.variable_store['test-task:SPEC_DRIFTED'], bool)
+        self.assertIsInstance(variable_store.variable_store['test-task:RESOURCE_DRIFTED'], bool)
+        self.assertTrue(variable_store.variable_store['test-task:SPEC_DRIFTED'])
+        self.assertTrue(variable_store.variable_store['test-task:RESOURCE_DRIFTED'])
 
-class TestClassTaskProcessor(unittest.TestCase):    # pragma: no cover
+
+class TestTaskProcessStore(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
-
-    def test_processor_1_init_with_successful_exec_of_a_task(self):
-        p1 = Processor1()
-        t1 = Task(
-            kind='Processor1',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-            },
-            logger=p1.logger
-        )
-        key_value_store = p1.process_task(task=t1, command='command1', context='c1', key_value_store=KeyValueStore(), state_persistence=StatePersistence())
-        self.assertIsNotNone(key_value_store)
-        self.assertIsInstance(key_value_store, KeyValueStore)
-        self.assertIsNotNone(key_value_store.store)
-        self.assertIsInstance(key_value_store.store, dict)
-        self.assertEqual(len(key_value_store.store), 1)
-        self.assertTrue('Processor1:Processed:{}:Success'.format(t1.task_id) in key_value_store.store)
-        self.assertTrue(key_value_store.store['Processor1:Processed:{}:Success'.format(t1.task_id)], 'key_value_store.store={}'.format(key_value_store.store))
-
-        p1_logger = p1.logger
-        self.assertIsNotNone(p1_logger)
-        self.assertTrue('[LOG] INFO: [Processor1]: can_process=True' in p1.logger.info_lines, 'info_lines={}'.format(p1.logger.info_lines))
-
-    def test_processor_1_init_with_none_matching_task(self):
-        p1 = Processor1()
-        t1 = Task(
-            kind='Processor2',  # !!!
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-            },
-            logger=TestLogger()
-        )
-        key_value_store = p1.process_task(task=t1, command='command1', context='c1', key_value_store=KeyValueStore())
-        self.assertIsNotNone(key_value_store)
-        self.assertIsInstance(key_value_store, KeyValueStore)
-        self.assertIsNotNone(key_value_store.store)
-        self.assertIsInstance(key_value_store.store, dict)
-        self.assertEqual(len(key_value_store.store), 1)
-        self.assertTrue('Processor1:Processed:{}:Success'.format(t1.task_id) in key_value_store.store)
-        self.assertFalse(key_value_store.store['Processor1:Processed:{}:Success'.format(t1.task_id)])
-
-        p1_logger = p1.logger
-        self.assertIsNotNone(p1_logger)
-        self.assertTrue('[LOG] INFO: [Processor1]: can_process=False' in p1.logger.info_lines, 'info_lines={}'.format(p1.logger.info_lines))
-
-    def test_method_task_pre_processing_check_with_valid_task_1(self):
-        p1 = Processor1()
-        t1 = Task(
-            kind='Processor2',  # !!!
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-            },
-            logger=TestLogger()
-        )
-        expected_key = 'PROCESSING_TASK:{}:command1:c1'.format(t1.task_id)
-        key_value_store = p1.task_pre_processing_check(task=t1, command='command1', context='c1', key_value_store=KeyValueStore())
-        self.assertIsNotNone(key_value_store)
-        self.assertIsInstance(key_value_store, KeyValueStore)
-        self.assertIsNotNone(key_value_store.store)
-        self.assertIsInstance(key_value_store.store, dict)
-        self.assertEqual(len(key_value_store.store), 2, 'key_value_store.store={}'.format(key_value_store.store))
-        self.assertTrue(expected_key in key_value_store.store)
-        self.assertEqual(key_value_store.store[expected_key], 1)
-
-    def test_method_task_pre_processing_check_with_valid_task__using_alternate_task_processing_method_1(self):
-        logger = TestLogger()
-        p1 = Processor2(logger=logger)
-        p1.register_process_task_functions(functions=get_processing_methods_from_task_processor(clazz=p1.__class__, class_name=p1.__class__.__name__, logger=logger))
-        p1.link_processing_function_name_to_command(processing_function_name='process_task_alternate_method', commands=['*',])
-        self.assertTrue('process_task_alternate_method' in p1.process_task_functions)
-        self.assertTrue('process_task' in p1.process_task_functions)
-        t1 = Task(
-            kind='Processor2',  # !!!
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
+        self.task = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task'},
+            spec={'testField': 'testValue'}
+        )
+
+    def test_basic_01(self):
+        task_processor_store = TaskProcessStore()
+        task_processor_store.register_task_processor(task_processor=DummyTaskProcessor1())
+        p = task_processor_store.get_task_processor_for_task(task=self.task)
+        self.assertIsNotNone(p)
+        self.assertIsInstance(p, DummyTaskProcessor1)
+
+    def test_basic_02(self):
+        task_processor_store = TaskProcessStore()
+        task_processor_store.register_task_processor(task_processor=DummyTaskProcessor1())
+        p = task_processor_store.get_task_processor(api_version='DummyTaskProcessor1/v1')
+        self.assertIsNotNone(p)
+        self.assertIsInstance(p, DummyTaskProcessor1)
+
+    def test_basic_03(self):
+        task_processor_store = TaskProcessStore()
+        task_processor_store.register_task_processor(task_processor=DummyTaskProcessor1())
+        with self.assertRaises(Exception):
+            task_processor_store.get_task_processor(api_version='NoneExisting')
+
+    def test_basic_04(self):
+        task_processor_store = TaskProcessStore()
+        task_processor_store.register_task_processor(task_processor=DummyTaskProcessor1())
+        with self.assertRaises(Exception):
+            task_processor_store.get_task_processor_for_task(
+                task=Task(
+                    api_version='NoneExisting',
+                    kind='DummyKind',
+                    metadata=dict(),
+                    spec={
+                        'key': 'value'
                     }
-                ],
-            },
-            logger=logger
+                )
+            )
+
+
+class TestTasks(unittest.TestCase):    # pragma: no cover
+
+    def setUp(self):
+        print()
+        print('-'*80)
+        self.task_01 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-01'},
+            spec={'testField': 'testValue'}
+        )
+        self.task_02 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-02'},
+            spec={'testField': 'testValue'}
+        )
+        self.task_03 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-03'},
+            spec={'testField': 'testValue'}
+        )
+        self.task_04 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-04'},
+            spec={'testField': 'testValue'}
         )
-        expected_key = 'PROCESSING_TASK:{}:command1:c1'.format(t1.task_id)
-        key_value_store = p1.task_pre_processing_check(task=t1, command='command1', context='c1', key_value_store=KeyValueStore(), call_process_task_if_check_pass=True, default_task_processing_function_name='process_task_alternate_method')
+        logger.reset()
+
+    def tearDown(self):
+        self.task_01 = None
+        self.task_02 = None
+        return super().tearDown()
+
+    def test_basic_task_dependency_01(self):
+        # setup most basic dependency
+        self.task_01.metadata['processingScope'] = [
+            {
+                'commands': ['command1', 'command2',],
+                'contexts': ['con1','con2'],
+            },
+        ]
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        result = tasks.get_task_names_in_order(command='command1', context='con1')
+
         print_logger_lines(logger=logger)
-        self.assertIsNotNone(key_value_store)
-        self.assertIsInstance(key_value_store, KeyValueStore)
-        self.assertIsNotNone(key_value_store.store)
-        self.assertIsInstance(key_value_store.store, dict)
-        self.assertEqual(len(key_value_store.store), 2, 'key_value_store.store={}'.format(key_value_store.store))
-        self.assertTrue(expected_key in key_value_store.store)
-        self.assertEqual(key_value_store.store[expected_key], 2, 'key_value_store.store={}'.format(key_value_store.store))
-
-    def test_method_task_pre_processing_check_with_valid_task_and_execute_1(self):
-        p1 = Processor1()
-        t1 = Task(
-            kind='Processor1',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-            },
-            logger=TestLogger()
-        )
-        key_value_store = KeyValueStore()
-        expected_key = 'PROCESSING_TASK:{}:command1:c1'.format(t1.task_id)
-        key_value_store = p1.task_pre_processing_check(task=t1, command='command1', context='c1', key_value_store=key_value_store, call_process_task_if_check_pass=True)
-        self.assertIsNotNone(key_value_store)
-        self.assertIsInstance(key_value_store, KeyValueStore)
-        self.assertIsNotNone(key_value_store.store)
-        self.assertIsInstance(key_value_store.store, dict)
-        self.assertEqual(len(key_value_store.store), 2, 'key_value_store={}'.format(key_value_store.store))
-        self.assertTrue(expected_key in key_value_store.store)
-        self.assertEqual(key_value_store.store[expected_key], 2, 'key_value_store={}'.format(key_value_store.store))
-        self.assertTrue('Processor1:Processed:{}:Success'.format(t1.task_id) in key_value_store.store)
-        self.assertTrue(key_value_store.store['Processor1:Processed:{}:Success'.format(t1.task_id)], 'key_value_store={}'.format(key_value_store.store))
-
-        key_value_store = p1.process_task(task=t1, command='command1', context='c1', key_value_store=key_value_store)
-        self.assertIsNotNone(key_value_store)
-        self.assertIsInstance(key_value_store, KeyValueStore)
-        self.assertIsNotNone(key_value_store.store)
-        self.assertIsInstance(key_value_store.store, dict)
-        self.assertEqual(len(key_value_store.store), 2)
-        self.assertTrue(expected_key in key_value_store.store)
-        self.assertEqual(key_value_store.store[expected_key], 2, 'key_value_store={}'.format(key_value_store.store))
-        self.assertTrue('Processor1:Processed:{}:Success'.format(t1.task_id) in key_value_store.store)
-        self.assertTrue(key_value_store.store['Processor1:Processed:{}:Success'.format(t1.task_id)], 'key_value_store={}'.format(key_value_store.store))
 
-        key_value_store = p1.task_pre_processing_check(task=t1, command='command1', context='c1', key_value_store=key_value_store, call_process_task_if_check_pass=True)
-        self.assertTrue('[LOG] WARNING: [Processor1:test1:command1:c1] Appears task was already previously validated and/or executed' in p1.logger.warn_lines, 'warn_lines={}'.format(p1.logger.warn_lines))
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, list)
+        self.assertEqual(len(result), 2)
+        self.assertEqual(result[0], 'test-task-01')
+        self.assertEqual(result[1], 'test-task-02')
+
+    def test_basic_task_dependency_with_command_and_context_01(self):
+        # setup most basic dependency
+        self.task_01.metadata['processingScope'] = [
+            {
+                'commands': ['command1', 'command2',],
+                'contexts': ['con1','con2'],
+            },
+        ]
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['command1', 'command2',],
+                'contexts': ['con1','con2',],
+            }
+        ]
+        self.task_03.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['command2', 'command3',],
+                'contexts': ['con2','con3'],
+            }
+        ]
+        self.task_03.metadata['processingScopes'] = [
+            {
+                'commands': ['command2', 'command3',],
+                'contexts': ['con2','con3'],
+            },
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_03))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        result = tasks.get_task_names_in_order(command='command2', context='con2')
+
+        print_logger_lines(logger=logger)
+
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, list)
+        self.assertEqual(len(result), 3)
+        self.assertEqual(result[0], 'test-task-01')
+        self.assertTrue('test-task-02' in result)
+        self.assertTrue('test-task-03' in result)
+
+    def test_basic_task_dependency_with_command_and_context_02(self):
+        # setup most basic dependency
+        self.task_01.metadata['processingScope'] = [
+            {
+                'commands': ['command1', 'command2',],
+                'contexts': ['con1','con2'],
+            },
+        ]
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['command1', 'command2',],
+                'contexts': ['con1','con2',],
+            },
+        ]
+        self.task_03.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['command2', 'command3',],
+                'contexts': ['con2','con3'],
+            },
+        ]
+        self.task_03.metadata['processingScope'] = [
+            {
+                'commands': ['command2', 'command3',],
+                'contexts': ['con2','con3'],
+            },
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_03))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        result = tasks.get_task_names_in_order(command='command1', context='con1')
+
+        print_logger_lines(logger=logger)
+
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, list)
+        self.assertEqual(len(result), 2)
+        self.assertEqual(result[0], 'test-task-01')
+        self.assertTrue('test-task-02' in result)
+        self.assertFalse('test-task-03' in result)
+
+    def test_basic_task_dependency_with_command_and_context_03(self):
+        """
+            setup most basic dependencies and processing scopes.
+
+            This test assumes the processing will be aborted because task named "test-task-01" is a dependency of 
+            "test-task-02", but the dependant task is NOT scoped for processing in this command and context
+        """
+        self.task_01.metadata['processingScope'] = [
+            {
+                'commands': ['command1', 'command2',],
+                'contexts': ['con1','con2'],
+            },
+        ]
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['command1', 'command2',],
+                'contexts': ['con1','con2',],
+            },
+        ]
+        self.task_03.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['command2', 'command3',],
+                'contexts': ['con2','con3'],
+            },
+        ]
+        self.task_03.metadata['processingScope'] = [
+            {
+                'commands': ['command2', 'command3',],
+                'contexts': ['con2','con3'],
+            },
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_03))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        result = None
+        with self.assertRaises(Exception):
+            result = tasks.get_task_names_in_order(command='command3', context='con3')
+
+        print_logger_lines(logger=logger)
 
+        self.assertIsNone(result)
 
-class TestClassTasks(unittest.TestCase):    # pragma: no cover
+    def test_task_ordering_in_multiple_daisy_chained_dependencies_01(self):
+        # setup most basic dependency
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01','test-task-03',],
+            }
+        ]
+        self.task_04.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01','test-task-02',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_04))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        tasks.add_task(task=copy.deepcopy(self.task_03))
+        result = tasks.get_task_names_in_order(command='command1', context='con1')
+
+        print_logger_lines(logger=logger)
+
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, list)
+        self.assertEqual(len(result), 4)
+        self.assertEqual(result[0], 'test-task-01')
+        self.assertEqual(result[1], 'test-task-03')
+        self.assertEqual(result[2], 'test-task-02')
+        self.assertEqual(result[3], 'test-task-04')
+
+    def test_task_ordering_in_multiple_daisy_chained_dependencies_02(self):
+        # setup most basic dependency
+        self.task_01.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-04',],
+            }
+        ]
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01','test-task-03',],
+            }
+        ]
+        self.task_04.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-03',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_04))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        tasks.add_task(task=copy.deepcopy(self.task_03))
+        result = tasks.get_task_names_in_order(command='command1', context='con1')
+
+        print_logger_lines(logger=logger)
+
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, list)
+        self.assertEqual(len(result), 4)
+        self.assertEqual(result[0], 'test-task-03')
+        self.assertEqual(result[1], 'test-task-04')
+        self.assertEqual(result[2], 'test-task-01')
+        self.assertEqual(result[3], 'test-task-02')
+
+    def test_task_multiple_dependency_scenarios_01(self):
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['command1',],
+                'contexts': ['con1',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        dependent_task_names_1 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command1', context='con1')
+        dependent_task_names_2 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command2', context='con1')
+        dependent_task_names_3 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command1', context='con2')
+        for result in (dependent_task_names_1, dependent_task_names_2, dependent_task_names_3,):
+            self.assertIsNotNone(result)
+            self.assertIsInstance(result, list)
+        self.assertEqual(len(dependent_task_names_1), 1)
+        self.assertEqual(len(dependent_task_names_2), 0)
+        self.assertEqual(len(dependent_task_names_3), 0)
+        self.assertTrue('test-task-01' in dependent_task_names_1)
+        self.assertFalse('test-task-01' in dependent_task_names_2)
+        self.assertFalse('test-task-01' in dependent_task_names_3)
+
+    def test_task_multiple_dependency_scenarios_02(self):
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['command1',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        dependent_task_names_1 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command1', context='con1')
+        dependent_task_names_2 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command2', context='con1')
+        dependent_task_names_3 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command1', context='con2')
+        for result in (dependent_task_names_1, dependent_task_names_2, dependent_task_names_3,):
+            self.assertIsNotNone(result)
+            self.assertIsInstance(result, list)
+        self.assertEqual(len(dependent_task_names_1), 1)
+        self.assertEqual(len(dependent_task_names_2), 0)
+        self.assertEqual(len(dependent_task_names_3), 1)
+        self.assertTrue('test-task-01' in dependent_task_names_1)
+        self.assertFalse('test-task-01' in dependent_task_names_2)
+        self.assertTrue('test-task-01' in dependent_task_names_3)
+
+    def test_task_multiple_dependency_scenarios_03(self):
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'contexts': ['con1',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        dependent_task_names_1 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command1', context='con1')
+        dependent_task_names_2 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command2', context='con1')
+        dependent_task_names_3 = tasks.get_task_dependencies_as_list_of_task_names(task_name='test-task-02', command='command1', context='con2')
+        for result in (dependent_task_names_1, dependent_task_names_2, dependent_task_names_3,):
+            self.assertIsNotNone(result)
+            self.assertIsInstance(result, list)
+        self.assertEqual(len(dependent_task_names_1), 1)
+        self.assertEqual(len(dependent_task_names_2), 1)
+        self.assertEqual(len(dependent_task_names_3), 0)
+        self.assertTrue('test-task-01' in dependent_task_names_1)
+        self.assertTrue('test-task-01' in dependent_task_names_2)
+        self.assertFalse('test-task-01' in dependent_task_names_3)
+
+    def test_task_processing_scope_scenarios_01(self):
+        self.task_01.metadata['processingScope'] = [
+            {
+                'commands': ['command1',],
+                'contexts': ['con1',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con1'))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con1'))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con2'))
+
+    def test_task_processing_scope_scenarios_02(self):
+        self.task_01.metadata['processingScope'] = [
+            {
+                'commands': ['command1',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con1'))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con1'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con2'))
+
+    def test_task_processing_scope_scenarios_03(self):
+        self.task_01.metadata['processingScope'] = [
+            {
+                'contexts': ['con1',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con1'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con1'))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con2'))
+
+
+    def test_task_processing_scope_scenarios_04(self):
+        self.task_01.metadata['processingScope'] = None
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con1'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con1'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con2'))
+
+    def test_task_processing_scope_scenarios_05(self):
+        self.task_01.metadata['processingScope'] = 'Invalid Type'
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con1'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con1'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con2'))
+
+    def test_task_processing_scope_scenarios_06(self):
+        self.task_01.metadata['processingScope'] = [
+            None,
+            {
+                'commands': ['command2',],
+                'contexts': ['con2',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con1'))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con1'))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con2'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con2'))
+
+    def test_task_processing_scope_scenarios_07(self):
+        self.task_01.metadata['processingScope'] = [
+            'Invalid Type',
+            {
+                'commands': ['command2',],
+                'contexts': ['con2',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con1'))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con1'))
+        self.assertFalse(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con2'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con2'))
+
+    def test_task_processing_scope_scenarios_08(self):
+        self.task_01.metadata['processingScope'] = [
+            {
+                'what?': 'This will produce a TRUE result',
+            },
+            {
+                'commands': ['command2',],
+                'contexts': ['con2',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con1'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con1'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command1', context='con2'))
+        self.assertTrue(tasks.task_scoped_for_processing(task_name='test-task-01', command='command2', context='con2'))
+
+    def test_loop_through_tasks_01(self):
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_03))
+        tasks.add_task(task=copy.deepcopy(self.task_04))
+        self.assertEqual(len(tasks), 4)
+        task: Task
+        for task in tasks:
+            self.assertIsNotNone(task)
+            self.assertIsInstance(task, Task)
+            self.assertTrue(task.task_id.startswith('test-task-0'))
+
+    def test_task_ordering_dependency_raises_exception_01(self):
+        # setup most basic dependency
+        self.task_01.metadata['processingScope'] = [
+            {
+                'commands': ['command1', 'command2',],
+                'contexts': ['con1','con2'],
+            },
+        ]
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+            }
+        ]
+        tasks = Tasks()
+        tasks.add_task(task=copy.deepcopy(self.task_02))
+        tasks.add_task(task=copy.deepcopy(self.task_01))
+        combinations = (
+            {
+                'command': 'command1',
+                'context': 'con1',
+                'expectException': False
+            },
+            {
+                'command': 'command2',
+                'context': 'con1',
+                'expectException': False
+            },
+            {
+                'command': 'command1',
+                'context': 'con2',
+                'expectException': False
+            },
+            {
+                'command': 'command2',
+                'context': 'con2',
+                'expectException': False
+            },
+            {
+                'command': 'command3',
+                'context': 'con1',
+                'expectException': True
+            },
+            {
+                'command': 'command1',
+                'context': 'con3',
+                'expectException': True
+            },
+            {
+                'command': 'command3',
+                'context': 'con3',
+                'expectException': True
+            },
+        )
+        for scenario in combinations:
+            if scenario['expectException'] is False:
+                result = tasks._task_ordering(current_processing_order=[], candidate_task_name='test-task-02',command=scenario['command'], context=scenario['context'])
+                self.assertIsNotNone(result)
+                self.assertIsInstance(result, list)
+                self.assertEqual(len(result), 2)
+                self.assertTrue('test-task-01' in result)
+                self.assertTrue('test-task-02' in result)
+            else:
+                with self.assertRaises(Exception):
+                    tasks._task_ordering(current_processing_order=[], candidate_task_name='test-task-02',command=scenario['command'], context=scenario['context'])
+            print_logger_lines(logger=logger)
+            logger.reset()
+
+
+class TestVariousFunctions(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
-        self.key_value_store = KeyValueStore()
+        logger.reset()
 
-    def test_tasks_basic_single_task_1(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore(), state_persistence=StatePersistence(logger=TestLogger()))
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor1',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata={
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test1"
-                        }
-                    ],
-                    "annotations": {
-                        "contexts": "c1,c2",
-                    }
-                },
-                logger=tasks.logger
-            )
-        )
-        tasks.process_context(command='command1', context='c1')
-        key_value_store = tasks.key_value_store
-        logger = tasks.logger
-        self.assertIsNotNone(key_value_store)
-        self.assertIsInstance(key_value_store, KeyValueStore)
-        self.assertEqual(len(key_value_store.store), 2, 'key_value_store={}'.format(key_value_store.store))
-        self.assertTrue(len(logger.info_lines) > 0, 'info_lines={}'.format(logger.info_lines))
-        self.assertTrue(len(logger.error_lines) == 0, 'error_lines={}'.format(logger.error_lines))
-        self.assertTrue(len(logger.critical_lines) == 0, 'critical_lines={}'.format(logger.critical_lines))
-        for line in logger.all_lines_in_sequence:
-            print(line)
-
-    def test_tasks_basic_single_task_with_invalid_processor_1(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore(), state_persistence=StatePersistence(logger=TestLogger()))
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        with self.assertRaises(Exception) as cm:
-            tasks.add_task(
-                task=Task(
-                    kind='Processor3',
-                    version='v1',
-                    spec={'field1': 'value1'},
-                    metadata={
-                        "identifiers": [
-                            {
-                                "type": "ManifestName",
-                                "key": "test1"
-                            }
-                        ],
-                        "annotations": {
-                            "contexts": "c1,c2",
-                        }
-                    },
-                    logger=tasks.logger
-                )
-            )
+    def tearDown(self):
+        return super().tearDown()
 
-    def test_tasks_basic_dependant_tasks_1(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor2',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata={
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test2"
-                        }
-                    ],
-                    "annotations": {
-                        "contexts": "c1,c2",
-                        "dependency/name": "test1",
-                    }
-                },
-                logger=tasks.logger
-            )
-        )
-        tasks.add_task(
-            task=Task(
-                kind='Processor1',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata={
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test1"
-                        }
-                    ],
-                    "annotations": {
-                        "contexts": "c1,c2",
-                    }
-                },
-                logger=tasks.logger
-            )
-        )
+    def test_function_produce_column_headers_normal_01(self):
+        result = produce_column_headers()
+        print('RESULT:\n\n{}\n\n'.format(result))
+        self.assertTrue('Manifest          Created  Created Timestamp          Spec Drifted       Resources Drifted' in result)
 
-        logger = tasks.logger
+    def test_function_produce_column_headers_with_checksums_01(self):
+        result = produce_column_headers(with_checksums=True)
+        print('RESULT:\n\n{}\n\n'.format(result))
+        self.assertTrue('Manifest          Created  Created Timestamp          Spec Drifted       Resources Drifted  Applied Spec CHecksum             Current Spec Checksum             Applied Resource Checksum         Current Resource Checksum' in result)
 
-        tasks.process_context(command='command2', context='c1')
-        self.assertIsNotNone(tasks.key_value_store)
-        self.assertIsInstance(tasks.key_value_store, KeyValueStore)
-        self.assertEqual(len(tasks.key_value_store.store), 4, 'key_value_store={}'.format(tasks.key_value_store.store))
-        self.assertTrue(len(logger.info_lines) > 0)
-        self.assertTrue(len(logger.error_lines) == 0)
-        self.assertTrue(len(logger.critical_lines) == 0)
-        for line in logger.all_lines_in_sequence:
-            print(line)
-
-    def test_tasks_basic_dependant_tasks_2(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-
-        task_1_metadata = {
-            "identifiers": [
-                {
-                    "type": "ManifestName",
-                    "key": "test1"
-                },
-                {
-                    "type": "Label",
-                    "key": "l1",
-                    "value": "lv1"
-                },
-                {
-                    "type": "Label",
-                    "key": "l2",
-                    "value": "lv2"
-                },
-            ],
-            "contextualIdentifiers": [
-                {
-                    "type": "ExecutionScope",
-                    "key": "INCLUDE",
-                    "contexts": [
-                        {
-                            "type": "Environment",
-                            "names": [
-                                "c1",
-                                "c2"
-                            ]
-                        }
-                    ]
-                }
-            ]
-        }
-        task_2_metadata = {
-            "identifiers": [
-                {
-                    "type": "ManifestName",
-                    "key": "test2"
-                },
-                {
-                    "type": "Label",
-                    "key": "l1",
-                    "value": "lv1"
-                },
-                {
-                    "type": "Label",
-                    "key": "l2",
-                    "value": "lv2"
-                },
-            ],
-            "contextualIdentifiers": [
-                {
-                    "type": "ExecutionScope",
-                    "key": "INCLUDE",
-                    "contexts": [
-                        {
-                            "type": "Environment",
-                            "names": [
-                                "c1",
-                                "c2"
-                            ]
-                        }
-                    ]
-                }
-            ],
-            "dependencies": [
-                {
-                    "identifierType": "Label",
-                    "identifiers": [
-                        { "key": "l1", "value": "lv1" },
-                        { "key": "l2", "value": "lv2" },
-                    ]
-                }
-            ]
-        }
-        task_3_metadata = {
-            "identifiers": [
-                {
-                    "type": "ManifestName",
-                    "key": "test3"
-                },
-            ],
-            "contextualIdentifiers": [
-                {
-                    "type": "ExecutionScope",
-                    "key": "INCLUDE",
-                    "contexts": [
-                        {
-                            "type": "Environment",
-                            "names": [
-                                "c1",
-                                "c2"
-                            ]
-                        },
-                        {
-                            "type": "Command",
-                            "names": ["command1",]
-                        }
-                    ]
-                }
-            ],
-            "dependencies": [
-                {
-                    "identifierType": "ManifestName",
-                    "identifiers": [
-                        { "key": "test2" },
-                    ]
-                },
-            ]
-        }
+    def test_produce_column_header_horizontal_line_basic_01(self):
+        result = produce_column_header_horizontal_line()
+        print('RESULT:\n\n{}\n\n'.format(result))
+        self.assertTrue('------------------------------------------------------------------------------------------' in result)
 
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor1',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata=task_1_metadata,
-                logger=tasks.logger
-            )
-        )
-        tasks.add_task(
-            task=Task(
-                kind='Processor2',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata=task_2_metadata,
-                logger=tasks.logger
-            )
-        )
-        tasks.add_task( # This task will NOT be processed...
-            task=Task(
-                kind='Processor2',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata=task_3_metadata,
-                logger=tasks.logger
-            )
-        )
+    def test_produce_column_header_horizontal_line_basic_02(self):
+        result = produce_column_header_horizontal_line(line_char='=')
+        print('RESULT:\n\n{}\n\n'.format(result))
+        self.assertTrue('==========================================================================================' in result)
+
+    def test_produce_column_header_horizontal_line_with_checksums_01(self):
+        result = produce_column_header_horizontal_line(with_checksums=True)
+        print('RESULT:\n\n{}\n\n'.format(result))
+        self.assertTrue('----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------' in result)
 
-        logger = tasks.logger
-
-        # order = tasks.calculate_current_task_order(command='command2', context='c1')
-        order = tasks.calculate_current_task_order(processing_target_identifier=build_command_identifier(command='command2', context='c1'))
-        print('order={}'.format(order))
-
-        tasks.process_context(command='command2', context='c1')
-        self.assertIsNotNone(tasks.key_value_store)
-        self.assertIsInstance(tasks.key_value_store, KeyValueStore)
-        self.assertEqual(len(tasks.key_value_store.store), 4, 'key_value_store={}'.format(tasks.key_value_store.store))
-        self.assertTrue(len(logger.info_lines) > 0)
-        self.assertTrue(len(logger.error_lines) == 0)
-        self.assertTrue(len(logger.critical_lines) == 0)
-        for line in logger.all_lines_in_sequence:
-            print(line)
-
-    def test_tasks_adding_same_task_twice_produces_exception_1(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor2',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata={
-                    'name': 'test2',
-                    'annotations': {
-                        'contexts': 'c1,c2',
-                        'dependency/label/command2/l1': 'lv1',
-                    }
-                },
-                logger=tasks.logger
-            )
-        )
-        with self.assertRaises(Exception) as cm:
-            tasks.add_task( # This task will NOT be processed...
-                task=Task(
-                    kind='Processor2',
-                    version='v1',
-                    spec={'field1': 'value1'},
-                    metadata={
-                        'name': 'test2',
-                        'annotations': {
-                            'contexts': 'c1,c2',
-                            'dependency/label/command2/l1': 'lv1',
-                        }
-                    },
-                    logger=tasks.logger
-                )
-            )
 
-    def test_tasks_basic_dependant_tasks_not_found_throws_exception_1(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor2',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata = {
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test2"
-                        },
-                    ],
-                    "contextualIdentifiers": [
-                        {
-                            "type": "ExecutionScope",
-                            "key": "INCLUDE",
-                            "contexts": [
-                                {
-                                    "type": "Environment",
-                                    "names": [
-                                        "c1",
-                                        "c2"
-                                    ]
-                                }
-                            ]
-                        }
-                    ],
-                    "dependencies": [
-                        {
-                            "identifierType": "ManifestName",
-                            "identifiers": [
-                                { "key": "test1" },
-                            ]
-                        }
-                    ]
-                },
-                logger=tasks.logger
-            )
-        )
-        with self.assertRaises(Exception) as cm:
-            tasks.process_context(command='command2', context='c1')
+class TestClassTaskState(unittest.TestCase):    # pragma: no cover
 
-    def test_tasks_non_qualifying_task_due_to_context_1(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor1',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata = {
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test1"
-                        },
-                    ],
-                    "contextualIdentifiers": [
-                        {
-                            "type": "ExecutionScope",
-                            "key": "INCLUDE",
-                            "contexts": [
-                                {
-                                    "type": "Environment",
-                                    "names": [
-                                        "c1",
-                                        "c2"
-                                    ]
-                                }
-                            ]
-                        }
-                    ]
-                },
-                logger=tasks.logger
-            )
+    def setUp(self):
+        print()
+        print('-'*80)
+        logger.reset()
+
+    def tearDown(self):
+        return super().tearDown()
+    
+    def test_basic_init_01(self):
+        task_state = TaskState()
+        self.assertIsNotNone(task_state)
+        self.assertIsInstance(task_state, TaskState)
+        self.assertFalse(task_state.is_created)
+
+    def test_method_update_applied_spec_existing_resource_updated_01(self):
+        # Initial state of a previously created resource
+        task_state = TaskState(
+            manifest_spec={'field_value': 2},
+            applied_spec={'field_value': 1},
+            resolved_spec={'field_value': 2},
+            manifest_metadata={'name': 'test-task-01'},
+            report_label='test-task-01',
+            created_timestamp=1000,
+            applied_resources_checksum='a',
+            current_resource_checksum='a'
         )
-        tasks.add_task(
-            task=Task(
-                kind='Processor1',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata = {
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test2"
-                        },
-                    ],
-                    "contextualIdentifiers": [
-                        {
-                            "type": "ExecutionScope",
-                            "key": "INCLUDE",
-                            "contexts": [
-                                {
-                                    "type": "Environment",
-                                    "names": [
-                                        "c2"
-                                    ]
-                                }
-                            ]
-                        }
-                    ]
-                },
-                logger=tasks.logger
-            )
+        print(str(task_state))
+        drift_results_1 = task_state.to_dict(with_checksums=True)
+        print('\nDRIFT DATA: {}\n\n'.format(json.dumps(drift_results_1, default=str)))
+        self.assertTrue(drift_results_1['SpecDrifted'])
+        self.assertEqual(drift_results_1['CreatedTimestamp'], 1000)
+        self.assertEqual(drift_results_1['AppliedResourcesChecksum'], 'a')
+        self.assertEqual(drift_results_1['CurrentResourceChecksum'], 'a')
+        self.assertTrue(task_state.is_created)
+
+        # Simulate a resource update
+        task_state.update_applied_spec(new_applied_spec={'field_value': 2}, new_applied_resource_checksum='b', updated_timestamp=2000)
+        drift_results_2 = task_state.to_dict(with_checksums=True)
+        print('\nDRIFT DATA: {}\n\n'.format(json.dumps(drift_results_2, default=str)))
+        self.assertFalse(drift_results_2['SpecDrifted'])
+        self.assertEqual(drift_results_2['CreatedTimestamp'], 2000)
+        self.assertEqual(drift_results_2['AppliedResourcesChecksum'], 'b')
+        self.assertEqual(drift_results_2['CurrentResourceChecksum'], 'b')
+        self.assertTrue(task_state.is_created)
+
+    def test_method_update_applied_spec_existing_resource_deleted_01(self):
+        # Initial state of a previously created resource
+        task_state = TaskState(
+            manifest_spec={'field_value': 1},
+            applied_spec={'field_value': 1},
+            resolved_spec={'field_value': 1},
+            manifest_metadata={'name': 'test-task-01'},
+            report_label='test-task-01',
+            created_timestamp=1000,
+            applied_resources_checksum='a',
+            current_resource_checksum='a'
         )
-
-        logger = tasks.logger
-
-        tasks.process_context(command='command1', context='c1')
-
-        self.assertIsNotNone(tasks.key_value_store)
-        self.assertIsInstance(tasks.key_value_store, KeyValueStore)
-        self.assertEqual(len(tasks.key_value_store.store), 2, 'key_value_store={}'.format(tasks.key_value_store.store))
-        self.assertTrue(len(logger.info_lines) > 0)
-        self.assertTrue(len(logger.error_lines) == 0)
-        self.assertTrue(len(logger.critical_lines) == 0)
-        for line in logger.all_lines_in_sequence:
-            print(line)
-
-    def test_tasks_method_find_task_by_name_task_not_found_returns_none(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor1',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata = {
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test1"
-                        },
-                    ],
-                    "contextualIdentifiers": [
-                        {
-                            "type": "ExecutionScope",
-                            "key": "INCLUDE",
-                            "contexts": [
-                                {
-                                    "type": "Environment",
-                                    "names": [
-                                        "c1",
-                                        "c2"
-                                    ]
-                                }
-                            ]
-                        }
-                    ]
-                },
-                logger=tasks.logger
-            )
+        print(str(task_state))
+        drift_results_1 = task_state.to_dict(with_checksums=True)
+        print('\nDRIFT DATA: {}\n\n'.format(json.dumps(drift_results_1, default=str)))
+        self.assertIsNone(drift_results_1['SpecDrifted'])
+        self.assertEqual(drift_results_1['CreatedTimestamp'], 1000)
+        self.assertEqual(drift_results_1['AppliedResourcesChecksum'], 'a')
+        self.assertEqual(drift_results_1['CurrentResourceChecksum'], 'a')
+
+        # Simulate a resource being deleted
+        task_state.update_applied_spec(new_applied_spec={'field_value': 1}, new_applied_resource_checksum=None, updated_timestamp=0)
+        drift_results_2 = task_state.to_dict(with_checksums=True)
+        print('\nDRIFT DATA: {}\n\n'.format(json.dumps(drift_results_2, default=str)))
+        self.assertFalse(drift_results_2['SpecDrifted'])
+        self.assertEqual(drift_results_2['CreatedTimestamp'], None)
+        self.assertEqual(drift_results_2['AppliedResourcesChecksum'], None)
+        self.assertEqual(drift_results_2['CurrentResourceChecksum'], None)
+        self.assertFalse(task_state.is_created)
+
+    def test_method_column_str_basic_01(self):
+        task_state = TaskState(
+            manifest_spec={'field_value': 1},
+            applied_spec={'field_value': 1},
+            resolved_spec={'field_value': 1},
+            manifest_metadata={'name': 'test-task-01'},
+            report_label='test-task-01',
+            created_timestamp=1000,
+            applied_resources_checksum='a',
+            current_resource_checksum='a'
         )
-        self.assertIsNone(tasks.find_task_by_name(name='test2'))
-
-    def test_tasks_method_find_task_by_name_1(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor1',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata = {
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test1"
-                        },
-                    ],
-                    "contextualIdentifiers": [
-                        {
-                            "type": "ExecutionScope",
-                            "key": "INCLUDE",
-                            "contexts": [
-                                {
-                                    "type": "Environment",
-                                    "names": [
-                                        "c1",
-                                        "c2"
-                                    ]
-                                }
-                            ]
-                        }
-                    ]
-                },
-                logger=tasks.logger
-            )
+        result = task_state.column_str(
+            human_readable=True,
+            current_resolved_spec={'field_value': 1},
+            current_resource_checksum='a'
+        )
+        print(produce_column_headers())
+        print(produce_column_header_horizontal_line())
+        print('{}'.format(result))
+        self.assertTrue('test-task-01      Yes      1970-01-01 01:16:40        No                 No' in result)
+
+    def test_method_column_str_resource_drifted_01(self):
+        task_state = TaskState(
+            manifest_spec={'field_value': 1},
+            applied_spec={'field_value': 1},
+            resolved_spec={'field_value': 1},
+            manifest_metadata={'name': 'test-task-01'},
+            report_label='test-task-01',
+            created_timestamp=1000,
+            applied_resources_checksum='a',
+            current_resource_checksum='a'
         )
-        task1 = tasks.find_task_by_name(name='test1', calling_task_id='test2')
-        self.assertIsNotNone(task1)
-        self.assertIsInstance(task1, Task)
-        self.assertEqual(task1.kind, 'Processor1')
-
-        task2 = tasks.find_task_by_name(name='test1', calling_task_id='test1')
-        self.assertIsNone(task2)
-
-    def test_tasks_method_get_task_by_task_id(self):
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore())
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(
-            task=Task(
-                kind='Processor1',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata = {
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test1"
-                        },
-                    ],
-                    "contextualIdentifiers": [
-                        {
-                            "type": "ExecutionScope",
-                            "key": "INCLUDE",
-                            "contexts": [
-                                {
-                                    "type": "Environment",
-                                    "names": [
-                                        "c1",
-                                        "c2"
-                                    ]
-                                }
-                            ]
-                        }
-                    ]
-                },
-                logger=tasks.logger
-            )
+        result = task_state.column_str(
+            human_readable=True,
+            current_resolved_spec={'field_value': 1},
+            current_resource_checksum='b'
+        )
+        print(produce_column_headers())
+        print(produce_column_header_horizontal_line())
+        print('{}'.format(result))
+        self.assertTrue('test-task-01      Yes      1970-01-01 01:16:40        No                 Yes' in result)
+
+    def test_method_column_str_spec_drifted_01(self):
+        task_state = TaskState(
+            manifest_spec={'field_value': 1},
+            applied_spec={'field_value': 1},
+            resolved_spec={'field_value': 1},
+            manifest_metadata={'name': 'test-task-01'},
+            report_label='test-task-01',
+            created_timestamp=1000,
+            applied_resources_checksum='a',
+            current_resource_checksum='a'
         )
-        tasks.add_task(
-            task=Task(
-                kind='Processor2',
-                version='v1',
-                spec={'field1': 'value1'},
-                metadata = {
-                    "identifiers": [
-                        {
-                            "type": "ManifestName",
-                            "key": "test2"
-                        },
-                    ]
-                },
-                logger=tasks.logger
-            )
+        result = task_state.column_str(
+            human_readable=True,
+            current_resolved_spec={'field_value': 2},
+            current_resource_checksum='a'
+        )
+        print(produce_column_headers())
+        print(produce_column_header_horizontal_line())
+        print('{}'.format(result))
+        self.assertTrue('test-task-01      Yes      1970-01-01 01:16:40        Yes                No' in result)
+
+    def test_method_column_str_spec_and_resource_drifted_01(self):
+        task_state = TaskState(
+            manifest_spec={'field_value': 1},
+            applied_spec={'field_value': 1},
+            resolved_spec={'field_value': 1},
+            manifest_metadata={'name': 'test-task-01'},
+            report_label='test-task-01',
+            created_timestamp=1000,
+            applied_resources_checksum='a',
+            current_resource_checksum='a'
         )
-        task1 = tasks.get_task_by_task_id(task_id='test1')
-        self.assertIsNotNone(task1)
-        self.assertIsInstance(task1, Task)
-        self.assertEqual(task1.kind, 'Processor1')
-        task2 = tasks.get_task_by_task_id(task_id='test2')
-        self.assertIsNotNone(task2)
-        self.assertIsInstance(task2, Task)
-        self.assertEqual(task2.kind, 'Processor2')
+        result = task_state.column_str(
+            human_readable=True,
+            current_resolved_spec={'field_value': 2},
+            current_resource_checksum='b'
+        )
+        print(produce_column_headers())
+        print(produce_column_header_horizontal_line())
+        print('{}'.format(result))
+        self.assertTrue('test-task-01      Yes      1970-01-01 01:16:40        Yes                Yes' in result)
+
+    def test_method_column_str_spec_and_resource_drifted_with_checksums_01(self):
+        task_state = TaskState(
+            manifest_spec={'field_value': 1},
+            applied_spec={'field_value': 1},
+            resolved_spec={'field_value': 1},
+            manifest_metadata={'name': 'test-task-01'},
+            report_label='test-task-01',
+            created_timestamp=1000,
+            applied_resources_checksum='a',
+            current_resource_checksum='a'
+        )
+        result = task_state.column_str(
+            human_readable=True,
+            current_resolved_spec={'field_value': 2},
+            current_resource_checksum='b',
+            with_checksums=True
+        )
+        print(produce_column_headers())
+        print(produce_column_header_horizontal_line())
+        print('{}'.format(result))
+        self.assertTrue('test-task-01      Yes      1970-01-01 01:16:40        Yes                Yes                38320c1e644eb074b24bb343e131e420  fcacd5b851d3ef945b3b11bf07ad1e17  a                                 b' in result)
+
+    def test_method_repr(self):
+        task_state = TaskState(
+            manifest_spec={'field_value': 1},
+            applied_spec={'field_value': 1},
+            resolved_spec={'field_value': 1},
+            manifest_metadata={'name': 'test-task-01'},
+            report_label='test-task-01',
+            created_timestamp=1000,
+            applied_resources_checksum='a',
+            current_resource_checksum='a'
+        )
+        result = repr(task_state)
+        print(result)
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, str)
 
-        with self.assertRaises(Exception) as cm:
-            tasks.get_task_by_task_id(task_id='test3')
-        
 
 class TestClassStatePersistence(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
+        logger.reset()
+
+    def tearDown(self):
+        return super().tearDown()
+    
+    def test_load_without_exception_01(self):
+        p = StatePersistence()
+        self.assertFalse(p.load())
+
+    def test_load_with_exception_01(self):
+        p = StatePersistence()
+        with self.assertRaises(Exception):
+            p.load(on_failure=Exception('TEST FAILURE'))
+
+    def test_update_and_get_01(self):
+        p = StatePersistence()
+        p.update_object_state(object_identifier='a', data={'result': 'it worked!'})
+        result = p.get(object_identifier='a')
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, dict)
+        self.assertEqual(result['result'], 'it worked!')
+
+    def test_get_with_refresh_returns_empty_dict_01(self):
+        p = StatePersistence()
+        result = p.get(object_identifier='a')
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, dict)
+        self.assertEqual(len(result), 0)
+
+    def test_get_without_refresh_returns_empty_dict_01(self):
+        p = StatePersistence()
+        result = p.get(object_identifier='a', refresh_cache_if_identifier_not_found=False)
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, dict)
+        self.assertEqual(len(result), 0)
 
-    def test_basic_state_persistence_1(self):
-        state_persistence = StatePersistence(logger=TestLogger(), configuration=dict())
-        state_persistence.save_object_state(object_identifier='test1', data={'key1': 'value1'})
-        state_persistence.persist_all_state()
-        object_data = state_persistence.get_object_state(object_identifier='test1')
-        self.assertEqual(object_data['key1'], 'value1')
-        self.assertTrue(len(state_persistence.state_cache), 1)
+    def test_get_with_refresh_returns_valid_dict_01(self):
+        class MyStatePersistence(StatePersistence):
+            def load(self, on_failure: object=False)->bool:
+                self.state_cache['a'] = {'value': 1}
+                return True
+        
+        p = MyStatePersistence(load_on_init=False)
+        result = p.get(object_identifier='a')
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, dict)
+        self.assertEqual(len(result), 1)
 
+    def test_update_and_commit_01(self):
+        p = StatePersistence()
+        p.update_object_state(object_identifier='a', data={'result': 'it worked!'})
+        p.commit()
+        self.assertIsNotNone(p.state_cache)
+        self.assertIsInstance(p.state_cache, dict)
+        self.assertEqual(len(p.state_cache), 1)
 
-class TestClassTaskLifecycleStages(unittest.TestCase):    # pragma: no cover
+class TestClassParameterValidation(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
+        logger.reset()
 
-    def test_basic_life_cycles_1(self):
-        task_life_cycle_stages = TaskLifecycleStages()
-        self.assertEqual(len(task_life_cycle_stages.stages), 12)
-
-    def test_basic_life_cycles_2(self):
-        task_life_cycle_stages = TaskLifecycleStages(init_default_stages=False)
-        self.assertEqual(len(task_life_cycle_stages.stages), 0)
-        task_life_cycle_stages.register_lifecycle_stage(task_life_cycle_stage=TaskLifecycleStage.TASK_REGISTERED)
-        task_life_cycle_stages.register_lifecycle_stage(task_life_cycle_stage=TaskLifecycleStage.TASK_REGISTERED_ERROR)
-        self.assertEqual(len(task_life_cycle_stages.stages), 2)
-
-        self.assertTrue(task_life_cycle_stages.stage_registered(stage=TaskLifecycleStage.TASK_REGISTERED))
-        self.assertTrue(task_life_cycle_stages.stage_registered(stage=TaskLifecycleStage.TASK_REGISTERED_ERROR))
-        self.assertFalse(task_life_cycle_stages.stage_registered(stage=TaskLifecycleStage.TASK_PRE_PROCESSING_COMPLETED))
-
-
-def hook_function_test_1(
-    hook_name:str,
-    task:Task,
-    key_value_store:KeyValueStore,
-    command:str,
-    context:str,
-    task_life_cycle_stage:int,
-    extra_parameters:dict,
-    logger:LoggerWrapper
-):
-    logger.info(
-        'Function "hook_function_test_1" called on hook_name "{}" for task "{}" during task_lifecycle_stage "{}"'.format(
-            hook_name,
-            task.task_id,
-            task_life_cycle_stage
-        )
-    )
-    key = '{}:{}:{}:{}:{}'.format(
-        hook_name,
-        task.task_id,
-        command,
-        context,
-        task_life_cycle_stage
-    )
-    key_value_store.save(key=key, value=True)
-    return key_value_store
+    def tearDown(self):
+        return super().tearDown()
+    
+    def test_basic_01(self):
+        pv = ParameterValidation(constraints=None)
+        result = pv.validation_passed(parameters=dict())
+        self.assertTrue(result)
 
 
-class TestClassHook(unittest.TestCase):    # pragma: no cover
+class TestClassTaskProcessingActionParameterValidation(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
+        logger.reset()
 
-    def test_exec_hook_on_every_lifecycle_stage_1(self):
-        logger = TestLogger()
-
-        hook = Hook(
-            name='test_hook_1',
-            commands=['command1'],
-            contexts=['c1'],
-            task_life_cycle_stages=TaskLifecycleStages(),
-            function_impl=hook_function_test_1,
-            logger=logger
-        )
-
-        t1 = Task(
-            kind='Processor2',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test2"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "test1" },
-                        ]
-                    }
-                ]
-            },
-            logger=logger
+    def tearDown(self):
+        return super().tearDown()
+    
+    def test_most_basic_01(self):
+        pv = TaskProcessingActionParameterValidation(constraints=None)
+        result = pv.validation_passed(
+            parameters={
+                'Action': 'CreateAction'
+            }
         )
-
-        lifecycle_stages_to_test = (
-            TaskLifecycleStage.TASK_PRE_REGISTER,
-            TaskLifecycleStage.TASK_REGISTERED,
-            TaskLifecycleStage.TASK_PRE_PROCESSING_START,
-            TaskLifecycleStage.TASK_PRE_PROCESSING_COMPLETED,
-            TaskLifecycleStage.TASK_PROCESSING_PRE_START,
-            TaskLifecycleStage.TASK_PROCESSING_POST_DONE,
-        )
-
-        for lifecycle_stage in lifecycle_stages_to_test:
-            result = hook.process_hook(
-                command='command1',
-                context='c1',
-                task_life_cycle_stage=lifecycle_stage,
-                key_value_store=KeyValueStore(),
-                task=t1,
-                task_id=t1.task_id,
-                logger=logger
-            )
-            expected_log_entry = '[LOG] INFO: Function "hook_function_test_1" called on hook_name "{}" for task "{}" during task_lifecycle_stage "{}"'.format(
-                hook.name,
-                t1.task_id,
-                lifecycle_stage
-            )
-            self.assertTrue(expected_log_entry in logger.info_lines, 'FAILED on lifecycle_stage "{}":  info_lines={}'.format(lifecycle_stage, logger.info_lines))
-
-            self.assertIsNotNone(result)
-            self.assertIsInstance(result, KeyValueStore)
-            expected_key = '{}:{}:command1:c1:{}'.format(
-                hook.name,
-                t1.task_id,
-                lifecycle_stage
-            )
-            self.assertTrue(expected_key in result.store)
-            self.assertTrue(result.store[expected_key])
-
         print_logger_lines(logger=logger)
+        self.assertTrue(result)
 
-    def test_exec_hook_skip_on_command_mismatch_1(self):
-        logger = TestLogger()
-
-        hook = Hook(
-            name='test_hook_1',
-            commands=['command1'],
-            contexts=['c1'],
-            task_life_cycle_stages=TaskLifecycleStages(),
-            function_impl=hook_function_test_1,
-            logger=logger
-        )
-
-        t1 = Task(
-            kind='Processor2',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test2"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "test1" },
-                        ]
-                    }
-                ]
-            },
-            logger=logger
+    def test_most_basic_02(self):
+        pv = TaskProcessingActionParameterValidation(
+            constraints=None,
+            auto_init_supported_actions=True
+        ).add_command(command='command1').add_context(context='context1')
+        result = pv.validation_passed(
+            parameters={
+                'Action': 'CreateAction',
+                'Command': 'command1',
+                'Context': 'context1'
+            }
         )
+        print_logger_lines(logger=logger)
+        self.assertTrue(result)
 
-        result = hook.process_hook(
-            command='command2',     # Mismatch
-            context='c1',
-            task_life_cycle_stage=TaskLifecycleStage.TASK_REGISTERED,
-            key_value_store=KeyValueStore(),
-            task=t1,
-            task_id=t1.task_id,
-            logger=TestLogger()
+    def test_most_basic_03(self):
+        pv = TaskProcessingActionParameterValidation(
+            constraints={
+                'SupportedCommands': ['command1','command2',],
+                'SupportedContexts': ['context1', 'context2', ],
+                'SupportedActions': ['action1', 'action2',],
+            },
+            auto_init_supported_actions=True
+        )
+        result = pv.validation_passed(
+            parameters={
+                'Action': 'action1',
+                'Command': 'command1',
+                'Context': 'context1'
+            }
         )
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, KeyValueStore)
-        self.assertEqual(len(result.store), 0)
-
         print_logger_lines(logger=logger)
+        self.assertTrue(result)
 
-    def test_exec_hook_skip_on_context_mismatch_1(self):
-        logger = TestLogger()
-
-        hook = Hook(
-            name='test_hook_1',
-            commands=['command1'],
-            contexts=['c1'],
-            task_life_cycle_stages=TaskLifecycleStages(),
-            function_impl=hook_function_test_1,
-            logger=logger
-        )
-
-        t1 = Task(
-            kind='Processor2',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test2"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "test1" },
-                        ]
-                    }
-                ]
-            },
-            logger=logger
+    def test_most_basic_negative_01(self):
+        pv = TaskProcessingActionParameterValidation(constraints=None)
+        result = pv.validation_passed(
+            parameters={
+                'Action': 'WrongAction'
+            }
         )
+        print_logger_lines(logger=logger)
+        self.assertFalse(result)
 
-        result = hook.process_hook(
-            command='command1',
-            context='c3',     # Mismatch
-            task_life_cycle_stage=TaskLifecycleStage.TASK_REGISTERED,
-            key_value_store=KeyValueStore(),
-            task=t1,
-            task_id=t1.task_id,
-            logger=TestLogger()
-        )
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, KeyValueStore)
-        self.assertEqual(len(result.store), 0)
+    def test_most_basic_negative_02(self):
+        pv = TaskProcessingActionParameterValidation(
+            constraints=None,
+            auto_init_supported_actions=True
+        ).add_command(command='command1').add_context(context='context1')
+
+        wrong_combinations = (
+            {
+                'Action': 'WrongAction',
+                'Command': 'command1',
+                'Context': 'context1'
+            },
+            {
+                'Action': 'CreateAction',
+                'Command': 'command99',
+                'Context': 'context1'
+            },
+            {
+                'Action': 'CreateAction',
+                'Command': 'command1',
+                'Context': 'context99'
+            }
+        )
+
+        for wrong_parameters in wrong_combinations:
+            result = pv.validation_passed(parameters=wrong_parameters)
+            print_logger_lines(logger=logger)
+            self.assertFalse(result)
+            logger.reset()
+
+    def test_most_basic_negative_03(self):
+        pv = TaskProcessingActionParameterValidation(
+            constraints={
+                'SupportedCommands': ['command1','command2',],
+                'SupportedContexts': ['context1', 'context2', ],
+                'SupportedActions': ['action1', 'action2',],
+            },
+            auto_init_supported_actions=True
+        )
+
+        wrong_combinations = (
+            {
+                'Action': 'WrongAction',
+                'Command': 'command1',
+                'Context': 'context1',
+            },
+            {
+                'Action': 'CreateAction',
+                'Command': 'command99',
+                'Context': 'context1',
+            },
+            {
+                'Action': 'CreateAction',
+                'Command': 'command1',
+                'Context': 'context99',
+            },
+            {
+                'Action': None,
+                'Command': 'command1',
+                'Context': 'context1',
+            },
+            {
+                'Action': 'CreateAction',
+                'Command': None,
+                'Context': 'context1',
+            },
+            {
+                'Action': 'CreateAction',
+                'Command': 'command1',
+                'Context': None,
+            },
+            None,
+            'wrong_type',
+        )
+
+        for wrong_parameters in wrong_combinations:
+            result = pv.validation_passed(parameters=wrong_parameters)
+            print_logger_lines(logger=logger)
+            self.assertFalse(result)
+            logger.reset()
 
-        print_logger_lines(logger=logger)
 
-    def test_exec_hook_skip_on_lifecycle_stage_mismatch_1(self):
-        logger = TestLogger()
+class TestClassVariableStore(unittest.TestCase):    # pragma: no cover
 
-        hook_lifecycle_stages = TaskLifecycleStages(init_default_stages=False)
-        hook_lifecycle_stages.register_lifecycle_stage(
-            task_life_cycle_stage=TaskLifecycleStage.TASK_REGISTERED
-        )
-        hook = Hook(
-            name='test_hook_1',
-            commands=['command1'],
-            contexts=['c1'],
-            task_life_cycle_stages=hook_lifecycle_stages,
-            function_impl=hook_function_test_1,
-            logger=logger
-        )
-
-        t1 = Task(
-            kind='Processor2',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test2"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "test1" },
-                        ]
-                    }
-                ]
-            },
-            logger=logger
-        )
+    def setUp(self):
+        print()
+        print('-'*80)
+        logger.reset()
 
-        result = hook.process_hook(
-            command='command1',
-            context='c1',
-            task_life_cycle_stage=TaskLifecycleStage.TASK_PRE_PROCESSING_START,   # Mismatch
-            key_value_store=KeyValueStore(),
-            task=t1,
-            task_id=t1.task_id,
-            logger=TestLogger()
-        )
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, KeyValueStore)
-        self.assertEqual(len(result.store), 0, 'result.store={}'.format(json.dumps(result.store)))
+    def tearDown(self):
+        return super().tearDown()
+    
+    def test_basic_01(self):
+        v = VariableStore()
+        with self.assertRaises(Exception):
+            v.get_variable(variable_name='a', pop_item=False)
+        with self.assertRaises(Exception):
+            v.get_variable(variable_name='a', pop_item=True)
+        v.add_variable(variable_name='a', value=100)
+        result1 = v.get_variable(variable_name='a', pop_item=False)
+        result2 = v.get_variable(variable_name='a', pop_item=True)
+        with self.assertRaises(Exception):
+            v.get_variable(variable_name='a', pop_item=False)
+        with self.assertRaises(Exception):
+            v.get_variable(variable_name='a', pop_item=True)
+        for result in (result1, result2, ):
+            self.assertIsNotNone(result)
+            self.assertIsInstance(result, int)
+            self.assertEqual(result, 100)
 
-        print_logger_lines(logger=logger)
 
-    def test_exec_hook_handle_function_exception_1(self):
-        logger = TestLogger()
+class TestClassTask(unittest.TestCase):    # pragma: no cover
 
-        def f1(*args, **kwargs):
-            raise Exception('I died !!')
-
-        hook = Hook(
-            name='test_hook_1',
-            commands=['command1'],  # INVALID COMMAND...
-            contexts=['c1'],
-            task_life_cycle_stages=TaskLifecycleStages(),
-            function_impl=f1,
-            logger=logger
-        )
-
-        t1 = Task(
-            kind='Processor2',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test2"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            },
-                            {
-                                "type": "Command",
-                                "names": ["command1",]
-                            }
-                        ]
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "test1" },
-                        ]
-                    }
-                ]
-            },
-            logger=logger
+    def setUp(self):
+        print()
+        print('-'*80)
+        logger.reset()
+
+    def tearDown(self):
+        return super().tearDown()
+    
+    def test_basic_01(self):
+        t = Task(
+            api_version='unittest',
+            kind='TestKind',
+            metadata={'name': 'test'},
+            spec={'name': 'value'}
         )
+        self.assertIsNotNone(t)
+        self.assertIsInstance(t, Task)
+        self.assertEqual(t.api_version, 'unittest')
+        self.assertEqual(t.kind, 'TestKind')
 
-        with self.assertRaises(Exception) as cm:
-            result = hook.process_hook(
-                command='command1',
-                context='c1',
-                task_life_cycle_stage=TaskLifecycleStage.TASK_REGISTERED,
-                key_value_store=KeyValueStore(),
-                task=t1,
-                task_id=t1.task_id,
-                logger=logger
-            )
+        self.assertIsNotNone(t.metadata)
+        self.assertIsInstance(t.metadata, dict)
+        self.assertEqual(len(t.metadata), 1)
+        self.assertTrue('name' in t.metadata)
+        self.assertEqual(t.metadata['name'], 'test')
+
+        self.assertIsNotNone(t.spec)
+        self.assertIsInstance(t.spec, dict)
+        self.assertEqual(len(t.spec), 1)
+        self.assertTrue('name' in t.spec)
+        self.assertEqual(t.spec['name'], 'value')
 
-        print_logger_lines(logger=logger)
+    def test_invalid_dicts_create_empty_dicts_basic_01(self):
+        t = Task(
+            api_version='unittest',
+            kind='TestKind',
+            metadata=None,
+            spec='invalid type'
+        )
+        self.assertIsNotNone(t)
+        self.assertIsInstance(t, Task)
+        self.assertEqual(t.api_version, 'unittest')
+        self.assertEqual(t.kind, 'TestKind')
 
+        self.assertIsNotNone(t.metadata)
+        self.assertIsInstance(t.metadata, dict)
+        self.assertEqual(len(t.metadata), 0)
+
+        self.assertIsNotNone(t.spec)
+        self.assertIsInstance(t.spec, dict)
+        self.assertEqual(len(t.spec), 0)
 
-class TestClassHooks(unittest.TestCase):    # pragma: no cover
+
+class TestClassTaskProcessor(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
-
-    def test_init_basic_1(self):
-        logger = TestLogger()
-
-        hook = Hook(
-            name='test_hook_1',
-            commands=list(),
-            contexts=list(),
-            task_life_cycle_stages=TaskLifecycleStages(),
-            function_impl=hook_function_test_1,
-            logger=logger
-        )
-
-        t1 = Task(
-            kind='Processor2',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test2"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "test1" },
-                        ]
-                    }
-                ]
-            },
-            logger=logger
+        logger.reset()
+        self.task = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task'},
+            spec={'testField': 'testValue'}
         )
 
-        lifecycle_stages_to_test = (
-            TaskLifecycleStage.TASK_PRE_REGISTER,
-            TaskLifecycleStage.TASK_REGISTERED,
-            TaskLifecycleStage.TASK_PRE_PROCESSING_START,
-            TaskLifecycleStage.TASK_PRE_PROCESSING_COMPLETED,
-            TaskLifecycleStage.TASK_PROCESSING_PRE_START,
-            TaskLifecycleStage.TASK_PROCESSING_POST_DONE,
+    def tearDown(self):
+        self.task = None
+        return super().tearDown()
+    
+    def test_basic_create_task_01(self):
+        tp = DummyTaskProcessor1()
+        variable_store = tp.process_task(
+            task=self.task,
+            action='CreateAction',
+            task_resolved_spec={'testField': 'testValue'}
         )
 
-        hooks = Hooks()
-        hooks.register_hook(hook=hook)
-        for lifecycle_stage in lifecycle_stages_to_test:
-            result = hooks.any_hook_exists(command='command1', context='c1', task_life_cycle_stage=lifecycle_stage)
-            self.assertTrue(result, 'No hook found for lifecycle_stage "{}"'.format(lifecycle_stage))
-
-            key_value_store = hooks.process_hook(
-                command='command1',
-                context='c1',
-                task_life_cycle_stage=lifecycle_stage,
-                key_value_store=KeyValueStore(),
-                task=t1,
-                task_id=t1.task_id,
-                logger=logger
-            )
-
-            self.assertIsNotNone(key_value_store)
-            self.assertIsInstance(key_value_store, KeyValueStore)
-            expected_key = '{}:{}:command1:c1:{}'.format(
-                hook.name,
-                t1.task_id,
-                lifecycle_stage
-            )
-            self.assertTrue(expected_key in key_value_store.store, 'expected_key "{}" was not found in key_value_store.store: "{}"'.format(expected_key, key_value_store.store))
-            self.assertTrue(key_value_store.store[expected_key])
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
+        )
+        dump_events(
+            task_id=self.task.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+
+    def test_basic_create_task_force_failure_and_rollback_01(self):
+        vs = VariableStore()
+        tp = DummyTaskProcessor1()
+        vs.add_variable(variable_name=tp.create_identifier(task=self.task, variable_name='UNITTEST_TROW_EXCEPTION'), value=True)
+        with self.assertRaises(Exception):
+            tp.process_task(
+                task=self.task,
+                action='CreateAction',
+                variable_store=copy.deepcopy(vs),
+                task_resolved_spec={'testField': 'testValue'}
+            )
 
         print_logger_lines(logger=logger)
 
-    def test_ensure_task_processing_covers_all_lifecycle_stages_1(self):
-        logger = TestLogger()
-
-        hook = Hook(
-            name='test_hook_1',
-            commands=['NOT_APPLICABLE', 'command1'],
-            contexts=['ALL', 'c1'],
-            task_life_cycle_stages=TaskLifecycleStages(),
-            function_impl=hook_function_test_1,
-            logger=logger
-        )
-
-        t1 = Task(
-            kind='Processor1',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ]
-            },
-            logger=logger
+    def test_basic_update_task_01(self):
+        tp = DummyTaskProcessor1()
+        variable_store = tp.process_task(
+            task=self.task,
+            action='UpdateAction',
+            task_resolved_spec={'testField': 'testValue'}
         )
 
-        hooks = Hooks()
-        hooks.register_hook(hook=hook)
-
-        tasks = Tasks(logger=TestLogger(), key_value_store=KeyValueStore(), state_persistence=StatePersistence(logger=TestLogger()), hooks=hooks)
-        tasks.register_task_processor(processor=Processor1())
-        tasks.register_task_processor(processor=Processor2())
-        tasks.add_task(task=t1)
-        tasks.process_context(command='command1', context='c1')
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
+        )
+        dump_events(
+            task_id=self.task.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+
+    def test_basic_update_task_force_failure_and_rollback_01(self):
+        vs = VariableStore()
+        tp = DummyTaskProcessor1()
+        vs.add_variable(variable_name=tp.create_identifier(task=self.task, variable_name='UNITTEST_TROW_EXCEPTION'), value=True)
+        with self.assertRaises(Exception):
+            tp.process_task(
+                task=self.task,
+                action='UpdateAction',
+                variable_store=copy.deepcopy(vs),
+                task_resolved_spec={'testField': 'testValue'}
+            )
 
-        print('key_value_store: {}'.format(tasks.key_value_store.store))
+        print_logger_lines(logger=logger)
 
-        lifecycle_stages_to_test = (
-            TaskLifecycleStage.TASK_PRE_REGISTER,
-            TaskLifecycleStage.TASK_REGISTERED,
+    def test_manual_rollback_after_create_action_01(self):
+        tp = DummyTaskProcessor1()
+        variable_store = tp.process_task(
+            task=self.task,
+            action='CreateAction',
+            task_resolved_spec={'testField': 'testValue'}
+        )
+        variable_store = tp.process_task(
+            task=self.task,
+            action='RollbackAction',
+            variable_store=copy.deepcopy(variable_store),
+            task_resolved_spec={'testField': 'testValue'}
         )
 
-        self.assertIsNotNone(tasks.key_value_store)
-        self.assertIsInstance(tasks.key_value_store, KeyValueStore)
-        for lifecycle_stage in lifecycle_stages_to_test:    
-            expected_key = '{}:{}:NOT_APPLICABLE:ALL:{}'.format(
-                hook.name,
-                t1.task_id,
-                lifecycle_stage
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
+        )
+        dump_events(
+            task_id=self.task.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+
+    def test_default_task_processor_raises_exceptions_01(self):
+        tp = TaskProcessor(api_version='unittest')
+        with self.assertRaises(Exception):
+            tp.process_task(
+                task=self.task,
+                action='CreateAction',
+                task_resolved_spec={'testField': 'testValue'}
+            )
+        with self.assertRaises(Exception):
+            tp.process_task(
+                task=self.task,
+                action='DeleteAction',
+                task_resolved_spec={'testField': 'testValue'}
+            )
+        with self.assertRaises(Exception):
+            tp.process_task(
+                task=self.task,
+                action='UpdateAction',
+                task_resolved_spec={'testField': 'testValue'}
+            )
+        with self.assertRaises(Exception):
+            tp.process_task(
+                task=self.task,
+                action='RollbackAction',
+                task_resolved_spec={'testField': 'testValue'}
+            )
+        with self.assertRaises(Exception):
+            tp.process_task(
+                task=self.task,
+                action='DescribeAction',
+                task_resolved_spec={'testField': 'testValue'}
+            )
+        with self.assertRaises(Exception):
+            tp.process_task(
+                task=self.task,
+                action='DetectDriftAction',
+                task_resolved_spec={'testField': 'testValue'}
+            )
+
+
+class UnitTestExceptionThrowingHook1(Hook):
+
+    def run(
+        self,
+        task: Task=None,
+        parameters: dict=dict(),
+        parameter_validator: ParameterValidation=ParameterValidation(constraints=None),
+        persistence: StatePersistence=StatePersistence(),
+        variable_store: VariableStore=VariableStore(),
+        task_process_store: TaskProcessStore=TaskProcessStore()
+    )->VariableStore:
+        if 'LogLevel' in parameters:
+            self._log(
+                message='I Quit!',
+                level=parameters['LogLevel']
+            )
+        else:
+            self._log(
+                message='I Quit!',
+                level='error'
             )
-            self.assertTrue(expected_key in tasks.key_value_store.store, 'FAILURE lifecycle_stage={} :: expected_key "{}" not found'.format(lifecycle_stage, expected_key))
-            self.assertTrue(tasks.key_value_store.store[expected_key], 'FAILURE lifecycle_stage={} :: expected_key "{}" is False'.format(lifecycle_stage, expected_key))
+        raise Exception('I really did quit!')
+    
 
-        lifecycle_stages_to_test = (
-            TaskLifecycleStage.TASK_PRE_PROCESSING_START,
-            TaskLifecycleStage.TASK_PRE_PROCESSING_COMPLETED,
-            TaskLifecycleStage.TASK_PROCESSING_PRE_START,
-            TaskLifecycleStage.TASK_PROCESSING_POST_DONE,
-        )
+class TestClassUnitTestExceptionThrowingHook1(unittest.TestCase):    # pragma: no cover
 
-        self.assertIsNotNone(tasks.key_value_store)
-        self.assertIsInstance(tasks.key_value_store, KeyValueStore)
-        for lifecycle_stage in lifecycle_stages_to_test:    
-            expected_key = '{}:{}:command1:c1:{}'.format(
-                hook.name,
-                t1.task_id,
-                lifecycle_stage
-            )
-            self.assertTrue(expected_key in tasks.key_value_store.store, 'FAILURE lifecycle_stage={} :: expected_key "{}" not found'.format(lifecycle_stage, expected_key))
-            self.assertTrue(tasks.key_value_store.store[expected_key], 'FAILURE lifecycle_stage={} :: expected_key "{}" is False'.format(lifecycle_stage, expected_key))
+    def setUp(self):
+        print()
+        print('-'*80)
+        logger.reset()
 
-        print_logger_lines(logger=logger)
+    def tearDown(self):
+        return super().tearDown()
+    
+
+    def test_info_level_01(self):
+        hook = UnitTestExceptionThrowingHook1(name='unittest')
+        with self.assertRaises(Exception):
+            hook.run(
+                parameters={'LogLevel': 'info'}
+            )
+        with self.assertRaises(Exception):
+            hook.run(
+                parameters={'LogLevel': 'debug'}
+            )
+        with self.assertRaises(Exception):
+            hook.run(
+                parameters={'LogLevel': 'warning'}
+            )
+        with self.assertRaises(Exception):
+            hook.run(
+                parameters={'LogLevel': 'critical'}
+            )
+        with self.assertRaises(Exception):
+            hook.run()
+        self.assertEqual(len(logger.critical_lines), 1)
+        self.assertEqual(len(logger.info_lines), 1)
+        self.assertEqual(len(logger.error_lines), 1)
+        self.assertEqual(len(logger.debug_lines), 1)
+        self.assertEqual(len(logger.warn_lines), 1)
+
+    def test_Default_hook_throws_exception(self):
+        h = Hook(name='unittest')
+        with self.assertRaises(Exception):
+            h.run()
 
 
-class TestFunctionHookFunctionAlwaysThrowException(unittest.TestCase):    # pragma: no cover
+class TestClassTaskProcessingHook(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
-
-    def test_init_basic_1(self):
-        logger = TestLogger()
-        t1 = Task(
-            kind='Processor1',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ]
-            },
-            logger=logger
+        logger.reset()
+        self.task = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task'},
+            spec={'testField': 'testValue'}
         )
 
-        hook_name = 'test_hook_1'
-        command = 'command1'
-        context = 'c1'
-        life_cycle_stage = TaskLifecycleStage.TASK_PRE_REGISTER
-
-        expected_error_message = 'Hook "{}" forced exception on command "{}" in context "{}" for life stage "{}" in task "{}"'.format(
-            hook_name,
-            command,
-            context,
-            life_cycle_stage,
-            t1.task_id
-        )
-
-        with self.assertRaises(Exception) as cm:
-            hook_function_always_throw_exception(
-                hook_name=hook_name,
-                task=t1,
-                key_value_store=KeyValueStore(),
-                command=command,
-                context=context,
-                task_life_cycle_stage=life_cycle_stage,
-                extra_parameters=dict(),
-                logger=logger
-            )
-
-            self.assertTrue(expected_error_message in cm.exception)
-
-    def test_init_custom_1(self):
-        logger = TestLogger()
-        t1 = Task(
-            kind='Processor1',
-            version='v1',
-            spec={'field1': 'value1'},
-            metadata = {
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "test1"
-                    },
-                ],
-                "contextualIdentifiers": [
-                    {
-                        "type": "ExecutionScope",
-                        "key": "INCLUDE",
-                        "contexts": [
-                            {
-                                "type": "Environment",
-                                "names": [
-                                    "c1",
-                                    "c2"
-                                ]
-                            }
-                        ]
-                    }
-                ]
-            },
-            logger=logger
+    def tearDown(self):
+        self.task = None
+        return super().tearDown()
+    
+    def test_basic_01(self):
+        parameters = dict()
+        parameters['Action'] = 'CreateAction'
+        parameters['Command'] = 'create'
+        parameters['Context'] = 'unittest'
+        vs = VariableStore()
+        param_validator = ParameterValidation(constraints=None)
+        tps = TaskProcessStore()
+        tps.register_task_processor(task_processor=DummyTaskProcessor1())
+
+        vs.add_variable(
+            variable_name='ResolvedSpec:{}'.format(self.task.task_id),
+            value=copy.deepcopy(self.task.spec)
+        )
+
+        tph = TaskProcessingHook()
+        vs = tph.run(
+            task=self.task,
+            parameters=parameters,
+            parameter_validator=param_validator,
+            variable_store=vs,
+            task_process_store=tps
+        )
+        
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(vs)
+        )
+        dump_events(
+            task_id=self.task.task_id,
+            variable_store=copy.deepcopy(vs)
         )
 
-        hook_name = 'test_hook_1'
-        command = 'command1'
-        context = 'c1'
-        life_cycle_stage = TaskLifecycleStage.TASK_PRE_REGISTER
-
-        expected_error_message = 'This is a custom message'
-
-        with self.assertRaises(Exception) as cm:
-            hook_function_always_throw_exception(
-                hook_name=hook_name,
-                task=t1,
-                key_value_store=KeyValueStore(),
-                command=command,
-                context=context,
-                task_life_cycle_stage=life_cycle_stage,
-                extra_parameters={
-                    'ExceptionMessage': expected_error_message
-                },
-                logger=logger
-            )
-
-            self.assertTrue(expected_error_message in cm.exception)
+        self.assertIsNotNone(vs)
+        self.assertIsInstance(vs, VariableStore)
+        self.assertTrue('test-task:TASK_ORIGINAL_SPEC_CHECKSUM' in vs.variable_store)
+        self.assertTrue('test-task:TASK_RESOLVED_SPEC_CHECKSUM' in vs.variable_store)
 
 
-class TestClassIdentifierContext(unittest.TestCase):    # pragma: no cover
+class TestClassResolveTaskSpecVariablesHook(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
+        logger.reset()
+        self.task_01 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-1'},
+            spec={
+                'test1': '${}VAR:Test1:Key1:Key2{}'.format('{', '}'),
+            }
+        )
+        self.task_02 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-2'},
+            spec={
+                'test2': '${}VAR:Test2:Key1{}'.format('{', '}'),
+            }
+        )
+        self.task_03 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-3'},
+            spec={
+                'test3': [
+                    '${}VAR:Test3:Key1{}'.format('{', '}'),
+                    '${}VAR:Test3:Key2{}'.format('{', '}'),
+                ],
+            }
+        )
+        self.task_04 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-4'},
+            spec={
+                'test4': {
+                    'listTest4': [
+                        '${}VAR:Test4:Key1{}'.format('{', '}'),
+                        None,
+                        'test4_ignore',
+                        '${}VAR:Test4:Key2{}'.format('{', '}'),
+                    ]
+                },
+            }
+        )
+        self.task_05 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-5'},
+            spec={
+                'test5': {
+                    'test5_1': {
+                        'test5_1_1': '${}VAR:Test5:Key1:Key1{}'.format('{', '}'),
+                        'test5_1_2': '${}VAR:Test5:Key1:Key2{}'.format('{', '}'),
+                        'test5_1_3': None,
+                        'test5_1_4': 'test5_1_4_ignore',
+                    }
+                }
+            }
+        )
+        self.task_06 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-6'},
+            spec={
+                'test1': '${}VAR:Test1:Key1:Key2{}'.format('{', '}'),
+                'test2': '${}VAR:Test2:Key1{}'.format('{', '}'),
+                'test3': [
+                    '${}VAR:Test3:Key1{}'.format('{', '}'),
+                    '${}VAR:Test3:Key2{}'.format('{', '}'),
+                ],
+                'test4': {
+                    'listTest4': [
+                        '${}VAR:Test4:Key1{}'.format('{', '}'),
+                        None,
+                        'test4_ignore',
+                        '${}VAR:Test4:Key2{}'.format('{', '}'),
+                    ]
+                },
+                'test5': {
+                    'test5_1': {
+                        'test5_1_1': '${}VAR:Test5:Key1:Key1{}'.format('{', '}'),
+                        'test5_1_2': '${}VAR:Test5:Key1:Key2{}'.format('{', '}'),
+                        'test5_1_3': None,
+                        'test5_1_4': 'test5_1_4_ignore',
+                    }
+                }
+            }
+        )
+        self.variable_store = VariableStore()
+        self.variable_store.add_variable(variable_name='Test1:Key1:Key2', value='result_01')
+        self.variable_store.add_variable(variable_name='Test2:Key1', value='result_02')
+        self.variable_store.add_variable(variable_name='Test3:Key1', value='result_03')
+        self.variable_store.add_variable(variable_name='Test3:Key2', value='result_04')
+        self.variable_store.add_variable(variable_name='Test4:Key1', value='result_05')
+        self.variable_store.add_variable(variable_name='Test4:Key2', value='result_06')
+        self.variable_store.add_variable(variable_name='Test5:Key1:Key1', value='result_07')
+        self.variable_store.add_variable(variable_name='Test5:Key1:Key2', value='result_08')
+        
 
-    def test_init_basic_1(self):
-        ic = IdentifierContext(context_type='type1', context_name='context1')
-        self.assertIsNotNone(ic)
-        self.assertIsInstance(ic, IdentifierContext)
-        result = ic.context()
-        self.assertEqual(result, 'type1:context1')
-
-    def test_contexts_matches_1(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type1', context_name='context1')
-        self.assertTrue(ic1 == ic2)
-
-    def test_contexts_does_not_match_1(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type2', context_name='context1') # wrong context_type
-        self.assertFalse(ic1 == ic2)
-
-    def test_contexts_does_not_match_2(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type1', context_name='context2') # wrong context_name
-        self.assertFalse(ic1 == ic2)
-
-    def test_contexts_does_not_match_3(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = None # Force exception, which is silently ignored
-        self.assertFalse(ic1 == ic2)
+    def tearDown(self):
+        self.task_01 = None
+        self.task_02 = None
+        self.task_03 = None
+        self.task_04 = None
+        self.task_05 = None
+        self.task_06 = None
+        self.variable_store = None
+        return super().tearDown()
 
+    def test_basic_substitution_01(self):
+        hook = ResolveTaskSpecVariablesHook()
+        result = hook.run(
+            task=self.task_01,
+            variable_store=copy.deepcopy(self.variable_store)
+        )
 
-class TestClassIdentifierContexts(unittest.TestCase):    # pragma: no cover
+        print('Resolved Spec: {}'.format(json.dumps(result.variable_store['ResolvedSpec:{}'.format(self.task_01.task_id)])))
 
-    def setUp(self):
-        print()
-        print('-'*80)
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, VariableStore)
+        self.assertTrue('ResolvedSpec:{}'.format(self.task_01.task_id) in result.variable_store)
 
-    def test_init_basic_1(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type2', context_name='context2')
-        ic3 = IdentifierContext(context_type='type3', context_name='context3')
-        ics = IdentifierContexts()
-        self.assertIsNotNone(ics)
-        self.assertTrue(ics.is_empty())
-        ics.add_identifier_context(identifier_context=ic1)
-        ics.add_identifier_context(identifier_context=ic2)
-        ics.add_identifier_context(identifier_context=ic2) # This duplicate will be ignored...
-        self.assertFalse(ics.is_empty())
-        self.assertEqual(len(ics), 2)
-        self.assertTrue(ics.contains_identifier_context(target_identifier_context=ic1))
-        self.assertTrue(ics.contains_identifier_context(target_identifier_context=ic2))
-        self.assertFalse(ics.contains_identifier_context(target_identifier_context=ic3))
-        counter = 0
-        for ic in ics:
-            self.assertIsNotNone(ic)
-            self.assertIsInstance(ic, IdentifierContext)
-            counter += 1
-        self.assertEqual(counter, 2)
-
-    def test_init_basic_2(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = 'Not the right type'
-        ic3 = None
-        ics = IdentifierContexts()
-        self.assertIsNotNone(ics)
-        self.assertTrue(ics.is_empty())
-        ics.add_identifier_context(identifier_context=ic1)
-        ics.add_identifier_context(identifier_context=ic2)
-        ics.add_identifier_context(identifier_context=ic3)
-        self.assertFalse(ics.is_empty())
-        self.assertEqual(len(ics), 1)
-
-    def test_find_matching_identifier_context_1(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type2', context_name='context2')
-        ics = IdentifierContexts()
-        ics.add_identifier_context(identifier_context=ic1)
-        ics.add_identifier_context(identifier_context=ic2)
-        matching_identifier_context = IdentifierContext(context_type='type2', context_name='context2')
-        non_matching_identifier_context = IdentifierContext(context_type='type3', context_name='context3')
-        self.assertTrue(ics.contains_identifier_context(target_identifier_context=matching_identifier_context))
-        self.assertFalse(ics.contains_identifier_context(target_identifier_context=non_matching_identifier_context))
+        resolved_spec = result.variable_store['ResolvedSpec:{}'.format(self.task_01.task_id)]
+        self.assertIsNotNone(resolved_spec)
+        self.assertIsInstance(resolved_spec, dict)
+        self.assertEqual(len(resolved_spec), 1)
+        self.assertTrue('test1' in resolved_spec)
+        self.assertEqual(resolved_spec['test1'], 'result_01')
+
+    def test_basic_substitution_02(self):
+        hook = ResolveTaskSpecVariablesHook()
+        result = hook.run(
+            task=self.task_02,
+            variable_store=copy.deepcopy(self.variable_store)
+        )
 
+        print('Resolved Spec: {}'.format(json.dumps(result.variable_store['ResolvedSpec:{}'.format(self.task_02.task_id)])))
 
-class TestClassIdentifier(unittest.TestCase):    # pragma: no cover
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, VariableStore)
+        self.assertTrue('ResolvedSpec:{}'.format(self.task_02.task_id) in result.variable_store)
+        
+        resolved_spec = result.variable_store['ResolvedSpec:{}'.format(self.task_02.task_id)]
+        self.assertIsNotNone(resolved_spec)
+        self.assertIsInstance(resolved_spec, dict)
+        self.assertEqual(len(resolved_spec), 1)
+        self.assertTrue('test2' in resolved_spec)
+        self.assertEqual(resolved_spec['test2'], 'result_02')
+
+    def test_basic_substitution_03(self):
+        hook = ResolveTaskSpecVariablesHook()
+        result = hook.run(
+            task=self.task_03,
+            variable_store=copy.deepcopy(self.variable_store)
+        )
 
-    def setUp(self):
-        print()
-        print('-'*80)
+        print('Resolved Spec: {}'.format(json.dumps(result.variable_store['ResolvedSpec:{}'.format(self.task_03.task_id)])))
 
-    def test_init_basic_1(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type2', context_name='context2')
-        ic3 = IdentifierContext(context_type='type3', context_name='context3')
-        main_ics = IdentifierContexts()
-        main_ics.add_identifier_context(identifier_context=ic1)
-        main_ics.add_identifier_context(identifier_context=ic2)
-        matching_ics1 = IdentifierContexts()
-        matching_ics1.add_identifier_context(identifier_context=ic1)
-        matching_ics2 = IdentifierContexts()
-        matching_ics2.add_identifier_context(identifier_context=ic2)
-        matching_ics3 = IdentifierContexts()
-        matching_ics3.add_identifier_context(identifier_context=ic1)
-        matching_ics3.add_identifier_context(identifier_context=ic2)
-        none_matching_ics1 = IdentifierContexts()
-        none_matching_ics1.add_identifier_context(identifier_context=ic3)
-        identifier = Identifier(identifier_type='id_type1', key='key1', val='val1', identifier_contexts=main_ics)
-        self.assertIsNotNone(identifier)
-        self.assertIsInstance(identifier, Identifier)
-        self.assertTrue(identifier.is_contextual_identifier)
-        self.assertTrue(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1', target_identifier_contexts=matching_ics1))
-        self.assertTrue(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1', target_identifier_contexts=matching_ics2))
-        self.assertTrue(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1', target_identifier_contexts=matching_ics3))
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1', target_identifier_contexts=none_matching_ics1)) # target_identifier_contexts mismatches
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key2', val='val1', target_identifier_contexts=matching_ics1)) # key mismatches
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type2', key='key1', val='val1', target_identifier_contexts=matching_ics1)) # type mismatches
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val2', target_identifier_contexts=matching_ics1)) # val mismatches
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1', target_identifier_contexts=matching_ics1)) # val mismatches
-
-    def test_init_basic_2(self):
-        identifier = Identifier(identifier_type='id_type1', key='key1', val='val1')
-        self.assertIsNotNone(identifier)
-        self.assertIsInstance(identifier, Identifier)
-        self.assertFalse(identifier.is_contextual_identifier)
-        self.assertTrue(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1'))
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key2', val='val1')) # key mismatches
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type2', key='key1', val='val1')) # type mismatches
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val2')) # val mismatches
-        self.assertFalse(identifier.identifier_matches_any_context(identifier_type='id_type1', key='key1')) # val mismatches
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, VariableStore)
+        self.assertTrue('ResolvedSpec:{}'.format(self.task_03.task_id) in result.variable_store)
+        
+        resolved_spec = result.variable_store['ResolvedSpec:{}'.format(self.task_03.task_id)]
+        self.assertIsNotNone(resolved_spec)
+        self.assertIsInstance(resolved_spec, dict)
+        self.assertEqual(len(resolved_spec), 1)
+        self.assertTrue('test3' in resolved_spec)
+        v = resolved_spec['test3']
+        self.assertIsNotNone(v)
+        self.assertIsInstance(v, list)
+        self.assertEqual(len(v), 2)
+        self.assertTrue('result_03' in v)
+        self.assertTrue('result_04' in v)
+
+    def test_basic_substitution_04(self):
+        hook = ResolveTaskSpecVariablesHook()
+        result = hook.run(
+            task=self.task_04,
+            variable_store=copy.deepcopy(self.variable_store)
+        )
 
-    # def test_init_to_dict_1(self):
-    #     identifier = Identifier(identifier_type='id_type1', key='key1', val='val1')
+        print('Resolved Spec: {}'.format(json.dumps(result.variable_store['ResolvedSpec:{}'.format(self.task_04.task_id)])))
 
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, VariableStore)
+        self.assertTrue('ResolvedSpec:{}'.format(self.task_04.task_id) in result.variable_store)
+        
+        resolved_spec = result.variable_store['ResolvedSpec:{}'.format(self.task_04.task_id)]
+        self.assertIsNotNone(resolved_spec)
+        self.assertIsInstance(resolved_spec, dict)
+        self.assertEqual(len(resolved_spec), 1)
+        self.assertTrue('test4' in resolved_spec)
+        
+        t = resolved_spec['test4']
+        self.assertIsNotNone(t)
+        self.assertIsInstance(t, dict)
+        self.assertEqual(len(t), 1)
+        self.assertTrue('listTest4' in t)
+
+        v = t['listTest4']
+        self.assertIsNotNone(v)
+        self.assertIsInstance(v, list)
+        self.assertEqual(len(v), 4)
+        self.assertTrue('result_05' in v)
+        self.assertTrue('result_06' in v)
+        self.assertTrue('test4_ignore' in v)
+        self.assertIsNone(v[1])
+
+    def test_basic_substitution_05(self):
+        hook = ResolveTaskSpecVariablesHook()
+        result = hook.run(
+            task=self.task_05,
+            variable_store=copy.deepcopy(self.variable_store)
+        )
 
-class TestClassIdentifiers(unittest.TestCase):    # pragma: no cover
+        print('Resolved Spec: {}'.format(json.dumps(result.variable_store['ResolvedSpec:{}'.format(self.task_05.task_id)])))
 
-    def setUp(self):
-        print()
-        print('-'*80)
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, VariableStore)
+        self.assertTrue('ResolvedSpec:{}'.format(self.task_05.task_id) in result.variable_store)
+        
+        resolved_spec = result.variable_store['ResolvedSpec:{}'.format(self.task_05.task_id)]
+        self.assertIsNotNone(resolved_spec)
+        self.assertIsInstance(resolved_spec, dict)
+        self.assertEqual(len(resolved_spec), 1)
+        self.assertTrue('test5' in resolved_spec)
+        
+        t = resolved_spec['test5']
+        self.assertIsNotNone(t)
+        self.assertIsInstance(t, dict)
+        self.assertEqual(len(t), 1)
+        self.assertTrue('test5_1' in t)
+
+        u = t['test5_1']
+        self.assertIsNotNone(u)
+        self.assertIsInstance(u, dict)
+        self.assertEqual(len(u), 4)
+        self.assertTrue('test5_1_1' in u)
+        self.assertEqual(u['test5_1_1'], 'result_07')
+        self.assertTrue('test5_1_2' in u)
+        self.assertEqual(u['test5_1_2'], 'result_08')
+        self.assertTrue('test5_1_3' in u)
+        self.assertEqual(u['test5_1_3'], None)
+        self.assertTrue('test5_1_4' in u)
+        self.assertEqual(u['test5_1_4'], 'test5_1_4_ignore')
+
+    def test_basic_substitution_06(self):
+        hook = ResolveTaskSpecVariablesHook()
+        result = hook.run(
+            task=self.task_06,
+            variable_store=copy.deepcopy(self.variable_store)
+        )
 
-    def test_init_basic_1(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type2', context_name='context2')
-        ic3 = IdentifierContext(context_type='type3', context_name='context3')
-        main_ics = IdentifierContexts()
-        main_ics.add_identifier_context(identifier_context=ic1)
-        main_ics.add_identifier_context(identifier_context=ic2)
-        identifier1 = Identifier(identifier_type='id_type1', key='key1', val='val1', identifier_contexts=main_ics)
-        identifier2 = Identifier(identifier_type='id_type2', key='key2')
-        identifiers = Identifiers()
-        identifiers.add_identifier(identifier=identifier1)
-        identifiers.add_identifier(identifier=identifier2)
-        identifiers.add_identifier(identifier=identifier2) # This will have no effect... identifier was already added and duplicates are ignored
-
-        self.assertIsNotNone(identifiers)
-        self.assertIsInstance(identifiers, Identifiers)
-        self.assertEqual(len(identifiers), 2)
-        for candidate_identifier in identifiers:
-            self.assertIsInstance(candidate_identifier, Identifier)
-
-        matching_ics1 = IdentifierContexts()
-        matching_ics1.add_identifier_context(identifier_context=ic1)
-        matching_ics2 = IdentifierContexts()
-        matching_ics2.add_identifier_context(identifier_context=ic2)
-        matching_ics3 = IdentifierContexts()
-        matching_ics3.add_identifier_context(identifier_context=ic1)
-        matching_ics3.add_identifier_context(identifier_context=ic2)
-        none_matching_ics1 = IdentifierContexts()
-        none_matching_ics1.add_identifier_context(identifier_context=ic3)
-
-        self.assertTrue(identifiers.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1', target_identifier_contexts=matching_ics1))
-        self.assertTrue(identifiers.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1', target_identifier_contexts=matching_ics2))
-        self.assertTrue(identifiers.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1', target_identifier_contexts=matching_ics3))
-        self.assertFalse(identifiers.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val1', target_identifier_contexts=none_matching_ics1)) # target_identifier_contexts mismatches
-        self.assertFalse(identifiers.identifier_matches_any_context(identifier_type='id_type1', key='key2', val='val1', target_identifier_contexts=matching_ics1)) # key mismatches
-        self.assertFalse(identifiers.identifier_matches_any_context(identifier_type='id_type2', key='key1', val='val1', target_identifier_contexts=matching_ics1)) # type mismatches
-        self.assertFalse(identifiers.identifier_matches_any_context(identifier_type='id_type1', key='key1', val='val2', target_identifier_contexts=matching_ics1)) # val mismatches
-        self.assertFalse(identifiers.identifier_matches_any_context(identifier_type='id_type1', key='key1', target_identifier_contexts=matching_ics1)) # val mismatches
-
-    def test_identifiers_matching_identifier(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type2', context_name='context2')
-        main_ics = IdentifierContexts()
-        main_ics.add_identifier_context(identifier_context=ic1)
-        main_ics.add_identifier_context(identifier_context=ic2)
-        
-        identifier1 = Identifier(identifier_type='id_type1', key='key1', val='val1', identifier_contexts=main_ics)
-        identifier2 = Identifier(identifier_type='id_type2', key='key2')
-        identifiers = Identifiers()
-        identifiers.add_identifier(identifier=identifier1)
-        identifiers.add_identifier(identifier=identifier2)
-
-        matching_identifier1 = Identifier(identifier_type='id_type1', key='key1', val='val1', identifier_contexts=main_ics)
-        self.assertTrue(identifiers.identifier_found(identifier=matching_identifier1))
-
-        matching_identifier2 = Identifier(identifier_type='id_type2', key='key2')
-        self.assertTrue(identifiers.identifier_found(identifier=matching_identifier2))
-
-    def test_identifiers_no_matching_identifier(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type2', context_name='context2')
-        main_ics = IdentifierContexts()
-        main_ics.add_identifier_context(identifier_context=ic1)
-        main_ics.add_identifier_context(identifier_context=ic2)
-        
-        identifier1 = Identifier(identifier_type='id_type1', key='key1', val='val1', identifier_contexts=main_ics)
-        identifier2 = Identifier(identifier_type='id_type2', key='key2')
-        identifiers = Identifiers()
-        identifiers.add_identifier(identifier=identifier1)
-        identifiers.add_identifier(identifier=identifier2)
-
-        no_matching_identifier1 = Identifier(identifier_type='id_type1', key='key3', val='val1', identifier_contexts=main_ics)
-        self.assertFalse(identifiers.identifier_found(identifier=no_matching_identifier1))
-
-        no_matching_identifier2 = Identifier(identifier_type='id_type4', key='key2')
-        self.assertFalse(identifiers.identifier_found(identifier=no_matching_identifier2))
-
-    def test_to_dict(self):
-        ic1 = IdentifierContext(context_type='type1', context_name='context1')
-        ic2 = IdentifierContext(context_type='type1', context_name='context2')
-        ic3 = IdentifierContext(context_type='type2', context_name='context3')
-        main_ics = IdentifierContexts()
-        main_ics.add_identifier_context(identifier_context=ic1)
-        main_ics.add_identifier_context(identifier_context=ic2)
-        main_ics.add_identifier_context(identifier_context=ic3)
-        
-        identifier1 = Identifier(identifier_type='id_type1', key='key1', val='val1', identifier_contexts=main_ics)
-        identifier2 = Identifier(identifier_type='id_type2', key='key2')
-        identifiers = Identifiers()
-        identifiers.add_identifier(identifier=identifier1)
-        identifiers.add_identifier(identifier=identifier2)
-
-        metadata = identifiers.to_metadata_dict()
-        self.assertIsNotNone(metadata)
-        self.assertIsInstance(metadata, dict)
-        self.assertTrue('identifiers' in metadata)
-        self.assertTrue('contextualIdentifiers' in metadata)
-        print('IDENTIFIERS METADATA DICT: {}'.format(json.dumps(metadata)))
-        self.assertEqual(len(metadata['contextualIdentifiers']), 1)
-        self.assertEqual(len(metadata['identifiers']), 1)
-        for non_contextual_identifier in metadata['identifiers']:
-            self.assertTrue('contexts' not in non_contextual_identifier)
-        for contextual_identifier in metadata['contextualIdentifiers']:
-            self.assertTrue('contexts' in contextual_identifier)
-            type1_found = False
-            for context in contextual_identifier['contexts']:
-                self.assertTrue('type' in context)
-                self.assertTrue('names' in context)
-                context_type = context['type']
-                context_names = context['names']
-                self.assertIsInstance(context_type, str)
-                self.assertIsInstance(context_names, list)
-                if context_type == 'type1':
-                    type1_found = True
-                    self.assertTrue(len(context_names), 2)
-                else:
-                    self.assertTrue(len(context_names), 1)
-                self.assertTrue(type1_found)
+        print('Resolved Spec: {}'.format(json.dumps(result.variable_store['ResolvedSpec:{}'.format(self.task_06.task_id)])))
 
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, VariableStore)
+        self.assertTrue('ResolvedSpec:{}'.format(self.task_06.task_id) in result.variable_store)
 
+        resolved_spec = result.variable_store['ResolvedSpec:{}'.format(self.task_06.task_id)]
+
+        self.assertIsNotNone(resolved_spec)
+        self.assertIsInstance(resolved_spec, dict)
+        self.assertEqual(len(resolved_spec), 5)
+
+        self.assertTrue('test1' in resolved_spec)
+        self.assertEqual(resolved_spec['test1'], 'result_01')
+
+        self.assertTrue('test2' in resolved_spec)
+        self.assertEqual(resolved_spec['test2'], 'result_02')
+
+        self.assertTrue('test3' in resolved_spec)
+        v = resolved_spec['test3']
+        self.assertIsNotNone(v)
+        self.assertIsInstance(v, list)
+        self.assertEqual(len(v), 2)
+        self.assertTrue('result_03' in v)
+        self.assertTrue('result_04' in v)
+
+        t1 = resolved_spec['test4']
+        self.assertIsNotNone(t1)
+        self.assertIsInstance(t1, dict)
+        self.assertEqual(len(t1), 1)
+        self.assertTrue('listTest4' in t1)
+
+        v1 = t1['listTest4']
+        self.assertIsNotNone(v1)
+        self.assertIsInstance(v1, list)
+        self.assertEqual(len(v1), 4)
+        self.assertTrue('result_05' in v1)
+        self.assertTrue('result_06' in v1)
+        self.assertTrue('test4_ignore' in v1)
+        self.assertIsNone(v1[1])
+
+        t2 = resolved_spec['test5']
+        self.assertIsNotNone(t2)
+        self.assertIsInstance(t2, dict)
+        self.assertEqual(len(t2), 1)
+        self.assertTrue('test5_1' in t2)
+
+        u = t2['test5_1']
+        self.assertIsNotNone(u)
+        self.assertIsInstance(u, dict)
+        self.assertEqual(len(u), 4)
+        self.assertTrue('test5_1_1' in u)
+        self.assertEqual(u['test5_1_1'], 'result_07')
+        self.assertTrue('test5_1_2' in u)
+        self.assertEqual(u['test5_1_2'], 'result_08')
+        self.assertTrue('test5_1_3' in u)
+        self.assertEqual(u['test5_1_3'], None)
+        self.assertTrue('test5_1_4' in u)
+        self.assertEqual(u['test5_1_4'], 'test5_1_4_ignore')
+
+    def test_method__is_iterable(self):
+        hook = ResolveTaskSpecVariablesHook()
+        self.assertFalse(hook._is_iterable(data='abc'))
+        self.assertTrue(hook._is_iterable(data='abc', exclude_string=False))
+        self.assertFalse(hook._is_iterable(data={'a': 1, 'b': 2}))
+        self.assertTrue(hook._is_iterable(data={'a': 1, 'b': 2}, exclude_dict=False))
+        self.assertFalse(hook._is_iterable(data=None))
+        self.assertFalse(hook._is_iterable(data=datetime.now()))
+
+    def test_method__lookup_value_invalid_key_01(self):
+        hook = ResolveTaskSpecVariablesHook()
+        with self.assertRaises(Exception):
+            hook._lookup_value(
+                raw_key='invalid',
+                command=None,
+                context=None,
+                variable_store=self.variable_store,
+                task=self.task_01
+            )
+
+    def test_method__analyse_data_01(self):
+        hook = ResolveTaskSpecVariablesHook()
+        original_data = datetime.now()
+        result = hook._analyse_data(
+            task=self.task_01,
+            data=original_data,
+            variable_store=self.variable_store,
+            command=None,
+            context=None
+        )
+        self.assertEqual(original_data, result)
 
-class TestFunctionBuildNonContextualIdentifiers(unittest.TestCase):    # pragma: no cover
+
+class TestClassTaskPostProcessingStateUpdateHook(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
+        logger.reset()
+        self.task = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task'},
+            spec={'testField': 'testValue'}
+        )
 
-    def test_basic_1(self):
-        metadata = {
-            "identifiers": [
-                {
-                    "type": "ManifestName",
-                    "key": "my-name"
-                },
-                {
-                    "type": "Label",
-                    "key": "my-key",
-                    "value": "my-value"
-                }
-            ]
-        }
-        identifiers = build_non_contextual_identifiers(metadata=metadata)
-        self.assertIsNotNone(identifiers)
-        self.assertIsInstance(identifiers, Identifiers)
-        self.assertEqual(len(identifiers), 2)
-
-        manifest_name_found = False
-        label_found = False
-        identifier: Identifier
-        for identifier in identifiers:
-            self.assertIsNotNone(identifier)
-            self.assertIsInstance(identifier, Identifier)
-            self.assertFalse(identifier.is_contextual_identifier)
-            if identifier.identifier_type == 'ManifestName':
-                manifest_name_found = True
-            elif identifier.identifier_type == 'Label':
-                label_found = True
-        self.assertTrue(manifest_name_found)
-        self.assertTrue(label_found)
+    def tearDown(self):
+        self.task = None
+        return super().tearDown()
+    
+    def test_basic_01(self):
+        persistence = StatePersistence()
+        persistence.update_object_state(
+            object_identifier='{}:TASK_STATE'.format(self.task.task_id),
+            data=self.task.state.to_dict(
+                with_checksums=True,
+                include_applied_spec=True
+            )
+        )
+        dump_state(task=self.task, persistence=persistence)
+        tp = DummyTaskProcessor1()
+        variable_store = VariableStore()
+        variable_store = tp.process_task(
+            task=self.task,
+            persistence=persistence,
+            variable_store=variable_store,
+            action='CreateAction',
+            task_resolved_spec={'testField': 'testValue'}
+        )
+        h = TaskPostProcessingStateUpdateHook()
+        variable_store = h.run(
+            task=self.task,
+            persistence=persistence,
+            variable_store=variable_store
+        )
 
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
+        )
+        dump_events(
+            task_id=self.task.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+        dump_state(task=self.task, persistence=persistence)
+
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+
+        current_state = persistence.get(object_identifier='{}:TASK_STATE'.format(self.task.task_id))
+
+        self.assertIsNotNone(current_state)
+        self.assertIsInstance(current_state, dict)
+        self.assertTrue(len(current_state) > 0)
+
+        expected_data = {
+            'Label': 'test-task',
+            'IsCreated': True,
+            'CreatedTimestamp': 1714105466,
+            'SpecDrifted': None,
+            'ResourceDrifted': False,
+            'AppliedSpecChecksum': '1fe51362297a1e0dbdce5c51d5130bac42d6edc2ce219ed0bebd4ea05083a039',
+            'CurrentResolvedSpecChecksum': '6b1791a6b1ebdffc9f2de2e7578c56c5d96c0601a95f2de48844c6f2f342a8b6',
+            'AppliedResourcesChecksum': '00f5889a18ebd1aa27d2129ec1efcfda62c03f662b6a3746bec274e40814a4a5',
+            'CurrentResourceChecksum': '00f5889a18ebd1aa27d2129ec1efcfda62c03f662b6a3746bec274e40814a4a5',
+            'AppliedSpec': {
+                'testField': 'testValue'
+            }
+        }
 
-class TestFunctionBuildContextualIdentifiers(unittest.TestCase):    # pragma: no cover
+        for field_name, expected_data in expected_data.items():
+            self.assertTrue(field_name in current_state)
+            self.assertIsInstance(current_state[field_name], type(expected_data))
+
+    def test_method__validate_data_missing_field_in_data_returns_false_01(self):
+        h = TaskPostProcessingStateUpdateHook()
+        data = {
+            'resource_checksum': '00f5889a18ebd1aa27d2129ec1efcfda62c03f662b6a3746bec274e40814a4a5', 
+            'resolved_spec_applied': {
+                'testField': 'testValue'
+            }, 
+            'state_changed': True, 
+            'is_created': True, 
+            # 'create_timestamp': 1714106083, 
+            'raw_spec': {
+                'testField': 'testValue'
+            }, 
+            'metadata': {
+                'name': 'test-task'
+            }
+        }
+        self.assertFalse(h._validate_data(data=data))
 
-    def setUp(self):
-        print()
-        print('-'*80)
+    def test_method__validate_data_null_field_in_data_returns_false_01(self):
+        h = TaskPostProcessingStateUpdateHook()
+        data = {
+            'resource_checksum': '00f5889a18ebd1aa27d2129ec1efcfda62c03f662b6a3746bec274e40814a4a5', 
+            'resolved_spec_applied': {
+                'testField': 'testValue'
+            }, 
+            'state_changed': None,  # ERROR 
+            'is_created': True, 
+            'create_timestamp': 1714106083, 
+            'raw_spec': {
+                'testField': 'testValue'
+            }, 
+            'metadata': {
+                'name': 'test-task'
+            }
+        }
+        self.assertFalse(h._validate_data(data=data))
 
-    def test_basic_1(self):
-        metadata = {
-            "contextualIdentifiers": [
-                {
-                    "type": "ExecutionScope",
-                    "key": "include",
-                    "contexts": [
-                        {
-                            "type": "environment",
-                            "names": [
-                                "env1",
-                                "env2",
-                                "env3"
-                            ]
-                        },
-                        {
-                            "type": "command",
-                            "names": [
-                                "cmd1",
-                                "cmd2"
-                            ]
-                        }
-                    ]
-                }
-            ]
+    def test_method__validate_data_incorrect_field_type_in_data_returns_false_01(self):
+        h = TaskPostProcessingStateUpdateHook()
+        data = {
+            'resource_checksum': '00f5889a18ebd1aa27d2129ec1efcfda62c03f662b6a3746bec274e40814a4a5', 
+            'resolved_spec_applied': {
+                'testField': 'testValue'
+            }, 
+            'state_changed': True, 
+            'is_created': True, 
+            'create_timestamp': datetime.now(), 
+            'raw_spec': {
+                'testField': 'testValue'
+            }, 
+            'metadata': {
+                'name': 'test-task'
+            }
         }
-        identifiers = build_contextual_identifiers(metadata=metadata)
-        self.assertIsNotNone(identifiers)
-        self.assertIsInstance(identifiers, Identifiers)
-        self.assertEqual(len(identifiers), 1)
-        identifier: Identifier
-        for identifier in identifiers:
-            self.assertIsNotNone(identifier)
-            self.assertIsInstance(identifier, Identifier)
-            self.assertTrue(identifier.is_contextual_identifier)
-
-
-def validate_order(must_be_before_input_task_name: str, input_task_name: str, list_of_tasks: list)->bool:
-    must_be_before_input_task_name_pos = list_of_tasks.index(must_be_before_input_task_name)
-    input_task_name_pos = list_of_tasks.index(input_task_name)
-    return must_be_before_input_task_name_pos < input_task_name_pos
+        self.assertFalse(h._validate_data(data=data))
+
+    def test_method_run_with_missing_key_in_variable_state_01(self):
+        h = TaskPostProcessingStateUpdateHook()
+        persistence = StatePersistence()
+        persistence.update_object_state(
+            object_identifier='{}:TASK_STATE'.format(self.task.task_id),
+            data=self.task.state.to_dict(
+                with_checksums=True,
+                include_applied_spec=True
+            )
+        )
+        variable_store = h.run(
+            task=self.task,
+            persistence=persistence
+        )
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertEqual(len(variable_store.variable_store), 0)
+
+    def test_method_run_with_invalid_data_in_variable_state_01(self):
+        h = TaskPostProcessingStateUpdateHook()
+        persistence = StatePersistence()
+        persistence.update_object_state(
+            object_identifier='{}:TASK_STATE'.format(self.task.task_id),
+            data=self.task.state.to_dict(
+                with_checksums=True,
+                include_applied_spec=True
+            )
+        )
+        variable_store = VariableStore()
+        variable_store.add_variable(
+            variable_name='{}:{}'.format(self.task.task_id, 'TASK_STATE_UPDATES'),
+            value={
+                'resource_checksum': 'abc'
+            }
+        )
+        variable_store = h.run(
+            task=self.task,
+            persistence=persistence,
+            variable_store=variable_store
+        )
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertEqual(len(variable_store.variable_store), 0)
+
+    def test_method_run_with_no_state_change_01(self):
+        h = TaskPostProcessingStateUpdateHook()
+        persistence = StatePersistence()
+        persistence.update_object_state(
+            object_identifier='{}:TASK_STATE'.format(self.task.task_id),
+            data=self.task.state.to_dict(
+                with_checksums=True,
+                include_applied_spec=True
+            )
+        )
+        variable_store = VariableStore()
+        variable_store.add_variable(
+            variable_name='{}:{}'.format(self.task.task_id, 'TASK_STATE_UPDATES'),
+            value={
+                'resource_checksum': 'abc',
+                'resolved_spec_applied': self.task.spec,
+                'state_changed': False,
+                'is_created': True,
+                'create_timestamp': 1000,
+                'raw_spec': self.task.spec,
+                'metadata': self.task.metadata,
+            }
+        )
+        variable_store = h.run(
+            task=self.task,
+            persistence=persistence,
+            variable_store=variable_store
+        )
+        self.assertIsNotNone(variable_store)
+        self.assertIsInstance(variable_store, VariableStore)
+        self.assertEqual(len(variable_store.variable_store), 0)
 
 
-class TestScenariosInLine(unittest.TestCase):    # pragma: no cover
+class TestClassGeneralErrorHook(unittest.TestCase):    # pragma: no cover
 
-    def setUp(self) -> None:
+    def setUp(self):
         print()
         print('-'*80)
-        self.logger = TestLogger()
-        return super().setUp()
+        logger.reset()
+        self.task = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task'},
+            spec={'testField': 'testValue'}
+        )
 
     def tearDown(self):
-        print_logger_lines(logger=self.logger)
-        self.logger = None
+        self.task = None
         return super().tearDown()
+    
+    def test_basic_general_error_hook_01(self):
+        h = GeneralErrorHook()
+        variable_store =  h.run()
 
-    def test_order_expected_to_work_01(self):
-        shell_script = Processor1(logger=self.logger)
-        t_1 = Task(
-            kind='Processor1',
-            version='v1',
-            metadata={
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "t_1"
-                    },
-                    {
-                        "type": "Label",
-                        "key": "is_unittest",
-                        "value": "TRUE"
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "t_2" },
-                            { "key": "t_3" },
-                        ]
-                    }
-                ]
-            },
-            spec={'field1': 'value1'},
-            logger=self.logger
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
         )
-        t_2 = Task(
-            kind='Processor1',
-            version='v1',
-            metadata={
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "t_2"
-                    },
-                    {
-                        "type": "Label",
-                        "key": "is_unittest",
-                        "value": "TRUE"
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "t_3" },
-                        ]
-                    }
-                ]
-            },
-            spec={'field1': 'value1'},
-            logger=self.logger
+        dump_events(
+            task_id=self.task.task_id,
+            variable_store=copy.deepcopy(variable_store)
         )
-        t_3 = Task(
-            kind='Processor1',
-            version='v1',
-            metadata={
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "t_3"
-                    },
-                    {
-                        "type": "Label",
-                        "key": "is_unittest",
-                        "value": "TRUE"
-                    }
-                ]
-            },
-            spec={'field1': 'value1'},
-            logger=self.logger
+
+        self.assertTrue('An Unspecified Error Occurred' in logger.error_lines[0])
+
+    def test_basic_general_error_hook_in_task_01(self):
+        h = GeneralErrorHook()
+        variable_store =  h.run(task=self.task)
+
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
+        )
+        dump_events(
+            task_id=self.task.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+        self.assertTrue('An Unspecified Error Occurred' in logger.error_lines[0])
+
+    def test_basic_general_error_hook_in_task_with_exception_01(self):
+        h = GeneralErrorHook()
+        variable_store = VariableStore()
+        variable_store.add_variable(variable_name='__GLOBAL__:ExceptionStacktrace', value='Test Exception Stack Trace')
+        with self.assertRaises(Exception):
+            h.run(task=self.task, variable_store=variable_store)
+
+        print_logger_lines(logger=logger)
+
+    def test_basic_general_error_hook_in_task_with_non_critical_error_01(self):
+        h = GeneralErrorHook()
+        variable_store = VariableStore()
+        variable_store.add_variable(variable_name='__GLOBAL__:NoneCriticalErrorMessage', value='Test Non Critical Error')
+        variable_store = h.run(task=self.task, variable_store=variable_store)
+
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
         )
-        t_4 = Task(
-            kind='Processor1',
-            version='v1',
-            metadata={
-                "identifiers": [
-                    {
-                        "type": "ManifestName",
-                        "key": "t_4"
-                    },
-                    {
-                        "type": "Label",
-                        "key": "is_unittest",
-                        "value": "TRUE"
-                    }
-                ],
-                "dependencies": [
-                    {
-                        "identifierType": "ManifestName",
-                        "identifiers": [
-                            { "key": "t_1" },
-                            { "key": "t_2" },
-                        ]
-                    }
-                ]
-            },
-            spec={'field1': 'value1'},
-            logger=self.logger
+        dump_events(
+            task_id=self.task.task_id,
+            variable_store=copy.deepcopy(variable_store)
         )
 
-        tasks_to_process = [t_1,t_2,t_3,t_4]
-        permutations_of_tasks = list(permutations(tasks_to_process))
+        self.assertTrue('Test Non Critical Error' in logger.error_lines[0])
 
-        processing_target_identifier = build_command_identifier(command='test', context='test')
-        set_nr = 0
-        for permutation_set in permutations_of_tasks:
-            set_nr += 1
-            print('Set #{}'.format(set_nr))
-            tasks = Tasks(logger=self.logger)
-            tasks.register_task_processor(processor=shell_script)
-            task: Task
-            added_task_order = list()
-            for task in permutation_set:
-                print('   Adding task "{}"'.format(task.task_id))
-                added_task_order.append(task.task_id)
-                tasks.add_task(task=task)
-            calculated_task_order = tasks.calculate_current_task_order(processing_target_identifier=processing_target_identifier)
-            print('   calculated_task_order={}'.format(calculated_task_order))
-            tasks = None
-            self.assertTrue(validate_order(must_be_before_input_task_name='t_2', input_task_name='t_1', list_of_tasks=calculated_task_order), 'Set #{} - Expected t_2 to be before t_1: added_task_order={}   calculated_task_order={}'.format(set_nr, added_task_order, calculated_task_order))
-            self.assertTrue(validate_order(must_be_before_input_task_name='t_3', input_task_name='t_1', list_of_tasks=calculated_task_order), 'Set #{} - Expected t_3 to be before t_1: added_task_order={}   calculated_task_order={}'.format(set_nr, added_task_order, calculated_task_order))
-            self.assertTrue(validate_order(must_be_before_input_task_name='t_3', input_task_name='t_2', list_of_tasks=calculated_task_order), 'Set #{} - Expected t_3 to be before t_2: added_task_order={}   calculated_task_order={}'.format(set_nr, added_task_order, calculated_task_order))
-            self.assertTrue(validate_order(must_be_before_input_task_name='t_1', input_task_name='t_4', list_of_tasks=calculated_task_order), 'Set #{} - Expected t_1 to be before t_4: added_task_order={}   calculated_task_order={}'.format(set_nr, added_task_order, calculated_task_order))
-            self.assertTrue(validate_order(must_be_before_input_task_name='t_2', input_task_name='t_4', list_of_tasks=calculated_task_order), 'Set #{} - Expected t_2 to be before t_4: added_task_order={}   calculated_task_order={}'.format(set_nr, added_task_order, calculated_task_order))
-            print_logger_lines(logger=self.logger)
-            self.logger = None
-            self.logger = TestLogger()
 
-
-class TestFunctionRandomString(unittest.TestCase):    # pragma: no cover
+class TestClassHooks(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
+        logger.reset()
+        self.task = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task'},
+            spec={'testField': 'testValue'}
+        )
 
-    def test_generate_random_str_1(self):
-        result = random_string(string_length=4, character_set='abc')
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, str)
-        characters_that_must_not_be_present = 'defghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ 0123456789'
-        for char in characters_that_must_not_be_present:
-            self.assertFalse(char in result, 'Unexpectedly found character "{}" in result "{}"'.format(char, result))
+    def tearDown(self):
+        self.task = None
+        return super().tearDown()
+    
+    def test_basic_hooks_class_init_01(self):
+        hooks = Hooks()
+        self.assertIsNotNone(hooks)
+        self.assertIsInstance(hooks, Hooks)
+        
+        self.assertIsNotNone(hooks.hooks)
+        self.assertIsInstance(hooks.hooks, list)
+        self.assertEqual(len(hooks.hooks), 0)
 
+        self.assertIsNotNone(hooks.general_error_hook)
+        self.assertIsInstance(hooks.general_error_hook, GeneralErrorHook)
 
-class TestFunctionProduceColumnHeaders(unittest.TestCase):    # pragma: no cover
+    def test_method_add_hook_01(self):
+        hooks = Hooks()
+        hooks.add_hook(hook=TaskProcessingHook())
+        hooks.add_hook(hook=TaskPostProcessingStateUpdateHook())
 
-    def setUp(self):
-        print()
-        print('-'*80)
+        self.assertIsNotNone(hooks.hooks)
+        self.assertIsInstance(hooks.hooks, list)
+        self.assertEqual(len(hooks.hooks), 2)
 
-    def test_generate_header_as_string_1(self):
-        result = produce_column_headers()
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, str)
+        self.assertIsInstance(hooks.hooks[0], TaskProcessingHook)
+        self.assertIsInstance(hooks.hooks[1], TaskPostProcessingStateUpdateHook)
 
+    def test_method_get_hook_by_name_returns_valid_requested_hook_01(self):
+        hooks = Hooks()
+        hooks.add_hook(hook=TaskProcessingHook())
+        hooks.add_hook(hook=TaskPostProcessingStateUpdateHook())
 
-class TestFunctionProduceColumnHeaderHorizontalLine(unittest.TestCase):    # pragma: no cover
+        task_processing_hook = hooks.get_hook_by_name(name='TaskProcessingHook')
+        self.assertIsInstance(task_processing_hook, TaskProcessingHook)
 
-    def setUp(self):
-        print()
-        print('-'*80)
+        task_post_processing_state_update_hook = hooks.get_hook_by_name(name='TaskPostProcessingStateUpdateHook')
+        self.assertIsInstance(task_post_processing_state_update_hook, TaskPostProcessingStateUpdateHook)
 
-    def test_generate_horizontal_line_as_string_1(self):
-        result = produce_column_header_horizontal_line()
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, str)
-        for char in result:
-            self.assertTrue('-' in char, 'Unexpected character "{}" found in horizontal line "{}"'.format(char,result))
+    def test_method_get_hook_by_name_returns_string_when_requesting_hook_not_registered_01(self):
+        hooks = Hooks()
+        hooks.add_hook(hook=TaskProcessingHook())
+        hooks.add_hook(hook=TaskPostProcessingStateUpdateHook())
 
+        non_hook = hooks.get_hook_by_name(name='NonExistingHook')
+        self.assertEqual(non_hook, 'not-a-hook')
+
+    def test_class_as_collection_01(self):
+        hooks = Hooks()
+        hooks.add_hook(hook=TaskProcessingHook())
+        hooks.add_hook(hook=TaskPostProcessingStateUpdateHook())
+
+        self.assertEqual(len(hooks), 2)
+        for hook in hooks:
+            self.assertIsInstance(hook, Hook)
 
-class TestClassTaskState(unittest.TestCase):    # pragma: no cover
+
+class TestClassWorkflowExecutor(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print()
         print('-'*80)
+        logger.reset()
+        self.task_01 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-01'},
+            spec={'testField': 'testValue'}
+        )
+        self.task_02 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-02'},
+            spec={'testField': 'testValue'}
+        )
+        self.task_03 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-03'},
+            spec={'testField': 'testValue'}
+        )
+        self.task_04 = Task(
+            api_version='DummyTaskProcessor1/v1',
+            kind='DummyTaskProcessor1',
+            metadata={'name': 'test-task-04'},
+            spec={'testField': 'testValue'}
+        )
+
+        # Add processing scopes to tasks
+        self.task_01.metadata['processingScope'] = [
+            {
+                'commands': ['create', 'delete',],
+                'contexts': ['con1','con2'],
+            },
+        ]
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['create', 'delete',],
+                'contexts': ['con1','con2',],
+            }
+        ]
+        self.task_03.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01',],
+                'commands': ['delete', 'update',],
+                'contexts': ['con2','con3'],
+            }
+        ]
+        self.task_03.metadata['processingScopes'] = [
+            {
+                'commands': ['delete', 'update',],
+                'contexts': ['con2','con3'],
+            },
+        ]
+
+        # Add task dependencies
+        self.task_01.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-04',],
+            }
+        ]
+        self.task_02.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-01','test-task-03',],
+            }
+        ]
+        self.task_04.metadata['dependencies'] = [
+            {
+                'tasks': ['test-task-03',],
+            }
+        ]
+
+        self.tasks = Tasks()
+        self.tasks.add_task(task=self.task_01)
+        self.tasks.add_task(task=self.task_02)
+        self.tasks.add_task(task=self.task_03)
+        self.tasks.add_task(task=self.task_04)
+        
+        self.task_processor_store = TaskProcessStore()
+        self.task_processor_store.register_task_processor(task_processor=DummyTaskProcessor1())
 
-    def test_produce_basic_report_string_1(self):
-        ts = TaskState(
-            manifest_spec={'field1': 'abc'},
-            applied_spec=None,
-            resolved_spec={'field1': 'abc'},
-            manifest_metadata={},
-            report_label='TEST_LABEL',
-            created_timestamp=0
-        )
-        report = str(ts)
-        print(report)
-        self.assertIsNotNone(report)
-        self.assertIsInstance(report, str)
-        self.assertTrue('\n' in report)
-
-    def test_produce_extended_report_string_1(self):
-        ts = TaskState(
-            manifest_spec={'field1': 'abc'},
-            applied_spec={'field1': 'abc'},
-            resolved_spec={'field1': 'abc'},
-            manifest_metadata={},
-            report_label='TEST_LABEL',
-            created_timestamp=1000,
-            applied_resources_checksum=hashlib.sha256('test'.encode('utf-8')).hexdigest(),
-            current_resource_checksum=hashlib.sha256('test'.encode('utf-8')).hexdigest()
-        )
-        report = '{}\n{}\n{}'.format(
-            produce_column_headers(with_checksums=True),
-            produce_column_header_horizontal_line(with_checksums=True, line_char='+'),
-            ts.column_str(human_readable=True, current_resolved_spec={'field1': 'abc'}, with_checksums=True)
-        )
-        print('JSON value of task_state_summary_as_dict: {}'.format(json.dumps(ts.to_dict(human_readable=True, current_resolved_spec={'field1': 'abc'}, with_checksums=True))))
-        print()
-        print(report)
-        print()
-        self.assertIsNotNone(report)
-        self.assertIsInstance(report, str)
-        self.assertTrue('\n' in report)
-
-    def _validate_task_state_summary_as_dict_against_dict_tests(self, task_state_summary_as_dict: dict, dict_tests: dict):
-        for key, test_config in dict_tests.items():
-            validate_value = True
-            if test_config['mustBePresent'] is True:
-                self.assertTrue(key in task_state_summary_as_dict, 'Expected key "{}" but it was NOT present. Keys: {}'.format(key, list(task_state_summary_as_dict.keys())))                
-            else:
-                self.assertFalse(key in task_state_summary_as_dict, 'NOT Expecting key "{}" but it was present. Keys: {}'.format(key, list(task_state_summary_as_dict.keys())))
-                validate_value = False
-                if key in task_state_summary_as_dict is True:
-                    validate_value = True
-            if validate_value is True:
-                if test_config['canBeNone'] is False:
-                    self.assertIsNotNone(task_state_summary_as_dict[key], 'Value of key "{}" can not be NONE.'.format(key))
-                if task_state_summary_as_dict[key] is not None:
-                    self.assertIsInstance(task_state_summary_as_dict[key], test_config['type'], 'Key "{}" type expected was "{}" but found "{}"'.format(key, test_config['type'], type(task_state_summary_as_dict[key])))
-                    self.assertEqual(task_state_summary_as_dict[key], test_config['expectedValue'], 'Key "{}" value expected was "{}" but found "{}"'.format(key, test_config['expectedValue'], task_state_summary_as_dict[key]))
-
-
-    def test_to_dict_basic_not_yet_applied_1(self):
-        ts = TaskState(
-            manifest_spec={'field1': 'abc'},
-            applied_spec=None,
-            resolved_spec={'field1': 'abc'},
-            manifest_metadata={},
-            report_label='TEST_LABEL',
-            created_timestamp=0
-        )
-        task_state_summary_as_dict = ts.to_dict(human_readable=False, current_resolved_spec={'field1': 'abc'}, with_checksums=False, include_applied_spec=False)
-        print('JSON value of task_state_summary_as_dict: {}'.format(json.dumps(task_state_summary_as_dict)))
-        print()
-        print(str(ts))
-        print()
-        self.assertIsNotNone(task_state_summary_as_dict)
-        self.assertIsInstance(task_state_summary_as_dict, dict)
-
-        dict_tests = {
-            'Label': {
-                'type': str,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': 'TEST_LABEL',
-            },
-            'IsCreated': {
-                'type': bool,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': False,
-            },
-            'CreatedTimestamp': {
-                'type': int,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': None,
-            },
-            'SpecDrifted': {
-                'type': bool,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': False,
-            },
-            'ResourceDrifted': {
-                'type': bool,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': None,
-            },
-            'AppliedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'CurrentResolvedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'AppliedResourcesChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'CurrentResourceChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'AppliedSpec': {
-                'type': dict,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-        }
-        self._validate_task_state_summary_as_dict_against_dict_tests(task_state_summary_as_dict=task_state_summary_as_dict, dict_tests=dict_tests)
+        self.hooks = Hooks()
+        self.hooks.add_hook(hook=TaskProcessingHook())
+        self.hooks.add_hook(hook=TaskPostProcessingStateUpdateHook())
 
-    def test_to_dict_basic_applied_and_no_diff_from_current_spec1(self):
-        ts = TaskState(
-            manifest_spec={},
-            applied_spec={'field1': 'abc'},
-            resolved_spec={'field1': 'abc'},
-            manifest_metadata={},
-            report_label='TEST_LABEL',
-            created_timestamp=1710686853
-        )
-        task_state_summary_as_dict = ts.to_dict(human_readable=False, current_resolved_spec={'field1': 'abc'}, with_checksums=False, include_applied_spec=False)
-        print('JSON value of task_state_summary_as_dict: {}'.format(json.dumps(task_state_summary_as_dict)))
-        print()
-        print(str(ts))
-        print()
-        self.assertIsNotNone(task_state_summary_as_dict)
-        self.assertIsInstance(task_state_summary_as_dict, dict)
+        logger.reset()
 
-        dict_tests = {
-            'Label': {
-                'type': str,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': 'TEST_LABEL',
-            },
-            'IsCreated': {
-                'type': bool,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': True,
-            },
-            'CreatedTimestamp': {
-                'type': int,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': 1710686853,
-            },
-            'SpecDrifted': {
-                'type': bool,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': False,
-            },
-            'ResourceDrifted': {
-                'type': bool,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': None,
-            },
-            'AppliedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'CurrentResolvedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'AppliedResourcesChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'CurrentResourceChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'AppliedSpec': {
-                'type': dict,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-        }
-        self._validate_task_state_summary_as_dict_against_dict_tests(task_state_summary_as_dict=task_state_summary_as_dict, dict_tests=dict_tests)
+    def tearDown(self):
+        self.task_01 = None
+        self.task_02 = None
+        self.task_03 = None
+        self.task_04 = None
+        self.tasks = None
+        self.task_processor_store = None
+        self.hooks = None
+        return super().tearDown()
+    
+    def test_class_workflow_executor_init_01(self):
+        we = WorkflowExecutor(task_process_store=self.task_processor_store)
+        self.assertIsNotNone(we)
+        self.assertIsInstance(we, WorkflowExecutor)
 
-    def test_to_dict_basic_applied_with_diff_from_current_spec_but_no_diff_to_detected_resources_1(self):
-        ts = TaskState(
-            manifest_spec={},
-            applied_spec={'field1': 'abc'},
-            resolved_spec={'field1': 'abc'},
-            manifest_metadata={},
-            report_label='TEST_LABEL',
-            created_timestamp=1710686853
-        )
-        task_state_summary_as_dict = ts.to_dict(human_readable=False, current_resolved_spec={'field1': 'xyz'}, with_checksums=False, include_applied_spec=False)
-        print('JSON value of task_state_summary_as_dict: {}'.format(json.dumps(task_state_summary_as_dict)))
-        print()
-        print(str(ts))
-        print()
-        self.assertIsNotNone(task_state_summary_as_dict)
-        self.assertIsInstance(task_state_summary_as_dict, dict)
+    def test_methods_to_add_custom_commands(self):
+        we = WorkflowExecutor(task_process_store=self.task_processor_store)
+        
+        for command in ('create', 'delete', 'update', 'rollback', 'describe', 'drift', ):
+            self.assertTrue(command in we.command_to_action_map)
+        self.assertEqual(we.command_to_action_map['create'], 'CreateAction')
+        self.assertEqual(we.command_to_action_map['delete'], 'DeleteAction')
+        self.assertEqual(we.command_to_action_map['update'], 'UpdateAction')
+        self.assertEqual(we.command_to_action_map['rollback'], 'RollbackAction')
+        self.assertEqual(we.command_to_action_map['describe'], 'DescribeAction')
+        self.assertEqual(we.command_to_action_map['drift'], 'DetectDriftAction')
+
+        we.link_command_to_create_action(command='custom_create_command')
+        we.link_command_to_delete_action(command='custom_delete_command')
+        we.link_command_to_update_action(command='custom_update_command')
+        we.link_command_to_rollback_action(command='custom_rollback_command')
+        we.link_command_to_describe_action(command='custom_describe_command')
+        we.link_command_to_detect_drift_action(command='custom_drift_command')
+
+        for command in ('create', 'delete', 'update', 'rollback', 'describe', 'drift', ):
+            self.assertFalse(command in we.command_to_action_map)
+        for command in ('custom_create_command', 'custom_delete_command', 'custom_update_command', 'custom_rollback_command', 'custom_describe_command', 'custom_drift_command', ):
+            self.assertTrue(command in we.command_to_action_map)
+        self.assertEqual(we.command_to_action_map['custom_create_command'], 'CreateAction')
+        self.assertEqual(we.command_to_action_map['custom_delete_command'], 'DeleteAction')
+        self.assertEqual(we.command_to_action_map['custom_update_command'], 'UpdateAction')
+        self.assertEqual(we.command_to_action_map['custom_rollback_command'], 'RollbackAction')
+        self.assertEqual(we.command_to_action_map['custom_describe_command'], 'DescribeAction')
+        self.assertEqual(we.command_to_action_map['custom_drift_command'], 'DetectDriftAction')
+
+    def test_method_add_workflow_step_by_hook_name_basic_01(self):
+        we = WorkflowExecutor(task_process_store=self.task_processor_store)
+        self.assertEqual(len(we.ordered_workflow_steps), 0)
+
+        we.add_workflow_step_by_hook_name(hook_name='TaskProcessingHook', hooks=self.hooks)
+        we.add_workflow_step_by_hook_name(hook_name='TaskPostProcessingStateUpdateHook', hooks=self.hooks)
+        we.add_workflow_step_by_hook_name(hook_name='NonExistingHookTYhatWillBeIgnored', hooks=self.hooks)
+
+        self.assertEqual(len(we.ordered_workflow_steps), 2)
+        self.assertIsInstance(we.ordered_workflow_steps[0], TaskProcessingHook)
+        self.assertIsInstance(we.ordered_workflow_steps[1], TaskPostProcessingStateUpdateHook)
+
+    def test_method_add_workflow_step_by_hook_instance_basic_01(self):
+        we = WorkflowExecutor(task_process_store=self.task_processor_store)
+        self.assertEqual(len(we.ordered_workflow_steps), 0)
+
+        we.add_workflow_step_by_hook_instance(hook=None)
+        we.add_workflow_step_by_hook_instance(hook='InvalidHookType')
+        we.add_workflow_step_by_hook_instance(hook=TaskProcessingHook())
+        we.add_workflow_step_by_hook_instance(hook=TaskPostProcessingStateUpdateHook())
+
+        self.assertEqual(len(we.ordered_workflow_steps), 2)
+        self.assertIsInstance(we.ordered_workflow_steps[0], TaskProcessingHook)
+        self.assertIsInstance(we.ordered_workflow_steps[1], TaskPostProcessingStateUpdateHook)
+
+    def test_method_add_task_01(self):
+        we = WorkflowExecutor(task_process_store=self.task_processor_store)
+        self.assertEqual(len(we.tasks), 0)
+
+        we.add_task(task=self.task_01)
+        we.add_task(task=self.task_02)
+        we.add_task(task=self.task_03)
+        we.add_task(task=self.task_04)
+
+        self.assertEqual(len(we.tasks), 4)
+
+    def test_method_execute_workflow_01(self):
+        variable_store = VariableStore()
+        we = WorkflowExecutor(task_process_store=self.task_processor_store, variable_store=variable_store)
+        we.add_task(task=self.task_01)
+        we.add_task(task=self.task_02)
+        we.add_task(task=self.task_03)
+        we.add_task(task=self.task_04)
+        we.add_workflow_step_by_hook_instance(hook=TaskProcessingHook())
+        we.add_workflow_step_by_hook_instance(hook=TaskPostProcessingStateUpdateHook())
+        variable_store = we.execute_workflow(command='create', context='con1')
 
-        dict_tests = {
-            'Label': {
-                'type': str,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': 'TEST_LABEL',
-            },
-            'IsCreated': {
-                'type': bool,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': True,
-            },
-            'CreatedTimestamp': {
-                'type': int,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': 1710686853,
-            },
-            'SpecDrifted': {
-                'type': bool,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': True,
-            },
-            'ResourceDrifted': {
-                'type': bool,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': None,
-            },
-            'AppliedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'CurrentResolvedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'AppliedResourcesChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'CurrentResourceChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-            'AppliedSpec': {
-                'type': dict,
-                'canBeNone': True,
-                'mustBePresent': False,
-                'expectedValue': None,
-            },
-        }
-        self._validate_task_state_summary_as_dict_against_dict_tests(task_state_summary_as_dict=task_state_summary_as_dict, dict_tests=dict_tests)
+        print_logger_lines(logger=logger)
+        dump_variable_store(
+            test_class_name=self.__class__.__name__,
+            test_method_name=stack()[0][3],
+            variable_store=copy.deepcopy(variable_store)
+        )
+        dump_events(
+            task_id=self.task_01.task_id,
+            variable_store=copy.deepcopy(variable_store)
+        )
+
+    def test_method_execute_workflow_no_ordered_workflow_produces_exception_01(self):
+        variable_store = VariableStore()
+        we = WorkflowExecutor(task_process_store=self.task_processor_store, variable_store=variable_store)
+        we.add_task(task=self.task_01)
+        we.add_task(task=self.task_02)
+        we.add_task(task=self.task_03)
+        we.add_task(task=self.task_04)
+        with self.assertRaises(Exception):
+            we.execute_workflow(command='create', context='con1')
 
+        print_logger_lines(logger=logger)
 
-    def test_to_dict_basic_applied_with_no_diff_from_current_spec_and_diff_detected_resources_1(self):
-        ts = TaskState(
-            manifest_spec={'field1': 'abc'},
-            applied_spec={'field1': 'abc'},
-            resolved_spec={'field1': 'abc'},
-            manifest_metadata={},
-            report_label='TEST_LABEL',
-            created_timestamp=1710686853,
-            applied_resources_checksum=hashlib.sha256('check-1'.encode('utf-8')).hexdigest()
-        )
-        task_state_summary_as_dict = ts.to_dict(
-            human_readable=False,
-            current_resolved_spec={'field1': 'abc'},
-            with_checksums=True,
-            include_applied_spec=True,
-            current_resource_checksum=hashlib.sha256('check-2'.encode('utf-8')).hexdigest()
-        )
-        print('JSON value of task_state_summary_as_dict: {}'.format(json.dumps(task_state_summary_as_dict)))
-        print()
-        print(str(ts))
-        print()
-        self.assertIsNotNone(task_state_summary_as_dict)
-        self.assertIsInstance(task_state_summary_as_dict, dict)
+    def test_method_execute_workflow_unrecognized_command_produces_exception_01(self):
+        variable_store = VariableStore()
+        we = WorkflowExecutor(task_process_store=self.task_processor_store, variable_store=variable_store)
+        we.add_task(task=self.task_01)
+        we.add_task(task=self.task_02)
+        we.add_task(task=self.task_03)
+        we.add_task(task=self.task_04)
+        we.add_workflow_step_by_hook_instance(hook=TaskProcessingHook())
+        we.add_workflow_step_by_hook_instance(hook=TaskPostProcessingStateUpdateHook())
+        with self.assertRaises(Exception):
+            we.execute_workflow(command='this_command_does_not_exist', context='con1')
+
+    def test_method_execute_workflow_task_exception_01(self):
+        variable_store = VariableStore()
+        variable_store.add_variable(
+            variable_name='{}:UNITTEST_TROW_EXCEPTION'.format(self.task_01.task_id),
+            value=True
+        )
+        we = WorkflowExecutor(task_process_store=self.task_processor_store, variable_store=variable_store)
+        we.add_task(task=self.task_01)
+        we.add_task(task=self.task_02)
+        we.add_task(task=self.task_03)
+        we.add_task(task=self.task_04)
+        we.add_workflow_step_by_hook_instance(hook=TaskProcessingHook())
+        we.add_workflow_step_by_hook_instance(hook=TaskPostProcessingStateUpdateHook())
+        with self.assertRaises(Exception):
+            we.execute_workflow(command='create', context='con1')
 
-        dict_tests = {
-            'Label': {
-                'type': str,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': 'TEST_LABEL',
-            },
-            'IsCreated': {
-                'type': bool,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': True,
-            },
-            'CreatedTimestamp': {
-                'type': int,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': 1710686853,
-            },
-            'SpecDrifted': {
-                'type': bool,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': False,
-            },
-            'ResourceDrifted': {
-                'type': bool,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': True,
-            },
-            'AppliedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': '83b5b0e4aa22036e6e64cc4a38bf4226d5c5b295d948ff7babefc6949ce2ac10',
-            },
-            'CurrentResolvedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': '83b5b0e4aa22036e6e64cc4a38bf4226d5c5b295d948ff7babefc6949ce2ac10',
-            },
-            'AppliedResourcesChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': hashlib.sha256('check-1'.encode('utf-8')).hexdigest(),
-            },
-            'CurrentResourceChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': hashlib.sha256('check-2'.encode('utf-8')).hexdigest(),
-            },
-            'AppliedSpec': {
-                'type': dict,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': {'field1': 'abc'},
-            },
-        }
-        self._validate_task_state_summary_as_dict_against_dict_tests(task_state_summary_as_dict=task_state_summary_as_dict, dict_tests=dict_tests)
+        print_logger_lines(logger=logger)
 
-    def test_helper_method__cut_str_no_effect(self):
-        s = 'abcdef'
-        ts = TaskState()
-        result = ts._cut_str(input_str=s, max_len=10)
-        self.assertEqual(result, s)
-
-    def test_helper_method__cut_str_shorten_string(self):
-        s = 'abcdefabcdef'
-        e = 'abcdefabcd'
-        ts = TaskState()
-        result = ts._cut_str(input_str=s, max_len=10)
-        self.assertEqual(result, e)
-
-    def test_repr_1(self):
-        ts = TaskState(
-            manifest_spec={'field1': 'abc'},
-            applied_spec={'field1': 'abc'},
-            resolved_spec={'field1': 'abc'},
-            manifest_metadata={},
-            report_label='TEST_LABEL',
-            created_timestamp=1710686853,
-            applied_resources_checksum=hashlib.sha256('check-1'.encode('utf-8')).hexdigest()
-        )
-        task_state_summary_as_str = repr(ts)
-        print('JSON value of task_state_summary_as_dict: {}'.format(task_state_summary_as_str))
-        print()
-        print(str(ts))
-        print()
-        self.assertIsNotNone(task_state_summary_as_str)
-        self.assertIsInstance(task_state_summary_as_str, str)
-        task_state_summary_as_dict = json.loads(task_state_summary_as_str)
-
-        dict_tests = {
-            'Label': {
-                'type': str,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': 'TEST_LABEL',
-            },
-            'IsCreated': {
-                'type': bool,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': True,
-            },
-            'CreatedTimestamp': {
-                'type': int,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': 1710686853,
-            },
-            'SpecDrifted': {
-                'type': bool,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': False,
-            },
-            'ResourceDrifted': {
-                'type': bool,
-                'canBeNone': False,
-                'mustBePresent': True,
-                'expectedValue': True,
-            },
-            'AppliedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': '83b5b0e4aa22036e6e64cc4a38bf4226d5c5b295d948ff7babefc6949ce2ac10',
-            },
-            'CurrentResolvedSpecChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': '6b1791a6b1ebdffc9f2de2e7578c56c5d96c0601a95f2de48844c6f2f342a8b6',
-            },
-            'AppliedResourcesChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': hashlib.sha256('check-1'.encode('utf-8')).hexdigest(),
-            },
-            'CurrentResourceChecksum': {
-                'type': str,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': hashlib.sha256('check-2'.encode('utf-8')).hexdigest(),
-            },
-            'AppliedSpec': {
-                'type': dict,
-                'canBeNone': True,
-                'mustBePresent': True,
-                'expectedValue': {'field1': 'abc'},
-            },
-        }
-        self._validate_task_state_summary_as_dict_against_dict_tests(task_state_summary_as_dict=task_state_summary_as_dict, dict_tests=dict_tests)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `magnum_opus-2.3/.gitignore` & `magnum_opus-3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `magnum_opus-2.3/LICENSE` & `magnum_opus-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_opus-2.3/README.md` & `magnum_opus-3.0/README.md`

 * *Files identical despite different names*

### Comparing `magnum_opus-2.3/pyproject.toml` & `magnum_opus-3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "magnum-opus"
-version = "2.3"
+version = "3.0"
 dependencies = []
 requires-python = ">= 3.10"
 authors = [
   {name = "Nico Coetzee", email = "nicc777@gmail.com"}
 ]
 maintainers = [
   {name = "Nico Coetzee", email = "nicc777@gmail.com"}
```

### Comparing `magnum_opus-2.3/PKG-INFO` & `magnum_opus-3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: magnum-opus
-Version: 2.3
+Version: 3.0
 Summary: An extendable general purpose task manager or workflow engine.
 Project-URL: Homepage, https://github.com/nicc777/magnum-opus
 Project-URL: Documentation, https://github.com/nicc777/magnum-opus
 Project-URL: Repository, https://github.com/nicc777/magnum-opus
 Project-URL: Issues, https://github.com/nicc777/magnum-opus/issues
 Project-URL: Changelog, https://raw.githubusercontent.com/nicc777/magnum-opus/main/CHANGELOG.md
 Author-email: Nico Coetzee <nicc777@gmail.com>
```

