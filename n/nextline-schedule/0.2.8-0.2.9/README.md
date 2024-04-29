# Comparing `tmp/nextline_schedule-0.2.8.tar.gz` & `tmp/nextline_schedule-0.2.9.tar.gz`

## Comparing `nextline_schedule-0.2.8.tar` & `nextline_schedule-0.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/setup.cfg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/dependabot.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/release.yml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/workflows/release.yml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/__about__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/default.toml
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/py.typed
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/scheduler.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/types.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/auto/__init__.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/auto/callback.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/auto/factory.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/auto/machine.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/queries/AutoMode.gql
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/queries/Scheduler.gql
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/queries/Version.gql
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/schema/__init__.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/schema/mutation.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/schema/query.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/schema/subscription.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_fsm.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_plugin.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_request.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_scratch.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/auto/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/auto/test_auto.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/auto/test_auto_on_raised.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/auto/test_auto_turn_off.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/schema/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/schema/queries/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/schema/queries/test_version.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/LICENSE.txt
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/README.md
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/setup.cfg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/release.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/__about__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/default.toml
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/py.typed
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/scheduler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/types.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/auto/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/auto/callback.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/auto/factory.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/auto/machine.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/queries/AutoMode.gql
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/queries/Scheduler.gql
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/queries/Version.gql
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/schema/__init__.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/schema/mutation.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/schema/query.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/schema/subscription.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_fsm.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_plugin.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_request.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_scratch.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/auto/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/auto/test_auto.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/auto/test_auto_on_raised.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/auto/test_auto_turn_off.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/schema/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/schema/queries/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/schema/queries/test_version.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/LICENSE.txt
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/README.md
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/PKG-INFO
```

### Comparing `nextline_schedule-0.2.8/.github/workflows/pypi.yml` & `nextline_schedule-0.2.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/.github/workflows/release.yml` & `nextline_schedule-0.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/.github/workflows/type-check.yml` & `nextline_schedule-0.2.9/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/.github/workflows/unit-test.yml` & `nextline_schedule-0.2.9/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/src/nextline_schedule/plugin.py` & `nextline_schedule-0.2.9/src/nextline_schedule/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/src/nextline_schedule/scheduler.py` & `nextline_schedule-0.2.9/src/nextline_schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/src/nextline_schedule/auto/callback.py` & `nextline_schedule-0.2.9/src/nextline_schedule/auto/callback.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 import asyncio
 from logging import getLogger
 from typing import Any, Callable, Coroutine
 
 from nextline import Nextline
+from nextline.plugin.spec import Context, hookimpl
 
 from nextline_schedule.types import Statement
 
 from .machine import AutoModeStateMachine
 
 
 def build_auto_mode_state_machine(
     nextline: Nextline,
     request_statement: Callable[[], Coroutine[Any, Any, Statement]],
 ) -> AutoModeStateMachine:
     callback = Callback(nextline=nextline, request_statement=request_statement)
     machine = AutoModeStateMachine(callback=callback)
     callback.auto_mode = machine
+    on_call = OnCall(auto_mode=machine)
+    nextline.register(on_call)
     return machine
 
 
+class OnCall:
+    def __init__(self, auto_mode: AutoModeStateMachine):
+        self.auto_mode = auto_mode
+
+    @hookimpl
+    async def on_initialize_run(self) -> None:
+        await self.auto_mode.on_initialized()  # type: ignore
+
+    @hookimpl
+    async def on_finished(self, context: Context) -> None:
+        nextline = context.nextline
+        if nextline.format_exception():
+            await self.auto_mode.on_raised()  # type: ignore
+            return
+        await self.auto_mode.on_finished()  # type: ignore
+
+
 class Callback:
     def __init__(
         self,
         nextline: Nextline,
         request_statement: Callable[[], Coroutine[Any, Any, Statement]],
     ):
         self._nextline = nextline
         self._request_statement = request_statement
-
         self._logger = getLogger(__name__)
-
         self.auto_mode: AutoModeStateMachine  # to be set
 
     async def wait(self) -> None:
-        try:
-            async for state in self._nextline.subscribe_state():
-                if state == 'initialized':
-                    await self.auto_mode.on_initialized()  # type: ignore
-                    break
-                if state == 'finished':
-                    await self.auto_mode.on_finished()  # type: ignore
-                    break
-        except asyncio.CancelledError:
-            self._logger.info(f'{self.__class__.__name__}.wait() cancelled')
-        return
+        match self._nextline.state:
+            case 'initialized':
+                await self.auto_mode.on_initialized()  # type: ignore
+            case 'finished':
+                await self.auto_mode.on_finished()  # type: ignore
 
     async def pull(self) -> None:
         try:
             try:
                 statement = await self._request_statement()
             except Exception:
                 self._logger.exception('')
@@ -57,13 +69,9 @@
             await self.auto_mode.run()  # type: ignore
         except asyncio.CancelledError:
             self._logger.info(f'{self.__class__.__name__}.pull() cancelled')
 
     async def run(self, started: asyncio.Event) -> None:
         try:
             await self._nextline.run_continue_and_wait(started)
-            if self._nextline.format_exception():
-                await self.auto_mode.on_raised()  # type: ignore
-                return
-            await self.auto_mode.on_finished()  # type: ignore
         except asyncio.CancelledError:
             self._logger.info(f'{self.__class__.__name__}.run() cancelled')
```

### Comparing `nextline_schedule-0.2.8/src/nextline_schedule/auto/factory.py` & `nextline_schedule-0.2.9/src/nextline_schedule/auto/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,43 +16,44 @@
                                 | start()
                                 |
                                 v
                          .-------------.
          .-------------->|     Off     |<--------------.
          |               '-------------'               |
          |                      | turn_on()            |
-       turn_off()               |                      |
-         |                      v                      |
-         |               .-------------.               |
-         |---------------|   Waiting   |          on_raised()
-         |               '-------------'               |
-         |                      | on_initialized()     |
-         |                      | on_finished()        |
+       turn_off()               |                 on_raised()
+         |                      |                      |
          |                      |                      |
          |   .------------------+------------------.   |
          |   |   Auto           |                  |   |
          |   |                  v                  |   |
          |   |           .-------------.           |   |
+         |   |           |   Waiting   |           |   |
+         |   |           '-------------'           |   |
+         |   |                  | on_initialized() |   |
+         |   |                  | on_finished()    |   |
+         |   |                  v                  |   |
+         |   |           .-------------.           |   |
          |   |           |   Pulling   |           |   |
          '---|           '-------------'           |---'
              |         run() |     ^               |
              |               |     |               |
              |               v     | on_finished() |
              |           .-------------.           |
              |           |   Running   |           |
              |           '-------------'           |
              |                                     |
              '-------------------------------------'
 
     >>> class Model:
-    ...     def on_enter_waiting(self):
+    ...     def on_enter_auto_waiting(self):
     ...         print('enter the waiting state')
     ...         self.on_finished()
     ...
-    ...     def on_exit_waiting(self):
+    ...     def on_exit_auto_waiting(self):
     ...        print('exit the waiting state')
     ...
     ...     def on_enter_auto_pulling(self):
     ...        print('enter the pulling state')
 
     >>> model = Model()
     >>> machine = build_state_machine(model=model, asyncio=False)
@@ -84,51 +85,50 @@
 
     # Build a state machine with nested states from dict configs with "remap"
     # in the way described in the docs:
     # https://github.com/pytransitions/transitions/tree/0.9.0#reuse-of-previously-created-hsms
 
     auto_state_conf = {
         'name': 'auto',
-        'states': ['pulling', 'running'],
+        'states': ['waiting', 'pulling', 'running'],
         'transitions': [
+            ['on_initialized', 'waiting', 'pulling'],
+            ['on_finished', 'waiting', 'pulling'],
             ['run', 'pulling', 'running'],
             ['on_finished', 'running', 'pulling'],
         ],
-        'initial': 'pulling',
+        'initial': 'waiting',
         'queued': True,
-        # 'ignore_invalid_triggers': True,
+        'ignore_invalid_triggers': True,
     }
 
     # Ideally, we would be able to pass the auto_state_conf dict directly to
     # the MachineClass constructor, but this doesn't work with "remap."
     # Instead, we have to create a new instance of the MachineClass and pass it
     # to the parent state machine.
     auto_state = MachineClass(model=None, **auto_state_conf)  # type: ignore
 
     state_conf = {
         'name': 'global',
         'states': [
             'created',
             'off',
-            'waiting',
             {'name': 'auto', 'children': auto_state},
         ],
         'transitions': [
             ['start', 'created', 'off'],
-            ['turn_on', 'off', 'waiting'],
-            ['on_initialized', 'waiting', 'auto'],
-            ['on_finished', 'waiting', 'auto'],
+            ['turn_on', 'off', 'auto'],
             ['on_raised', 'auto', 'off'],
             {
                 'trigger': 'turn_off',
-                'source': ['waiting', 'auto'],
+                'source': 'auto',
                 'dest': 'off',
                 'before': 'cancel_task',
             },
         ],
         'initial': 'created',
         'queued': True,
-        # 'ignore_invalid_triggers': True,
+        'ignore_invalid_triggers': True,
     }
 
     machine = MachineClass(model=model, **state_conf)  # type: ignore
     return machine
```

### Comparing `nextline_schedule-0.2.8/src/nextline_schedule/auto/machine.py` & `nextline_schedule-0.2.9/src/nextline_schedule/auto/machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self._logger = getLogger(__name__)
         machine = build_state_machine(model=self)
         machine.after_state_change = self.after_state_change.__name__  # type: ignore
 
     def subscribe_state(self) -> AsyncIterator[str]:
         return self._pubsub_state.subscribe()
 
-    async def on_enter_waiting(self) -> None:
+    async def on_enter_auto_waiting(self) -> None:
         task = asyncio.create_task(self._callback.wait())
         self._task = task
         self._tasks.add(task)
 
     async def on_enter_auto_pulling(self) -> None:
         task = asyncio.create_task(self._callback.pull())
         self._task = task
```

### Comparing `nextline_schedule-0.2.8/src/nextline_schedule/graphql/__init__.py` & `nextline_schedule-0.2.9/src/nextline_schedule/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/src/nextline_schedule/schema/mutation.py` & `nextline_schedule-0.2.9/src/nextline_schedule/schema/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/src/nextline_schedule/schema/query.py` & `nextline_schedule-0.2.9/src/nextline_schedule/schema/query.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/tests/test_fsm.py` & `nextline_schedule-0.2.9/tests/test_fsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from copy import deepcopy
 from typing import Any
 from unittest.mock import AsyncMock
 
 import pytest
 from hypothesis import given
 from hypothesis import strategies as st
-from transitions import Machine, MachineError
+from transitions import Machine
 from transitions.extensions.markup import HierarchicalMarkupMachine
 
 from nextline_schedule.auto.factory import build_state_machine
 
 
 def test_model_default():
     machine = build_state_machine()
@@ -42,20 +42,21 @@
     max_n_paths = draw(st.integers(min_value=1, max_value=30))
 
     state_map = {
         'created': {
             'start': {'dest': 'off'},
         },
         'off': {
-            'turn_on': {'dest': 'waiting'},
+            'turn_on': {'dest': 'auto_waiting'},
         },
-        'waiting': {
+        'auto_waiting': {
             'turn_off': {'dest': 'off', 'before': 'cancel_task'},
             'on_initialized': {'dest': 'auto_pulling'},
             'on_finished': {'dest': 'auto_pulling'},
+            'on_raised': {'dest': 'off'},
         },
         'auto_pulling': {
             'run': {'dest': 'auto_running'},
             'turn_off': {'dest': 'off', 'before': 'cancel_task'},
             'on_raised': {'dest': 'off'},
         },
         'auto_running': {
@@ -80,15 +81,15 @@
     while len(paths) < max_n_paths:
         trigger_map = state_map[state]
         trigger = draw(st.sampled_from(all_triggers))
         if trigger in trigger_map:
             paths.append((trigger, trigger_map[trigger]))
             state = trigger_map[trigger]['dest']
         else:
-            paths.append((trigger, {'error': MachineError}))
+            paths.append((trigger, {'invalid': True}))
 
     while state not in final_states:
         trigger_map = state_map_reduced[state]
         triggers = list(trigger_map.keys())
         trigger = draw(st.sampled_from(triggers))
         paths.append((trigger, trigger_map[trigger]))
         state = trigger_map[trigger]['dest']
@@ -98,17 +99,16 @@
 
 @given(paths=st_paths())
 async def test_transitions_hypothesis(paths: list[tuple[str, dict[str, Any]]]):
     machine = build_state_machine(model=Machine.self_literal)
     assert machine.is_created()
 
     for method, map in paths:
-        if error := map.get('error'):
-            with pytest.raises(error):
-                await getattr(machine, method)()
+        if map.get('invalid'):
+            await getattr(machine, method)()
             continue
 
         if before := map.get('before'):
             setattr(machine, before, AsyncMock())
 
         await getattr(machine, method)()
         dest = map['dest']
```

### Comparing `nextline_schedule-0.2.8/tests/test_plugin.py` & `nextline_schedule-0.2.9/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/tests/test_request.py` & `nextline_schedule-0.2.9/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/tests/test_scratch.py` & `nextline_schedule-0.2.9/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/tests/auto/test_auto.py` & `nextline_schedule-0.2.9/tests/auto/test_auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     async with auto_mode:
         async with nextline:
             await control(auto_mode, nextline)
 
     expected = [
         'off',
-        'waiting',
+        'auto_waiting',
         'auto_pulling',
         'auto_running',
         'auto_pulling',
         'auto_running',
         'off',
     ]
     assert expected == await states
```

### Comparing `nextline_schedule-0.2.8/tests/auto/test_auto_on_raised.py` & `nextline_schedule-0.2.9/tests/auto/test_auto_on_raised.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     async with auto_mode:
         async with nextline:
             await auto_mode.turn_on()
             async for state in auto_mode.subscribe_state():
                 if state == 'off':
                     break
 
-    expected = ['off', 'waiting', 'auto_pulling', 'off']
+    expected = ['off', 'auto_waiting', 'auto_pulling', 'off']
     assert expected == await states
 
 
 async def test_on_raised_while_running():
     async def request_statement():
         return g
 
@@ -57,13 +57,13 @@
     async with auto_mode:
         async with nextline:
             await auto_mode.turn_on()
             async for state in auto_mode.subscribe_state():
                 if state == 'off':
                     break
 
-    expected = ['off', 'waiting', 'auto_pulling', 'auto_running', 'off']
+    expected = ['off', 'auto_waiting', 'auto_pulling', 'auto_running', 'off']
     assert expected == await states
 
 
 async def subscribe_state(auto_mode: AutoModeStateMachine):
     return [state async for state in auto_mode.subscribe_state()]
```

### Comparing `nextline_schedule-0.2.8/tests/auto/test_auto_turn_off.py` & `nextline_schedule-0.2.9/tests/auto/test_auto_turn_off.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
             await auto_mode.turn_off()
             await nextline.send_pdb_command(
                 command='continue',
                 prompt_no=prompt.prompt_no,
                 trace_no=prompt.trace_no,
             )
 
-    expected = ['off', 'waiting', 'off']
+    expected = ['off', 'auto_waiting', 'off']
     assert expected == await states
 
 
 async def subscribe_state(auto_mode: AutoModeStateMachine):
     return [state async for state in auto_mode.subscribe_state()]
```

### Comparing `nextline_schedule-0.2.8/.gitignore` & `nextline_schedule-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/LICENSE.txt` & `nextline_schedule-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/README.md` & `nextline_schedule-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.8/pyproject.toml` & `nextline_schedule-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["transitions>=0.9", "httpx>=0.23"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-host = ["nextline-graphql>=0.7.6"]
+host = ["nextline-graphql>=0.7.7"]
 tests = [
   "async-asgi-testclient>=1.4",
   "pytest-asyncio>=0.18",
   "pytest-cov>=3.0",
   "pytest-timeout>=2.1",
   "pytest>=7.0",
   "hypothesis>=6.65",
```

### Comparing `nextline_schedule-0.2.8/PKG-INFO` & `nextline_schedule-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextline-schedule
-Version: 0.2.8
+Version: 0.2.9
 Summary: A plugin of nextline-graphql. An interface to the SO scheduler.
 Project-URL: Documentation, https://github.com/simonsobs/nextline-schedule#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline-schedule/issues
 Project-URL: Source, https://github.com/simonsobs/nextline-schedule
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: httpx>=0.23
 Requires-Dist: transitions>=0.9
 Provides-Extra: host
-Requires-Dist: nextline-graphql>=0.7.6; extra == 'host'
+Requires-Dist: nextline-graphql>=0.7.7; extra == 'host'
 Provides-Extra: tests
 Requires-Dist: async-asgi-testclient>=1.4; extra == 'tests'
 Requires-Dist: hypothesis>=6.65; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.18; extra == 'tests'
 Requires-Dist: pytest-cov>=3.0; extra == 'tests'
 Requires-Dist: pytest-httpx>=0.21; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.1; extra == 'tests'
```

