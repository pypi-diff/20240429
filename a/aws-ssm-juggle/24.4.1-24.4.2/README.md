# Comparing `tmp/aws_ssm_juggle-24.4.1.tar.gz` & `tmp/aws_ssm_juggle-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ssm_juggle-24.4.1.tar", max compression
+gzip compressed data, was "aws_ssm_juggle-24.4.2.tar", max compression
```

## Comparing `aws_ssm_juggle-24.4.1.tar` & `aws_ssm_juggle-24.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.4.1/LICENSE
--rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.4.1/README.md
--rw-r--r--   0        0        0     2014 2024-04-26 13:12:27.776698 aws_ssm_juggle-24.4.1/aws_ssm_juggle/__init__.py
--rw-r--r--   0        0        0     6499 2024-04-26 13:12:27.776966 aws_ssm_juggle-24.4.1/aws_ssm_juggle/ec2.py
--rw-r--r--   0        0        0    10440 2024-04-26 13:12:27.777179 aws_ssm_juggle-24.4.1/aws_ssm_juggle/ecs.py
--rw-r--r--   0        0        0      686 2024-04-26 13:24:25.748917 aws_ssm_juggle-24.4.1/pyproject.toml
--rw-r--r--   0        0        0     2945 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.1/setup.py
--rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.4.2/LICENSE
+-rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.4.2/README.md
+-rw-r--r--   0        0        0     2014 2024-04-26 13:12:27.776698 aws_ssm_juggle-24.4.2/aws_ssm_juggle/__init__.py
+-rw-r--r--   0        0        0     6548 2024-04-29 06:42:52.071092 aws_ssm_juggle-24.4.2/aws_ssm_juggle/ec2.py
+-rw-r--r--   0        0        0    10316 2024-04-29 06:42:52.071092 aws_ssm_juggle-24.4.2/aws_ssm_juggle/ecs.py
+-rw-r--r--   0        0        0      729 2024-04-29 06:42:27.007253 aws_ssm_juggle-24.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.2/setup.py
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.2/PKG-INFO
```

### Comparing `aws_ssm_juggle-24.4.1/LICENSE` & `aws_ssm_juggle-24.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.1/README.md` & `aws_ssm_juggle-24.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.1/aws_ssm_juggle/__init__.py` & `aws_ssm_juggle-24.4.2/aws_ssm_juggle/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.1/aws_ssm_juggle/ec2.py` & `aws_ssm_juggle-24.4.2/aws_ssm_juggle/ec2.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 import configargparse
 import shtab
 from boto3 import session
 from botocore import exceptions
 
-from aws_ssm_juggle import show_menu, port_forward
+from aws_ssm_juggle import port_forward, show_menu
 
 
 class EC2Session:
     """
     EC2Session
     """
 
@@ -46,17 +46,17 @@
             "SessionId": ssm_start_session.get("SessionId"),
             "TokenValue": ssm_start_session.get("TokenValue"),
             "StreamUrl": ssm_start_session.get("StreamUrl"),
         }
         args = [
             "session-manager-plugin",
             json.dumps(session_response),
-            self.ssm.region_name,
+            self.boto3_session.region_name,
             "StartSession",
-            self.ssm.profile_name,
+            self.boto3_session.profile_name,
             json.dumps(session_parameters),
         ]
         os.execvp(
             "session-manager-plugin",
             args,
         )
 
@@ -74,23 +74,23 @@
             print(err)
             exit(1)
         session_response = {
             "SessionId": ssm_start_session.get("SessionId"),
             "TokenValue": ssm_start_session.get("TokenValue"),
             "StreamUrl": ssm_start_session.get("StreamUrl"),
         }
-        proxy_command = f"ProxyCommand=session-manager-plugin '{json.dumps(session_response)}' {self.ssm.region_name} StartSession {self.ssm.profile_name} '{json.dumps(session_parameters)}'"
+        proxy_command = f"ProxyCommand=session-manager-plugin '{json.dumps(session_response)}' {self.boto3_session.region_name} StartSession {self.boto3_session.profile_name} '{json.dumps(session_parameters)}'"
         args = ["ssh"]
         if self.ssh_args:
             args.extend(self.ssh_args.split(" "))
         args.extend(
             [
                 "-o",
                 proxy_command,
-                f"{self.instance_id}.{self.ssm.region_name}.compute.internal",
+                f"{self.instance_id}.{self.boto3_session.region_name}.compute.internal",
             ]
         )
         os.execvp(
             "ssh",
             args,
         )
 
@@ -99,15 +99,14 @@
             boto3_session=self.boto3_session,
             remote_port=self.remote_port,
             local_port=self.local_port,
             target=self.target,
         )
 
 
-
 def get_parser():
     """argument parser"""
     parser = configargparse.ArgParser(
         prog="ec2-juggle",
         auto_env_var_prefix="EC2_JUGGLE_",
     )
     shtab.add_argument_to(
```

### Comparing `aws_ssm_juggle-24.4.1/aws_ssm_juggle/ecs.py` & `aws_ssm_juggle-24.4.2/aws_ssm_juggle/ecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 import configargparse
 import shtab
 from boto3 import session
 from botocore import exceptions
 
-from aws_ssm_juggle import show_menu, port_forward
+from aws_ssm_juggle import port_forward, show_menu
 
 
 class ECSSession:
     """
     ECSSession
     """
 
@@ -41,29 +41,25 @@
         self.container_index = container_index
         self.ecs = self.boto3_session.client("ecs")
         self.local_port = local_port
         self.remote_port = remote_port
         self.ssm = self.boto3_session.client("ssm")
         self.task = task
         self.task_details = task_details
-        self.runtime_id = (
-            task_details.get("tasks")[0].get("containers")[container_index].get("runtimeId")
-        )
+        self.runtime_id = task_details.get("tasks")[0].get("containers")[container_index].get("runtimeId")
         self.target = f"ecs:{self.cluster}_{self.runtime_id.split('-')[0]}_{self.runtime_id}"
 
-
     def port_forward(self):
         port_forward(
             boto3_session=self.boto3_session,
             remote_port=self.remote_port,
             local_port=self.local_port,
             target=self.target,
         )
 
-
     def execute_command(self):
         """
         execute command
         """
         try:
             ecs_execute_command_session = self.ecs.execute_command(
                 cluster=self.cluster,
@@ -74,17 +70,17 @@
             ).get("session")
         except exceptions.ClientError as err:
             print(err)
             exit(1)
         args = [
             "session-manager-plugin",
             json.dumps(ecs_execute_command_session),
-            self.ssm.region_name,
+            self.boto3_session.region_name,
             "StartSession",
-            self.ssm.profile_name,
+            self.boto3_session.profile_name,
             json.dumps(
                 {"Target": self.target},
             ),
         ]
         try:
             os.execvp(
                 "session-manager-plugin",
@@ -229,17 +225,15 @@
         title=f"[{cluster}|{service}] Select task",
     )
     if ret[0] is None:
         return (cluster, None, *ret)
     return (cluster, service, *ret)
 
 
-def get_container(
-    cluster: str, service: str, task: str, containers: list, container: str
-):
+def get_container(cluster: str, service: str, task: str, containers: list, container: str):
     """
     get container
     """
     if container:
         return task, container, containers.index(container)
     ret = show_menu(
         items=containers,
@@ -269,17 +263,15 @@
         title=f"[{cluster}|{service}|{task}|{container}] Select port",
     )
     if ret[0] is None:
         return (None, *ret)
     return (container, *ret)
 
 
-def menu_loop_condition(
-    cluster: str, service: str, task: str, container: str, remote_port: int, action: str
-):
+def menu_loop_condition(cluster: str, service: str, task: str, container: str, remote_port: int, action: str):
     menu_loop_condition = cluster and service and task and container
     if action == "forward":
         menu_loop_condition = menu_loop_condition and remote_port
     return menu_loop_condition
 
 
 def run():
@@ -313,42 +305,35 @@
         task=task,
         container=container,
         remote_port=remote_port,
         action=arguments.action,
     ):
         cluster, _ = get_cluster(ecs=ecs, cluster=cluster)
         cluster, service, _ = get_service(ecs=ecs, cluster=cluster, service=service)
-        cluster, service, task, _ = get_task(
-            ecs=ecs, cluster=cluster, service=service, task=task
-        )
+        cluster, service, task, _ = get_task(ecs=ecs, cluster=cluster, service=service, task=task)
         if cluster and task:
             task_details = ecs.describe_tasks(cluster=cluster, tasks=[task])
-            containers = [
-                container.get("name")
-                for container in task_details.get("tasks")[0].get("containers")
-            ]
+            containers = [container.get("name") for container in task_details.get("tasks")[0].get("containers")]
             # task, container, container_index = get_container(
             ret = get_container(
                 cluster=cluster,
                 service=service,
                 task=task,
                 containers=containers,
                 container=container,
             )
             task, container, container_index = ret
         if (arguments.action == "forward" and container) and not remote_port:
             task_definition_arn = task_details.get("tasks")[0].get("taskDefinitionArn")
-            task_definition = task_definition or ecs.describe_task_definition(
-                taskDefinition=task_definition_arn
-            ).get("taskDefinition")
+            task_definition = task_definition or ecs.describe_task_definition(taskDefinition=task_definition_arn).get(
+                "taskDefinition"
+            )
             ports = [
                 str(container.get("containerPort"))
-                for container in task_definition.get("containerDefinitions")[
-                    container_index
-                ].get("portMappings")
+                for container in task_definition.get("containerDefinitions")[container_index].get("portMappings")
             ]
             container, remote_port, _ = get_port(
                 cluster=cluster,
                 service=service,
                 task=task,
                 container=container,
                 containers=containers,
```

### Comparing `aws_ssm_juggle-24.4.1/setup.py` & `aws_ssm_juggle-24.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 entry_points = \
 {'console_scripts': ['ec2-juggle = aws_ssm_juggle.ec2:run',
                      'ecs-juggle = aws_ssm_juggle.ecs:run']}
 
 setup_kwargs = {
     'name': 'aws-ssm-juggle',
-    'version': '24.4.1',
-    'description': 'AWS SSM tool',
+    'version': '24.4.2',
+    'description': 'AWS SSM tool for ECS/EC2 (Shell, Port Forwardingm, ...)',
     'long_description': '# aws-ssm-juggle\n\n## Installation\n\n```\npip install aws-ssm-juggle\n```\n\n## Pre-requisites\n\n### [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)\n\n#### Linux\n\n```bash\ncurl https://s3.amazonaws.com/session-manager-downloads/plugin/latest/ubuntu_64bit/session-manager-plugin.deb -o "/tmp/session-manager-plugin.deb"\nmkdir -p ~/bin\ndpkg-deb --fsys-tarfile /tmp/session-manager-plugin.deb | tar --strip-components=4 -C ~/bin/ -xvf - usr/local/sessionmanagerplugin/bin/session-manager-plugin\n```\n\n#### MacOS\n\n`brew install --cask session-manager-plugin`\n\n### Infrastructure\n\nUse [ecs-exec-checker](https://github.com/aws-containers/amazon-ecs-exec-checker) to check for the pre-requisites to use ECS exec.\n\n## ecs-juggle\n\nInspired by [ecsgo](https://github.com/tedsmitt/ecsgo).\n\nProvides a tool to interact with AWS ECS tasks.\n\nCurrently provides:\n\n* interactive execute-command (e.g. shell)\n* port-forwarding\n\nYou can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted with a nice menu.\n\n\n### Usage\n\nSee `ecs-juggle --help` for all features.\n\n#### Execute command\n\nSelect all from menu:\n\n```bash\necs-juggle command\n```\n\n#### Port forwarding\n\nSelect all from menu:\n\n```bash\necs-juggle forward\n```\n\nSpecify port and select the rest from menu:\n\n```bash\necs-juggle forward --remote-port 8080\n```\n\n## ec2-juggle\n\nInspired by [gossm](https://github.com/gjbae1212/gossm/).\n\nProvides a tool to interact with AWS EC2 instances.\n\nCurrently provides:\n\n* interactive shell (e.g. shell)\n* ssh shell\n* port-forwarding\n\n### Usage\n\nSee `ec2-juggle --help` for all features.\n\n#### Start session\n\n```bash\nec2-juggle start\n```\n\n#### Start ssh session\n\nDefault:\n\n```bash\nec2-juggle ssh\n```\n\nWith extra arguments:\n\n```bash\nec2-juggle ssh --ssh-args="-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null -l ubuntu"\n```\n\n#### Port forwarding\n\n```bash\necs-juggle forward --remote-port 80\n```\n',
     'author': 'Stefan Heitmüller',
     'author_email': 'stefan.heitmueller@gmx.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/morph027/aws-ssm-juggle',
     'packages': packages,
```

### Comparing `aws_ssm_juggle-24.4.1/PKG-INFO` & `aws_ssm_juggle-24.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aws-ssm-juggle
-Version: 24.4.1
-Summary: AWS SSM tool
+Version: 24.4.2
+Summary: AWS SSM tool for ECS/EC2 (Shell, Port Forwardingm, ...)
 Home-page: https://github.com/morph027/aws-ssm-juggle
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

