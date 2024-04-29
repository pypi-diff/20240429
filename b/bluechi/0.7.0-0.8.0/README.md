# Comparing `tmp/bluechi-0.7.0-py3-none-any.whl.zip` & `tmp/bluechi-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 18916 bytes, number of entries: 9
--rw-r--r--  2.0 unx       44 b- defN 23-Sep-05 15:21 bluechi/__init__.py
--rw-r--r--  2.0 unx    32330 b- defN 24-Jan-19 09:33 bluechi/api.py
--rw-r--r--  2.0 unx     2711 b- defN 24-Jan-19 06:38 bluechi/ext.py
--rw-rw-r--  2.0 unx    26530 b- defN 24-Jan-19 09:33 bluechi-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1474 b- defN 24-Jan-19 09:33 bluechi-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-19 09:33 bluechi-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Jan-19 09:33 bluechi-0.7.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Jan-19 09:33 bluechi-0.7.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx      689 b- defN 24-Jan-19 09:33 bluechi-0.7.0.dist-info/RECORD
-9 files, 63879 bytes uncompressed, 17734 bytes compressed:  72.2%
+Zip file size: 19440 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      105 b- defN 24-Apr-11 11:56 bluechi/__init__.py
+-rw-rw-r--  2.0 unx    35241 b- defN 24-Apr-29 11:35 bluechi/api.py
+-rw-rw-r--  2.0 unx     2771 b- defN 24-Apr-11 11:56 bluechi/ext.py
+-rw-rw-r--  2.0 unx    26530 b- defN 24-Apr-29 11:36 bluechi-0.8.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1474 b- defN 24-Apr-29 11:36 bluechi-0.8.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-29 11:36 bluechi-0.8.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-29 11:36 bluechi-0.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 24-Apr-29 11:36 bluechi-0.8.0.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      690 b- defN 24-Apr-29 11:36 bluechi-0.8.0.dist-info/RECORD
+9 files, 66912 bytes uncompressed, 18258 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: bluechi/api.py
 Comment: 
 
 Filename: bluechi/ext.py
 Comment: 
 
-Filename: bluechi-0.7.0.dist-info/LICENSE
+Filename: bluechi-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: bluechi-0.7.0.dist-info/METADATA
+Filename: bluechi-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: bluechi-0.7.0.dist-info/WHEEL
+Filename: bluechi-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: bluechi-0.7.0.dist-info/top_level.txt
+Filename: bluechi-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bluechi-0.7.0.dist-info/zip-safe
+Filename: bluechi-0.8.0.dist-info/zip-safe
 Comment: 
 
-Filename: bluechi-0.7.0.dist-info/RECORD
+Filename: bluechi-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bluechi/__init__.py

```diff
@@ -1 +1,4 @@
-# SPDX-License-Identifier: LGPL-2.1-or-later
+#
+# Copyright Contributors to the Eclipse BlueChi project
+#
+# SPDX-License-Identifier: LGPL-2.1-or-later
```

## bluechi/api.py

```diff
@@ -1,59 +1,62 @@
+#
+# Copyright Contributors to the Eclipse BlueChi project
+#
 # SPDX-License-Identifier: LGPL-2.1-or-later
 #
 # Generated file. DO NOT EDIT!
 #
 
 from __future__ import annotations
 
-from typing import Callable, Tuple, Dict, List, Any
+from typing import Any, Callable, Dict, List, Tuple
+
 from dasbus.typing import (
     Bool,
+    Byte,
     Double,
-    Str,
     Int,
-    Byte,
     Int16,
-    UInt16,
     Int32,
-    UInt32,
     Int64,
-    UInt64,
     ObjPath,
+    Str,
     Structure,
+    UInt16,
+    UInt32,
+    UInt64,
 )
 
 # File has been renamed to UnixFD in following PR included in v1.7
 # https://github.com/rhinstaller/dasbus/pull/70
 try:
     from dasbus.typing import File
 except ImportError:
     from dasbus.typing import UnixFD
 
-from dasbus.client.proxy import InterfaceProxy, ObjectProxy
-from dasbus.connection import MessageBus, SystemMessageBus, SessionMessageBus
-
 import gi
+from dasbus.client.proxy import InterfaceProxy, ObjectProxy
+from dasbus.connection import MessageBus, SessionMessageBus, SystemMessageBus
 
 gi.require_version("GLib", "2.0")
 from gi.repository.GLib import Variant  # noqa: E402
 
-
 BC_DEFAULT_PORT = 842
 BC_DEFAULT_HOST = "127.0.0.1"
 
 BC_DBUS_INTERFACE = "org.eclipse.bluechi"
 BC_OBJECT_PATH = "/org/eclipse/bluechi"
 BC_AGENT_DBUS_INTERFACE = "org.eclipse.bluechi.Agent"
 BC_METRICS_OBJECT_PATH = "/org/eclipse/bluechi/metrics"
 
 DBUS_PROPERTIES_INTERFACE = "org.freedesktop.DBus.Properties"
 
 
 class ApiBase:
+
     def __init__(
         self,
         interface: str,
         object_path: str,
         bus: MessageBus = None,
         use_systembus=True,
     ) -> None:
@@ -85,295 +88,240 @@
             self.cached_properties_proxy = self.bus.get_proxy(
                 self.interface, self.object_path, DBUS_PROPERTIES_INTERFACE
             )
 
         return self.cached_properties_proxy
 
 
-class Monitor(ApiBase):
+class Agent(ApiBase):
     """
-    org.eclipse.bluechi.Monitor:
-    @short_description: Public interface of BlueChi on the managing node providing monitoring functionality.
+    org.eclipse.bluechi.Agent:
+    @short_description: Public interface of BlueChi on the managed node providing methods and signals for the respective node.
 
-    This interface is only available if a monitor has been created before via the Controller interface.
-    It provides methods to subscribe to changes in systemd units on managed nodes as well as signals for those changes.
+    This interface is used to create proxy services resolving dependencies on services of other managed nodes.
     """
 
-    def __init__(
-        self, monitor_path: ObjPath, bus: MessageBus = None, use_systembus=True
-    ) -> None:
-        super().__init__(BC_DBUS_INTERFACE, monitor_path, bus, use_systembus)
-
-        self.monitor_path = monitor_path
+    def __init__(self, bus: MessageBus = None, use_systembus=True) -> None:
+        super().__init__(BC_AGENT_DBUS_INTERFACE, BC_OBJECT_PATH, bus, use_systembus)
 
-    def close(self) -> None:
+    def create_proxy(self, local_service_name: str, node: str, unit: str) -> None:
         """
-          Close:
+          CreateProxy:
+        @local_service_name: The service name which requests the external dependency
+        @node: The requested node to provide the service
+        @unit: The external unit requested from the local service
 
-        Close the monitor.
+        BlueChi internal usage only.
+        CreateProxy() creates a new proxy service. It is part in the chain of resolving dependencies on services running on other managed nodes.
         """
-        self.get_proxy().Close()
+        self.get_proxy().CreateProxy(
+            local_service_name,
+            node,
+            unit,
+        )
 
-    def subscribe(self, node: str, unit: str) -> UInt32:
+    def remove_proxy(self, local_service_name: str, node: str, unit: str) -> None:
         """
-            Subscribe:
-          @node: The name of the node to subscribe to
-          @unit: The name of the unit to subscribe to
-          @id: The id of the created subscription.
+          RemoveProxy:
+        @local_service_name: The service name which requests the external dependency
+        @node: The requested node to provide the service
+        @unit: The external unit requested from the local service
 
-          Subscribe to changes of a unit on a node. Both fields support a wildcard '*'. A wildcard in the node name will create the subscription for all nodes.
-        If the unit name is a wildcard, then the subscription matches changes for all units on the node.
+        BlueChi internal usage only.
+        RemoveProxy() removes a new proxy service. It is part in the chain of resolving dependencies on services running on other managed nodes.
         """
-        return self.get_proxy().Subscribe(
+        self.get_proxy().RemoveProxy(
+            local_service_name,
             node,
             unit,
         )
 
-    def unsubscribe(self, id: UInt32) -> None:
+    def switch_controller(self, dbus_address: str) -> None:
         """
-          Unsubscribe:
-        @id: The id of the subscription to cancel
+          SwitchController:
+        @dbus_address: SD Bus address used to connect to the BlueChi controller
 
-        Cancel the subscription by ID.
+        SwitchController() changes SD Bus address used to connect to the BlueChi controller and
+        triggers a reconnect to the BlueChi controller with the new address.
         """
-        self.get_proxy().Unsubscribe(
-            id,
+        self.get_proxy().SwitchController(
+            dbus_address,
         )
 
-    def subscribe_list(self, node: str, units: List[str]) -> UInt32:
+    @property
+    def controller_address(self) -> str:
         """
-            SubscribeList:
-          @node: The name of the node to subscribe to
-          @units: A list of unit names to subscribe to
-          @id: The id of the created subscription
+          ControllerAddress:
 
-          Subscribe to changes of a list of units on a node. The node field supports a wildcard '*'. A wildcard in the node name will create the subscription
-        for all nodes.
+        SD Bus address used to connect to the BlueChi controller.
+        On any change, a signal is emitted on the org.freedesktop.DBus.Properties interface.
         """
-        return self.get_proxy().SubscribeList(
-            node,
-            units,
-        )
+        return self.get_proxy().ControllerAddress
 
-    def add_peer(self, name: str) -> UInt32:
+    def on_controller_address_changed(self, callback: Callable[[Variant], None]):
         """
-          AddPeer:
-        @name: The name of the peer to add as listener to all monitor events. Needs to be unique name on the bus.
-        @id: The id of the created peer
+          ControllerAddress:
 
-        Add a new peer to the monitor. A peer will receive all events that the monitor subscribes to.
+        SD Bus address used to connect to the BlueChi controller.
+        On any change, a signal is emitted on the org.freedesktop.DBus.Properties interface.
         """
-        return self.get_proxy().AddPeer(
-            name,
-        )
 
-    def remove_peer(self, id: UInt32, reason: str) -> None:
-        """
-          RemovePeer:
-        @id: The id of the peer to remove
-        @reason: The reason for removing the peer
+        def on_properties_changed(
+            interface: str,
+            changed_props: Dict[str, Variant],
+            invalidated_props: Dict[str, Variant],
+        ) -> None:
+            value = changed_props.get("ControllerAddress")
+            if value is not None:
+                callback(value)
 
-        Remove a previously added peer from the monitor. The reason will be part of the PeerRemoved signal, which is only sent to the respective peer.
-        """
-        self.get_proxy().RemovePeer(
-            id,
-            reason,
-        )
+        self.get_properties_proxy().PropertiesChanged.connect(on_properties_changed)
 
-    def on_unit_properties_changed(
-        self,
-        callback: Callable[
-            [
-                str,
-                str,
-                str,
-                Structure,
-            ],
-            None,
-        ],
-    ) -> None:
+    @property
+    def disconnect_timestamp(self) -> UInt64:
         """
-          UnitPropertiesChanged:
-        @node: The node name this signal originated from
-        @unit: The unit for which the properties changed
-        @interface: The originating interface
-        @props: The changed properties as key-value pair with the name of the property as key
+          DisconnectTimestamp:
 
-        Whenever the properties change for any of the units that are currently subscribed to, this signal is emitted.
+        A timestamp indicating when the agent lost connection to the BlueChi controller.
+        If the connection is active (agent is online), this value is 0.
         """
-        self.get_proxy().UnitPropertiesChanged.connect(callback)
+        return self.get_proxy().DisconnectTimestamp
 
-    def on_unit_state_changed(
-        self,
-        callback: Callable[
-            [
-                str,
-                str,
-                str,
-                str,
-                str,
-            ],
-            None,
-        ],
-    ) -> None:
+    @property
+    def log_level(self) -> str:
         """
-          UnitStateChanged:
-        @node: The node name this signal originated from
-        @unit: The unit for which the properties changed
-        @active_state: The active state of the unit
-        @sub_state: The sub state of the unit
-        @reason: The reason for the state change, the value is either real or virtual
+          LogLevel:
 
-        Emitted when the active state (and substate) of a monitored unit changes.
+        The LogLevel of the agent node that is currently used. Its value is one of:
+          INFO, DEBUG, ERROR and WARN
         """
-        self.get_proxy().UnitStateChanged.connect(callback)
+        return self.get_proxy().LogLevel
 
-    def on_unit_new(
-        self,
-        callback: Callable[
-            [
-                str,
-                str,
-                str,
-            ],
-            None,
-        ],
-    ) -> None:
+    @property
+    def log_target(self) -> str:
         """
-            UnitNew:
-          @node: The node name this signal originated from
-          @unit: The unit for which the properties changed
-          @reason: The reason for the state change, the value is either real or virtual
+          LogTarget:
 
-          Emitted when a new unit is loaded by systemd, for example when a service is started (reason=real), or if BlueChi learns of an already loaded unit
-        (reason=virtual).
+        The LogTarget of the agent node that is currently used. Its value is one of:
+          stderr, stderr-full, journald
         """
-        self.get_proxy().UnitNew.connect(callback)
+        return self.get_proxy().LogTarget
 
-    def on_unit_removed(
-        self,
-        callback: Callable[
-            [
-                str,
-                str,
-                str,
-            ],
-            None,
-        ],
-    ) -> None:
+    @property
+    def status(self) -> str:
         """
-            UnitRemoved:
-          @node: The node name this signal originated from
-          @unit: The unit for which the properties changed
-          @reason: The reason for the state change, the value is either real or virtual
+          Status:
 
-          Emitted when a unit is unloaded by systemd (reason=real), or when the agent disconnects and we previously reported the unit as loaded
-        (reason=virtual).
+        The connection status of the agent with the BlueChi controller.
+        On any change, a signal is emitted on the org.freedesktop.DBus.Properties interface.
         """
-        self.get_proxy().UnitRemoved.connect(callback)
+        return self.get_proxy().Status
 
-    def on_peer_removed(
-        self,
-        callback: Callable[
-            [
-                str,
-            ],
-            None,
-        ],
-    ) -> None:
+    def on_status_changed(self, callback: Callable[[Variant], None]):
         """
-          PeerRemoved:
-        @reason: The reason the peer got removed from the monitor.
+          Status:
 
-        Emitted when a peer is removed from the monitor, e.g. when the monitor has been closed, and only sent to the respective peer.
+        The connection status of the agent with the BlueChi controller.
+        On any change, a signal is emitted on the org.freedesktop.DBus.Properties interface.
         """
-        self.get_proxy().PeerRemoved.connect(callback)
+
+        def on_properties_changed(
+            interface: str,
+            changed_props: Dict[str, Variant],
+            invalidated_props: Dict[str, Variant],
+        ) -> None:
+            value = changed_props.get("Status")
+            if value is not None:
+                callback(value)
+
+        self.get_properties_proxy().PropertiesChanged.connect(on_properties_changed)
 
 
 class Controller(ApiBase):
     """
     org.eclipse.bluechi.Controller:
     @short_description: Public interface of BlueChi on the managing node providing methods and signals for all nodes.
 
     This interface can be used to get information about all nodes and their units, create monitors and listen for job signals.
     """
 
     def __init__(self, bus: MessageBus = None, use_systembus=True) -> None:
         super().__init__(BC_DBUS_INTERFACE, BC_OBJECT_PATH, bus, use_systembus)
 
-    def list_units(
-        self,
-    ) -> List[Tuple[str, str, str, str, str, str, str, ObjPath, UInt32, str, ObjPath]]:
+    def create_monitor(self) -> ObjPath:
         """
-          ListUnits:
-        @units: A list of all units on each node:
-          - The node name
-          - The primary unit name as string
-          - The human readable description string
-          - The load state (i.e. whether the unit file has been loaded successfully)
-          - The active state (i.e. whether the unit is currently started or not)
-          - The sub state (a more fine-grained version of the active state that is specific to the unit type, which the active state is not)
-          - A unit that is being followed in its state by this unit, if there is any, otherwise the empty string.
-          - The unit object path
-          - If there is a job queued for the job unit the numeric job id, 0 otherwise
-          - The job type as string
-          - The job object path
+          CreateMonitor:
+        @monitor: The path of the created monitor.
 
-        List all loaded systemd units on all nodes which are online.
+        Create a new monitor on which subscriptions can be added. It will automatically be closed as soon as the connection is closed.
         """
-        return self.get_proxy().ListUnits()
+        return self.get_proxy().CreateMonitor()
 
-    def list_nodes(self) -> List[Tuple[str, ObjPath, str]]:
+    def disable_metrics(self) -> None:
         """
-          ListNodes:
-        @nodes: A list of all nodes:
-          - The node name
-          - The object path of the node
-          - the current state of that node, either online or offline
+          DisableMetrics:
 
-        List all nodes managed by BlueChi regardless if they are offline or online.
+        Disable collecting performance metrics.
         """
-        return self.get_proxy().ListNodes()
+        self.get_proxy().DisableMetrics()
+
+    def enable_metrics(self) -> None:
+        """
+          EnableMetrics:
+
+        Enable collecting performance metrics.
+        """
+        self.get_proxy().EnableMetrics()
 
     def get_node(self, name: str) -> ObjPath:
         """
           GetNode:
         @name: Name of the node
         @path: The path of the requested node
 
         Get the object path of the named node.
         """
         return self.get_proxy().GetNode(
             name,
         )
 
-    def create_monitor(self) -> ObjPath:
-        """
-          CreateMonitor:
-        @monitor: The path of the created monitor.
-
-        Create a new monitor on which subscriptions can be added. It will automatically be closed as soon as the connection is closed.
+    def list_nodes(self) -> List[Tuple[str, ObjPath, str, str]]:
         """
-        return self.get_proxy().CreateMonitor()
-
-    def enable_metrics(self) -> None:
-        """
-          EnableMetrics:
+          ListNodes:
+        @nodes: A list of all nodes:
+          - node name
+          - object path of the node
+          - current state of that node, either online or offline
+          - IP of the connected node
 
-        Enable collecting performance metrics.
+        List all nodes managed by BlueChi regardless if they are offline or online.
         """
-        self.get_proxy().EnableMetrics()
+        return self.get_proxy().ListNodes()
 
-    def disable_metrics(self) -> None:
+    def list_units(
+        self,
+    ) -> List[Tuple[str, str, str, str, str, str, str, ObjPath, UInt32, str, ObjPath]]:
         """
-          DisableMetrics:
+          ListUnits:
+        @units: A list of all units on each node:
+          - The node name
+          - The primary unit name as string
+          - The human readable description string
+          - The load state (i.e. whether the unit file has been loaded successfully)
+          - The active state (i.e. whether the unit is currently started or not)
+          - The sub state (a more fine-grained version of the active state that is specific to the unit type, which the active state is not)
+          - A unit that is being followed in its state by this unit, if there is any, otherwise the empty string.
+          - The unit object path
+          - If there is a job queued for the job unit the numeric job id, 0 otherwise
+          - The job type as string
+          - The job object path
 
-        Disable collecting performance metrics.
+        List all loaded systemd units on all nodes which are online.
         """
-        self.get_proxy().DisableMetrics()
+        return self.get_proxy().ListUnits()
 
     def set_log_level(self, loglevel: str) -> None:
         """
           SetLogLevel:
         @loglevel: The new loglevel to use.
 
         Change the loglevel of the controller.
@@ -425,14 +373,34 @@
           Emitted each time a new job is dequeued or the underlying systemd job finished. result is one of: done, failed, cancelled, timeout, dependency,
         skipped. This is either the result from systemd on the node, or cancelled if the job was cancelled in BlueChi before any systemd job was started
         for it.
         """
         self.get_proxy().JobRemoved.connect(callback)
 
     @property
+    def log_level(self) -> str:
+        """
+          LogLevel:
+
+        The LogLevel of the controller node that is currently used. Its value is one of:
+          INFO, DEBUG, ERROR and WARN
+        """
+        return self.get_proxy().LogLevel
+
+    @property
+    def log_target(self) -> str:
+        """
+          LogTarget:
+
+        The LogTarget of the controller node that is currently used. Its value is one of:
+          stderr, stderr-full, journald
+        """
+        return self.get_proxy().LogTarget
+
+    @property
     def status(self) -> str:
         """
           Status:
 
         The status of the overall system. Its value is one of:
           down:  no node is connected
           degraded: at least one node is not connected
@@ -464,75 +432,14 @@
             value = changed_props.get("Status")
             if value is not None:
                 callback(value)
 
         self.get_properties_proxy().PropertiesChanged.connect(on_properties_changed)
 
 
-class Metrics(ApiBase):
-    """
-    org.eclipse.bluechi.Metrics:
-    @short_description: Public interface of BlueChi on the managing node providing signals for performance metrics.
-
-    This interface is only available if the metrics have been enabled before via the Controller interface.
-    """
-
-    def __init__(self, bus: MessageBus = None, use_systembus=True) -> None:
-        super().__init__(BC_DBUS_INTERFACE, BC_METRICS_OBJECT_PATH, bus, use_systembus)
-
-    def on_start_unit_job_metrics(
-        self,
-        callback: Callable[
-            [
-                str,
-                str,
-                str,
-                UInt64,
-                UInt64,
-            ],
-            None,
-        ],
-    ) -> None:
-        """
-          StartUnitJobMetrics:
-        @node_name: The node name this metrics has been collected for
-        @job_id: The id of the job linked to the collected metrics
-        @unit: The unit name this metrics has been collected for
-        @job_measured_time_micros: The measured time it took starting the unit on the node in microseconds
-        @unit_start_prop_time_micros: The systemd time it took starting the unit on the node in microseconds
-
-        Emitted when a start operation processed by BlueChi finishes and the collection of metrics has been enabled previously.
-        """
-        self.get_proxy().StartUnitJobMetrics.connect(callback)
-
-    def on_agent_job_metrics(
-        self,
-        callback: Callable[
-            [
-                str,
-                str,
-                str,
-                UInt64,
-            ],
-            None,
-        ],
-    ) -> None:
-        """
-            AgentJobMetrics:
-          @node_name: The node name this metrics has been collected for
-          @unit: The unit name this metrics has been collected for
-          @method: The lifecycle operation
-          @systemd_job_time_micros: The systemd time it took starting the unit on the node in microseconds
-
-          Emitted for all unit lifecycle operations (e.g. Start, Stop, Reload, etc.) processed by BlueChi when these finish and the collection of metrics has
-        been enabled previously.
-        """
-        self.get_proxy().AgentJobMetrics.connect(callback)
-
-
 class Job(ApiBase):
     """
     org.eclipse.bluechi.Job:
     @short_description: Public interface of BlueChi on the managing node for all job objects.
 
     This interface is used to either cancel a job, get its properties and monitor its state.
     """
@@ -559,39 +466,30 @@
           Id:
 
         An integer giving the id of the job.
         """
         return self.get_proxy().Id
 
     @property
-    def node(self) -> str:
-        """
-          Node:
-
-        The name of the node the job is on.
-        """
-        return self.get_proxy().Node
-
-    @property
-    def unit(self) -> str:
+    def job_type(self) -> str:
         """
-          Unit:
+          JobType:
 
-        The name of the unit the job works on.
+        Type of the job, either Start or Stop.
         """
-        return self.get_proxy().Unit
+        return self.get_proxy().JobType
 
     @property
-    def job_type(self) -> str:
+    def node(self) -> str:
         """
-          JobType:
+          Node:
 
-        Type of the job, either Start or Stop.
+        The name of the node the job is on.
         """
-        return self.get_proxy().JobType
+        return self.get_proxy().Node
 
     @property
     def state(self) -> str:
         """
           State:
 
         The current state of the job, one of: waiting (queued jobs) or running.
@@ -614,168 +512,327 @@
         ) -> None:
             value = changed_props.get("State")
             if value is not None:
                 callback(value)
 
         self.get_properties_proxy().PropertiesChanged.connect(on_properties_changed)
 
+    @property
+    def unit(self) -> str:
+        """
+          Unit:
 
-class Node(ApiBase):
+        The name of the unit the job works on.
+        """
+        return self.get_proxy().Unit
+
+
+class Metrics(ApiBase):
     """
-    org.eclipse.bluechi.Node:
-    @short_description: Public interface of BlueChi on the managing node providing methods, signals and  for a specific node.
+    org.eclipse.bluechi.Metrics:
+    @short_description: Public interface of BlueChi on the managing node providing signals for performance metrics.
 
-    This interface can be used to get information about a specific node and its units as well as control them, e.g. by starting or stopping them.
+    This interface is only available if the metrics have been enabled before via the Controller interface.
     """
 
-    def __init__(
-        self, node_name: str, bus: MessageBus = None, use_systembus=True
+    def __init__(self, bus: MessageBus = None, use_systembus=True) -> None:
+        super().__init__(BC_DBUS_INTERFACE, BC_METRICS_OBJECT_PATH, bus, use_systembus)
+
+    def on_agent_job_metrics(
+        self,
+        callback: Callable[
+            [
+                str,
+                str,
+                str,
+                UInt64,
+            ],
+            None,
+        ],
     ) -> None:
-        # set empty node path temporary, needs to be resolved after the bus has been set
-        super().__init__(BC_DBUS_INTERFACE, "", bus, use_systembus)
+        """
+            AgentJobMetrics:
+          @node_name: The node name this metrics has been collected for
+          @unit: The unit name this metrics has been collected for
+          @method: The lifecycle operation
+          @systemd_job_time_micros: The systemd time it took starting the unit on the node in microseconds
 
-        controller = self.bus.get_proxy(BC_DBUS_INTERFACE, BC_OBJECT_PATH)
-        self.object_path = controller.GetNode(node_name)
+          Emitted for all unit lifecycle operations (e.g. Start, Stop, Reload, etc.) processed by BlueChi when these finish and the collection of metrics has
+        been enabled previously.
+        """
+        self.get_proxy().AgentJobMetrics.connect(callback)
 
-        self.node_name = node_name
+    def on_start_unit_job_metrics(
+        self,
+        callback: Callable[
+            [
+                str,
+                str,
+                str,
+                UInt64,
+                UInt64,
+            ],
+            None,
+        ],
+    ) -> None:
+        """
+          StartUnitJobMetrics:
+        @node_name: The node name this metrics has been collected for
+        @job_id: The id of the job linked to the collected metrics
+        @unit: The unit name this metrics has been collected for
+        @job_measured_time_micros: The measured time it took starting the unit on the node in microseconds
+        @unit_start_prop_time_micros: The systemd time it took starting the unit on the node in microseconds
 
-    def start_unit(self, name: str, mode: str) -> ObjPath:
+        Emitted when a start operation processed by BlueChi finishes and the collection of metrics has been enabled previously.
         """
-            StartUnit:
-          @name: The name of the unit to start
-          @mode: The mode used to start the unit
-          @job: The path for the job associated with the start operation
+        self.get_proxy().StartUnitJobMetrics.connect(callback)
 
-          Queues a unit activate job for the named unit on this node. The queue is per-unit name, which means there is only ever one active job per unit. Mode
-        can be one of replace or fail. If there is an outstanding queued (but not running) job, that is replaced if mode is replace, or the job
-        fails if mode is fail.
 
-          The job returned is an object path for an object implementing org.eclipse.bluechi.Job, and which be monitored for the progress of the job, or used
-        to cancel the job. To track the result of the job, follow the JobRemoved signal on the Controller.
+class Monitor(ApiBase):
+    """
+    org.eclipse.bluechi.Monitor:
+    @short_description: Public interface of BlueChi on the managing node providing monitoring functionality.
+
+    This interface is only available if a monitor has been created before via the Controller interface.
+    It provides methods to subscribe to changes in systemd units on managed nodes as well as signals for those changes.
+    """
+
+    def __init__(
+        self, monitor_path: ObjPath, bus: MessageBus = None, use_systembus=True
+    ) -> None:
+        super().__init__(BC_DBUS_INTERFACE, monitor_path, bus, use_systembus)
+
+        self.monitor_path = monitor_path
+
+    def add_peer(self, name: str) -> UInt32:
         """
-        return self.get_proxy().StartUnit(
+          AddPeer:
+        @name: The name of the peer to add as listener to all monitor events. Needs to be unique name on the bus.
+        @id: The id of the created peer
+
+        Add a new peer to the monitor. A peer will receive all events that the monitor subscribes to.
+        """
+        return self.get_proxy().AddPeer(
             name,
-            mode,
         )
 
-    def stop_unit(self, name: str, mode: str) -> ObjPath:
+    def close(self) -> None:
         """
-          StopUnit:
-        @name: The name of the unit to stop
-        @mode: The mode used to stop the unit
-        @job: The path for the job associated with the stop operation
+          Close:
 
-        StopUnit() is similar to StartUnit() but stops the specified unit rather than starting it.
+        Close the monitor.
         """
-        return self.get_proxy().StopUnit(
-            name,
-            mode,
-        )
+        self.get_proxy().Close()
 
-    def freeze_unit(self, name: str) -> None:
+    def remove_peer(self, id: UInt32, reason: str) -> None:
         """
-            FreezeUnit:
-          @name: The name of the unit to freeze
+          RemovePeer:
+        @id: The id of the peer to remove
+        @reason: The reason for removing the peer
 
-          Freezing the unit will cause all processes contained within the cgroup corresponding to the unit to be suspended. Being suspended means that unit's
-        processes won't be scheduled to run on CPU until thawed.
+        Remove a previously added peer from the monitor. The reason will be part of the PeerRemoved signal, which is only sent to the respective peer.
         """
-        self.get_proxy().FreezeUnit(
-            name,
+        self.get_proxy().RemovePeer(
+            id,
+            reason,
         )
 
-    def thaw_unit(self, name: str) -> None:
+    def subscribe(self, node: str, unit: str) -> UInt32:
         """
-          ThawUnit:
-        @name: The name of the unit to thaw
+            Subscribe:
+          @node: The name of the node to subscribe to
+          @unit: The name of the unit to subscribe to
+          @id: The id of the created subscription.
 
-        This is the inverse operation to the freeze command and resumes the execution of processes in the unit's cgroup.
+          Subscribe to changes of a unit on a node. Both fields support a wildcard '*'. A wildcard in the node name will create the subscription for all nodes.
+        If the unit name is a wildcard, then the subscription matches changes for all units on the node.
         """
-        self.get_proxy().ThawUnit(
-            name,
+        return self.get_proxy().Subscribe(
+            node,
+            unit,
         )
 
-    def reload_unit(self, name: str, mode: str) -> ObjPath:
+    def subscribe_list(self, node: str, units: List[str]) -> UInt32:
         """
-          ReloadUnit:
-        @name: The name of the unit to reload
-        @mode: The mode used to reload the unit
-        @job: The path for the job associated with the reload operation
+            SubscribeList:
+          @node: The name of the node to subscribe to
+          @units: A list of unit names to subscribe to
+          @id: The id of the created subscription
 
-        ReloadUnit() is similar to StartUnit() but can be used to reload a unit instead. See equivalent systemd methods for details.
+          Subscribe to changes of a list of units on a node. The node field supports a wildcard '*'. A wildcard in the node name will create the subscription
+        for all nodes.
         """
-        return self.get_proxy().ReloadUnit(
-            name,
-            mode,
+        return self.get_proxy().SubscribeList(
+            node,
+            units,
         )
 
-    def restart_unit(self, name: str, mode: str) -> ObjPath:
+    def unsubscribe(self, id: UInt32) -> None:
         """
-          RestartUnit:
-        @name: The name of the unit to restart
-        @mode: The mode used to restart the unit
-        @job: The path for the job associated with the restart operation
+          Unsubscribe:
+        @id: The id of the subscription to cancel
 
-        RestartUnit() is similar to StartUnit() but can be used to restart a unit instead. See equivalent systemd methods for details.
+        Cancel the subscription by ID.
         """
-        return self.get_proxy().RestartUnit(
-            name,
-            mode,
+        self.get_proxy().Unsubscribe(
+            id,
         )
 
-    def get_unit_properties(self, name: str, interface: str) -> Structure:
+    def on_peer_removed(
+        self,
+        callback: Callable[
+            [
+                str,
+            ],
+            None,
+        ],
+    ) -> None:
         """
-          GetUnitProperties:
-        @name: The name of unit
-        @interface: The interface name
-        @props: The  as key-value pair with the name of the property as key
+          PeerRemoved:
+        @reason: The reason the peer got removed from the monitor.
 
-        Returns the current  for a named unit on the node. The returned  are the same as you would get in the systemd  apis.
+        Emitted when a peer is removed from the monitor, e.g. when the monitor has been closed, and only sent to the respective peer.
         """
-        return self.get_proxy().GetUnitProperties(
-            name,
-            interface,
-        )
+        self.get_proxy().PeerRemoved.connect(callback)
 
-    def get_unit_property(self, name: str, interface: str, property: str) -> Variant:
+    def on_unit_new(
+        self,
+        callback: Callable[
+            [
+                str,
+                str,
+                str,
+            ],
+            None,
+        ],
+    ) -> None:
         """
-          GetUnitProperty:
-        @name: The name of unit
-        @interface: The interface name
-        @property: The property name
-        @value: The value of the property
+            UnitNew:
+          @node: The node name this signal originated from
+          @unit: The unit for which the properties changed
+          @reason: The reason for the state change, the value is either real or virtual
 
-        Get one named property, otherwise similar to GetUnit.
+          Emitted when a new unit is loaded by systemd, for example when a service is started (reason=real), or if BlueChi learns of an already loaded unit
+        (reason=virtual).
         """
-        return self.get_proxy().GetUnitProperty(
-            name,
-            interface,
-            property,
-        )
+        self.get_proxy().UnitNew.connect(callback)
 
-    def set_unit_properties(
-        self, name: str, runtime: bool, keyvalues: List[Tuple[str, Variant]]
+    def on_unit_properties_changed(
+        self,
+        callback: Callable[
+            [
+                str,
+                str,
+                str,
+                Structure,
+            ],
+            None,
+        ],
     ) -> None:
         """
-          SetUnitProperties:
-        @name: The name of the unit
+          UnitPropertiesChanged:
+        @node: The node name this signal originated from
+        @unit: The unit for which the properties changed
+        @interface: The originating interface
+        @props: The changed properties as key-value pair with the name of the property as key
+
+        Whenever the properties change for any of the units that are currently subscribed to, this signal is emitted.
+        """
+        self.get_proxy().UnitPropertiesChanged.connect(callback)
+
+    def on_unit_removed(
+        self,
+        callback: Callable[
+            [
+                str,
+                str,
+                str,
+            ],
+            None,
+        ],
+    ) -> None:
+        """
+            UnitRemoved:
+          @node: The node name this signal originated from
+          @unit: The unit for which the properties changed
+          @reason: The reason for the state change, the value is either real or virtual
+
+          Emitted when a unit is unloaded by systemd (reason=real), or when the agent disconnects and we previously reported the unit as loaded
+        (reason=virtual).
+        """
+        self.get_proxy().UnitRemoved.connect(callback)
+
+    def on_unit_state_changed(
+        self,
+        callback: Callable[
+            [
+                str,
+                str,
+                str,
+                str,
+                str,
+            ],
+            None,
+        ],
+    ) -> None:
+        """
+          UnitStateChanged:
+        @node: The node name this signal originated from
+        @unit: The unit for which the properties changed
+        @active_state: The active state of the unit
+        @sub_state: The sub state of the unit
+        @reason: The reason for the state change, the value is either real or virtual
+
+        Emitted when the active state (and substate) of a monitored unit changes.
+        """
+        self.get_proxy().UnitStateChanged.connect(callback)
+
+
+class Node(ApiBase):
+    """
+    org.eclipse.bluechi.Node:
+    @short_description: Public interface of BlueChi on the managing node providing methods, signals and  for a specific node.
+
+    This interface can be used to get information about a specific node and its units as well as control them, e.g. by starting or stopping them.
+    """
+
+    def __init__(
+        self, node_name: str, bus: MessageBus = None, use_systembus=True
+    ) -> None:
+        # set empty node path temporary, needs to be resolved after the bus has been set
+        super().__init__(BC_DBUS_INTERFACE, "", bus, use_systembus)
+
+        controller = self.bus.get_proxy(BC_DBUS_INTERFACE, BC_OBJECT_PATH)
+        self.object_path = controller.GetNode(node_name)
+
+        self.node_name = node_name
+
+    def disable_unit_files(
+        self, files: List[str], runtime: bool
+    ) -> List[Tuple[str, str, str]]:
+        """
+          DisableUnitFiles:
+        @files: A list of units to enable
         @runtime: Specify if the changes should persist after reboot or not
-        @keyvalues: A list of the new values as key-value pair with the key being the name of the property
+        @changes: The changes made
+          - type of change (one of: symlink, unlink)
+          - file name of the symlink
+          - destination of the symlink
 
-        Set named . If runtime is true the property changes do not persist across reboots.
+        DisableUnitFiles() is similar to EnableUnitFiles() but disables the specified units by removing all symlinks to them in /etc/ and /run/
         """
-        self.get_proxy().SetUnitProperties(
-            name,
+        return self.get_proxy().DisableUnitFiles(
+            files,
             runtime,
-            keyvalues,
         )
 
-    def enable_unit_files(
-        self, files: List[str], runtime: bool, force: bool
-    ) -> Tuple[bool, List[Tuple[str, str, str]],]:
+    def enable_unit_files(self, files: List[str], runtime: bool, force: bool) -> Tuple[
+        bool,
+        List[Tuple[str, str, str]],
+    ]:
         """
           EnableUnitFiles:
         @files: A list of units to enable
         @runtime: Specify if the changes should persist after reboot or not
         @force: Specify if replacing the symlinks pointing to other units should be enforced
         @carries_install_info: True if the units contained enablement information
         @changes: The changes made
@@ -787,31 +844,54 @@
         """
         return self.get_proxy().EnableUnitFiles(
             files,
             runtime,
             force,
         )
 
-    def disable_unit_files(
-        self, files: List[str], runtime: bool
-    ) -> List[Tuple[str, str, str]]:
+    def freeze_unit(self, name: str) -> None:
         """
-          DisableUnitFiles:
-        @files: A list of units to enable
-        @runtime: Specify if the changes should persist after reboot or not
-        @changes: The changes made
-          - type of change (one of: symlink, unlink)
-          - file name of the symlink
-          - destination of the symlink
+            FreezeUnit:
+          @name: The name of the unit to freeze
 
-        DisableUnitFiles() is similar to EnableUnitFiles() but disables the specified units by removing all symlinks to them in /etc/ and /run/
+          Freezing the unit will cause all processes contained within the cgroup corresponding to the unit to be suspended. Being suspended means that unit's
+        processes won't be scheduled to run on CPU until thawed.
         """
-        return self.get_proxy().DisableUnitFiles(
-            files,
-            runtime,
+        self.get_proxy().FreezeUnit(
+            name,
+        )
+
+    def get_unit_properties(self, name: str, interface: str) -> Structure:
+        """
+          GetUnitProperties:
+        @name: The name of unit
+        @interface: The interface name
+        @props: The  as key-value pair with the name of the property as key
+
+        Returns the current  for a named unit on the node. The returned  are the same as you would get in the systemd  apis.
+        """
+        return self.get_proxy().GetUnitProperties(
+            name,
+            interface,
+        )
+
+    def get_unit_property(self, name: str, interface: str, property: str) -> Variant:
+        """
+          GetUnitProperty:
+        @name: The name of unit
+        @interface: The interface name
+        @property: The property name
+        @value: The value of the property
+
+        Get one named property, otherwise similar to GetUnit.
+        """
+        return self.get_proxy().GetUnitProperty(
+            name,
+            interface,
+            property,
         )
 
     def list_units(
         self,
     ) -> List[Tuple[str, str, str, str, str, str, ObjPath, UInt32, str, ObjPath]]:
         """
           ListUnits:
@@ -835,147 +915,163 @@
         """
           Reload:
 
         Reload() may be invoked to reload all unit files.
         """
         self.get_proxy().Reload()
 
+    def reload_unit(self, name: str, mode: str) -> ObjPath:
+        """
+          ReloadUnit:
+        @name: The name of the unit to reload
+        @mode: The mode used to reload the unit
+        @job: The path for the job associated with the reload operation
+
+        ReloadUnit() is similar to StartUnit() but can be used to reload a unit instead. See equivalent systemd methods for details.
+        """
+        return self.get_proxy().ReloadUnit(
+            name,
+            mode,
+        )
+
+    def restart_unit(self, name: str, mode: str) -> ObjPath:
+        """
+          RestartUnit:
+        @name: The name of the unit to restart
+        @mode: The mode used to restart the unit
+        @job: The path for the job associated with the restart operation
+
+        RestartUnit() is similar to StartUnit() but can be used to restart a unit instead. See equivalent systemd methods for details.
+        """
+        return self.get_proxy().RestartUnit(
+            name,
+            mode,
+        )
+
     def set_log_level(self, level: str) -> None:
         """
           SetLogLevel:
         @loglevel: The new loglevel to use.
 
         Change the loglevel of the controller.
         """
         self.get_proxy().SetLogLevel(
             level,
         )
 
-    @property
-    def name(self) -> str:
+    def set_unit_properties(
+        self, name: str, runtime: bool, keyvalues: List[Tuple[str, Variant]]
+    ) -> None:
         """
-          Name:
+          SetUnitProperties:
+        @name: The name of the unit
+        @runtime: Specify if the changes should persist after reboot or not
+        @keyvalues: A list of the new values as key-value pair with the key being the name of the property
 
-        The name of the node.
+        Set named . If runtime is true the property changes do not persist across reboots.
         """
-        return self.get_proxy().Name
+        self.get_proxy().SetUnitProperties(
+            name,
+            runtime,
+            keyvalues,
+        )
 
-    @property
-    def status(self) -> str:
+    def start_unit(self, name: str, mode: str) -> ObjPath:
         """
-          Status:
+            StartUnit:
+          @name: The name of the unit to start
+          @mode: The mode used to start the unit
+          @job: The path for the job associated with the start operation
 
-        The connection status of the node with the BlueChi controller.
-        On any change, a signal is emitted on the org.freedesktop.DBus.Properties interface.
+          Queues a unit activate job for the named unit on this node. The queue is per-unit name, which means there is only ever one active job per unit. Mode
+        can be one of replace or fail. If there is an outstanding queued (but not running) job, that is replaced if mode is replace, or the job
+        fails if mode is fail.
+
+          The job returned is an object path for an object implementing org.eclipse.bluechi.Job, and which be monitored for the progress of the job, or used
+        to cancel the job. To track the result of the job, follow the JobRemoved signal on the Controller.
         """
-        return self.get_proxy().Status
+        return self.get_proxy().StartUnit(
+            name,
+            mode,
+        )
 
-    def on_status_changed(self, callback: Callable[[Variant], None]):
+    def stop_unit(self, name: str, mode: str) -> ObjPath:
         """
-          Status:
+          StopUnit:
+        @name: The name of the unit to stop
+        @mode: The mode used to stop the unit
+        @job: The path for the job associated with the stop operation
 
-        The connection status of the node with the BlueChi controller.
-        On any change, a signal is emitted on the org.freedesktop.DBus.Properties interface.
+        StopUnit() is similar to StartUnit() but stops the specified unit rather than starting it.
         """
+        return self.get_proxy().StopUnit(
+            name,
+            mode,
+        )
 
-        def on_properties_changed(
-            interface: str,
-            changed_props: Dict[str, Variant],
-            invalidated_props: Dict[str, Variant],
-        ) -> None:
-            value = changed_props.get("Status")
-            if value is not None:
-                callback(value)
+    def thaw_unit(self, name: str) -> None:
+        """
+          ThawUnit:
+        @name: The name of the unit to thaw
 
-        self.get_properties_proxy().PropertiesChanged.connect(on_properties_changed)
+        This is the inverse operation to the freeze command and resumes the execution of processes in the unit's cgroup.
+        """
+        self.get_proxy().ThawUnit(
+            name,
+        )
 
     @property
     def last_seen_timestamp(self) -> UInt64:
         """
           LastSeenTimestamp:
 
         A timestamp indicating when the last connection test (e.g. via heartbeat) was successful.
         """
         return self.get_proxy().LastSeenTimestamp
 
-
-class Agent(ApiBase):
-    """
-    org.eclipse.bluechi.Agent:
-    @short_description: Public interface of BlueChi on the managed node providing methods and signals for the respective node.
-
-    This interface is used to create proxy services resolving dependencies on services of other managed nodes.
-    """
-
-    def __init__(self, bus: MessageBus = None, use_systembus=True) -> None:
-        super().__init__(BC_AGENT_DBUS_INTERFACE, BC_OBJECT_PATH, bus, use_systembus)
-
-    def create_proxy(self, local_service_name: str, node: str, unit: str) -> None:
+    @property
+    def name(self) -> str:
         """
-          CreateProxy:
-        @local_service_name: The service name which requests the external dependency
-        @node: The requested node to provide the service
-        @unit: The external unit requested from the local service
+          Name:
 
-        BlueChi internal usage only.
-        CreateProxy() creates a new proxy service. It is part in the chain of resolving dependencies on services running on other managed nodes.
+        The name of the node.
         """
-        self.get_proxy().CreateProxy(
-            local_service_name,
-            node,
-            unit,
-        )
+        return self.get_proxy().Name
 
-    def remove_proxy(self, local_service_name: str, node: str, unit: str) -> None:
+    @property
+    def peer_ip(self) -> str:
         """
-          RemoveProxy:
-        @local_service_name: The service name which requests the external dependency
-        @node: The requested node to provide the service
-        @unit: The external unit requested from the local service
+          PeerIp:
 
-        BlueChi internal usage only.
-        RemoveProxy() removes a new proxy service. It is part in the chain of resolving dependencies on services running on other managed nodes.
+        The current IP of the connected node.
+        The address might be set even though the node is still offline since a call to org.eclipse.bluechi.Controller.Register hasn't been made.
         """
-        self.get_proxy().RemoveProxy(
-            local_service_name,
-            node,
-            unit,
-        )
+        return self.get_proxy().PeerIp
 
     @property
     def status(self) -> str:
         """
           Status:
 
-        The connection status of the agent with the BlueChi controller.
+        The connection status of the node with the BlueChi controller.
         On any change, a signal is emitted on the org.freedesktop.DBus.Properties interface.
         """
         return self.get_proxy().Status
 
     def on_status_changed(self, callback: Callable[[Variant], None]):
         """
           Status:
 
-        The connection status of the agent with the BlueChi controller.
+        The connection status of the node with the BlueChi controller.
         On any change, a signal is emitted on the org.freedesktop.DBus.Properties interface.
         """
 
         def on_properties_changed(
             interface: str,
             changed_props: Dict[str, Variant],
             invalidated_props: Dict[str, Variant],
         ) -> None:
             value = changed_props.get("Status")
             if value is not None:
                 callback(value)
 
         self.get_properties_proxy().PropertiesChanged.connect(on_properties_changed)
-
-    @property
-    def disconnect_timestamp(self) -> UInt64:
-        """
-          DisconnectTimestamp:
-
-        A timestamp indicating when the agent lost connection to the BlueChi controller.
-        If the connection is active (agent is online), this value is 0.
-        """
-        return self.get_proxy().DisconnectTimestamp
```

## bluechi/ext.py

```diff
@@ -1,7 +1,10 @@
+#
+# Copyright Contributors to the Eclipse BlueChi project
+#
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
 from dasbus.connection import MessageBus
 from typing import Callable, List, NamedTuple, Tuple
 from collections import namedtuple
 from dasbus.loop import EventLoop
 from dasbus.typing import UInt32, ObjPath
```

## Comparing `bluechi-0.7.0.dist-info/LICENSE` & `bluechi-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bluechi-0.7.0.dist-info/METADATA` & `bluechi-0.8.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluechi
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python bindings for BlueChi's D-Bus API
 Home-page: https://github.com/eclipse-bluechi/bluechi/
 Author: BlueChi developers
 License: LGPL-2.1-or-later
 Keywords: bluechi,python,D-Bus,systemd
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `bluechi-0.7.0.dist-info/RECORD` & `bluechi-0.8.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-bluechi/__init__.py,sha256=9dEZ4DPdQrhxpHeO_t5JKGT7Hi6x7CXL9oNmZ7z8jgc,44
-bluechi/api.py,sha256=K7PsLkcB7ZSvps6xuPn1wdcFFdodbg7PMbGcT2CHmNc,32330
-bluechi/ext.py,sha256=eoQHHFA0FgER7f5XFLkiGl7C6BoIbNs9ooanbDkedRY,2711
-bluechi-0.7.0.dist-info/LICENSE,sha256=3GJlINzVOiL3J68-5Cx3DlbJemT-OtsGN5nYqwMv5VE,26530
-bluechi-0.7.0.dist-info/METADATA,sha256=6UNJlV20015sbOUGMkQgbH8Gdr7P7Akugcry2aT9O20,1474
-bluechi-0.7.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-bluechi-0.7.0.dist-info/top_level.txt,sha256=i4SfNxlXM2F1a3dKJ3Z8Wyu9X2IGBWs4o3lqq7nDij0,8
-bluechi-0.7.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-bluechi-0.7.0.dist-info/RECORD,,
+bluechi/__init__.py,sha256=DijWGu1QqE85bvB8cKDxw6AaVxWmVY1qrVTdXowhU58,105
+bluechi/api.py,sha256=77MB_Judwux32y60R6adQZAoE37_L5lxzAyLinmsAu8,35241
+bluechi/ext.py,sha256=PtY21nC3iuLgNZRJESPPmm_n4Y0ugxPoypqfHt56xnk,2771
+bluechi-0.8.0.dist-info/LICENSE,sha256=3GJlINzVOiL3J68-5Cx3DlbJemT-OtsGN5nYqwMv5VE,26530
+bluechi-0.8.0.dist-info/METADATA,sha256=xEvBFsN1wvgtp_6M-py5Vwg43ge5APhHeRixcXRbGU0,1474
+bluechi-0.8.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+bluechi-0.8.0.dist-info/top_level.txt,sha256=i4SfNxlXM2F1a3dKJ3Z8Wyu9X2IGBWs4o3lqq7nDij0,8
+bluechi-0.8.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+bluechi-0.8.0.dist-info/RECORD,,
```

