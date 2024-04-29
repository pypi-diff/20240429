# Comparing `tmp/esp-idf-sbom-0.8.0.tar.gz` & `tmp/esp-idf-sbom-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-sbom/esp-idf-sbom/dist/.tmp-k2kyiidf/esp-idf-sbom-0.8.0.tar", last modified: Thu Oct  5 10:28:09 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-sbom/esp-idf-sbom/dist/.tmp-cdvvjinr/esp-idf-sbom-0.9.0.tar", last modified: Tue Dec  5 07:29:55 2023, max compression
```

## Comparing `esp-idf-sbom-0.8.0.tar` & `esp-idf-sbom-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22262 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21234 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/mft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/nvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12406 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    42511 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/spdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23641 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/esp_idf_sbom/sbom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22262 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 10:28:09.000000 esp-idf-sbom-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2023-10-05 10:27:51.000000 esp-idf-sbom-0.8.0/test/test_sbom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22262 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21234 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/mft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/nvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40975 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/spdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23220 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/esp_idf_sbom/sbom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22262 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 07:29:55.000000 esp-idf-sbom-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2023-12-05 07:29:41.000000 esp-idf-sbom-0.9.0/test/test_sbom.py
```

### Comparing `esp-idf-sbom-0.8.0/LICENSE` & `esp-idf-sbom-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.8.0/PKG-INFO` & `esp-idf-sbom-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-sbom
-Version: 0.8.0
+Version: 0.9.0
 Summary: SPDX SBOM generator for ESP-IDF projects
 Home-page: https://github.com/espressif/esp-idf-sbom
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,spdx,sbom
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-sbom-0.8.0/README.md` & `esp-idf-sbom-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/git.py` & `esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/git.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/mft.py` & `esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/mft.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     if not os.path.isfile(path):
         return manifest
 
     try:
         with open(path, 'r') as f:
             manifest = yaml.safe_load(f.read()) or {}
     except (OSError, yaml.parser.ParserError) as e:
-        log.err.die(f'Cannot parse manifest file "{path}": {e}')
+        log.die(f'Cannot parse manifest file "{path}": {e}')
 
     # Convert cpe into a list
     if 'cpe' in manifest and type(manifest['cpe']) is not list:
         manifest['cpe'] = [manifest['cpe']]
 
     return manifest
 
@@ -124,15 +124,15 @@
         elif os.path.isdir(source):
             for root, dirs, files in utils.pwalk(source):
                 for file in files:
                     if file not in manifest_files.keys():
                         continue
                     add_file(os.path.join(root, file))
         else:
-            log.err.die(f'"{source}" is not file nor directory')
+            log.die(f'"{source}" is not file nor directory')
 
     return manifest_files
 
 
 def get_manifests(sources: List[str]) -> List[Dict[str, Any]]:
     """Go through sources list and gather all manifest. Manifest files are loaded and
     processed for referenced manifests, which are also included.
@@ -233,15 +233,15 @@
         if git_sha is None:
             # Even though the manifest contains hash variable, it may happen
             # that it's no longer part of git. For example the component might
             # have been exported or simply copied out of the git tree.
             # This is the case for managed components. Since there is no git information
             # available, we just skip this check.
             return True
-        msg = (f'Manifest in  \"{source}\" contains SHA \"{sha}\", which does not '
+        msg = (f'Manifest in \"{source}\" contains SHA \"{sha}\", which does not '
                f'match SHA \"{git_sha}\" recorded in git-tree for directory "{directory}". '
                f'Please update \"hash\" in \"{source}\" manifest '
                f'and also please do not forget to update version and other '
                f'information if necessary. It is important to keep this information '
                f'up-to-date for SBOM generation.')
         if sha == git_sha:
             return True
@@ -276,9 +276,9 @@
         }, ignore_extra_keys=True)
 
     try:
         sbom_schema.validate(manifest)
     except schema.SchemaError as e:
         msg = f'Manifest in "{source}" for "{directory}" is not valid: {e}'
         if die:
-            log.err.die(msg)
+            log.die(msg)
         raise RuntimeError(msg)
```

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/nvd.py` & `esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/nvd.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 https://nvd.nist.gov/developers/request-an-api-key and set the NVDAPIKEY
 environmental variable. For more information please see
 https://nvd.nist.gov/developers/start-here, section "Rate Limits".'''
 WARNED = False
 
 
 # https://nvd.nist.gov/developers/vulnerabilities
-def check(cpe: str, progress: bool=False) -> List[Dict[str, Any]]:
+def check(cpe: str) -> List[Dict[str, Any]]:
     """Checks given CPE against NVD and returns its reponse.
     When NVD API key is not provided, sleeps for 30 seconds to
     meet NVD's 5 requests per rolling 30 seconds windows limit.
     """
     base_url = 'https://services.nvd.nist.gov/rest/json/cves/2.0'
     vulns = []
     start_idx = 0
@@ -37,40 +37,36 @@
 
     while True:
         url = f'{base_url}?cpeName={cpe}&startIndex={start_idx}'
         req = urllib.request.Request(url)
         if apikey:
             req.add_header('apikey', apikey)
 
-        log.err.debug(f'NVD request url: {url}')
-        log.err.debug('NVD request headers:')
-        log.err.debug('\n'.join([f'{h}: {v}' for h, v in req.header_items()]))
+        log.debug(f'NVD request url: {url}')
+        log.debug('NVD request headers:')
+        log.debug('\n'.join([f'{h}: {v}' for h, v in req.header_items()]))
 
         try:
             res = urllib.request.urlopen(req)
         except urllib.error.HTTPError as e:
             if e.code == 403:
                 # https://nvd.nist.gov/developers/start-here Rate Limits
-                if progress:
-                    # if progress takes place echo new line, so the warning
-                    # is on new line
-                    log.err.warn('')
                 if not WARNED:
-                    log.err.warn(HINT)
+                    log.warn(HINT)
                     WARNED = True
-                log.err.warn(f'Sleeping for 30 seconds...')
+                log.warn(f'Sleeping for 30 seconds...')
                 time.sleep(30)
                 continue
 
             raise RuntimeError(f'HTTP GET for "{url}" returned error: "{e}"')
 
         data = json.loads(res.read().decode())
 
-        log.err.debug('NVD response:')
-        log.err.debug(json.dumps(data, indent=4))
+        log.debug('NVD response:')
+        log.debug(json.dumps(data, indent=4))
 
         vulns += data['vulnerabilities']
 
         start_idx += int(data['resultsPerPage'])
         if int(data['totalResults']) == start_idx:
             break
```

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/report.py` & `esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 
 import datetime
 import json
 import sys
 from argparse import Namespace
 from typing import Any, Dict, List
 
-from rich.align import Align
-from rich.console import Console
 from rich.table import Table
 
 from esp_idf_sbom import __version__
-from esp_idf_sbom.libsbom import utils
+from esp_idf_sbom.libsbom import log, utils
 
 empty_record = {
     'vulnerable': '',
     'pkg_name': '',
     'pkg_version': '',
     'cve_id': '',
     'cvss_base_score': '',
@@ -100,24 +98,22 @@
         severity = r['cvss_base_severity'] or 'unknown'
         severity_dict = summary['cves_summary'][severity.lower()]
         severity_dict['count'] += 1
         severity_dict['cves'].append(r['cve_id'])
         if r['pkg_name'] not in severity_dict['packages']:
             severity_dict['packages'].append(r['pkg_name'])
 
-    console = Console(no_color=args.no_colors, emoji=False)
-
     if args.format == 'json':
         summary['records'] = record_list
-        console.print_json(json.dumps(summary))
+        log.print_json(json.dumps(summary))
         return
     elif args.format == 'csv':
-        console.print(','.join(utils.csv_escape(empty_record.keys())))
+        log.print(','.join(utils.csv_escape(empty_record.keys())))
         for r in record_list:
-            console.print(','.join(utils.csv_escape(r.values())))
+            log.print(','.join(utils.csv_escape(r.values())))
         return
 
     cvss_severity_color_map = {
         'CRITICAL': '[red]',
         'HIGH': '[dark_orange]',
         'MEDIUM': '[yellow]',
         'LOW': '[green]',
@@ -161,15 +157,15 @@
     table.add_row('Packages affect by UNKNOWN CVEs:', ', '.join(severity_dict['packages']))
     table.add_row('Number of UNKNOWN CVEs:', str(severity_dict['count']), end_section=True)
 
     table.add_row('[bright_blue]All CVEs found:', ', '.join(summary['cves_summary']['all_cves']))
     table.add_row('[bright_blue]All packages affect by CVEs:', ', '.join(summary['cves_summary']['all_packages']))
     table.add_row('[bright_blue]Total number of CVEs:', str(summary['cves_summary']['total_cves_count']))
 
-    console.print(Align(table, align='center'), '\n')
+    log.print(table, '\n')
 
     # Table with newly identified vulnerabilities
     table = Table(title='[red]Packages with Identified Vulnerabilities',
                   caption='Newly identified vulnerabilities. Further analysis may be required for confirmation.')
     table.add_column('Package', vertical='middle', justify='center', overflow='fold')
     table.add_column('Version', vertical='middle', justify='center', overflow='fold')
     table.add_column('CVE ID', vertical='middle', justify='center', overflow='fold')
@@ -185,29 +181,29 @@
                r['cvss_version'],
                r['cpe'],
                r['cve_link'],
                r['cve_desc']]):
             info_table.add_column('key', overflow='fold')
             info_table.add_column('value', overflow='fold')
             info_table.add_row('[yellow]CVSS', r['cvss_version'])
-            info_table.add_row(f'[yellow]Vec.', r['cvss_vector_string'])
+            info_table.add_row('[yellow]Vec.', r['cvss_vector_string'])
             info_table.add_row('[yellow]CPE', r['cpe'])
             info_table.add_row('[yellow]Link', r['cve_link'])
             info_table.add_row('[yellow]Desc.', r['cve_desc'])
 
         table.add_row('[bright_blue]' + r['pkg_name'],
                       r['pkg_version'],
                       cvss_severity_color_map[r['cvss_base_severity']] + r['cve_id'],
                       cvss_severity_color_map[r['cvss_base_severity']] + r['cvss_base_score'],
                       cvss_severity_color_map[r['cvss_base_severity']] + r['cvss_base_severity'],
                       info_table,
                       end_section=True)
 
     if table.row_count:
-        console.print(Align(table, align='center'), '\n')
+        log.print(table, '\n')
 
     # Table with vulnerabilities in cve-exclude-list
     table = Table(title='[green]Packages with Excluded Vulnerabilities',
                   caption='Already assessed vulnerabilities that do not apply to packages.')
     table.add_column('Package', vertical='middle', justify='center', overflow='fold')
     table.add_column('Version', vertical='middle', justify='center', overflow='fold')
     table.add_column('CVE ID', vertical='middle', justify='center', overflow='fold')
@@ -224,30 +220,30 @@
                r['cpe'],
                r['cve_link'],
                r['cve_desc'],
                r['exclude_reason']]):
             info_table.add_column('key', overflow='fold')
             info_table.add_column('value', overflow='fold')
             info_table.add_row('[yellow]CVSS', r['cvss_version'])
-            info_table.add_row(f'[yellow]Vec.', r['cvss_vector_string'])
+            info_table.add_row('[yellow]Vec.', r['cvss_vector_string'])
             info_table.add_row('[yellow]CPE', r['cpe'])
             info_table.add_row('[yellow]Link', r['cve_link'])
             info_table.add_row('[yellow]Desc.', r['cve_desc'])
             info_table.add_row('[yellow]Reason', r['exclude_reason'])
 
         table.add_row('[bright_blue]' + r['pkg_name'],
                       r['pkg_version'],
                       cvss_severity_color_map[r['cvss_base_severity']] + r['cve_id'],
                       cvss_severity_color_map[r['cvss_base_severity']] + r['cvss_base_score'],
                       cvss_severity_color_map[r['cvss_base_severity']] + r['cvss_base_severity'],
                       info_table,
                       end_section=True)
 
     if table.row_count:
-        console.print(Align(table, align='center'), '\n')
+        log.print(table, '\n')
 
     # Table with packages which were scanned and no vulnerability was found
     table = Table(title='[green]Packages with No Identified Vulnerabilities',
                   caption='Packages checked against NVD with no vulnerabilities found.')
     table.add_column('Package', vertical='middle', justify='center', overflow='fold')
     table.add_column('Version', vertical='middle', justify='center', overflow='fold')
     table.add_column('CPE', vertical='middle', justify='center', overflow='fold')
@@ -257,15 +253,15 @@
             continue
         table.add_row('[bright_blue]' + r['pkg_name'],
                       r['pkg_version'],
                       '[yellow]' + r['cpe'],
                       end_section=True)
 
     if table.row_count:
-        console.print(Align(table, align='center'), '\n')
+        log.print(table, '\n')
 
     # Table with packages which were not scanned because of missing CPE
     table = Table(title='[green]Packages without CPE Information',
                   caption='Packages not checked against NVD.')
     table.add_column('Package', vertical='middle', justify='center', overflow='fold')
     table.add_column('Version', vertical='middle', justify='center', overflow='fold')
 
@@ -273,8 +269,8 @@
         if r['vulnerable'] != 'SKIPPED':
             continue
         table.add_row('[bright_blue]' + r['pkg_name'],
                       r['pkg_version'],
                       end_section=True)
 
     if table.row_count:
-        console.print(Align(table, align='center'))
+        log.print(table)
```

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/spdx.py` & `esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/spdx.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                     continue
                 match = self.SPDX_LICENSE_RE.search(line)
                 if match:
                     expr = match.group(1)
                     try:
                         parsed = self.licensing.parse(expr, validate=True)
                     except ExpressionError as e:
-                        log.err.warn(f'License expression "{expr}" found in "{self.path}" is not valid: {e}')
+                        log.warn(f'License expression "{expr}" found in "{self.path}" is not valid: {e}')
                         parsed = self.licensing.parse(expr)
                     self.licenses_expressions.add(expr)
                     for lic in parsed.objects:
                         self.licenses.add(lic)
 
 
 class SPDXFilesTags(SPDXTags):
@@ -171,22 +171,21 @@
 
     def __init__(self, args: Namespace, proj_desc: Dict[str, Any]) -> None:
         self.args = args
         self.proj_desc = proj_desc
         self.spdx: Dict[str, List[str]] = {}
         self.tags = SPDXTags()
 
-    def dump(self, colors=False) -> str:
+    def dump(self) -> str:
         """Return SPDX tag/value string representing the SPDX object."""
-        out = log.LogString(colors=colors)
-        out += ''
+        out = ''
         for tag, value in self.spdx.items():
             for v in value:
-                out += f'{out.GREEN}{tag}{out.RESET}: {out.YELLOW}{v}{out.RESET}\n'
-        return str(out)
+                out += f'[green]{tag}[/green]: [yellow]{v}[/yellow]\n'
+        return out
 
     def _check_spdx_tag(self, tag: str) -> None:
         if tag not in self.SPDX_TAGS:
             raise KeyError(f'Key "{tag}" is not supported SPDX tag')
 
     def __getitem__(self, key: str) -> List[str]:
         # If key doesn't exists return empty list.
@@ -367,63 +366,35 @@
         self['Relationship'] += [f'{self["SPDXID"][0]} DESCRIBES {self.project["SPDXID"][0]}']
 
     def _get_proj_desc(self, proj_desc_path: str) -> Dict[str, Any]:
         try:
             with open(proj_desc_path, 'r') as f:
                 proj_desc = json.load(f)
         except (OSError, ValueError) as e:
-            log.err.die(f'cannot read project description file: {e}')
+            log.die(f'cannot read project description file: {e}')
 
         if 'version' not in proj_desc:
-            log.err.die((f'Project description file "{proj_desc_path}" does not support SBOM generation. '
-                         f'Please see the list of IDF versions required by esp-idf-sbom.'))
+            log.die((f'Project description file "{proj_desc_path}" does not support SBOM generation. '
+                     f'Please see the list of IDF versions required by esp-idf-sbom.'))
 
         return proj_desc  # type: ignore
 
-    def dump(self, colors=False) -> str:
-        out = log.LogString(colors=colors)
+    def dump(self) -> str:
         header = ' '.join('\"' + arg + '\"' if ' ' in arg else arg for arg in sys.argv)
-        out.set_color(out.BLUE)
+        out = '[blue]'
         out += f'# Generated by esp-idf-sbom {__version__} with {header}\n\n'
         out += f'# SPDX document for project {self.name}\n'
-        out.reset_color()
-        out += super().dump(colors)
+        out += '[/blue]'
+        out += super().dump()
         out += '\n'
 
-        out += f'{out.BLUE}# project {self.project.name}{out.RESET}\n'
-        out += self.project.dump(colors)
+        out += f'[blue]# project {self.project.name}[/blue]\n'
+        out += self.project.dump()
 
-        return str(out)
-
-    def write(self, fn: Optional[str]=None, force_colors=False) -> None:
-        """Write full SPDX document to stdout or file."""
-        try:
-            if fn:
-                dirpath = os.path.dirname(fn)
-                if dirpath:
-                    os.makedirs(dirpath, exist_ok=True)
-                fd = open(fn, 'w')
-            else:
-                fd = sys.stdout  # type: ignore
-
-            colors = not self.args.no_colors
-            if colors and not fd.isatty() and not force_colors:
-                colors = False
-
-            fd.write(self.dump(colors))
-            fd.flush()
-        except OSError as e:
-            # This also catches BrokenPipeError in case the output is redirected
-            # and the receiver is closed. Some additional hardening is probably needed
-            # but this works for most of the time.
-            # https://docs.python.org/3/library/signal.html#note-on-sigpipe
-            log.err.die('cannot write to "{}": {}'.format(fn or 'stdout', e))
-        finally:
-            if fn:
-                fd.close()
+        return out
 
 
 class SPDXPackage(SPDXObject):
     """Base class for all SPDX packages: project, toolchain, component, subpackage, submodule.
     It implements basic functionality, which may be customized by overriding selected methods.
     get_subpackages:   Create packages for subpackages and submodules. If package doesn't have
                        any subpackages, e.g. toolchain o project, it may return empty list, so
@@ -464,16 +435,16 @@
         # Add referenced manifests into the global list
         for referenced_manifest in self.manifest['manifests']:
             # get full paths to the referenced manifest file and its destination directory
             path = utils.pjoin(self.dir, referenced_manifest['path'])
             dest = utils.pjoin(self.dir, referenced_manifest['dest'])
             if dest in self.REFERENCED_MANIFESTS:
                 existing_path = self.REFERENCED_MANIFESTS[dest]
-                log.err.die((f'Destination "{dest}" for referenced manifest "{path}" already has manifest '
-                             f'file "{existing_path}". Two manifest files are referencing same destination.'))
+                log.die((f'Destination "{dest}" for referenced manifest "{path}" already has manifest '
+                         f'file "{existing_path}". Two manifest files are referencing same destination.'))
 
             self.REFERENCED_MANIFESTS[dest] = path
 
         self.subpackages = self.get_subpackages()
 
         # exclude subpackage paths if any
         exclude_dirs = [subpkg.dir for subpkg in self.subpackages]
@@ -575,31 +546,30 @@
         tags: SPDXTags = SPDXTags()
         if self.files:
             tags = SPDXFileObjsTags(self.files)
         else:
             tags = SPDXDirTags(self.dir, exclude_dirs)
         return tags
 
-    def dump(self, colors=False) -> str:
-        out = log.LogString(colors=colors)
-        out += super().dump(colors)
+    def dump(self) -> str:
+        out = super().dump()
 
         if self.files:
             out += '\n'
-            out += f'{out.BLUE}# {self.name} {self.mark} files{out.RESET}'
+            out += f'[blue]# {self.name} {self.mark} files[/blue]'
             for f in self.files:
                 out += '\n'
-                out += f.dump(colors)
+                out += f.dump()
 
         for subpkg in self.subpackages:
             out += '\n'
-            out += f'{out.BLUE}# {subpkg.name} {subpkg.mark}{out.RESET}\n'
-            out += subpkg.dump(colors)
+            out += f'[blue]# {subpkg.name} {subpkg.mark}[blue]\n'
+            out += subpkg.dump()
 
-        return str(out)
+        return out
 
 
 class SPDXProject(SPDXPackage):
     """SPDX Package Information for the project binary."""
     def __init__(self, args: Namespace, proj_desc: Dict[str, Any]):
         self.args = args
         self.proj_desc = proj_desc
@@ -641,16 +611,16 @@
 
     def _get_linked_libs(self) -> List[str]:
         # Return list of libraries linked to the final binary based on info in linker map file.
         map_file = utils.pjoin(self.proj_desc['build_dir'],
                                self.proj_desc['project_name']) + '.map'
 
         if not os.path.isfile(map_file):
-            log.err.die((f'file "{map_file}" does not exist, please make '
-                         f'sure your project is configured and built'))
+            log.die((f'file "{map_file}" does not exist, please make '
+                     f'sure your project is configured and built'))
 
         with open(map_file, 'r') as f:
             lines = f.read().splitlines()
 
         libs = set()
         for line in lines[2:]:
             if not line:
@@ -707,15 +677,15 @@
         components: Dict[str, SPDXComponent] = {}
 
         for name, info in build_components.items():
             components[name] = SPDXComponent(self.args, self.proj_desc, name, info)
 
         for name, info in build_components.items():
             reqs = set(info['reqs'] + info['priv_reqs'] + info['managed_reqs'] + info['managed_priv_reqs'])
-            log.err.debug(f'component {name} requires: {reqs}')
+            log.debug(f'component {name} requires: {reqs}')
             for req in reqs:
                 if not self._component_used(build_components[req]):
                     continue
                 components[name]['Relationship'] += [f'{components[name]["SPDXID"][0]} DEPENDS_ON {components[req]["SPDXID"][0]}']
 
         return components
 
@@ -780,28 +750,27 @@
         for name, info in build_components.items():
             if name in reqs:
                 continue
             if not self._component_used(build_components[name]):
                 continue
             self['Relationship'] += [f'{self["SPDXID"][0]} DEPENDS_ON {self.components[name]["SPDXID"][0]}']
 
-    def dump(self, colors=False) -> str:
-        out = log.LogString(colors=colors)
-        out += super().dump(colors)
+    def dump(self) -> str:
+        out = super().dump()
 
         out += '\n'
-        out += f'{out.BLUE}# {self.toolchain.name} toolchain{out.RESET}\n'
-        out += self.toolchain.dump(colors)
+        out += f'[blue]# {self.toolchain.name} toolchain[/blue]\n'
+        out += self.toolchain.dump()
 
         for comp_name, comp in self.components.items():
             out += '\n'
-            out += f'{out.BLUE}# {comp_name} component{out.RESET}\n'
-            out += comp.dump(colors)
+            out += f'[blue]# {comp_name} component[/blue]\n'
+            out += comp.dump()
 
-        return str(out)
+        return out
 
 
 class SPDXToolchain(SPDXPackage):
     """SPDX Package Information for toolchain."""
     def __init__(self, args: Namespace, proj_desc: Dict[str, Any]):
         self.proj_desc = proj_desc
         self.info = self._get_toolchain_info()
@@ -838,45 +807,45 @@
         version = compiler_path_components[-4]
         platform = self._get_current_platform()
         tools_fn = utils.pjoin(self.proj_desc['idf_path'], 'tools', 'tools.json')
         try:
             with open(tools_fn, 'r') as f:
                 tools = json.load(f)
         except (OSError, ValueError) as e:
-            log.err.die(f'cannot read idf tools description file: {e}')
+            log.die(f'cannot read idf tools description file: {e}')
 
-        log.err.debug(f'toolchain: tools.json:')
-        log.err.debug(json.dumps(tools, indent=4))
+        log.debug(f'toolchain: tools.json:')
+        log.debug(json.dumps(tools, indent=4))
 
         # Get toolchain info based on name found in compiler's path.
         tool_info = next((t for t in tools['tools'] if t['name'] == name), None)
         if not tool_info:
-            log.err.die(f'cannot find "{name}" tool in "{tools_fn}"')
+            log.die(f'cannot find "{name}" tool in "{tools_fn}"')
 
         # Get tool version based on version found in compiler's path.
         tool_version = next((v for v in tool_info['versions'] if v['name'] == version), None)  # type: ignore
         if not tool_version:
-            log.err.die(f'cannot find "{version}" for "{name}" tool in "{tools_fn}"')
+            log.die(f'cannot find "{version}" for "{name}" tool in "{tools_fn}"')
 
         if platform not in tool_version:  # type: ignore
-            log.err.die((f'cannot find "{platform}" platform for "{version}" '
-                         f'for "{name}" tool in "{tools_fn}"'))
+            log.die((f'cannot find "{platform}" platform for "{version}" '
+                     f'for "{name}" tool in "{tools_fn}"'))
 
         info['name'] = name
         info['path'] = utils.pjoin('/',*compiler_path_components[:-4])
         info['version'] = version
         info['platform'] = platform
         info['description'] = tool_info['description']  # type: ignore
         info['info_url'] = tool_info['info_url']  # type: ignore
         info['url'] = tool_version[platform]['url']  # type: ignore
         info['size'] = tool_version[platform]['size']  # type: ignore
         info['sha256'] = tool_version[platform]['sha256']  # type: ignore
 
-        log.err.debug('toolchain info:')
-        log.err.debug(json.dumps(info, indent=4))
+        log.debug('toolchain info:')
+        log.debug(json.dumps(info, indent=4))
 
         return info
 
 
 class SPDXComponent(SPDXPackage):
     """SPDX Package Information for component."""
     def __init__(self, args: Namespace, proj_desc: Dict[str, Any], name: str, info: dict):
@@ -945,16 +914,16 @@
             self['FileCopyrightText'] = ['<text>' + '\n'.join(self.tags.copyrights) + '</text>']
         else:
             self['FileCopyrightText'] = ['NOASSERTION']
 
         if self.tags.contributors:
             self['FileContributor'] = list(self.tags.contributors)
 
-    def dump(self, colors=False) -> str:
-        return super().dump(colors)
+    def dump(self) -> str:
+        return super().dump()
 
 
 def parse_packages(buf: str) -> Dict[str, Dict[str, List[str]]]:
     """Very dummy SPDX file parser. Returns dictionary, where key is
     package SPDXID and value is dictionary with SPDX tag/values."""
     in_package = False
     in_text = False
@@ -1012,16 +981,16 @@
             in_package = True
             idx += 1
             packages[idx] = {}
 
         add_tag_value(tag, val)
 
     spdx_packages = {pkg['SPDXID'][0]: pkg for pkg in packages.values()}
-    log.err.debug('parsed spdx packages:')
-    log.err.debug(json.dumps(spdx_packages, indent=4))
+    log.debug('parsed spdx packages:')
+    log.debug(json.dumps(spdx_packages, indent=4))
     return spdx_packages
 
 
 def filter_packages(packages: Dict[str, Dict[str, List[str]]]):
     """Return only packages which are project package dependencies.
     For example configuration only packages are by default included, but not
     linked via relationship to the main project package. Such packages will
@@ -1044,10 +1013,10 @@
         for relationship in packages[pkg_spdxid]['Relationship']:
             src, rel, dst = relationship.split()
             if rel != 'DEPENDS_ON':
                 continue
             if dst not in seen:
                 queue.append(dst)
 
-    log.err.debug('filtered spdx packages:')
-    log.err.debug(json.dumps(out, indent=4))
+    log.debug('filtered spdx packages:')
+    log.debug(json.dumps(out, indent=4))
     return out
```

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom/libsbom/utils.py` & `esp-idf-sbom-0.9.0/esp_idf_sbom/libsbom/utils.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom/sbom.py` & `esp-idf-sbom-0.9.0/esp_idf_sbom/sbom.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,23 @@
 import argparse
 import os
 import sys
 from argparse import Namespace
 from typing import Dict, List
 
 import yaml
-from rich.console import Console
 from rich.progress import (BarColumn, MofNCompleteColumn, Progress, TextColumn,
                            TimeElapsedColumn)
 
 from esp_idf_sbom.libsbom import log, mft, nvd, report, spdx
 
 
 def cmd_create(args: Namespace) -> int:
     spdx_sbom = spdx.SPDXDocument(args, args.input_file)
-    spdx_sbom.write(args.output_file)
-    if args.print and args.output_file:
-        spdx_sbom.write(force_colors=args.force_colors)
+    log.print(spdx_sbom.dump())
     return 0
 
 
 def cmd_check(args: Namespace) -> int:
     if args.input_file == '-':
         buf = sys.stdin.read()
     else:
@@ -38,22 +35,21 @@
     record_list: List[Dict[str,str]] = []
     exit_code = 0
 
     packages = spdx.parse_packages(buf)
     if not args.check_all_packages:
         packages = spdx.filter_packages(packages)
 
-    progress_disabled = args.quiet or args.no_progress
     progress = Progress(
         BarColumn(),
         MofNCompleteColumn(),
         TimeElapsedColumn(),
         TextColumn('{task.description}'),
-        disable=progress_disabled,
-        console=Console(stderr=True, no_color=args.no_colors, emoji=False))
+        disable=args.no_progress,
+        console=log.console_stderr)
 
     progress.start()
 
     try:
         progress_task = progress.add_task('Checking pakcages', total=len(packages))
         for pkg in packages.values():
             package_added = False
@@ -76,18 +72,18 @@
                 comment = pkg['PackageComment'][0]
                 comment = comment[len('<text>'):-len('</text>')]
                 comment_yaml = yaml.safe_load(comment)
                 cve_exclude_list = {cve['cve']: cve['reason'] for cve in comment_yaml['cve-exclude-list']}
 
             for cpe in cpes:
                 try:
-                    vulns = nvd.check(cpe, not progress_disabled)
+                    vulns = nvd.check(cpe)
                 except RuntimeError as e:
                     progress.stop()
-                    log.err.die(f'{e}')
+                    log.die(f'{e}')
                 for vuln in vulns:
                     cve_id = vuln['cve']['id']
                     cve_link = f'https://nvd.nist.gov/vuln/detail/{cve_id}'
                     cve_desc = [desc['value'] for desc in vuln['cve']['descriptions'] if desc['lang'] == 'en'][0]
                     vulnerable = ''
                     exclude_reason = ''
                     cvss_version = ''
@@ -143,37 +139,36 @@
                     # CPE record used to check package against NVD
                     record['vulnerable'] = 'NO'
                     record['cpe'] = ', '.join(cpes)
                 record_list.append(record)
 
     except KeyboardInterrupt:
         progress.stop()
-        log.err.die('Process terminated')
+        log.die('Process terminated')
 
     progress.update(progress_task,advance=0, refresh=True, description='')
     progress.stop()
 
     # Project package is the first one
     project_pkg = packages[next(iter(packages))]
     proj_name = project_pkg['PackageName'][0]
     proj_ver = project_pkg['PackageVersion'][0]
     report.show(record_list, args, proj_name, proj_ver)
 
     return exit_code
 
 
 def cmd_manifest_validate(args: Namespace) -> int:
-    progress_disabled = args.quiet or args.no_progress
     progress = Progress(
         BarColumn(),
         MofNCompleteColumn(),
         TimeElapsedColumn(),
         TextColumn('{task.description}'),
-        disable=progress_disabled,
-        console=Console(stderr=True, no_color=args.no_colors, emoji=False))
+        disable=args.no_progress,
+        console=log.console_stderr)
 
     progress.start()
     try:
         progress_task = progress.add_task('Validating manifests')
         progress.update(progress_task, refresh=True, description='searching for manifest files')
 
         manifests = mft.get_manifests(args.validate_paths)
@@ -181,37 +176,36 @@
 
         for manifest in manifests:
             progress.update(progress_task, advance=1, refresh=True, description=manifest['_src'])
             mft.validate(manifest, manifest['_src'], manifest['_dst'], die=False)
 
     except RuntimeError as e:
         progress.stop()
-        log.err.die(str(e))
+        log.die(str(e))
     except KeyboardInterrupt:
         progress.stop()
-        log.err.die('Process terminated')
+        log.die('Process terminated')
 
     progress.update(progress_task,advance=0, refresh=True, description='')
     progress.stop()
 
     return 0
 
 
 def cmd_manifest_check(args: Namespace) -> int:
     record_list: List[Dict[str,str]] = []
     exit_code = 0
 
-    progress_disabled = args.quiet or args.no_progress
     progress = Progress(
         BarColumn(),
         MofNCompleteColumn(),
         TimeElapsedColumn(),
         TextColumn('{task.description}'),
-        disable=progress_disabled,
-        console=Console(stderr=True, no_color=args.no_colors, emoji=False))
+        disable=args.no_progress,
+        console=log.console_stderr)
 
     progress.start()
     try:
         progress_task = progress.add_task('Checking manifest files for vulnerabilities')
         progress.update(progress_task, refresh=True, description='searching for manifest files')
 
         manifests = mft.get_manifests(args.check_paths)
@@ -226,15 +220,15 @@
             cpes = manifest['cpe'] if isinstance(manifest['cpe'], list) else [manifest['cpe']]
             # Add version to CPEs
             version = manifest.get('version', '')
             cpes = [cpe.format(version) for cpe in cpes]
             name = manifest.get('name', manifest['cpe'][0].split(':')[4])
             cve_exclude_list = {cve['cve']: cve['reason'] for cve in manifest.get('cve-exclude-list', [])}
             for cpe in cpes:
-                vulns = nvd.check(cpe, not progress_disabled)
+                vulns = nvd.check(cpe)
 
                 for vuln in vulns:
                     cve_id = vuln['cve']['id']
                     cve_link = f'https://nvd.nist.gov/vuln/detail/{cve_id}'
                     cve_desc = [desc['value'] for desc in vuln['cve']['descriptions'] if desc['lang'] == 'en'][0]
                     vulnerable = ''
                     exclude_reason = ''
@@ -286,53 +280,46 @@
                 record['pkg_version'] = version
                 record['vulnerable'] = 'NO'
                 record['cpe'] = ', '.join(cpes)
                 record_list.append(record)
 
     except RuntimeError as e:
         progress.stop()
-        log.err.die(str(e))
+        log.die(str(e))
     except KeyboardInterrupt:
         progress.stop()
-        log.err.die('Process terminated')
+        log.die('Process terminated')
 
     progress.update(progress_task,advance=0, refresh=True, description='')
     progress.stop()
     report.show(record_list, args)
 
     return exit_code
 
 
 def main():
     parser = argparse.ArgumentParser(prog='esp-idf-sbom', description='ESP-IDF SBOM tool')
     parser.add_argument('-q', '--quiet',
                         action='store_true',
                         default=bool(os.environ.get('SBOM_QUIET')),
-                        help=('By default auxiliary messages like errors, warnings, debug messages '
-                              'or progress are reported to the standard error stream. With this option '
-                              'set, all such messages are suppressed.'))
-    parser.add_argument('-n', '--no-colors',
+                        help='Suppress all output.')
+    parser.add_argument('-n', '--no-color',
                         action='store_true',
-                        default=bool(os.environ.get('SBOM_NO_COLORS')),
+                        default=bool(os.environ.get('SBOM_NO_COLOR')),
                         help=('Do not emit color codes. By default color codes are used when stdout '
                               'or stderr is connected to a terminal.'))
-    parser.add_argument('-f', '--force-colors',
+    parser.add_argument('-f', '--force-terminal',
                         action='store_true',
-                        default=bool(os.environ.get('SBOM_FORCE_COLORS')),
-                        help=('Emit color codes even when stdout or stderr '
-                              'is not connected to a terminal.'))
-    parser.add_argument('-v', '--verbose',
-                        action='store_true',
-                        default=bool(os.environ.get('SBOM_VERBOSE')),
-                        help=('Be verbose. Messages are printed to standard error output.'))
+                        default=bool(os.environ.get('SBOM_FORCE_TERMINAL')) or None,
+                        help=('Enable terminal control codes even if out is not attached to terminal. '
+                              'This option is ignored if used along with the "--output-file" option.'))
     parser.add_argument('-d', '--debug',
                         action='store_true',
                         default=bool(os.environ.get('SBOM_DEBUG')),
                         help=('Print debug information. Messages are printed to standard error output.'))
-
     parser.add_argument('--no-progress',
                         action='store_true',
                         default=bool(os.environ.get('SBOM_CHECK_NO_PROGRESS')),
                         help=('Disable progress bar.'))
 
     subparsers = parser.add_subparsers(help='sub-command help')
 
@@ -391,18 +378,14 @@
                                default=bool(os.environ.get('SBOM_CREATE_NO_GUESS')),
                                help=('Don\'t try to identify PackageSupplier and PackageVersion. '
                                      'By default URLs are checked for known suppliers, currently only '
                                      'Espressif Systems, and project version or git describe is used '
                                      'to identify versions. With this option PackageSupplier and '
                                      'PackageVersion will be omitted, unless explicitly stated in '
                                      'sbom.yml, idf_component.yml or .gitmodules.'))
-    create_parser.add_argument('-p', '--print',
-                               action='store_true',
-                               default=bool(os.environ.get('SBOM_CREATE_PRINT')),
-                               help=('Print generated SBOM file to stdout even if "--output-file" is used.'))
     create_parser.add_argument('--file-tags',
                                action='store_true',
                                default=bool(os.environ.get('SBOM_CREATE_NO_FILE_TAGS')),
                                help=('Scan files for SPDX file tags. This includes SPDX-License-Identifier, '
                                      'SPDX-FileCopyrightText and SPDX-FileContributor'))
 
     check_parser = subparsers.add_parser('check',
@@ -413,14 +396,18 @@
     check_parser.add_argument('input_file',
                               metavar='SBOM_FILE',
                               default='-',
                               nargs='?',
                               help=('Path to the SBOM file generated by the ESP-IDF sbom tool. '
                                     'If not provided or "-", read from stdin.'))
 
+    check_parser.add_argument('-o', '--output-file',
+                              metavar='OUTPUT_FILE',
+                              help=('Print output to the specified file instead of stdout.'))
+
     check_parser.add_argument('--check-all-packages',
                               action='store_true',
                               default=bool(os.environ.get('SBOM_CHECK_ALL')),
                               help=('Check all packages in the SBOM file. By default only packages, '
                                     'linked via the SPDX relationship to the main project package, '
                                     'are checked. This may report vulnerabilities, which do not '
                                     'affect the resulting binary! For example components with libraries, '
@@ -446,45 +433,60 @@
                                           nargs='*',
                                           help=('Manifest file(sbom.yml, idf_manifest.yml or .gitmodules) or '
                                                 'directory, which will be searched for manifest files.'))
 
     manifest_check_parser = manifest_subparsers.add_parser('check',
                                                            help=('Check manifest files for vulnerabilities.'))
     manifest_check_parser.set_defaults(func=cmd_manifest_check)
+
+    manifest_check_parser.add_argument('-o', '--output-file',
+                                       metavar='OUTPUT_FILE',
+                                       help=('Print output to the specified file instead of stdout.'))
+
     manifest_check_parser.add_argument('--format',
                                        choices=['table', 'json', 'csv'],
                                        help=('table - Print report table. This is default.'
                                              'json - Print report in JSON format. '
                                              'csv - Print report in CSV format.'))
     manifest_check_parser.add_argument('check_paths',
                                        metavar='PATH_TO_CHECK',
                                        default=[os.path.curdir],
                                        nargs='*',
                                        help=('Manifest file(sbom.yml, idf_manifest.yml or .gitmodules) or '
                                              'directory, which will be searched for manifest files.'))
 
-    args = parser.parse_args()
-    if args.quiet:
-        log_level = log.NEVER
-    elif args.debug:
-        log_level = log.DEBUG
-    elif args.verbose:
-        log_level = log.INFO
-    else:
-        log_level = log.WARN
-
-    log.err.config(not args.no_colors, log_level, args.force_colors)
-    log.out.config(not args.no_colors, log.ALWAYS, args.force_colors)
+    ofile = sys.stdout
+    try:
+        args = parser.parse_args()
+        if args.force_terminal:
+            force_terminal_stdout = True
+            force_terminal_stderr = True
+        else:
+            force_terminal_stdout = None
+            force_terminal_stderr = None
+
+        if hasattr(args, 'output_file') and args.output_file:
+            force_terminal_stdout = False
+            ofile = open(args.output_file, 'w')
+
+        log.set_console(ofile, args.quiet, args.no_color, force_terminal_stdout,
+                        force_terminal_stderr, args.debug)
+
+        env = {key: value for key, value in os.environ.items() if key.startswith('SBOM_')}
+        log.debug(f'environ: {env}')
+        log.debug(f'args: {args}')
+
+        if 'func' not in args:
+            parser.print_help(sys.stderr)
+            sys.exit(1)
 
-    env = {key: value for key, value in os.environ.items() if key.startswith('SBOM_')}
-    log.err.debug(f'environ: {env}')
-    log.err.debug(f'args: {args}')
+        return args.func(args)
 
-    if 'func' not in args:
-        parser.print_help(sys.stderr)
+    except KeyboardInterrupt:
         sys.exit(1)
-
-    return args.func(args)
+    finally:
+        if ofile:
+            ofile.close()
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/PKG-INFO` & `esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-sbom
-Version: 0.8.0
+Version: 0.9.0
 Summary: SPDX SBOM generator for ESP-IDF projects
 Home-page: https://github.com/espressif/esp-idf-sbom
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,spdx,sbom
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-sbom-0.8.0/esp_idf_sbom.egg-info/SOURCES.txt` & `esp-idf-sbom-0.9.0/esp_idf_sbom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.8.0/setup.py` & `esp-idf-sbom-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.8.0/test/test_sbom.py` & `esp-idf-sbom-0.9.0/test/test_sbom.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 def test_check_sbom(hello_world_build: Path) -> None:
     tmpdir = TemporaryDirectory()
     output_fn = Path(tmpdir.name) / 'sbom.spdx'
     proj_desc_path = hello_world_build / 'build' / 'project_description.json'
     run([sys.executable, '-m', 'esp_idf_sbom', 'create', '-o', output_fn, proj_desc_path], check=True)
-    run([sys.executable, '-m', 'esp_idf_sbom', '-v', 'check', output_fn], check=True)
+    run([sys.executable, '-m', 'esp_idf_sbom', 'check', output_fn], check=True)
 
 
 def test_sbom_project_manifest(hello_world_build: Path) -> None:
     manifest = hello_world_build / 'sbom.yml'
     content = '''
               name: MY-PROJECT-NAME
               version: 999.999.999
```

