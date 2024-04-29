# Comparing `tmp/aws_ssm_juggle-24.4.2.tar.gz` & `tmp/aws_ssm_juggle-24.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ssm_juggle-24.4.2.tar", max compression
+gzip compressed data, was "aws_ssm_juggle-24.4.3.tar", max compression
```

## Comparing `aws_ssm_juggle-24.4.2.tar` & `aws_ssm_juggle-24.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.4.2/LICENSE
--rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.4.2/README.md
--rw-r--r--   0        0        0     2014 2024-04-26 13:12:27.776698 aws_ssm_juggle-24.4.2/aws_ssm_juggle/__init__.py
--rw-r--r--   0        0        0     6548 2024-04-29 06:42:52.071092 aws_ssm_juggle-24.4.2/aws_ssm_juggle/ec2.py
--rw-r--r--   0        0        0    10316 2024-04-29 06:42:52.071092 aws_ssm_juggle-24.4.2/aws_ssm_juggle/ecs.py
--rw-r--r--   0        0        0      729 2024-04-29 06:42:27.007253 aws_ssm_juggle-24.4.2/pyproject.toml
--rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.2/setup.py
--rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.4.3/LICENSE
+-rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.4.3/README.md
+-rw-r--r--   0        0        0     2014 2024-04-26 13:12:27.776698 aws_ssm_juggle-24.4.3/aws_ssm_juggle/__init__.py
+-rw-r--r--   0        0        0     6593 2024-04-29 07:49:45.446020 aws_ssm_juggle-24.4.3/aws_ssm_juggle/ec2.py
+-rw-r--r--   0        0        0    10316 2024-04-29 06:42:52.071092 aws_ssm_juggle-24.4.3/aws_ssm_juggle/ecs.py
+-rw-r--r--   0        0        0      729 2024-04-29 07:49:57.940545 aws_ssm_juggle-24.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.3/setup.py
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.3/PKG-INFO
```

### Comparing `aws_ssm_juggle-24.4.2/LICENSE` & `aws_ssm_juggle-24.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.2/README.md` & `aws_ssm_juggle-24.4.3/README.md`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.2/aws_ssm_juggle/__init__.py` & `aws_ssm_juggle-24.4.3/aws_ssm_juggle/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.2/aws_ssm_juggle/ec2.py` & `aws_ssm_juggle-24.4.3/aws_ssm_juggle/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,17 +172,18 @@
         return instance_id, None
     reservations = ec2_paginator(
         boto3_session=boto3_session,
         paginator="describe_instances",
         leaf="Reservations",
     )
     instances = []
-    for instance in reservations[0].get("Instances"):
-        tags = {tag["Key"]: tag["Value"] for tag in instance.get("Tags", [])}
-        instances.append(f'{instance.get("InstanceId")} - {tags.get("Name")}')
+    for reservation in reservations:
+        for instance in reservation.get("Instances"):
+            tags = {tag["Key"]: tag["Value"] for tag in instance.get("Tags", [])}
+            instances.append(f'{instance.get("InstanceId")} - {tags.get("Name")}')
     return show_menu(
         items=instances,
         title="Select instance id",
         back=False,
     )
```

### Comparing `aws_ssm_juggle-24.4.2/aws_ssm_juggle/ecs.py` & `aws_ssm_juggle-24.4.3/aws_ssm_juggle/ecs.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.2/pyproject.toml` & `aws_ssm_juggle-24.4.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-ssm-juggle"
-version = "24.4.2"
+version = "24.4.3"
 description = "AWS SSM tool for ECS/EC2 (Shell, Port Forwardingm, ...)"
 authors = ["Stefan Heitmüller <stefan.heitmueller@gmx.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/morph027/aws-ssm-juggle"
 
 [tool.poetry.dependencies]
```

### Comparing `aws_ssm_juggle-24.4.2/setup.py` & `aws_ssm_juggle-24.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 entry_points = \
 {'console_scripts': ['ec2-juggle = aws_ssm_juggle.ec2:run',
                      'ecs-juggle = aws_ssm_juggle.ecs:run']}
 
 setup_kwargs = {
     'name': 'aws-ssm-juggle',
-    'version': '24.4.2',
+    'version': '24.4.3',
     'description': 'AWS SSM tool for ECS/EC2 (Shell, Port Forwardingm, ...)',
     'long_description': '# aws-ssm-juggle\n\n## Installation\n\n```\npip install aws-ssm-juggle\n```\n\n## Pre-requisites\n\n### [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)\n\n#### Linux\n\n```bash\ncurl https://s3.amazonaws.com/session-manager-downloads/plugin/latest/ubuntu_64bit/session-manager-plugin.deb -o "/tmp/session-manager-plugin.deb"\nmkdir -p ~/bin\ndpkg-deb --fsys-tarfile /tmp/session-manager-plugin.deb | tar --strip-components=4 -C ~/bin/ -xvf - usr/local/sessionmanagerplugin/bin/session-manager-plugin\n```\n\n#### MacOS\n\n`brew install --cask session-manager-plugin`\n\n### Infrastructure\n\nUse [ecs-exec-checker](https://github.com/aws-containers/amazon-ecs-exec-checker) to check for the pre-requisites to use ECS exec.\n\n## ecs-juggle\n\nInspired by [ecsgo](https://github.com/tedsmitt/ecsgo).\n\nProvides a tool to interact with AWS ECS tasks.\n\nCurrently provides:\n\n* interactive execute-command (e.g. shell)\n* port-forwarding\n\nYou can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted with a nice menu.\n\n\n### Usage\n\nSee `ecs-juggle --help` for all features.\n\n#### Execute command\n\nSelect all from menu:\n\n```bash\necs-juggle command\n```\n\n#### Port forwarding\n\nSelect all from menu:\n\n```bash\necs-juggle forward\n```\n\nSpecify port and select the rest from menu:\n\n```bash\necs-juggle forward --remote-port 8080\n```\n\n## ec2-juggle\n\nInspired by [gossm](https://github.com/gjbae1212/gossm/).\n\nProvides a tool to interact with AWS EC2 instances.\n\nCurrently provides:\n\n* interactive shell (e.g. shell)\n* ssh shell\n* port-forwarding\n\n### Usage\n\nSee `ec2-juggle --help` for all features.\n\n#### Start session\n\n```bash\nec2-juggle start\n```\n\n#### Start ssh session\n\nDefault:\n\n```bash\nec2-juggle ssh\n```\n\nWith extra arguments:\n\n```bash\nec2-juggle ssh --ssh-args="-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null -l ubuntu"\n```\n\n#### Port forwarding\n\n```bash\necs-juggle forward --remote-port 80\n```\n',
     'author': 'Stefan Heitmüller',
     'author_email': 'stefan.heitmueller@gmx.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/morph027/aws-ssm-juggle',
```

### Comparing `aws_ssm_juggle-24.4.2/PKG-INFO` & `aws_ssm_juggle-24.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-juggle
-Version: 24.4.2
+Version: 24.4.3
 Summary: AWS SSM tool for ECS/EC2 (Shell, Port Forwardingm, ...)
 Home-page: https://github.com/morph027/aws-ssm-juggle
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

