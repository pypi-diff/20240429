# Comparing `tmp/issx-0.4.0.tar.gz` & `tmp/issx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issx-0.4.0.tar", max compression
+gzip compressed data, was "issx-0.5.0.tar", max compression
```

## Comparing `issx-0.4.0.tar` & `issx-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1101 2024-04-21 21:35:12.594056 issx-0.4.0/LICENCE
--rw-r--r--   0        0        0     5557 2024-04-21 21:35:12.594056 issx-0.4.0/README.md
--rw-r--r--   0        0        0     3507 2024-04-21 21:35:12.594056 issx-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/__init__.py
--rw-r--r--   0        0        0     4783 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/cli.py
--rw-r--r--   0        0        0      137 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/clients/__init__.py
--rw-r--r--   0        0        0      317 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/clients/exceptions.py
--rw-r--r--   0        0        0     3829 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/clients/gitlab.py
--rw-r--r--   0        0        0     2595 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/clients/interfaces.py
--rw-r--r--   0        0        0     3678 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/clients/redmine.py
--rw-r--r--   0        0        0      106 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/domain/__init__.py
--rw-r--r--   0        0        0      513 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/domain/config.py
--rw-r--r--   0        0        0      205 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/domain/issues.py
--rw-r--r--   0        0        0        0 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/instance_managers/__init__.py
--rw-r--r--   0        0        0     2339 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/instance_managers/config_parser.py
--rw-r--r--   0        0        0     1372 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/instance_managers/managers.py
--rw-r--r--   0        0        0        0 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/py.typed
--rw-r--r--   0        0        0     2360 2024-04-21 21:35:12.594056 issx-0.4.0/src/issx/services.py
--rw-r--r--   0        0        0     6617 1970-01-01 00:00:00.000000 issx-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-29 12:39:08.915533 issx-0.5.0/LICENCE
+-rw-r--r--   0        0        0     6557 2024-04-29 12:39:08.915533 issx-0.5.0/README.md
+-rw-r--r--   0        0        0     3535 2024-04-29 12:39:08.915533 issx-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 12:39:08.915533 issx-0.5.0/src/issx/__init__.py
+-rw-r--r--   0        0        0     6733 2024-04-29 12:39:08.915533 issx-0.5.0/src/issx/cli.py
+-rw-r--r--   0        0        0      969 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/cli_utils.py
+-rw-r--r--   0        0        0      137 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/clients/__init__.py
+-rw-r--r--   0        0        0      317 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/clients/exceptions.py
+-rw-r--r--   0        0        0     4008 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/clients/gitlab.py
+-rw-r--r--   0        0        0     3258 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/clients/interfaces.py
+-rw-r--r--   0        0        0     3857 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/clients/redmine.py
+-rw-r--r--   0        0        0      106 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/domain/__init__.py
+-rw-r--r--   0        0        0     1707 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/domain/config.py
+-rw-r--r--   0        0        0      205 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/domain/issues.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/instance_managers/__init__.py
+-rw-r--r--   0        0        0     2420 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/instance_managers/config_parser.py
+-rw-r--r--   0        0        0     2557 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/instance_managers/managers.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/py.typed
+-rw-r--r--   0        0        0     2360 2024-04-29 12:39:08.919533 issx-0.5.0/src/issx/services.py
+-rw-r--r--   0        0        0     7617 1970-01-01 00:00:00.000000 issx-0.5.0/PKG-INFO
```

### Comparing `issx-0.4.0/LICENCE` & `issx-0.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `issx-0.4.0/README.md` & `issx-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -41,14 +41,48 @@
 The basic functionality of `issx` is provided through the `issx` command-line interface (CLI).
 For a full list of available commands and options, please refer to the [CLI reference](https://nekeal.github.io/issx/cli_reference).
 
 !!! warning
     The `issx` CLI requires a configuration file to be present in the working directory (`issx.toml`) or in `~/.config/issx.toml`.
     Refer to the [Configuration file](#configuration-file) section for more information.
 
+### Initializing the configuration file
+
+There is a set of dedicated commands to initialize the configuration file and add instances and projects to it.
+
+#### Generate a new instance's configuration
+
+```shell
+> issx config generate-instance --instance gitlab-cloud
+
+Enter backend [gitlab/redmine]: gitlab
+Enter url: https://gitlab.com
+Enter token: token
+
+[instances.gitlab-cloud]
+backend = 'gitlab'
+url = 'https://gitlab.com'
+token = 'token'
+```
+The output should be then copied to the [Configuration file](#configuration-file).
+
+#### Generate a new project's configuration
+
+```shell
+> issx config generate-project --project my-personal-project
+Enter instance: gitlab-cloud   # The name of the instance that is already configured
+Enter project: 11111111        # Identifier of the project characteristic for the instance's backend
+
+[projects.my-personal-project]
+instance = 'gitlab-cloud'
+project = '11111111'
+````
+
+The output should be then copied to the [Configuration file](#configuration-file).
+
 ### Copying issues
 It allows to copy issues from one [configured](#configuration-file) project to another.
 
 ```shell title="Copy an issue"
 issx copy --source=<project_name> --target=<project_name> <issue-id>
 ```
```

### Comparing `issx-0.4.0/pyproject.toml` & `issx-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "issx"
-version = "0.4.0"
+version = "0.5.0"
 description = "Tool for synchronizing issues between different services"
 authors = [
     "nekeal <szymon.sc.cader@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -120,15 +120,16 @@
     --no-cov-on-fail \
 """
 
 [tool.coverage.report]
 #fail_under = 100 # uncomment after reaching 100% coverage
 exclude_lines = [
     'if TYPE_CHECKING:',
-    'pragma: no cover'
+    'pragma: no cover',
+    '@abc.abstractmethod',
 ]
 
 [tool.mypy]
 disallow_any_unimported = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 strict_equality = true
```

### Comparing `issx-0.4.0/src/issx/clients/gitlab.py` & `issx-0.5.0/src/issx/clients/gitlab.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Self, cast
 
+from attr import asdict
 from gitlab import Gitlab, GitlabGetError
 from gitlab.v4.objects import CurrentUser, Project, ProjectIssue
 
 from issx.clients.exceptions import IssueDoesNotExistError, ProjectDoesNotExistError
 from issx.clients.interfaces import InstanceClientInterface, IssueClientInterface
 from issx.domain.config import InstanceConfig, ProjectFlatConfig
 from issx.domain.issues import Issue
@@ -26,18 +27,14 @@
 
     @classmethod
     def issues_to_domain_list(cls, issues: list[ProjectIssue]) -> list[Issue]:
         return [cls.issue_to_domain(issue) for issue in issues]
 
 
 class GitlabInstanceClient(InstanceClientInterface):
-    @classmethod
-    def instance_from_config(cls, instance_config: InstanceConfig) -> Self:
-        return cls(Gitlab(instance_config.url, private_token=instance_config.token))
-
     def __init__(self, client: Gitlab):
         self.client = client
 
     async def auth(self) -> str | None:
         self.client.auth()
         if user := self.client.user:
             return cast(str, user.username)
@@ -48,14 +45,19 @@
         if not self.client.user:
             raise ValueError("Cannot get user from Gitlab client")
         return self.client.user
 
     def get_instance_url(self) -> str:
         return self.client.url
 
+    @classmethod
+    def instance_from_config(cls, instance_config: InstanceConfig) -> Self:
+        instance_config = cls.instance_config_class(**asdict(instance_config))
+        return cls(Gitlab(instance_config.url, private_token=instance_config.token))
+
 
 class GitlabClient(IssueClientInterface, GitlabInstanceClient):
     """Gitlab client implementations"""
 
     def __init__(self, client: Gitlab, project_id: int):
         self.project_id = project_id
         self._project: Project | None = None
@@ -103,11 +105,12 @@
         except GitlabGetError as e:
             raise IssueDoesNotExistError(issue_id) from e
 
     @classmethod
     def from_config(
         cls, instance_config: InstanceConfig, project_config: ProjectFlatConfig
     ) -> Self:
+        project_config = cls.project_config_class(**asdict(project_config))
         return cls(
             GitlabInstanceClient.instance_from_config(instance_config).client,
             project_id=int(project_config.project),
         )
```

### Comparing `issx-0.4.0/src/issx/clients/interfaces.py` & `issx-0.5.0/src/issx/clients/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import abc
-from typing import Self
+from typing import ClassVar, Self
 
 from issx.domain.config import InstanceConfig, ProjectFlatConfig
 from issx.domain.issues import Issue
 
 
 class InstanceClientInterface(abc.ABC):
     """
     Interface for a client that interacts with an issue tracker instance
     """
 
+    instance_config_class: ClassVar[type[InstanceConfig]] = InstanceConfig
+
     @abc.abstractmethod
     async def auth(self) -> str | None:
         """
         Authenticate the client with the instance.
         Raises an internal error if the authentication fails or returns None.
         :return: The username of the authenticated user or None
         """
@@ -27,22 +29,27 @@
         pass
 
     @classmethod
     @abc.abstractmethod
     def instance_from_config(cls, instance_config: InstanceConfig) -> Self:
         """
         Create an instance of the client from a configuration dictionary.
-        :param config: The configuration dictionary. Higher level code should validate
-        the configuration.
+        If required, the instance_config can be converted to an instance-specific
+        configuration according to the `instance_config_class` attribute of the client.
+
+        :param instance_config: The configuration object. Higher level code
+        should validate the configuration.
         :return: An instance of the client
         """
         pass
 
 
 class IssueClientInterface(abc.ABC):
+    project_config_class: ClassVar[type[ProjectFlatConfig]] = ProjectFlatConfig
+
     @abc.abstractmethod
     async def get_issue(self, issue_id: int) -> Issue:
         """
         Retrieve an issue by its ID.
         Raises IssueDoesNotExistError if the issue does not exist.
         :param issue_id: The ID of the issue
         :return: Issue object
@@ -74,17 +81,22 @@
     @classmethod
     @abc.abstractmethod
     def from_config(
         cls, instance_config: InstanceConfig, project_config: ProjectFlatConfig
     ) -> Self:
         """
         Create an instance of the client from configuration classes.
+        If required, the project_config can be converted to a project-specific
+        configuration according to the `project_config_class` attribute of the client.
+
         Args:
             instance_config: InstanceConfig to configure the client to the instance
-            project_config: ProjectFlatConfig to configure client
+            project_config: ProjectFlatConfig to configure client. This config can then
+            be converted to a project-specific config according to
+            the `project_config_class` attribute of the client.
             to the particular project
 
         Returns:
             An instance of the client
 
         """
         pass
```

### Comparing `issx-0.4.0/src/issx/clients/redmine.py` & `issx-0.5.0/src/issx/clients/redmine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Self
 
+from attr import asdict
 from redminelib import Redmine
 from redminelib.exceptions import ResourceNotFoundError
 from redminelib.resources import Issue as RedmineIssue
 from redminelib.resources import Project
 from redminelib.resultsets import ResourceSet
 
 from issx.clients.exceptions import IssueDoesNotExistError, ProjectDoesNotExistError
@@ -40,14 +41,15 @@
         return str(self.client.auth())
 
     def get_instance_url(self) -> str:
         return str(self.client.url)
 
     @classmethod
     def instance_from_config(cls, instance_config: InstanceConfig) -> Self:
+        instance_config = cls.instance_config_class(**asdict(instance_config))
         return cls(
             Redmine(
                 instance_config.url,
                 key=instance_config.token,
             )
         )
 
@@ -95,11 +97,12 @@
                 ) from e
         return self._project
 
     @classmethod
     def from_config(
         cls, instance_config: InstanceConfig, project_config: ProjectFlatConfig
     ) -> Self:
+        project_config = cls.project_config_class(**asdict(project_config))
         return cls(
             RedmineInstanceClient.instance_from_config(instance_config).client,
             project_id=int(project_config.project),
         )
```

### Comparing `issx-0.4.0/src/issx/instance_managers/config_parser.py` & `issx-0.5.0/src/issx/instance_managers/config_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,21 +42,23 @@
     def from_dict(cls, data: dict) -> Self:
         parsed_data = GenericConfig(
             instances={
                 name: InstanceConfig(
                     backend=SupportedBackend(instance.get("backend")),
                     url=instance.get("url"),
                     token=instance.get("token"),
+                    raw_config=instance,
                 )
                 for name, instance in data["instances"].items()
             },
             projects={
                 name: ProjectFlatConfig(
                     instance=project.get("instance"),
                     project=project.get("project"),
+                    raw_config=project,
                 )
                 for name, project in data.get("projects", {}).items()
             },
         )
         return cls(parsed_data)
 
     @staticmethod
```

### Comparing `issx-0.4.0/src/issx/instance_managers/managers.py` & `issx-0.5.0/src/issx/instance_managers/managers.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,17 +17,53 @@
         cls,
         backend: SupportedBackend,
         instance_client_class: type[InstanceClientInterface],
         project_client_class: type[IssueClientInterface],
     ) -> None:
         cls.backends[backend] = (instance_client_class, project_client_class)
 
+    @classmethod
+    def clear_backends(cls) -> None:
+        cls.backends.clear()
+
     def get_instance_client(self, instance: str) -> InstanceClientInterface:
+        """
+        Get an instance client for a given instance name.
+
+        Converts the instance config to the appropriate config class
+         and creates an instance client.
+        Args:
+            instance: Instance name
+
+        Returns: Instance of an instance client
+        """
         instance_config = self.config.get_instance_config(instance)
         client_class = self.backends[instance_config.backend][0]
+        instance_config = client_class.instance_config_class(
+            **instance_config.raw_config, raw_config=instance_config.raw_config
+        )
         return client_class.instance_from_config(instance_config)
 
     def get_project_client(self, project: str) -> IssueClientInterface:
+        """
+        Get a project client for a given project name.
+
+        Converts the project config to the appropriate config class
+        and creates a project client.
+        Args:
+            project: Project name
+
+        Returns: Instance of a project client
+
+        """
         project_config = self.config.get_project_config(project)
         instance_config = self.config.get_instance_config(project_config.instance)
-        client_class = self.backends[instance_config.backend][1]
-        return client_class.from_config(instance_config, project_config)
+        instance_client_class, project_client_class = self.backends[
+            instance_config.backend
+        ]
+        instance_config = instance_client_class.instance_config_class(
+            **instance_config.raw_config, raw_config=instance_config.raw_config
+        )
+        project_config = project_client_class.project_config_class(
+            **project_config.raw_config, raw_config=project_config.raw_config
+        )
+        return project_client_class.from_config(instance_config, project_config)
```

### Comparing `issx-0.4.0/src/issx/services.py` & `issx-0.5.0/src/issx/services.py`

 * *Files identical despite different names*

### Comparing `issx-0.4.0/PKG-INFO` & `issx-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issx
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tool for synchronizing issues between different services
 Home-page: https://nekeal.github.io/issx
 License: MIT
 Author: nekeal
 Author-email: szymon.sc.cader@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -68,14 +68,48 @@
 The basic functionality of `issx` is provided through the `issx` command-line interface (CLI).
 For a full list of available commands and options, please refer to the [CLI reference](https://nekeal.github.io/issx/cli_reference).
 
 !!! warning
     The `issx` CLI requires a configuration file to be present in the working directory (`issx.toml`) or in `~/.config/issx.toml`.
     Refer to the [Configuration file](#configuration-file) section for more information.
 
+### Initializing the configuration file
+
+There is a set of dedicated commands to initialize the configuration file and add instances and projects to it.
+
+#### Generate a new instance's configuration
+
+```shell
+> issx config generate-instance --instance gitlab-cloud
+
+Enter backend [gitlab/redmine]: gitlab
+Enter url: https://gitlab.com
+Enter token: token
+
+[instances.gitlab-cloud]
+backend = 'gitlab'
+url = 'https://gitlab.com'
+token = 'token'
+```
+The output should be then copied to the [Configuration file](#configuration-file).
+
+#### Generate a new project's configuration
+
+```shell
+> issx config generate-project --project my-personal-project
+Enter instance: gitlab-cloud   # The name of the instance that is already configured
+Enter project: 11111111        # Identifier of the project characteristic for the instance's backend
+
+[projects.my-personal-project]
+instance = 'gitlab-cloud'
+project = '11111111'
+````
+
+The output should be then copied to the [Configuration file](#configuration-file).
+
 ### Copying issues
 It allows to copy issues from one [configured](#configuration-file) project to another.
 
 ```shell title="Copy an issue"
 issx copy --source=<project_name> --target=<project_name> <issue-id>
 ```
```

