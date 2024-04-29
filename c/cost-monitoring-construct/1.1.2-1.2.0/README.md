# Comparing `tmp/cost-monitoring-construct-1.1.2.tar.gz` & `tmp/cost-monitoring-construct-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-monitoring-construct-1.1.2.tar", last modified: Thu May 11 08:03:42 2023, max compression
+gzip compressed data, was "cost-monitoring-construct-1.2.0.tar", last modified: Mon Apr 29 12:52:43 2024, max compression
```

## Comparing `cost-monitoring-construct-1.1.2.tar` & `cost-monitoring-construct-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:03:42.686594 cost-monitoring-construct-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-11 08:03:42.686594 cost-monitoring-construct-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:03:42.686594 cost-monitoring-construct-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:03:42.682594 cost-monitoring-construct-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:03:42.686594 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct/
--rw-r--r--   0 runner    (1001) docker     (123)    61281 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:03:42.686594 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76189 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.1.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:03:24.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:03:42.686594 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-11 08:03:42.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-11 08:03:42.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:03:42.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 08:03:42.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 08:03:42.000000 cost-monitoring-construct-1.1.2/src/cost_monitoring_construct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.756587 cost-monitoring-construct-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/
+-rw-r--r--   0 runner    (1001) docker     (127)    70040 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77521 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/top_level.txt
```

### Comparing `cost-monitoring-construct-1.1.2/LICENSE` & `cost-monitoring-construct-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cost-monitoring-construct-1.1.2/PKG-INFO` & `cost-monitoring-construct-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-monitoring-construct
-Version: 1.1.2
+Version: 1.2.0
 Summary: A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage
 Home-page: https://github.com/DataChefHQ/cost-monitoring-construct.git
 Author: DataChef<support@datachef.co>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataChefHQ/cost-monitoring-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cost-monitoring-construct-1.1.2/README.md` & `cost-monitoring-construct-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cost-monitoring-construct-1.1.2/setup.py` & `cost-monitoring-construct-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cost-monitoring-construct",
-    "version": "1.1.2",
+    "version": "1.2.0",
     "description": "A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage",
     "license": "Apache-2.0",
     "url": "https://github.com/DataChefHQ/cost-monitoring-construct.git",
     "long_description_content_type": "text/markdown",
     "author": "DataChef<support@datachef.co>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cost_monitoring_construct",
         "cost_monitoring_construct._jsii"
     ],
     "package_data": {
         "cost_monitoring_construct._jsii": [
-            "cost-monitoring-construct@1.1.2.jsii.tgz"
+            "cost-monitoring-construct@1.2.0.jsii.tgz"
         ],
         "cost_monitoring_construct": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cost-monitoring-construct-1.1.2/src/cost_monitoring_construct/__init__.py` & `cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -993,15 +993,15 @@
     IBudgetStrategy,
     metaclass=jsii.JSIIMeta,
     jsii_type="cost-monitoring-construct.ApplicationCostMonitoring",
 ):
     def __init__(
         self,
         stack: _aws_cdk_ceddda9d.Stack,
-        props: "IApplicationCostMonitoringProps",
+        props: "ApplicationCostMonitoringProps",
     ) -> None:
         '''Default Application CostMonitoring class that implements daily and monthly budgets.
 
         :param stack: - default stack to track its resources and it will be used to define Budget resources in it.
         :param props: -
 
         Example::
@@ -1107,14 +1107,23 @@
         ...
 
     @application_name.setter
     def application_name(self, value: builtins.str) -> None:
         ...
 
     @builtins.property
+    @jsii.member(jsii_name="costAllocationTag")
+    def cost_allocation_tag(self) -> typing.Optional[builtins.str]:
+        ...
+
+    @cost_allocation_tag.setter
+    def cost_allocation_tag(self, value: typing.Optional[builtins.str]) -> None:
+        ...
+
+    @builtins.property
     @jsii.member(jsii_name="otherStacksIncludedInBudget")
     def other_stacks_included_in_budget(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]]:
         ...
 
     @other_stacks_included_in_budget.setter
@@ -1139,14 +1148,26 @@
     def application_name(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0908894562bb6b1e002cfc2998d89bf3aa6fd8824c3de1bb8bec8ef25bb81a73)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "applicationName", value)
 
     @builtins.property
+    @jsii.member(jsii_name="costAllocationTag")
+    def cost_allocation_tag(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "costAllocationTag"))
+
+    @cost_allocation_tag.setter
+    def cost_allocation_tag(self, value: typing.Optional[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0672d13ac4327bb5a1ad546e7a493f18b1ad64186dde6abe7e36ad71223a3f67)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "costAllocationTag", value)
+
+    @builtins.property
     @jsii.member(jsii_name="otherStacksIncludedInBudget")
     def other_stacks_included_in_budget(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]]:
         return typing.cast(typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]], jsii.get(self, "otherStacksIncludedInBudget"))
 
     @other_stacks_included_in_budget.setter
@@ -1159,17 +1180,128 @@
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "otherStacksIncludedInBudget", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IApplicationCostMonitoringProps).__jsii_proxy_class__ = lambda : _IApplicationCostMonitoringPropsProxy
 
 
+@jsii.implements(IApplicationCostMonitoringProps)
+class ApplicationCostMonitoringProps(
+    metaclass=jsii.JSIIMeta,
+    jsii_type="cost-monitoring-construct.ApplicationCostMonitoringProps",
+):
+    def __init__(
+        self,
+        application_name: builtins.str,
+        monthly_limit_in_dollars: jsii.Number,
+        other_stacks_included_in_budget: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.Stack]] = None,
+        default_topic: typing.Optional[builtins.str] = None,
+        subscribers: typing.Optional[typing.Sequence[builtins.str]] = None,
+        cost_allocation_tag: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param application_name: -
+        :param monthly_limit_in_dollars: -
+        :param other_stacks_included_in_budget: -
+        :param default_topic: -
+        :param subscribers: -
+        :param cost_allocation_tag: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__016611925949da4facbba95bcddcf14217d235eea769e2db3a3d240c6ca86d73)
+            check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
+            check_type(argname="argument monthly_limit_in_dollars", value=monthly_limit_in_dollars, expected_type=type_hints["monthly_limit_in_dollars"])
+            check_type(argname="argument other_stacks_included_in_budget", value=other_stacks_included_in_budget, expected_type=type_hints["other_stacks_included_in_budget"])
+            check_type(argname="argument default_topic", value=default_topic, expected_type=type_hints["default_topic"])
+            check_type(argname="argument subscribers", value=subscribers, expected_type=type_hints["subscribers"])
+            check_type(argname="argument cost_allocation_tag", value=cost_allocation_tag, expected_type=type_hints["cost_allocation_tag"])
+        jsii.create(self.__class__, self, [application_name, monthly_limit_in_dollars, other_stacks_included_in_budget, default_topic, subscribers, cost_allocation_tag])
+
+    @builtins.property
+    @jsii.member(jsii_name="applicationName")
+    def application_name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "applicationName"))
+
+    @application_name.setter
+    def application_name(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4fd4ce542700b2deac40811890f4429d90eac081bd29d08415e6ce8667697422)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "applicationName", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="monthlyLimitInDollars")
+    def monthly_limit_in_dollars(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "monthlyLimitInDollars"))
+
+    @monthly_limit_in_dollars.setter
+    def monthly_limit_in_dollars(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__57b7dbe15daa64f31317dedf1362713156a13c2d526b10bae05bb824fb1852b5)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "monthlyLimitInDollars", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="costAllocationTag")
+    def cost_allocation_tag(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "costAllocationTag"))
+
+    @cost_allocation_tag.setter
+    def cost_allocation_tag(self, value: typing.Optional[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3bd683e50b33baeaf6f59fc99784ce52773a612c0f5a480e422ab4972f7f6e2b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "costAllocationTag", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="defaultTopic")
+    def default_topic(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "defaultTopic"))
+
+    @default_topic.setter
+    def default_topic(self, value: typing.Optional[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a36b5adee3e84bbffda1fbfb9801304b1780cd8ef3dc089586a0aeee043a09a7)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "defaultTopic", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="otherStacksIncludedInBudget")
+    def other_stacks_included_in_budget(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]]:
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]], jsii.get(self, "otherStacksIncludedInBudget"))
+
+    @other_stacks_included_in_budget.setter
+    def other_stacks_included_in_budget(
+        self,
+        value: typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__27ca7aaaa6cac405f55855e5078ed65603a6f03c771242fe182f13cf406a81a0)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "otherStacksIncludedInBudget", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="subscribers")
+    def subscribers(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "subscribers"))
+
+    @subscribers.setter
+    def subscribers(self, value: typing.Optional[typing.List[builtins.str]]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__bac5a7c82099fee82a0b4f1e50169bd023e5de76ee7c699ab88840159ea951e2)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "subscribers", value)
+
+
 __all__ = [
     "AccountCostMonitoring",
     "ApplicationCostMonitoring",
+    "ApplicationCostMonitoringProps",
     "Budget",
     "ComparisonOperator",
     "IApplicationCostMonitoringProps",
     "IBudgetAlertCondition",
     "IBudgetProps",
     "IBudgetStrategy",
     "IBudgetStrategyProps",
@@ -1411,15 +1543,15 @@
     _subscribers: typing.Sequence[typing.Union[_aws_cdk_aws_budgets_ceddda9d.CfnBudget.SubscriberProperty, typing.Dict[builtins.str, typing.Any]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__361ff8775d5ca30a358315f98c5b27b9eb15f57051ae67ebfad4c5e0c037aedf(
     stack: _aws_cdk_ceddda9d.Stack,
-    props: IApplicationCostMonitoringProps,
+    props: ApplicationCostMonitoringProps,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__60a43e31b85a1187100c257ebb94b68ea4041c3f8a9670ca7f5d4e6d18a1d910(
     daily_limit: jsii.Number,
     subscribers: typing.Sequence[typing.Union[_aws_cdk_aws_budgets_ceddda9d.CfnBudget.SubscriberProperty, typing.Dict[builtins.str, typing.Any]]],
@@ -1450,12 +1582,65 @@
 
 def _typecheckingstub__0908894562bb6b1e002cfc2998d89bf3aa6fd8824c3de1bb8bec8ef25bb81a73(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__0672d13ac4327bb5a1ad546e7a493f18b1ad64186dde6abe7e36ad71223a3f67(
+    value: typing.Optional[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__1b6cbb5b07678e3fafe88dc1a98554194ef0f287b295a5a466ce4f76da7ea988(
     value: typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]],
 ) -> None:
     """Type checking stubs"""
     pass
+
+def _typecheckingstub__016611925949da4facbba95bcddcf14217d235eea769e2db3a3d240c6ca86d73(
+    application_name: builtins.str,
+    monthly_limit_in_dollars: jsii.Number,
+    other_stacks_included_in_budget: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.Stack]] = None,
+    default_topic: typing.Optional[builtins.str] = None,
+    subscribers: typing.Optional[typing.Sequence[builtins.str]] = None,
+    cost_allocation_tag: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4fd4ce542700b2deac40811890f4429d90eac081bd29d08415e6ce8667697422(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__57b7dbe15daa64f31317dedf1362713156a13c2d526b10bae05bb824fb1852b5(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3bd683e50b33baeaf6f59fc99784ce52773a612c0f5a480e422ab4972f7f6e2b(
+    value: typing.Optional[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a36b5adee3e84bbffda1fbfb9801304b1780cd8ef3dc089586a0aeee043a09a7(
+    value: typing.Optional[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__27ca7aaaa6cac405f55855e5078ed65603a6f03c771242fe182f13cf406a81a0(
+    value: typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bac5a7c82099fee82a0b4f1e50169bd023e5de76ee7c699ab88840159ea951e2(
+    value: typing.Optional[typing.List[builtins.str]],
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `cost-monitoring-construct-1.1.2/src/cost_monitoring_construct.egg-info/PKG-INFO` & `cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-monitoring-construct
-Version: 1.1.2
+Version: 1.2.0
 Summary: A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage
 Home-page: https://github.com/DataChefHQ/cost-monitoring-construct.git
 Author: DataChef<support@datachef.co>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataChefHQ/cost-monitoring-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cost-monitoring-construct-1.1.2/src/cost_monitoring_construct.egg-info/SOURCES.txt` & `cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cost_monitoring_construct/py.typed
 src/cost_monitoring_construct.egg-info/PKG-INFO
 src/cost_monitoring_construct.egg-info/SOURCES.txt
 src/cost_monitoring_construct.egg-info/dependency_links.txt
 src/cost_monitoring_construct.egg-info/requires.txt
 src/cost_monitoring_construct.egg-info/top_level.txt
 src/cost_monitoring_construct/_jsii/__init__.py
-src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.1.2.jsii.tgz
+src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.2.0.jsii.tgz
```

