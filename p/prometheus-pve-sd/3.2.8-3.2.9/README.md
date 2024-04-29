# Comparing `tmp/prometheus_pve_sd-3.2.8.tar.gz` & `tmp/prometheus_pve_sd-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_pve_sd-3.2.8.tar", max compression
+gzip compressed data, was "prometheus_pve_sd-3.2.9.tar", max compression
```

## Comparing `prometheus_pve_sd-3.2.8.tar` & `prometheus_pve_sd-3.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1123 2024-04-14 09:46:59.460627 prometheus_pve_sd-3.2.8/LICENSE
--rw-r--r--   0        0        0     2497 2024-04-14 09:46:59.460627 prometheus_pve_sd-3.2.8/README.md
--rw-r--r--   0        0        0        0 2024-04-14 09:47:00.236628 prometheus_pve_sd-3.2.8/prometheuspvesd/.drone.yml
--rw-r--r--   0        0        0       46 2024-04-14 09:47:13.496636 prometheus_pve_sd-3.2.8/prometheuspvesd/__init__.py
--rw-r--r--   0        0        0     6197 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/cli.py
--rw-r--r--   0        0        0     3981 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/client.py
--rw-r--r--   0        0        0     9929 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/config.py
--rw-r--r--   0        0        0     8123 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/discovery.py
--rw-r--r--   0        0        0      498 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/exception.py
--rw-r--r--   0        0        0     7685 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/logger.py
--rw-r--r--   0        0        0     1904 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/model.py
--rw-r--r--   0        0        0       30 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/__init__.py
--rw-r--r--   0        0        0      451 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/data/config.yml
--rw-r--r--   0        0        0       28 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/fixtures/__init__.py
--rw-r--r--   0        0        0    10561 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/fixtures/fixtures.py
--rw-r--r--   0        0        0     1366 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/conftest.py
--rw-r--r--   0        0        0     4861 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_cli.py
--rw-r--r--   0        0        0     1117 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_config.py
--rw-r--r--   0        0        0     3972 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_discovery.py
--rw-r--r--   0        0        0     1505 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_model.py
--rw-r--r--   0        0        0      900 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/utils.py
--rw-r--r--   0        0        0     3094 2024-04-14 09:47:13.492636 prometheus_pve_sd-3.2.8/pyproject.toml
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 prometheus_pve_sd-3.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1123 2024-04-29 09:01:00.783187 prometheus_pve_sd-3.2.9/LICENSE
+-rw-r--r--   0        0        0     2497 2024-04-29 09:01:00.783187 prometheus_pve_sd-3.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 09:01:01.567220 prometheus_pve_sd-3.2.9/prometheuspvesd/.drone.yml
+-rw-r--r--   0        0        0       46 2024-04-29 09:01:14.171746 prometheus_pve_sd-3.2.9/prometheuspvesd/__init__.py
+-rw-r--r--   0        0        0     6197 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/cli.py
+-rw-r--r--   0        0        0     3981 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/client.py
+-rw-r--r--   0        0        0     9929 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/config.py
+-rw-r--r--   0        0        0     8107 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/discovery.py
+-rw-r--r--   0        0        0      498 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/exception.py
+-rw-r--r--   0        0        0     7685 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/logger.py
+-rw-r--r--   0        0        0     1904 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/model.py
+-rw-r--r--   0        0        0       30 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/data/config.yml
+-rw-r--r--   0        0        0       28 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/fixtures/__init__.py
+-rw-r--r--   0        0        0    10561 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/fixtures/fixtures.py
+-rw-r--r--   0        0        0     1366 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/conftest.py
+-rw-r--r--   0        0        0     4861 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/test_cli.py
+-rw-r--r--   0        0        0     1117 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/test_config.py
+-rw-r--r--   0        0        0     3972 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/test_discovery.py
+-rw-r--r--   0        0        0     1505 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/test_model.py
+-rw-r--r--   0        0        0      900 2024-04-29 09:01:00.787187 prometheus_pve_sd-3.2.9/prometheuspvesd/utils.py
+-rw-r--r--   0        0        0     3094 2024-04-29 09:01:14.171746 prometheus_pve_sd-3.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 prometheus_pve_sd-3.2.9/PKG-INFO
```

### Comparing `prometheus_pve_sd-3.2.8/LICENSE` & `prometheus_pve_sd-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/README.md` & `prometheus_pve_sd-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/cli.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/client.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/client.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/config.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/config.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/discovery.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         self.host_list.clear()
         nodelist = self._get_names(self.client.get_nodes(), "node")
         self.logger.info(f"Discovered nodes: {','.join(nodelist)}")
         for node in nodelist:
             try:
                 qemu_list = self._filter(self.client.get_all_vms(node))
                 container_list = self._filter(self.client.get_all_containers(node))
-            except Exception as e:  # noqa
+            except Exception as e:
                 raise APIError(str(e)) from e
 
             # Merge QEMU and Containers lists from this node
             instances = self._get_variables(qemu_list, "qemu").copy()
             instances.update(self._get_variables(container_list, "container"))
 
             HOST_GAUGE.set(len(instances))
@@ -188,15 +188,15 @@
 
                 config = self.client.get_instance_config(node, pve_type, vmid)
 
                 try:
                     description = config["description"]
                 except KeyError:
                     description = None
-                except Exception as e:  # noqa
+                except Exception as e:
                     raise APIError(str(e)) from e
 
                 try:
                     metadata = json.loads(description)
                 except TypeError:
                     metadata = {}
                 except ValueError:
```

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/logger.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/logger.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/model.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/model.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/test/fixtures/fixtures.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/test/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/conftest.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_cli.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_config.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_discovery.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_model.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/test/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/prometheuspvesd/utils.py` & `prometheus_pve_sd-3.2.9/prometheuspvesd/utils.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.8/pyproject.toml` & `prometheus_pve_sd-3.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 include = ["LICENSE"]
 keywords = ["prometheus", "sd", "pve", "metrics"]
 license = "MIT"
 name = "prometheus-pve-sd"
 packages = [{ include = "prometheuspvesd" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/prometheus-pve-sd/"
-version = "3.2.8"
+version = "3.2.9"
 
 [tool.poetry.dependencies]
 anyconfig = "0.14.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 environs = "11.0.0"
 jsonschema = "4.21.1"
@@ -43,16 +43,16 @@
 requests = "2.31.0"
 "ruamel.yaml" = "0.18.6"
 
 [tool.poetry.scripts]
 prometheus-pve-sd = "prometheuspvesd.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.3.5"
-pytest = "8.1.1"
+ruff = "0.4.2"
+pytest = "8.2.0"
 pytest-mock = "3.14.0"
 pytest-cov = "5.0.0"
 toml = "0.10.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
```

### Comparing `prometheus_pve_sd-3.2.8/PKG-INFO` & `prometheus_pve_sd-3.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-sd
-Version: 3.2.8
+Version: 3.2.9
 Summary: Prometheus Service Discovery for Proxmox VE.
 Home-page: https://github.com/thegeeklab/prometheus-pve-sd/
 License: MIT
 Keywords: prometheus,sd,pve,metrics
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.8.0,<4.0.0
```

