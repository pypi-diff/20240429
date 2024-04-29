# Comparing `tmp/jupyterlab_courselevels-0.6.4.tar.gz` & `tmp/jupyterlab_courselevels-0.8.1.tar.gz`

## Comparing `jupyterlab_courselevels-0.6.4.tar` & `jupyterlab_courselevels-0.8.1.tar`

### file list

```diff
@@ -1,43 +1,51 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.eslintignore
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.eslintrc.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.prettierignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.yarnrc.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/CHANGELOG.md
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/RELEASE.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/install.json
--rw-r--r--   0        0        0   286095 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/package-lock.json
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/package.json
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/package.json.version
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/tsconfig.json
--rw-r--r--   0        0        0   211518 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/yarn.lock
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.macnb/log
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.macnb/pid
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.macnb/port
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.macnb/token
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/examples/admonitions.ipynb
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/examples/courselevels.ipynb
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/_version.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/package.json
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/schemas/jupyterlab-courselevels/package.json.orig
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/schemas/jupyterlab-courselevels/plugin.json
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/static/127.8ad3c40fd9931b31c227.js
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/static/606.9b0d8e09a6d2ad7c7ada.js
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/static/747.d451ccdabb6593af957e.js
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/static/remoteEntry.f775066622bb7b0b8e94.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/static/style.js
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/schema/plugin.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/src/admonitions.ts
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/src/index.ts
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/style/index.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/style/index.js
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/LICENSE
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/README.md
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/.eslintignore
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/.eslintrc.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/.prettierignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/.yarnrc.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/RELEASE.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/install.json
+-rw-r--r--   0        0        0   286095 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/package-lock.json
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/package.json
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/package.json.version
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/tsconfig.json
+-rw-r--r--   0        0        0   211518 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/yarn.lock
+-rw-r--r--   0        0        0     7008 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/.macnb/log
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/examples/courselevels.ipynb
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/_version.py
+-rw-r--r--   0        0        0    20698 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/build_log.json
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/package.json
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/schemas/jupyterlab-courselevels/package.json.orig
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/schemas/jupyterlab-courselevels/plugin.json
+-rw-r--r--   0        0        0    11301 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.25fbe2f6581d0a777b1f.js
+-rw-r--r--   0        0        0     9979 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.25fbe2f6581d0a777b1f.js.map
+-rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.3de9501ec3a0c88836bb.js
+-rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.3de9501ec3a0c88836bb.js.map
+-rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.a5145521343950b351b7.js
+-rw-r--r--   0        0        0    13974 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.a5145521343950b351b7.js.map
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.cf91f028dc5a1c30b067.js
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.cf91f028dc5a1c30b067.js.map
+-rw-r--r--   0        0        0    29415 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/remoteEntry.4d4f620bee2c920894b2.js.map
+-rw-r--r--   0        0        0    29415 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/remoteEntry.6579e183dbe72c61ee72.js.map
+-rw-r--r--   0        0        0    30540 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/remoteEntry.e815a346e6f671d2071f.js
+-rw-r--r--   0        0        0    29415 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/remoteEntry.e815a346e6f671d2071f.js.map
+-rw-r--r--   0        0        0    29415 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/remoteEntry.ec5834f3f0aa867fa91d.js.map
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/style.js
+-rw-r--r--   0        0        0    21423 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/style_index_js.d252b5bdc2549f39f627.js
+-rw-r--r--   0        0        0    17550 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/style_index_js.d252b5bdc2549f39f627.js.map
+-rw-r--r--   0        0        0    30667 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.089892fd7b7347882ee4.js
+-rw-r--r--   0        0        0    27917 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.089892fd7b7347882ee4.js.map
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/schema/plugin.json
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/src/index.ts
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/style/index.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/style/index.js
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/README.md
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.8.1/PKG-INFO
```

### Comparing `jupyterlab_courselevels-0.6.4/.eslintrc.js` & `jupyterlab_courselevels-0.8.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.6.4/RELEASE.md` & `jupyterlab_courselevels-0.8.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.6.4/package-lock.json` & `jupyterlab_courselevels-0.8.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.6.4/package.json` & `jupyterlab_courselevels-0.8.1/package.json.version`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.6.3'"}*

```diff
@@ -94,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.4"
+    "version": "0.6.3"
 }
```

### Comparing `jupyterlab_courselevels-0.6.4/package.json.version` & `jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/schemas/jupyterlab-courselevels/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.8.0'"}*

```diff
@@ -94,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.3"
+    "version": "0.8.0"
 }
```

### Comparing `jupyterlab_courselevels-0.6.4/tsconfig.json` & `jupyterlab_courselevels-0.8.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.6.4/yarn.lock` & `jupyterlab_courselevels-0.8.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.6.4/examples/courselevels.ipynb` & `jupyterlab_courselevels-0.8.1/examples/courselevels.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'cells'": "{insert: [(12, OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'5065f758-64bd-4feb-95da-25d1b49a95b4'), ('metadata', OrderedDict([('tags', "*

 * *            "['level_intermediate'])])), ('outputs', []), ('source', ['# as of 0.8, level toggling "*

 * *            "applies on Scope.Multiple, meaning all selected cells if relevant'])])), (13, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'e5bbb07a-cb66-4097-9490-4703 […]*

```diff
@@ -187,14 +187,56 @@
                     "level_basic",
                     "framed_cell"
                 ]
             },
             "source": [
                 "note that a framed cell can also be with a level, here basic"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "5065f758-64bd-4feb-95da-25d1b49a95b4",
+            "metadata": {
+                "tags": [
+                    "level_intermediate"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "# as of 0.8, level toggling applies on Scope.Multiple, meaning all selected cells if relevant"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e5bbb07a-cb66-4097-9490-470311049c93",
+            "metadata": {
+                "tags": [
+                    "level_intermediate"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "# so we can change "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "22d709d7-9d0d-4169-9542-79d840282fed",
+            "metadata": {
+                "tags": [
+                    "level_intermediate"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "# a whole region in one shot"
+            ]
         }
     ],
     "metadata": {
         "jupytext": {
             "cell_metadata_filter": "all,-hidden,-heading_collapsed,-run_control,-trusted",
             "notebook_metadata_filter": "all,-language_info,-toc,-jupytext.text_representation.jupytext_version,-jupytext.text_representation.format_version"
         },
```

### Comparing `jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/package.json` & `jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e815a346e6f671d2071f.js'}}",*

 * * "'version'": "'0.8.0'"}*

```diff
@@ -44,15 +44,15 @@
         "style/index.js",
         "schema/*.json"
     ],
     "homepage": "https://github.com/parmentelat/jupyterlab-courselevels",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f775066622bb7b0b8e94.js",
+            "load": "static/remoteEntry.e815a346e6f671d2071f.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_courselevels/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.4"
+    "version": "0.8.0"
 }
```

### Comparing `jupyterlab_courselevels-0.6.4/jupyterlab_courselevels/labextension/schemas/jupyterlab-courselevels/package.json.orig` & `jupyterlab_courselevels-0.8.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.8.1'"}*

```diff
@@ -94,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.4"
+    "version": "0.8.1"
 }
```

### Comparing `jupyterlab_courselevels-0.6.4/src/index.ts` & `jupyterlab_courselevels-0.8.1/jupyterlab_courselevels/labextension/static/lib_index_js.25fbe2f6581d0a777b1f.js`

 * *Files 24% similar despite different names*

```diff
@@ -1,696 +1,707 @@
-00000000: 2f2a 0a20 2a20 666f 7220 6174 7461 6368  /*. * for attach
-00000010: 696e 6720 6b65 7962 696e 6469 6e67 7320  ing keybindings 
-00000020: 6c61 7465 7220 6f6e 2c20 7365 650a 202a  later on, see. *
-00000030: 2068 7474 7073 3a2f 2f74 6f77 6172 6473   https://towards
-00000040: 6461 7461 7363 6965 6e63 652e 636f 6d2f  datascience.com/
-00000050: 686f 772d 746f 2d63 7573 746f 6d69 7a65  how-to-customize
-00000060: 2d6a 7570 7974 6572 6c61 622d 6b65 7962  -jupyterlab-keyb
-00000070: 6f61 7264 2d73 686f 7274 6375 7473 2d37  oard-shortcuts-7
-00000080: 3233 3231 6637 3337 3533 640a 202a 2f0a  2321f73753d. */.
-00000090: 0a2f 2a20 6573 6c69 6e74 2d64 6973 6162  ./* eslint-disab
-000000a0: 6c65 2070 7265 7474 6965 722f 7072 6574  le prettier/pret
-000000b0: 7469 6572 202a 2f0a 0a69 6d70 6f72 7420  tier */..import 
-000000c0: 7b20 4a75 7079 7465 7246 726f 6e74 456e  { JupyterFrontEn
-000000d0: 642c 204a 7570 7974 6572 4672 6f6e 7445  d, JupyterFrontE
-000000e0: 6e64 506c 7567 696e 207d 2066 726f 6d20  ndPlugin } from 
-000000f0: 2740 6a75 7079 7465 726c 6162 2f61 7070  '@jupyterlab/app
-00000100: 6c69 6361 7469 6f6e 270a 696d 706f 7274  lication'.import
-00000110: 207b 2049 436f 6d6d 616e 6450 616c 6574   { ICommandPalet
-00000120: 7465 207d 2066 726f 6d20 2740 6a75 7079  te } from '@jupy
-00000130: 7465 726c 6162 2f61 7070 7574 696c 7327  terlab/apputils'
-00000140: 0a69 6d70 6f72 7420 7b0a 2020 494e 6f74  .import {.  INot
-00000150: 6562 6f6f 6b54 7261 636b 6572 2c0a 2020  ebookTracker,.  
-00000160: 4e6f 7465 626f 6f6b 5061 6e65 6c2c 0a20  NotebookPanel,. 
-00000170: 2049 4e6f 7465 626f 6f6b 4d6f 6465 6c0a   INotebookModel.
-00000180: 7d20 6672 6f6d 2027 406a 7570 7974 6572  } from '@jupyter
-00000190: 6c61 622f 6e6f 7465 626f 6f6b 270a 696d  lab/notebook'.im
-000001a0: 706f 7274 207b 2043 656c 6c20 7d20 6672  port { Cell } fr
-000001b0: 6f6d 2027 406a 7570 7974 6572 6c61 622f  om '@jupyterlab/
-000001c0: 6365 6c6c 7327 0a69 6d70 6f72 7420 7b20  cells'.import { 
-000001d0: 4953 6574 7469 6e67 5265 6769 7374 7279  ISettingRegistry
-000001e0: 207d 2066 726f 6d20 2740 6a75 7079 7465   } from '@jupyte
-000001f0: 726c 6162 2f73 6574 7469 6e67 7265 6769  rlab/settingregi
-00000200: 7374 7279 270a 0a69 6d70 6f72 7420 7b20  stry'..import { 
-00000210: 4944 6973 706f 7361 626c 652c 2044 6973  IDisposable, Dis
-00000220: 706f 7361 626c 6544 656c 6567 6174 6520  posableDelegate 
-00000230: 7d20 6672 6f6d 2027 406c 756d 696e 6f2f  } from '@lumino/
-00000240: 6469 7370 6f73 6162 6c65 270a 696d 706f  disposable'.impo
-00000250: 7274 207b 2044 6f63 756d 656e 7452 6567  rt { DocumentReg
-00000260: 6973 7472 7920 7d20 6672 6f6d 2027 406a  istry } from '@j
-00000270: 7570 7974 6572 6c61 622f 646f 6372 6567  upyterlab/docreg
-00000280: 6973 7472 7927 0a69 6d70 6f72 7420 7b20  istry'.import { 
-00000290: 546f 6f6c 6261 7242 7574 746f 6e20 7d20  ToolbarButton } 
-000002a0: 6672 6f6d 2027 406a 7570 7974 6572 6c61  from '@jupyterla
-000002b0: 622f 6170 7075 7469 6c73 270a 0a69 6d70  b/apputils'..imp
-000002c0: 6f72 7420 7b0a 2020 6d64 5f67 6574 2c0a  ort {.  md_get,.
-000002d0: 2020 6d64 5f75 6e73 6574 2c0a 2020 6d64    md_unset,.  md
-000002e0: 5f74 6f67 676c 652c 0a20 206d 645f 746f  _toggle,.  md_to
-000002f0: 6767 6c65 5f6d 756c 7469 2c0a 7d20 6672  ggle_multi,.} fr
-00000300: 6f6d 2027 6a75 7079 7465 726c 6162 2d63  om 'jupyterlab-c
-00000310: 656c 6c74 6167 7363 6c61 7373 6573 270a  elltagsclasses'.
-00000320: 696d 706f 7274 207b 2053 636f 7065 2c20  import { Scope, 
-00000330: 6170 706c 795f 6f6e 5f63 656c 6c73 207d  apply_on_cells }
-00000340: 2066 726f 6d20 276a 7570 7974 6572 6c61   from 'jupyterla
-00000350: 622d 6365 6c6c 7461 6773 636c 6173 7365  b-celltagsclasse
-00000360: 7327 0a0a 696d 706f 7274 207b 2074 6f67  s'..import { tog
-00000370: 676c 655f 6164 6d6f 6e69 7469 6f6e 207d  gle_admonition }
-00000380: 2066 726f 6d20 272e 2f61 646d 6f6e 6974   from './admonit
-00000390: 696f 6e73 270a 0a63 6f6e 7374 2050 4c55  ions'..const PLU
-000003a0: 4749 4e5f 4944 203d 2027 6a75 7079 7465  GIN_ID = 'jupyte
-000003b0: 726c 6162 2d63 6f75 7273 656c 6576 656c  rlab-courselevel
-000003c0: 733a 706c 7567 696e 270a 0a2f 2f20 6d64  s:plugin'..// md
-000003d0: 5f63 6c65 616e 206d 6179 2062 6520 6272  _clean may be br
-000003e0: 6f6b 656e 0a2f 2f20 696d 706f 7274 207b  oken.// import {
-000003f0: 206d 645f 7365 742c 202c 206d 645f 696e   md_set, , md_in
-00000400: 7365 7274 2c20 6d64 5f72 656d 6f76 6520  sert, md_remove 
-00000410: 7d20 6672 6f6d 2027 6a75 7079 7465 726c  } from 'jupyterl
-00000420: 6162 2d63 656c 6c74 6167 7363 6c61 7373  ab-celltagsclass
-00000430: 6573 270a 0a63 6f6e 7374 2063 6c65 616e  es'..const clean
-00000440: 5f63 656c 6c5f 6d65 7461 6461 7461 203d  _cell_metadata =
-00000450: 2028 6365 6c6c 3a20 4365 6c6c 2920 3d3e   (cell: Cell) =>
-00000460: 207b 0a20 2063 6f6e 736f 6c65 2e6c 6f67   {.  console.log
-00000470: 2827 436c 6561 6e69 6e67 206d 6574 6164  ('Cleaning metad
-00000480: 6174 6120 666f 7220 6365 6c6c 272c 2063  ata for cell', c
-00000490: 656c 6c29 0a20 2063 6f6e 7374 2065 6469  ell).  const edi
-000004a0: 7461 626c 6520 3d20 6365 6c6c 2e6d 6f64  table = cell.mod
-000004b0: 656c 2e67 6574 4d65 7461 6461 7461 2827  el.getMetadata('
-000004c0: 6564 6974 6162 6c65 2729 0a20 2069 6620  editable').  if 
-000004d0: 2865 6469 7461 626c 6520 3d3d 3d20 7472  (editable === tr
-000004e0: 7565 2920 7b0a 2020 2020 6d64 5f75 6e73  ue) {.    md_uns
-000004f0: 6574 2863 656c 6c2c 2027 6564 6974 6162  et(cell, 'editab
-00000500: 6c65 2729 0a20 207d 0a20 2063 6f6e 7374  le').  }.  const
-00000510: 2074 6167 7320 3d20 6365 6c6c 2e6d 6f64   tags = cell.mod
-00000520: 656c 2e67 6574 4d65 7461 6461 7461 2827  el.getMetadata('
-00000530: 7461 6773 2729 0a20 2069 6620 2874 6167  tags').  if (tag
-00000540: 733f 2e6c 656e 6774 6820 3d3d 3d20 3029  s?.length === 0)
-00000550: 207b 0a20 2020 206d 645f 756e 7365 7428   {.    md_unset(
-00000560: 6365 6c6c 2c20 2774 6167 7327 290a 2020  cell, 'tags').  
-00000570: 7d0a 2020 636f 6e73 7420 736c 6964 655f  }.  const slide_
-00000580: 7479 7065 203d 206d 645f 6765 7428 6365  type = md_get(ce
-00000590: 6c6c 2c20 2773 6c69 6465 7368 6f77 2e73  ll, 'slideshow.s
-000005a0: 6c69 6465 5f74 7970 6527 290a 2020 6966  lide_type').  if
-000005b0: 2028 736c 6964 655f 7479 7065 203d 3d3d   (slide_type ===
-000005c0: 2027 2729 207b 0a20 2020 206d 645f 756e   '') {.    md_un
-000005d0: 7365 7428 6365 6c6c 2c20 2773 6c69 6465  set(cell, 'slide
-000005e0: 7368 6f77 2e73 6c69 6465 5f74 7970 6527  show.slide_type'
-000005f0: 290a 2020 7d0a 2020 636f 6e73 7420 736c  ).  }.  const sl
-00000600: 6964 6573 686f 7720 3d20 6d64 5f67 6574  ideshow = md_get
-00000610: 2863 656c 6c2c 2027 736c 6964 6573 686f  (cell, 'slidesho
-00000620: 7727 290a 2020 6966 2028 736c 6964 6573  w').  if (slides
-00000630: 686f 7720 213d 3d20 756e 6465 6669 6e65  how !== undefine
-00000640: 6420 2626 204a 534f 4e2e 7374 7269 6e67  d && JSON.string
-00000650: 6966 7928 736c 6964 6573 686f 7729 203d  ify(slideshow) =
-00000660: 3d3d 2027 7b7d 2729 207b 0a20 2020 206d  == '{}') {.    m
-00000670: 645f 756e 7365 7428 6365 6c6c 2c20 2773  d_unset(cell, 's
-00000680: 6c69 6465 7368 6f77 2729 0a20 207d 0a20  lideshow').  }. 
-00000690: 2063 6f6e 7374 2075 7365 725f 6578 7072   const user_expr
-000006a0: 6573 7369 6f6e 7320 3d20 6d64 5f67 6574  essions = md_get
-000006b0: 2863 656c 6c2c 2027 7573 6572 5f65 7870  (cell, 'user_exp
-000006c0: 7265 7373 696f 6e73 2729 0a20 2069 6620  ressions').  if 
-000006d0: 2875 7365 725f 6578 7072 6573 7369 6f6e  (user_expression
-000006e0: 733f 2e6c 656e 6774 6820 3d3d 3d20 3029  s?.length === 0)
-000006f0: 207b 0a20 2020 206d 645f 756e 7365 7428   {.    md_unset(
-00000700: 6365 6c6c 2c20 2775 7365 725f 6578 7072  cell, 'user_expr
-00000710: 6573 7369 6f6e 7327 290a 2020 7d0a 7d0a  essions').  }.}.
-00000720: 0a63 6f6e 7374 2041 4c4c 5f4c 4556 454c  .const ALL_LEVEL
-00000730: 5320 3d20 5b27 6261 7369 6327 2c20 2769  S = ['basic', 'i
-00000740: 6e74 6572 6d65 6469 6174 6527 2c20 2761  ntermediate', 'a
-00000750: 6476 616e 6365 6427 5d0a 636f 6e73 7420  dvanced'].const 
-00000760: 706c 7567 696e 3a20 4a75 7079 7465 7246  plugin: JupyterF
-00000770: 726f 6e74 456e 6450 6c75 6769 6e3c 766f  rontEndPlugin<vo
-00000780: 6964 3e20 3d20 7b0a 2020 6964 3a20 504c  id> = {.  id: PL
-00000790: 5547 494e 5f49 442c 0a20 2061 7574 6f53  UGIN_ID,.  autoS
-000007a0: 7461 7274 3a20 7472 7565 2c0a 2020 7265  tart: true,.  re
-000007b0: 7175 6972 6573 3a20 5b49 436f 6d6d 616e  quires: [IComman
-000007c0: 6450 616c 6574 7465 2c20 494e 6f74 6562  dPalette, INoteb
-000007d0: 6f6f 6b54 7261 636b 6572 2c20 4953 6574  ookTracker, ISet
-000007e0: 7469 6e67 5265 6769 7374 7279 5d2c 0a20  tingRegistry],. 
-000007f0: 2061 6374 6976 6174 653a 2028 0a20 2020   activate: (.   
-00000800: 2061 7070 3a20 4a75 7079 7465 7246 726f   app: JupyterFro
-00000810: 6e74 456e 642c 0a20 2020 2070 616c 6574  ntEnd,.    palet
-00000820: 7465 3a20 4943 6f6d 6d61 6e64 5061 6c65  te: ICommandPale
-00000830: 7474 652c 0a20 2020 206e 6f74 6562 6f6f  tte,.    noteboo
-00000840: 6b54 7261 636b 6572 3a20 494e 6f74 6562  kTracker: INoteb
-00000850: 6f6f 6b54 7261 636b 6572 2c0a 2020 2020  ookTracker,.    
-00000860: 7365 7474 696e 6752 6567 6973 7472 793a  settingRegistry:
-00000870: 2049 5365 7474 696e 6752 6567 6973 7472   ISettingRegistr
-00000880: 790a 2020 2920 3d3e 207b 0a20 2020 2063  y.  ) => {.    c
-00000890: 6f6e 736f 6c65 2e6c 6f67 2827 6578 7465  onsole.log('exte
-000008a0: 6e73 696f 6e20 6a75 7079 7465 726c 6162  nsion jupyterlab
-000008b0: 2d63 6f75 7273 656c 6576 656c 7320 6973  -courselevels is
-000008c0: 2061 6374 6976 6174 696e 6727 290a 2020   activating').  
-000008d0: 2020 2f2f 2068 7474 7073 3a2f 2f6c 756d    // https://lum
-000008e0: 696e 6f2e 7265 6164 7468 6564 6f63 732e  ino.readthedocs.
-000008f0: 696f 2f65 6e2f 312e 782f 6170 692f 636f  io/en/1.x/api/co
-00000900: 6d6d 616e 6473 2f69 6e74 6572 6661 6365  mmands/interface
-00000910: 732f 636f 6d6d 616e 6472 6567 6973 7472  s/commandregistr
-00000920: 792e 696b 6579 6269 6e64 696e 676f 7074  y.ikeybindingopt
-00000930: 696f 6e73 2e68 746d 6c0a 2020 2020 2f2f  ions.html.    //
-00000940: 2054 6865 2073 7570 706f 7274 6564 206d   The supported m
-00000950: 6f64 6966 6965 7273 2061 7265 3a20 4163  odifiers are: Ac
-00000960: 6365 6c2c 2041 6c74 2c20 436d 642c 2043  cel, Alt, Cmd, C
-00000970: 7472 6c2c 2061 6e64 2053 6869 6674 2e20  trl, and Shift. 
-00000980: 5468 6520 4163 6365 6c0a 2020 2020 2f2f  The Accel.    //
-00000990: 206d 6f64 6966 6965 7220 6973 2074 7261   modifier is tra
-000009a0: 6e73 6c61 7465 6420 746f 2043 6d64 206f  nslated to Cmd o
-000009b0: 6e20 4d61 6320 616e 6420 4374 726c 206f  n Mac and Ctrl o
-000009c0: 6e20 616c 6c20 6f74 6865 7220 706c 6174  n all other plat
-000009d0: 666f 726d 732e 2054 6865 0a20 2020 202f  forms. The.    /
-000009e0: 2f20 436d 6420 6d6f 6469 6669 6572 2069  / Cmd modifier i
-000009f0: 7320 6967 6e6f 7265 6420 6f6e 206e 6f6e  s ignored on non
-00000a00: 2d4d 6163 2070 6c61 7466 6f72 6d73 2e0a  -Mac platforms..
-00000a10: 2020 2020 2f2f 2041 6c74 2069 7320 6f70      // Alt is op
-00000a20: 7469 6f6e 206f 6e20 6d61 630a 0a20 2020  tion on mac..   
-00000a30: 206c 6574 205b 7368 6f77 5f6c 6576 656c   let [show_level
-00000a40: 5f62 7574 746f 6e73 5d20 3d20 5b66 616c  _buttons] = [fal
-00000a50: 7365 5d0a 0a20 2020 2063 6f6e 7374 2041  se]..    const A
-00000a60: 4c4c 5f46 554c 4c5f 4c45 5645 4c53 203d  LL_FULL_LEVELS =
-00000a70: 2041 4c4c 5f4c 4556 454c 532e 6d61 7028   ALL_LEVELS.map(
-00000a80: 286c 6576 656c 2920 3d3e 2060 6c65 7665  (level) => `leve
-00000a90: 6c5f 247b 6c65 7665 6c7d 6029 0a0a 2020  l_${level}`)..  
-00000aa0: 2020 636f 6e73 7420 6365 6c6c 5f74 6f67    const cell_tog
-00000ab0: 676c 655f 6c65 7665 6c20 3d20 2863 656c  gle_level = (cel
-00000ac0: 6c3a 2043 656c 6c2c 206c 6576 656c 3a20  l: Cell, level: 
-00000ad0: 7374 7269 6e67 293a 2076 6f69 6420 3d3e  string): void =>
-00000ae0: 207b 0a20 2020 2020 2063 6f6e 7374 2066   {.      const f
-00000af0: 756c 6c5f 6c65 7665 6c20 3d20 606c 6576  ull_level = `lev
-00000b00: 656c 5f24 7b6c 6576 656c 7d60 0a20 2020  el_${level}`.   
-00000b10: 2020 2072 6574 7572 6e20 6d64 5f74 6f67     return md_tog
-00000b20: 676c 655f 6d75 6c74 6928 6365 6c6c 2c20  gle_multi(cell, 
-00000b30: 2774 6167 7327 2c20 6675 6c6c 5f6c 6576  'tags', full_lev
-00000b40: 656c 2c20 414c 4c5f 4655 4c4c 5f4c 4556  el, ALL_FULL_LEV
-00000b50: 454c 5329 0a20 2020 207d 0a0a 2020 2020  ELS).    }..    
-00000b60: 636f 6e73 7420 746f 6767 6c65 5f6c 6576  const toggle_lev
-00000b70: 656c 203d 2028 6c65 7665 6c3a 2073 7472  el = (level: str
-00000b80: 696e 6729 203d 3e20 7b0a 2020 2020 2020  ing) => {.      
-00000b90: 6170 706c 795f 6f6e 5f63 656c 6c73 286e  apply_on_cells(n
-00000ba0: 6f74 6562 6f6f 6b54 7261 636b 6572 2c20  otebookTracker, 
-00000bb0: 5363 6f70 652e 4163 7469 7665 2c20 2863  Scope.Active, (c
-00000bc0: 656c 6c3a 2043 656c 6c29 203d 3e20 7b0a  ell: Cell) => {.
-00000bd0: 2020 2020 2020 2020 6365 6c6c 5f74 6f67          cell_tog
-00000be0: 676c 655f 6c65 7665 6c28 6365 6c6c 2c20  gle_level(cell, 
-00000bf0: 6c65 7665 6c29 0a20 2020 2020 207d 290a  level).      }).
-00000c00: 2020 2020 7d0a 0a20 2020 206c 6574 2063      }..    let c
-00000c10: 6f6d 6d61 6e64 0a0a 2020 2020 666f 7220  ommand..    for 
-00000c20: 2863 6f6e 7374 205b 6c65 7665 6c2c 206b  (const [level, k
-00000c30: 6579 5d20 6f66 205b 0a20 2020 2020 205b  ey] of [.      [
-00000c40: 2762 6173 6963 272c 2027 4374 726c 2058  'basic', 'Ctrl X
-00000c50: 275d 2c0a 2020 2020 2020 5b27 696e 7465  '],.      ['inte
-00000c60: 726d 6564 6961 7465 272c 2027 4374 726c  rmediate', 'Ctrl
-00000c70: 2059 275d 2c0a 2020 2020 2020 5b27 6164   Y'],.      ['ad
-00000c80: 7661 6e63 6564 272c 2027 4374 726c 205a  vanced', 'Ctrl Z
-00000c90: 275d 0a20 2020 205d 2920 7b0a 2020 2020  '].    ]) {.    
-00000ca0: 2020 636f 6d6d 616e 6420 3d20 6063 6f75    command = `cou
-00000cb0: 7273 656c 6576 656c 733a 746f 6767 6c65  rselevels:toggle
-00000cc0: 2d6c 6576 656c 2d24 7b6c 6576 656c 7d60  -level-${level}`
-00000cd0: 0a20 2020 2020 2061 7070 2e63 6f6d 6d61  .      app.comma
-00000ce0: 6e64 732e 6164 6443 6f6d 6d61 6e64 2863  nds.addCommand(c
-00000cf0: 6f6d 6d61 6e64 2c20 7b0a 2020 2020 2020  ommand, {.      
-00000d00: 2020 6c61 6265 6c3a 2060 746f 6767 6c65    label: `toggle
-00000d10: 2024 7b6c 6576 656c 7d20 6c65 7665 6c60   ${level} level`
-00000d20: 2c0a 2020 2020 2020 2020 6578 6563 7574  ,.        execut
-00000d30: 653a 2028 2920 3d3e 2074 6f67 676c 655f  e: () => toggle_
-00000d40: 6c65 7665 6c28 6c65 7665 6c29 0a20 2020  level(level).   
-00000d50: 2020 207d 290a 2020 2020 2020 7061 6c65     }).      pale
-00000d60: 7474 652e 6164 6449 7465 6d28 7b20 636f  tte.addItem({ co
-00000d70: 6d6d 616e 642c 2063 6174 6567 6f72 793a  mmand, category:
-00000d80: 2027 636f 7572 7365 6c65 7665 6c73 2720   'courselevels' 
-00000d90: 7d29 0a20 2020 2020 2061 7070 2e63 6f6d  }).      app.com
-00000da0: 6d61 6e64 732e 6164 644b 6579 4269 6e64  mands.addKeyBind
-00000db0: 696e 6728 7b0a 2020 2020 2020 2020 636f  ing({.        co
-00000dc0: 6d6d 616e 642c 0a20 2020 2020 2020 206b  mmand,.        k
-00000dd0: 6579 733a 205b 2743 7472 6c20 5c5c 272c  eys: ['Ctrl \\',
-00000de0: 206b 6579 5d2c 0a20 2020 2020 2020 2073   key],.        s
-00000df0: 656c 6563 746f 723a 2027 2e6a 702d 4e6f  elector: '.jp-No
-00000e00: 7465 626f 6f6b 270a 2020 2020 2020 7d29  tebook'.      })
-00000e10: 0a20 2020 207d 0a0a 2020 2020 636f 6e73  .    }..    cons
-00000e20: 7420 746f 6767 6c65 5f66 7261 6d65 203d  t toggle_frame =
-00000e30: 2028 2920 3d3e 207b 0a20 2020 2020 2061   () => {.      a
-00000e40: 7070 6c79 5f6f 6e5f 6365 6c6c 7328 6e6f  pply_on_cells(no
-00000e50: 7465 626f 6f6b 5472 6163 6b65 722c 2053  tebookTracker, S
-00000e60: 636f 7065 2e41 6374 6976 652c 2028 6365  cope.Active, (ce
-00000e70: 6c6c 3a20 4365 6c6c 2920 3d3e 207b 0a20  ll: Cell) => {. 
-00000e80: 2020 2020 2020 206d 645f 746f 6767 6c65         md_toggle
-00000e90: 2863 656c 6c2c 2027 7461 6773 272c 2027  (cell, 'tags', '
-00000ea0: 6672 616d 6564 5f63 656c 6c27 290a 2020  framed_cell').  
-00000eb0: 2020 2020 7d29 0a20 2020 207d 0a0a 2020      }).    }..  
-00000ec0: 2020 636f 6d6d 616e 6420 3d20 2763 6f75    command = 'cou
-00000ed0: 7273 656c 6576 656c 733a 746f 6767 6c65  rselevels:toggle
-00000ee0: 2d66 7261 6d65 270a 2020 2020 6170 702e  -frame'.    app.
-00000ef0: 636f 6d6d 616e 6473 2e61 6464 436f 6d6d  commands.addComm
-00000f00: 616e 6428 636f 6d6d 616e 642c 207b 0a20  and(command, {. 
-00000f10: 2020 2020 206c 6162 656c 3a20 2774 6f67       label: 'tog
-00000f20: 676c 6520 6672 616d 6527 2c0a 2020 2020  gle frame',.    
-00000f30: 2020 6578 6563 7574 653a 2028 2920 3d3e    execute: () =>
-00000f40: 2074 6f67 676c 655f 6672 616d 6528 290a   toggle_frame().
-00000f50: 2020 2020 7d29 0a20 2020 2070 616c 6574      }).    palet
-00000f60: 7465 2e61 6464 4974 656d 287b 2063 6f6d  te.addItem({ com
-00000f70: 6d61 6e64 2c20 6361 7465 676f 7279 3a20  mand, category: 
-00000f80: 2763 6f75 7273 656c 6576 656c 7327 207d  'courselevels' }
-00000f90: 290a 2020 2020 6170 702e 636f 6d6d 616e  ).    app.comman
-00000fa0: 6473 2e61 6464 4b65 7942 696e 6469 6e67  ds.addKeyBinding
-00000fb0: 287b 0a20 2020 2020 2063 6f6d 6d61 6e64  ({.      command
-00000fc0: 2c0a 2020 2020 2020 6b65 7973 3a20 5b27  ,.      keys: ['
-00000fd0: 4374 726c 205c 5c27 2c20 2743 7472 6c20  Ctrl \\', 'Ctrl 
-00000fe0: 4d27 5d2c 0a20 2020 2020 2073 656c 6563  M'],.      selec
-00000ff0: 746f 723a 2027 2e6a 702d 4e6f 7465 626f  tor: '.jp-Notebo
-00001000: 6f6b 270a 2020 2020 7d29 0a0a 2020 2020  ok'.    })..    
-00001010: 636f 6e73 7420 746f 6767 6c65 5f6c 6963  const toggle_lic
-00001020: 656e 6365 203d 2028 2920 3d3e 207b 0a20  ence = () => {. 
-00001030: 2020 2020 2061 7070 6c79 5f6f 6e5f 6365       apply_on_ce
-00001040: 6c6c 7328 6e6f 7465 626f 6f6b 5472 6163  lls(notebookTrac
-00001050: 6b65 722c 2053 636f 7065 2e41 6374 6976  ker, Scope.Activ
-00001060: 652c 2028 6365 6c6c 3a20 4365 6c6c 2920  e, (cell: Cell) 
-00001070: 3d3e 207b 0a20 2020 2020 2020 206d 645f  => {.        md_
-00001080: 746f 6767 6c65 2863 656c 6c2c 2027 7461  toggle(cell, 'ta
-00001090: 6773 272c 2027 6c69 6365 6e63 6527 290a  gs', 'licence').
-000010a0: 2020 2020 2020 7d29 0a20 2020 207d 0a0a        }).    }..
-000010b0: 2020 2020 636f 6d6d 616e 6420 3d20 2763      command = 'c
-000010c0: 6f75 7273 656c 6576 656c 733a 746f 6767  ourselevels:togg
-000010d0: 6c65 2d6c 6963 656e 6365 270a 2020 2020  le-licence'.    
-000010e0: 6170 702e 636f 6d6d 616e 6473 2e61 6464  app.commands.add
-000010f0: 436f 6d6d 616e 6428 636f 6d6d 616e 642c  Command(command,
-00001100: 207b 0a20 2020 2020 206c 6162 656c 3a20   {.      label: 
-00001110: 2774 6f67 676c 6520 6c69 6365 6e63 6527  'toggle licence'
-00001120: 2c0a 2020 2020 2020 6578 6563 7574 653a  ,.      execute:
-00001130: 2028 2920 3d3e 2074 6f67 676c 655f 6c69   () => toggle_li
-00001140: 6365 6e63 6528 290a 2020 2020 7d29 0a20  cence().    }). 
-00001150: 2020 2070 616c 6574 7465 2e61 6464 4974     palette.addIt
-00001160: 656d 287b 2063 6f6d 6d61 6e64 2c20 6361  em({ command, ca
-00001170: 7465 676f 7279 3a20 2763 6f75 7273 656c  tegory: 'coursel
-00001180: 6576 656c 7327 207d 290a 2020 2020 6170  evels' }).    ap
-00001190: 702e 636f 6d6d 616e 6473 2e61 6464 4b65  p.commands.addKe
-000011a0: 7942 696e 6469 6e67 287b 0a20 2020 2020  yBinding({.     
-000011b0: 2063 6f6d 6d61 6e64 2c0a 2020 2020 2020   command,.      
-000011c0: 6b65 7973 3a20 5b27 4374 726c 205c 5c27  keys: ['Ctrl \\'
-000011d0: 2c20 2743 7472 6c20 4c27 5d2c 0a20 2020  , 'Ctrl L'],.   
-000011e0: 2020 2073 656c 6563 746f 723a 2027 2e6a     selector: '.j
-000011f0: 702d 4e6f 7465 626f 6f6b 270a 2020 2020  p-Notebook'.    
-00001200: 7d29 0a0a 2020 2020 636f 6d6d 616e 6420  })..    command 
-00001210: 3d20 2763 6f75 7273 656c 6576 656c 733a  = 'courselevels:
-00001220: 6d65 7461 6461 7461 2d63 6c65 616e 2d73  metadata-clean-s
-00001230: 656c 6563 7465 6427 0a20 2020 2061 7070  elected'.    app
-00001240: 2e63 6f6d 6d61 6e64 732e 6164 6443 6f6d  .commands.addCom
-00001250: 6d61 6e64 2863 6f6d 6d61 6e64 2c20 7b0a  mand(command, {.
-00001260: 2020 2020 2020 6c61 6265 6c3a 2027 636c        label: 'cl
-00001270: 6561 6e20 6d65 7461 6461 7461 2066 6f72  ean metadata for
-00001280: 2061 6c6c 2073 656c 6563 7465 6420 6365   all selected ce
-00001290: 6c6c 7327 2c0a 2020 2020 2020 6578 6563  lls',.      exec
-000012a0: 7574 653a 2028 2920 3d3e 0a20 2020 2020  ute: () =>.     
-000012b0: 2020 2061 7070 6c79 5f6f 6e5f 6365 6c6c     apply_on_cell
-000012c0: 7328 6e6f 7465 626f 6f6b 5472 6163 6b65  s(notebookTracke
-000012d0: 722c 2053 636f 7065 2e4d 756c 7469 706c  r, Scope.Multipl
-000012e0: 652c 2063 6c65 616e 5f63 656c 6c5f 6d65  e, clean_cell_me
-000012f0: 7461 6461 7461 290a 2020 2020 7d29 0a20  tadata).    }). 
-00001300: 2020 2070 616c 6574 7465 2e61 6464 4974     palette.addIt
-00001310: 656d 287b 2063 6f6d 6d61 6e64 2c20 6361  em({ command, ca
-00001320: 7465 676f 7279 3a20 2763 6f75 7273 656c  tegory: 'coursel
-00001330: 6576 656c 7327 207d 290a 2020 2020 6170  evels' }).    ap
-00001340: 702e 636f 6d6d 616e 6473 2e61 6464 4b65  p.commands.addKe
-00001350: 7942 696e 6469 6e67 287b 0a20 2020 2020  yBinding({.     
-00001360: 2063 6f6d 6d61 6e64 2c0a 2020 2020 2020   command,.      
-00001370: 6b65 7973 3a20 5b27 416c 7420 436d 6420  keys: ['Alt Cmd 
-00001380: 3727 5d2c 0a20 2020 2020 2073 656c 6563  7'],.      selec
-00001390: 746f 723a 2027 2e6a 702d 4e6f 7465 626f  tor: '.jp-Notebo
-000013a0: 6f6b 270a 2020 2020 7d29 0a0a 2020 2020  ok'.    })..    
-000013b0: 636f 6d6d 616e 6420 3d20 2763 6f75 7273  command = 'cours
-000013c0: 656c 6576 656c 733a 6d65 7461 6461 7461  elevels:metadata
-000013d0: 2d63 6c65 616e 2d61 6c6c 270a 2020 2020  -clean-all'.    
-000013e0: 6170 702e 636f 6d6d 616e 6473 2e61 6464  app.commands.add
-000013f0: 436f 6d6d 616e 6428 636f 6d6d 616e 642c  Command(command,
-00001400: 207b 0a20 2020 2020 206c 6162 656c 3a20   {.      label: 
-00001410: 2763 6c65 616e 206d 6574 6164 6174 6120  'clean metadata 
-00001420: 666f 7220 616c 6c20 6365 6c6c 7327 2c0a  for all cells',.
-00001430: 2020 2020 2020 6578 6563 7574 653a 2028        execute: (
-00001440: 2920 3d3e 0a20 2020 2020 2020 2061 7070  ) =>.        app
-00001450: 6c79 5f6f 6e5f 6365 6c6c 7328 6e6f 7465  ly_on_cells(note
-00001460: 626f 6f6b 5472 6163 6b65 722c 2053 636f  bookTracker, Sco
-00001470: 7065 2e41 6c6c 2c20 636c 6561 6e5f 6365  pe.All, clean_ce
-00001480: 6c6c 5f6d 6574 6164 6174 6129 0a20 2020  ll_metadata).   
-00001490: 207d 290a 2020 2020 7061 6c65 7474 652e   }).    palette.
-000014a0: 6164 6449 7465 6d28 7b20 636f 6d6d 616e  addItem({ comman
-000014b0: 642c 2063 6174 6567 6f72 793a 2027 636f  d, category: 'co
-000014c0: 7572 7365 6c65 7665 6c73 2720 7d29 0a20  urselevels' }). 
-000014d0: 2020 2061 7070 2e63 6f6d 6d61 6e64 732e     app.commands.
-000014e0: 6164 644b 6579 4269 6e64 696e 6728 7b0a  addKeyBinding({.
-000014f0: 2020 2020 2020 636f 6d6d 616e 642c 0a20        command,. 
-00001500: 2020 2020 206b 6579 733a 205b 2743 7472       keys: ['Ctr
-00001510: 6c20 416c 7420 3727 5d2c 0a20 2020 2020  l Alt 7'],.     
-00001520: 2073 656c 6563 746f 723a 2027 2e6a 702d   selector: '.jp-
-00001530: 4e6f 7465 626f 6f6b 270a 2020 2020 7d29  Notebook'.    })
-00001540: 0a0a 2020 2020 2f2f 2074 6865 2062 7574  ..    // the but
-00001550: 746f 6e73 2069 6e20 7468 6520 746f 6f6c  tons in the tool
-00001560: 6261 720a 2020 2020 636f 6e73 7420 6372  bar.    const cr
-00001570: 6561 7465 5f6c 6576 656c 5f62 7574 746f  eate_level_butto
-00001580: 6e73 203d 2028 2920 3d3e 207b 0a20 2020  ns = () => {.   
-00001590: 2020 2063 6f6e 7374 2066 696e 645f 7370     const find_sp
-000015a0: 6163 6572 203d 2028 7061 6e65 6c3a 204e  acer = (panel: N
-000015b0: 6f74 6562 6f6f 6b50 616e 656c 293a 206e  otebookPanel): n
-000015c0: 756d 6265 7220 3d3e 207b 0a20 2020 2020  umber => {.     
-000015d0: 2020 206c 6574 2069 6e64 6578 203d 2030     let index = 0
-000015e0: 0a20 2020 2020 2020 2066 6f72 2028 636f  .        for (co
-000015f0: 6e73 7420 6368 696c 6420 6f66 2070 616e  nst child of pan
-00001600: 656c 2e74 6f6f 6c62 6172 2e63 6869 6c64  el.toolbar.child
-00001610: 7265 6e28 2929 207b 0a20 2020 2020 2020  ren()) {.       
-00001620: 2020 2069 6620 2863 6869 6c64 2e6e 6f64     if (child.nod
-00001630: 652e 636c 6173 734c 6973 742e 636f 6e74  e.classList.cont
-00001640: 6169 6e73 2827 6a70 2d54 6f6f 6c62 6172  ains('jp-Toolbar
-00001650: 2d73 7061 6365 7227 2929 207b 0a20 2020  -spacer')) {.   
-00001660: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001670: 696e 6465 780a 2020 2020 2020 2020 2020  index.          
-00001680: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
-00001690: 2020 2020 2069 6e64 6578 202b 3d20 310a       index += 1.
-000016a0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000016b0: 2020 2020 7d0a 2020 2020 2020 2020 7265      }.        re
-000016c0: 7475 726e 2030 0a20 2020 2020 207d 0a0a  turn 0.      }..
-000016d0: 2020 2020 2020 636c 6173 7320 4261 7369        class Basi
-000016e0: 6342 7574 746f 6e0a 2020 2020 2020 2020  cButton.        
-000016f0: 696d 706c 656d 656e 7473 0a20 2020 2020  implements.     
-00001700: 2020 2020 2044 6f63 756d 656e 7452 6567       DocumentReg
-00001710: 6973 7472 792e 4957 6964 6765 7445 7874  istry.IWidgetExt
-00001720: 656e 7369 6f6e 3c4e 6f74 6562 6f6f 6b50  ension<NotebookP
-00001730: 616e 656c 2c20 494e 6f74 6562 6f6f 6b4d  anel, INotebookM
-00001740: 6f64 656c 3e0a 2020 2020 2020 7b0a 2020  odel>.      {.  
-00001750: 2020 2020 2020 6372 6561 7465 4e65 7728        createNew(
-00001760: 0a20 2020 2020 2020 2020 2070 616e 656c  .          panel
-00001770: 3a20 4e6f 7465 626f 6f6b 5061 6e65 6c2c  : NotebookPanel,
-00001780: 0a20 2020 2020 2020 2020 2063 6f6e 7465  .          conte
-00001790: 7874 3a20 446f 6375 6d65 6e74 5265 6769  xt: DocumentRegi
-000017a0: 7374 7279 2e49 436f 6e74 6578 743c 494e  stry.IContext<IN
-000017b0: 6f74 6562 6f6f 6b4d 6f64 656c 3e0a 2020  otebookModel>.  
-000017c0: 2020 2020 2020 293a 2049 4469 7370 6f73        ): IDispos
-000017d0: 6162 6c65 207b 0a20 2020 2020 2020 2020  able {.         
-000017e0: 2063 6f6e 7374 2062 7574 746f 6e20 3d20   const button = 
-000017f0: 6e65 7720 546f 6f6c 6261 7242 7574 746f  new ToolbarButto
-00001800: 6e28 7b0a 2020 2020 2020 2020 2020 2020  n({.            
-00001810: 636c 6173 734e 616d 653a 2027 636f 7572  className: 'cour
-00001820: 7365 6c65 7665 6c73 2d62 7574 746f 6e27  selevels-button'
-00001830: 2c0a 2020 2020 2020 2020 2020 2020 6963  ,.            ic
-00001840: 6f6e 436c 6173 733a 2027 6661 7220 6661  onClass: 'far fa
-00001850: 2d68 616e 642d 706f 696e 7465 7227 2c0a  -hand-pointer',.
-00001860: 2020 2020 2020 2020 2020 2020 6f6e 436c              onCl
-00001870: 6963 6b3a 2028 2920 3d3e 2074 6f67 676c  ick: () => toggl
-00001880: 655f 6c65 7665 6c28 2762 6173 6963 2729  e_level('basic')
-00001890: 2c0a 2020 2020 2020 2020 2020 2020 746f  ,.            to
-000018a0: 6f6c 7469 703a 2027 546f 6767 6c65 2062  oltip: 'Toggle b
-000018b0: 6173 6963 206c 6576 656c 270a 2020 2020  asic level'.    
-000018c0: 2020 2020 2020 7d29 0a20 2020 2020 2020        }).       
-000018d0: 2020 202f 2f20 636f 6d70 7574 6520 7768     // compute wh
-000018e0: 6572 6520 746f 2069 6e73 6572 7420 6974  ere to insert it
-000018f0: 0a20 2020 2020 2020 2020 2063 6f6e 7374  .          const
-00001900: 2069 6e64 6578 203d 2066 696e 645f 7370   index = find_sp
-00001910: 6163 6572 2870 616e 656c 290a 2020 2020  acer(panel).    
-00001920: 2020 2020 2020 7061 6e65 6c2e 746f 6f6c        panel.tool
-00001930: 6261 722e 696e 7365 7274 4974 656d 2869  bar.insertItem(i
-00001940: 6e64 6578 2c20 2762 6173 6963 4c65 7665  ndex, 'basicLeve
-00001950: 6c27 2c20 6275 7474 6f6e 290a 2020 2020  l', button).    
-00001960: 2020 2020 2020 7265 7475 726e 206e 6577        return new
-00001970: 2044 6973 706f 7361 626c 6544 656c 6567   DisposableDeleg
-00001980: 6174 6528 2829 203d 3e20 7b0a 2020 2020  ate(() => {.    
-00001990: 2020 2020 2020 2020 6275 7474 6f6e 2e64          button.d
-000019a0: 6973 706f 7365 2829 0a20 2020 2020 2020  ispose().       
-000019b0: 2020 207d 290a 2020 2020 2020 2020 7d0a     }).        }.
-000019c0: 2020 2020 2020 7d0a 2020 2020 2020 6170        }.      ap
-000019d0: 702e 646f 6352 6567 6973 7472 792e 6164  p.docRegistry.ad
-000019e0: 6457 6964 6765 7445 7874 656e 7369 6f6e  dWidgetExtension
-000019f0: 2827 4e6f 7465 626f 6f6b 272c 206e 6577  ('Notebook', new
-00001a00: 2042 6173 6963 4275 7474 6f6e 2829 290a   BasicButton()).
-00001a10: 0a20 2020 2020 2063 6c61 7373 2049 6e74  .      class Int
-00001a20: 6572 6d65 6469 6174 6542 7574 746f 6e0a  ermediateButton.
-00001a30: 2020 2020 2020 2020 696d 706c 656d 656e          implemen
-00001a40: 7473 0a20 2020 2020 2020 2020 2044 6f63  ts.          Doc
-00001a50: 756d 656e 7452 6567 6973 7472 792e 4957  umentRegistry.IW
-00001a60: 6964 6765 7445 7874 656e 7369 6f6e 3c4e  idgetExtension<N
-00001a70: 6f74 6562 6f6f 6b50 616e 656c 2c20 494e  otebookPanel, IN
-00001a80: 6f74 6562 6f6f 6b4d 6f64 656c 3e0a 2020  otebookModel>.  
-00001a90: 2020 2020 7b0a 2020 2020 2020 2020 6372      {.        cr
-00001aa0: 6561 7465 4e65 7728 0a20 2020 2020 2020  eateNew(.       
-00001ab0: 2020 2070 616e 656c 3a20 4e6f 7465 626f     panel: Notebo
-00001ac0: 6f6b 5061 6e65 6c2c 0a20 2020 2020 2020  okPanel,.       
-00001ad0: 2020 2063 6f6e 7465 7874 3a20 446f 6375     context: Docu
-00001ae0: 6d65 6e74 5265 6769 7374 7279 2e49 436f  mentRegistry.ICo
-00001af0: 6e74 6578 743c 494e 6f74 6562 6f6f 6b4d  ntext<INotebookM
-00001b00: 6f64 656c 3e0a 2020 2020 2020 2020 293a  odel>.        ):
-00001b10: 2049 4469 7370 6f73 6162 6c65 207b 0a20   IDisposable {. 
-00001b20: 2020 2020 2020 2020 2063 6f6e 7374 2062           const b
-00001b30: 7574 746f 6e20 3d20 6e65 7720 546f 6f6c  utton = new Tool
-00001b40: 6261 7242 7574 746f 6e28 7b0a 2020 2020  barButton({.    
-00001b50: 2020 2020 2020 2020 636c 6173 734e 616d          classNam
-00001b60: 653a 2027 636f 7572 7365 6c65 7665 6c73  e: 'courselevels
-00001b70: 2d62 7574 746f 6e27 2c0a 2020 2020 2020  -button',.      
-00001b80: 2020 2020 2020 6963 6f6e 436c 6173 733a        iconClass:
-00001b90: 2027 6661 7220 6661 2d68 616e 642d 7065   'far fa-hand-pe
-00001ba0: 6163 6527 2c0a 2020 2020 2020 2020 2020  ace',.          
-00001bb0: 2020 6f6e 436c 6963 6b3a 2028 2920 3d3e    onClick: () =>
-00001bc0: 2074 6f67 676c 655f 6c65 7665 6c28 2769   toggle_level('i
-00001bd0: 6e74 6572 6d65 6469 6174 6527 292c 0a20  ntermediate'),. 
-00001be0: 2020 2020 2020 2020 2020 2074 6f6f 6c74             toolt
-00001bf0: 6970 3a20 2754 6f67 676c 6520 696e 7465  ip: 'Toggle inte
-00001c00: 726d 6564 6961 7465 206c 6576 656c 270a  rmediate level'.
-00001c10: 2020 2020 2020 2020 2020 7d29 0a20 2020            }).   
-00001c20: 2020 2020 2020 202f 2f20 636f 6d70 7574         // comput
-00001c30: 6520 7768 6572 6520 746f 2069 6e73 6572  e where to inser
-00001c40: 7420 6974 0a20 2020 2020 2020 2020 2063  t it.          c
-00001c50: 6f6e 7374 2069 6e64 6578 203d 2066 696e  onst index = fin
-00001c60: 645f 7370 6163 6572 2870 616e 656c 290a  d_spacer(panel).
-00001c70: 2020 2020 2020 2020 2020 7061 6e65 6c2e            panel.
-00001c80: 746f 6f6c 6261 722e 696e 7365 7274 4974  toolbar.insertIt
-00001c90: 656d 2869 6e64 6578 2c20 2769 6e74 6572  em(index, 'inter
-00001ca0: 6d65 6469 6174 654c 6576 656c 272c 2062  mediateLevel', b
-00001cb0: 7574 746f 6e29 0a20 2020 2020 2020 2020  utton).         
-00001cc0: 2072 6574 7572 6e20 6e65 7720 4469 7370   return new Disp
-00001cd0: 6f73 6162 6c65 4465 6c65 6761 7465 2828  osableDelegate((
-00001ce0: 2920 3d3e 207b 0a20 2020 2020 2020 2020  ) => {.         
-00001cf0: 2020 2062 7574 746f 6e2e 6469 7370 6f73     button.dispos
-00001d00: 6528 290a 2020 2020 2020 2020 2020 7d29  e().          })
-00001d10: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00001d20: 207d 0a20 2020 2020 2061 7070 2e64 6f63   }.      app.doc
-00001d30: 5265 6769 7374 7279 2e61 6464 5769 6467  Registry.addWidg
-00001d40: 6574 4578 7465 6e73 696f 6e28 274e 6f74  etExtension('Not
-00001d50: 6562 6f6f 6b27 2c20 6e65 7720 496e 7465  ebook', new Inte
-00001d60: 726d 6564 6961 7465 4275 7474 6f6e 2829  rmediateButton()
-00001d70: 290a 0a20 2020 2020 2063 6c61 7373 2041  )..      class A
-00001d80: 6476 616e 6365 6442 7574 746f 6e0a 2020  dvancedButton.  
-00001d90: 2020 2020 2020 696d 706c 656d 656e 7473        implements
-00001da0: 0a20 2020 2020 2020 2020 2044 6f63 756d  .          Docum
-00001db0: 656e 7452 6567 6973 7472 792e 4957 6964  entRegistry.IWid
-00001dc0: 6765 7445 7874 656e 7369 6f6e 3c4e 6f74  getExtension<Not
-00001dd0: 6562 6f6f 6b50 616e 656c 2c20 494e 6f74  ebookPanel, INot
-00001de0: 6562 6f6f 6b4d 6f64 656c 3e0a 2020 2020  ebookModel>.    
-00001df0: 2020 7b0a 2020 2020 2020 2020 6372 6561    {.        crea
-00001e00: 7465 4e65 7728 0a20 2020 2020 2020 2020  teNew(.         
-00001e10: 2070 616e 656c 3a20 4e6f 7465 626f 6f6b   panel: Notebook
-00001e20: 5061 6e65 6c2c 0a20 2020 2020 2020 2020  Panel,.         
-00001e30: 2063 6f6e 7465 7874 3a20 446f 6375 6d65   context: Docume
-00001e40: 6e74 5265 6769 7374 7279 2e49 436f 6e74  ntRegistry.ICont
-00001e50: 6578 743c 494e 6f74 6562 6f6f 6b4d 6f64  ext<INotebookMod
-00001e60: 656c 3e0a 2020 2020 2020 2020 293a 2049  el>.        ): I
-00001e70: 4469 7370 6f73 6162 6c65 207b 0a20 2020  Disposable {.   
-00001e80: 2020 2020 2020 2063 6f6e 7374 2062 7574         const but
-00001e90: 746f 6e20 3d20 6e65 7720 546f 6f6c 6261  ton = new Toolba
-00001ea0: 7242 7574 746f 6e28 7b0a 2020 2020 2020  rButton({.      
-00001eb0: 2020 2020 2020 636c 6173 734e 616d 653a        className:
-00001ec0: 2027 636f 7572 7365 6c65 7665 6c73 2d62   'courselevels-b
-00001ed0: 7574 746f 6e27 2c0a 2020 2020 2020 2020  utton',.        
-00001ee0: 2020 2020 6963 6f6e 436c 6173 733a 2027      iconClass: '
-00001ef0: 6661 7220 6661 2d68 616e 642d 7370 6f63  far fa-hand-spoc
-00001f00: 6b27 2c0a 2020 2020 2020 2020 2020 2020  k',.            
-00001f10: 6f6e 436c 6963 6b3a 2028 2920 3d3e 2074  onClick: () => t
-00001f20: 6f67 676c 655f 6c65 7665 6c28 2761 6476  oggle_level('adv
-00001f30: 616e 6365 6427 292c 0a20 2020 2020 2020  anced'),.       
-00001f40: 2020 2020 2074 6f6f 6c74 6970 3a20 2754       tooltip: 'T
-00001f50: 6f67 676c 6520 6164 7661 6e63 6564 206c  oggle advanced l
-00001f60: 6576 656c 270a 2020 2020 2020 2020 2020  evel'.          
-00001f70: 7d29 0a20 2020 2020 2020 2020 202f 2f20  }).          // 
-00001f80: 636f 6d70 7574 6520 7768 6572 6520 746f  compute where to
-00001f90: 2069 6e73 6572 7420 6974 0a20 2020 2020   insert it.     
-00001fa0: 2020 2020 2063 6f6e 7374 2069 6e64 6578       const index
-00001fb0: 203d 2066 696e 645f 7370 6163 6572 2870   = find_spacer(p
-00001fc0: 616e 656c 290a 2020 2020 2020 2020 2020  anel).          
-00001fd0: 7061 6e65 6c2e 746f 6f6c 6261 722e 696e  panel.toolbar.in
-00001fe0: 7365 7274 4974 656d 2869 6e64 6578 2c20  sertItem(index, 
-00001ff0: 2761 6476 616e 6365 644c 6576 656c 272c  'advancedLevel',
-00002000: 2062 7574 746f 6e29 0a20 2020 2020 2020   button).       
-00002010: 2020 2072 6574 7572 6e20 6e65 7720 4469     return new Di
-00002020: 7370 6f73 6162 6c65 4465 6c65 6761 7465  sposableDelegate
-00002030: 2828 2920 3d3e 207b 0a20 2020 2020 2020  (() => {.       
-00002040: 2020 2020 2062 7574 746f 6e2e 6469 7370       button.disp
-00002050: 6f73 6528 290a 2020 2020 2020 2020 2020  ose().          
-00002060: 7d29 0a20 2020 2020 2020 207d 0a20 2020  }).        }.   
-00002070: 2020 207d 0a20 2020 2020 2061 7070 2e64     }.      app.d
-00002080: 6f63 5265 6769 7374 7279 2e61 6464 5769  ocRegistry.addWi
-00002090: 6467 6574 4578 7465 6e73 696f 6e28 274e  dgetExtension('N
-000020a0: 6f74 6562 6f6f 6b27 2c20 6e65 7720 4164  otebook', new Ad
-000020b0: 7661 6e63 6564 4275 7474 6f6e 2829 290a  vancedButton()).
-000020c0: 0a20 2020 2020 2063 6c61 7373 2046 7261  .      class Fra
-000020d0: 6d65 4275 7474 6f6e 0a20 2020 2020 2020  meButton.       
-000020e0: 2069 6d70 6c65 6d65 6e74 730a 2020 2020   implements.    
-000020f0: 2020 2020 2020 446f 6375 6d65 6e74 5265        DocumentRe
-00002100: 6769 7374 7279 2e49 5769 6467 6574 4578  gistry.IWidgetEx
-00002110: 7465 6e73 696f 6e3c 4e6f 7465 626f 6f6b  tension<Notebook
-00002120: 5061 6e65 6c2c 2049 4e6f 7465 626f 6f6b  Panel, INotebook
-00002130: 4d6f 6465 6c3e 0a20 2020 2020 207b 0a20  Model>.      {. 
-00002140: 2020 2020 2020 2063 7265 6174 654e 6577         createNew
-00002150: 280a 2020 2020 2020 2020 2020 7061 6e65  (.          pane
-00002160: 6c3a 204e 6f74 6562 6f6f 6b50 616e 656c  l: NotebookPanel
-00002170: 2c0a 2020 2020 2020 2020 2020 636f 6e74  ,.          cont
-00002180: 6578 743a 2044 6f63 756d 656e 7452 6567  ext: DocumentReg
-00002190: 6973 7472 792e 4943 6f6e 7465 7874 3c49  istry.IContext<I
-000021a0: 4e6f 7465 626f 6f6b 4d6f 6465 6c3e 0a20  NotebookModel>. 
-000021b0: 2020 2020 2020 2029 3a20 4944 6973 706f         ): IDispo
-000021c0: 7361 626c 6520 7b0a 2020 2020 2020 2020  sable {.        
-000021d0: 2020 636f 6e73 7420 6275 7474 6f6e 203d    const button =
-000021e0: 206e 6577 2054 6f6f 6c62 6172 4275 7474   new ToolbarButt
-000021f0: 6f6e 287b 0a20 2020 2020 2020 2020 2020  on({.           
-00002200: 2063 6c61 7373 4e61 6d65 3a20 2763 6f75   className: 'cou
-00002210: 7273 656c 6576 656c 732d 6275 7474 6f6e  rselevels-button
-00002220: 272c 0a20 2020 2020 2020 2020 2020 2069  ',.            i
-00002230: 636f 6e43 6c61 7373 3a20 2766 6173 2066  conClass: 'fas f
-00002240: 612d 6372 6f70 2d61 6c74 272c 0a20 2020  a-crop-alt',.   
-00002250: 2020 2020 2020 2020 206f 6e43 6c69 636b           onClick
-00002260: 3a20 2829 203d 3e20 746f 6767 6c65 5f66  : () => toggle_f
-00002270: 7261 6d65 2829 2c0a 2020 2020 2020 2020  rame(),.        
-00002280: 2020 2020 746f 6f6c 7469 703a 2027 546f      tooltip: 'To
-00002290: 6767 6c65 2066 7261 6d65 2061 726f 756e  ggle frame aroun
-000022a0: 6420 6365 6c6c 270a 2020 2020 2020 2020  d cell'.        
-000022b0: 2020 7d29 0a20 2020 2020 2020 2020 202f    }).          /
-000022c0: 2f20 636f 6d70 7574 6520 7768 6572 6520  / compute where 
-000022d0: 746f 2069 6e73 6572 7420 6974 0a20 2020  to insert it.   
-000022e0: 2020 2020 2020 2063 6f6e 7374 2069 6e64         const ind
-000022f0: 6578 203d 2066 696e 645f 7370 6163 6572  ex = find_spacer
-00002300: 2870 616e 656c 290a 2020 2020 2020 2020  (panel).        
-00002310: 2020 7061 6e65 6c2e 746f 6f6c 6261 722e    panel.toolbar.
-00002320: 696e 7365 7274 4974 656d 2869 6e64 6578  insertItem(index
-00002330: 2c20 2766 7261 6d65 4c65 7665 6c27 2c20  , 'frameLevel', 
-00002340: 6275 7474 6f6e 290a 2020 2020 2020 2020  button).        
-00002350: 2020 7265 7475 726e 206e 6577 2044 6973    return new Dis
-00002360: 706f 7361 626c 6544 656c 6567 6174 6528  posableDelegate(
-00002370: 2829 203d 3e20 7b0a 2020 2020 2020 2020  () => {.        
-00002380: 2020 2020 6275 7474 6f6e 2e64 6973 706f      button.dispo
-00002390: 7365 2829 0a20 2020 2020 2020 2020 207d  se().          }
-000023a0: 290a 2020 2020 2020 2020 7d0a 2020 2020  ).        }.    
-000023b0: 2020 7d0a 2020 2020 2020 6170 702e 646f    }.      app.do
-000023c0: 6352 6567 6973 7472 792e 6164 6457 6964  cRegistry.addWid
-000023d0: 6765 7445 7874 656e 7369 6f6e 2827 4e6f  getExtension('No
-000023e0: 7465 626f 6f6b 272c 206e 6577 2046 7261  tebook', new Fra
-000023f0: 6d65 4275 7474 6f6e 2829 290a 2020 2020  meButton()).    
-00002400: 7d0a 0a20 2020 202f 2f20 6164 6d6f 6e69  }..    // admoni
-00002410: 7469 6f6e 730a 2020 2020 666f 7220 2863  tions.    for (c
-00002420: 6f6e 7374 205b 6e61 6d65 2c20 6b65 795d  onst [name, key]
-00002430: 206f 6620 5b0a 2020 2020 2020 5b27 6164   of [.      ['ad
-00002440: 6d6f 6e69 7469 6f6e 272c 2027 4374 726c  monition', 'Ctrl
-00002450: 2041 275d 2c0a 2020 2020 2020 5b27 7469   A'],.      ['ti
-00002460: 7027 2c20 2743 7472 6c20 5427 5d2c 0a20  p', 'Ctrl T'],. 
-00002470: 2020 2020 205b 276e 6f74 6527 2c20 2743       ['note', 'C
-00002480: 7472 6c20 4e27 5d2c 0a20 2020 2020 205b  trl N'],.      [
-00002490: 2761 7474 656e 7469 6f6e 272c 206e 756c  'attention', nul
-000024a0: 6c5d 2c0a 2020 2020 2020 5b27 6361 7574  l],.      ['caut
-000024b0: 696f 6e27 2c20 6e75 6c6c 5d2c 0a20 2020  ion', null],.   
-000024c0: 2020 205b 2764 616e 6765 7227 2c20 6e75     ['danger', nu
-000024d0: 6c6c 5d2c 0a20 2020 2020 205b 2765 7272  ll],.      ['err
-000024e0: 6f72 272c 206e 756c 6c5d 2c0a 2020 2020  or', null],.    
-000024f0: 2020 5b27 6869 6e74 272c 206e 756c 6c5d    ['hint', null]
-00002500: 2c0a 2020 2020 2020 5b27 696d 706f 7274  ,.      ['import
-00002510: 616e 7427 2c20 6e75 6c6c 5d2c 0a20 2020  ant', null],.   
-00002520: 2020 205b 2773 6565 616c 736f 272c 206e     ['seealso', n
-00002530: 756c 6c5d 2c0a 2020 2020 2020 5b27 7761  ull],.      ['wa
-00002540: 726e 696e 6727 2c20 6e75 6c6c 5d0a 2020  rning', null].  
-00002550: 2020 5d29 207b 0a20 2020 2020 202f 2f20    ]) {.      // 
-00002560: 6e65 6564 2074 6f20 6361 7374 2062 6563  need to cast bec
-00002570: 6175 7365 206e 616d 6520 6973 2074 7970  ause name is typ
-00002580: 6564 2061 7320 7374 7269 6e67 207c 206e  ed as string | n
-00002590: 756c 6c20 3f21 3f0a 2020 2020 2020 636f  ull ?!?.      co
-000025a0: 6e73 7420 6164 6d6f 6e69 7469 6f6e 203d  nst admonition =
-000025b0: 206e 616d 6520 6173 2073 7472 696e 670a   name as string.
-000025c0: 2020 2020 2020 636f 6d6d 616e 6420 3d20        command = 
-000025d0: 2763 6f75 7273 656c 6576 656c 733a 746f  'courselevels:to
-000025e0: 6767 6c65 2d61 646d 6f6e 6974 696f 6e27  ggle-admonition'
-000025f0: 0a20 2020 2020 206c 6574 206c 6162 656c  .      let label
-00002600: 203d 2027 746f 6767 6c65 2061 646d 6f6e   = 'toggle admon
-00002610: 6974 696f 6e27 0a20 2020 2020 2069 6620  ition'.      if 
-00002620: 2861 646d 6f6e 6974 696f 6e20 213d 3d20  (admonition !== 
-00002630: 2761 646d 6f6e 6974 696f 6e27 2920 7b0a  'admonition') {.
-00002640: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
-00002650: 2b3d 2060 2d24 7b61 646d 6f6e 6974 696f  += `-${admonitio
-00002660: 6e7d 600a 2020 2020 2020 2020 6c61 6265  n}`.        labe
-00002670: 6c20 2b3d 2060 2024 7b61 646d 6f6e 6974  l += ` ${admonit
-00002680: 696f 6e7d 600a 2020 2020 2020 7d0a 2020  ion}`.      }.  
-00002690: 2020 2020 6170 702e 636f 6d6d 616e 6473      app.commands
-000026a0: 2e61 6464 436f 6d6d 616e 6428 636f 6d6d  .addCommand(comm
-000026b0: 616e 642c 207b 0a20 2020 2020 2020 206c  and, {.        l
-000026c0: 6162 656c 2c0a 2020 2020 2020 2020 6578  abel,.        ex
-000026d0: 6563 7574 653a 2028 2920 3d3e 207b 0a20  ecute: () => {. 
-000026e0: 2020 2020 2020 2020 2063 6f6e 7374 206e           const n
-000026f0: 6f74 6562 6f6f 6b20 3d20 6e6f 7465 626f  otebook = notebo
-00002700: 6f6b 5472 6163 6b65 722e 6375 7272 656e  okTracker.curren
-00002710: 7457 6964 6765 743f 2e63 6f6e 7465 6e74  tWidget?.content
-00002720: 0a20 2020 2020 2020 2020 2069 6620 286e  .          if (n
-00002730: 6f74 6562 6f6f 6b20 3d3d 3d20 756e 6465  otebook === unde
-00002740: 6669 6e65 6429 207b 0a20 2020 2020 2020  fined) {.       
-00002750: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00002760: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002770: 2020 746f 6767 6c65 5f61 646d 6f6e 6974    toggle_admonit
-00002780: 696f 6e28 6e6f 7465 626f 6f6b 2c20 6164  ion(notebook, ad
-00002790: 6d6f 6e69 7469 6f6e 290a 2020 2020 2020  monition).      
-000027a0: 2020 7d0a 2020 2020 2020 7d29 0a20 2020    }.      }).   
-000027b0: 2020 2070 616c 6574 7465 2e61 6464 4974     palette.addIt
-000027c0: 656d 287b 2063 6f6d 6d61 6e64 2c20 6361  em({ command, ca
-000027d0: 7465 676f 7279 3a20 2763 6f75 7273 656c  tegory: 'coursel
-000027e0: 6576 656c 7327 207d 290a 2020 2020 2020  evels' }).      
-000027f0: 6966 2028 6b65 7920 213d 3d20 6e75 6c6c  if (key !== null
-00002800: 2920 7b0a 2020 2020 2020 2020 6170 702e  ) {.        app.
-00002810: 636f 6d6d 616e 6473 2e61 6464 4b65 7942  commands.addKeyB
-00002820: 696e 6469 6e67 287b 0a20 2020 2020 2020  inding({.       
-00002830: 2020 2063 6f6d 6d61 6e64 2c0a 2020 2020     command,.    
-00002840: 2020 2020 2020 6b65 7973 3a20 5b27 4374        keys: ['Ct
-00002850: 726c 205c 5c27 2c20 6b65 795d 2c0a 2020  rl \\', key],.  
-00002860: 2020 2020 2020 2020 7365 6c65 6374 6f72          selector
-00002870: 3a20 272e 6a70 2d4e 6f74 6562 6f6f 6b27  : '.jp-Notebook'
-00002880: 0a20 2020 2020 2020 207d 290a 2020 2020  .        }).    
-00002890: 2020 7d0a 2020 2020 7d0a 0a20 2020 202f    }.    }..    /
-000028a0: 2f20 6c6f 6164 2073 6574 7469 6e67 7320  / load settings 
-000028b0: 616e 6420 6372 6561 7465 2062 7574 746f  and create butto
-000028c0: 6e73 2069 6620 7265 7175 6573 7465 640a  ns if requested.
-000028d0: 2020 2020 6675 6e63 7469 6f6e 206c 6f61      function loa
-000028e0: 6453 6574 7469 6e67 2873 6574 7469 6e67  dSetting(setting
-000028f0: 3a20 4953 6574 7469 6e67 5265 6769 7374  : ISettingRegist
-00002900: 7279 2e49 5365 7474 696e 6773 293a 2076  ry.ISettings): v
-00002910: 6f69 6420 7b0a 2020 2020 2020 2f2f 2052  oid {.      // R
-00002920: 6561 6420 7468 6520 7365 7474 696e 6773  ead the settings
-00002930: 2061 6e64 2063 6f6e 7665 7274 2074 6f20   and convert to 
-00002940: 7468 6520 636f 7272 6563 7420 7479 7065  the correct type
-00002950: 0a20 2020 2020 2073 686f 775f 6c65 7665  .      show_leve
-00002960: 6c5f 6275 7474 6f6e 7320 3d20 7365 7474  l_buttons = sett
-00002970: 696e 672e 6765 7428 2773 686f 775f 6c65  ing.get('show_le
-00002980: 7665 6c5f 6275 7474 6f6e 7327 290a 2020  vel_buttons').  
-00002990: 2020 2020 2020 2e63 6f6d 706f 7369 7465        .composite
-000029a0: 2061 7320 626f 6f6c 6561 6e0a 0a20 2020   as boolean..   
-000029b0: 2020 2063 6f6e 736f 6c65 2e6c 6f67 280a     console.log(.
-000029c0: 2020 2020 2020 2020 606a 7570 7974 6572          `jupyter
-000029d0: 6c61 622d 636f 7572 7365 6c65 7665 6c73  lab-courselevels
-000029e0: 2065 7874 656e 7369 6f6e 3a20 7368 6f77   extension: show
-000029f0: 5f6c 6576 656c 5f62 7574 746f 6e73 2069  _level_buttons i
-00002a00: 7320 7365 7420 746f 2024 7b73 686f 775f  s set to ${show_
-00002a10: 6c65 7665 6c5f 6275 7474 6f6e 737d 600a  level_buttons}`.
-00002a20: 2020 2020 2020 290a 2020 2020 2020 6966        ).      if
-00002a30: 2028 7368 6f77 5f6c 6576 656c 5f62 7574   (show_level_but
-00002a40: 746f 6e73 2920 7b0a 2020 2020 2020 2020  tons) {.        
-00002a50: 6372 6561 7465 5f6c 6576 656c 5f62 7574  create_level_but
-00002a60: 746f 6e73 2829 0a20 2020 2020 207d 0a20  tons().      }. 
-00002a70: 2020 207d 0a0a 2020 2020 2f2f 2062 7574     }..    // but
-00002a80: 2064 6f20 6974 206f 6e6c 7920 6166 7465   do it only afte
-00002a90: 7220 7468 6520 6170 7020 6861 7320 7374  r the app has st
-00002aa0: 6172 7465 640a 2020 2020 5072 6f6d 6973  arted.    Promis
-00002ab0: 652e 616c 6c28 5b61 7070 2e72 6573 746f  e.all([app.resto
-00002ac0: 7265 642c 2073 6574 7469 6e67 5265 6769  red, settingRegi
-00002ad0: 7374 7279 2e6c 6f61 6428 504c 5547 494e  stry.load(PLUGIN
-00002ae0: 5f49 4429 5d29 2e74 6865 6e28 0a20 2020  _ID)]).then(.   
-00002af0: 2020 2028 5b5f 2c20 7365 7474 696e 675d     ([_, setting]
-00002b00: 2920 3d3e 207b 0a20 2020 2020 2020 206c  ) => {.        l
-00002b10: 6f61 6453 6574 7469 6e67 2873 6574 7469  oadSetting(setti
-00002b20: 6e67 290a 2020 2020 2020 2020 7365 7474  ng).        sett
-00002b30: 696e 672e 6368 616e 6765 642e 636f 6e6e  ing.changed.conn
-00002b40: 6563 7428 6c6f 6164 5365 7474 696e 6729  ect(loadSetting)
-00002b50: 0a20 2020 2020 207d 0a20 2020 2029 0a20  .      }.    ). 
-00002b60: 207d 0a7d 0a0a 6578 706f 7274 2064 6566   }.}..export def
-00002b70: 6175 6c74 2070 6c75 6769 6e0a            ault plugin.
+00000000: 2275 7365 2073 7472 6963 7422 3b0a 2873  "use strict";.(s
+00000010: 656c 665b 2277 6562 7061 636b 4368 756e  elf["webpackChun
+00000020: 6b6a 7570 7974 6572 6c61 625f 636f 7572  kjupyterlab_cour
+00000030: 7365 6c65 7665 6c73 225d 203d 2073 656c  selevels"] = sel
+00000040: 665b 2277 6562 7061 636b 4368 756e 6b6a  f["webpackChunkj
+00000050: 7570 7974 6572 6c61 625f 636f 7572 7365  upyterlab_course
+00000060: 6c65 7665 6c73 225d 207c 7c20 5b5d 292e  levels"] || []).
+00000070: 7075 7368 285b 5b22 6c69 625f 696e 6465  push([["lib_inde
+00000080: 785f 6a73 225d 2c7b 0a0a 2f2a 2a2a 2f20  x_js"],{../***/ 
+00000090: 222e 2f6c 6962 2f69 6e64 6578 2e6a 7322  "./lib/index.js"
+000000a0: 3a0a 2f2a 212a 2a2a 2a2a 2a2a 2a2a 2a2a  :./*!***********
+000000b0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a21 2a5c 0a20  ***********!*\. 
+000000c0: 2021 2a2a 2a20 2e2f 6c69 622f 696e 6465   !*** ./lib/inde
+000000d0: 782e 6a73 202a 2a2a 210a 2020 5c2a 2a2a  x.js ***!.  \***
+000000e0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000000f0: 2a2a 2a2f 0a2f 2a2a 2a2f 2028 285f 5f75  ***/./***/ ((__u
+00000100: 6e75 7365 645f 7765 6270 6163 6b5f 6d6f  nused_webpack_mo
+00000110: 6475 6c65 2c20 5f5f 7765 6270 6163 6b5f  dule, __webpack_
+00000120: 6578 706f 7274 735f 5f2c 205f 5f77 6562  exports__, __web
+00000130: 7061 636b 5f72 6571 7569 7265 5f5f 2920  pack_require__) 
+00000140: 3d3e 207b 0a0a 5f5f 7765 6270 6163 6b5f  => {..__webpack_
+00000150: 7265 7175 6972 655f 5f2e 7228 5f5f 7765  require__.r(__we
+00000160: 6270 6163 6b5f 6578 706f 7274 735f 5f29  bpack_exports__)
+00000170: 3b0a 2f2a 2068 6172 6d6f 6e79 2065 7870  ;./* harmony exp
+00000180: 6f72 7420 2a2f 205f 5f77 6562 7061 636b  ort */ __webpack
+00000190: 5f72 6571 7569 7265 5f5f 2e64 285f 5f77  _require__.d(__w
+000001a0: 6562 7061 636b 5f65 7870 6f72 7473 5f5f  ebpack_exports__
+000001b0: 2c20 7b0a 2f2a 2068 6172 6d6f 6e79 2065  , {./* harmony e
+000001c0: 7870 6f72 7420 2a2f 2020 2022 6465 6661  xport */   "defa
+000001d0: 756c 7422 3a20 2829 203d 3e20 285f 5f57  ult": () => (__W
+000001e0: 4542 5041 434b 5f44 4546 4155 4c54 5f45  EBPACK_DEFAULT_E
+000001f0: 5850 4f52 545f 5f29 0a2f 2a20 6861 726d  XPORT__)./* harm
+00000200: 6f6e 7920 6578 706f 7274 202a 2f20 7d29  ony export */ })
+00000210: 3b0a 2f2a 2068 6172 6d6f 6e79 2069 6d70  ;./* harmony imp
+00000220: 6f72 7420 2a2f 2076 6172 205f 6a75 7079  ort */ var _jupy
+00000230: 7465 726c 6162 5f61 7070 7574 696c 735f  terlab_apputils_
+00000240: 5f57 4542 5041 434b 5f49 4d50 4f52 5445  _WEBPACK_IMPORTE
+00000250: 445f 4d4f 4455 4c45 5f30 5f5f 203d 205f  D_MODULE_0__ = _
+00000260: 5f77 6562 7061 636b 5f72 6571 7569 7265  _webpack_require
+00000270: 5f5f 282f 2a21 2040 6a75 7079 7465 726c  __(/*! @jupyterl
+00000280: 6162 2f61 7070 7574 696c 7320 2a2f 2022  ab/apputils */ "
+00000290: 7765 6270 6163 6b2f 7368 6172 696e 672f  webpack/sharing/
+000002a0: 636f 6e73 756d 652f 6465 6661 756c 742f  consume/default/
+000002b0: 406a 7570 7974 6572 6c61 622f 6170 7075  @jupyterlab/appu
+000002c0: 7469 6c73 2229 3b0a 2f2a 2068 6172 6d6f  tils");./* harmo
+000002d0: 6e79 2069 6d70 6f72 7420 2a2f 2076 6172  ny import */ var
+000002e0: 205f 6a75 7079 7465 726c 6162 5f61 7070   _jupyterlab_app
+000002f0: 7574 696c 735f 5f57 4542 5041 434b 5f49  utils__WEBPACK_I
+00000300: 4d50 4f52 5445 445f 4d4f 4455 4c45 5f30  MPORTED_MODULE_0
+00000310: 5f5f 5f64 6566 6175 6c74 203d 202f 2a23  ___default = /*#
+00000320: 5f5f 5055 5245 5f5f 2a2f 5f5f 7765 6270  __PURE__*/__webp
+00000330: 6163 6b5f 7265 7175 6972 655f 5f2e 6e28  ack_require__.n(
+00000340: 5f6a 7570 7974 6572 6c61 625f 6170 7075  _jupyterlab_appu
+00000350: 7469 6c73 5f5f 5745 4250 4143 4b5f 494d  tils__WEBPACK_IM
+00000360: 504f 5254 4544 5f4d 4f44 554c 455f 305f  PORTED_MODULE_0_
+00000370: 5f29 3b0a 2f2a 2068 6172 6d6f 6e79 2069  _);./* harmony i
+00000380: 6d70 6f72 7420 2a2f 2076 6172 205f 6a75  mport */ var _ju
+00000390: 7079 7465 726c 6162 5f6e 6f74 6562 6f6f  pyterlab_noteboo
+000003a0: 6b5f 5f57 4542 5041 434b 5f49 4d50 4f52  k__WEBPACK_IMPOR
+000003b0: 5445 445f 4d4f 4455 4c45 5f31 5f5f 203d  TED_MODULE_1__ =
+000003c0: 205f 5f77 6562 7061 636b 5f72 6571 7569   __webpack_requi
+000003d0: 7265 5f5f 282f 2a21 2040 6a75 7079 7465  re__(/*! @jupyte
+000003e0: 726c 6162 2f6e 6f74 6562 6f6f 6b20 2a2f  rlab/notebook */
+000003f0: 2022 7765 6270 6163 6b2f 7368 6172 696e   "webpack/sharin
+00000400: 672f 636f 6e73 756d 652f 6465 6661 756c  g/consume/defaul
+00000410: 742f 406a 7570 7974 6572 6c61 622f 6e6f  t/@jupyterlab/no
+00000420: 7465 626f 6f6b 2229 3b0a 2f2a 2068 6172  tebook");./* har
+00000430: 6d6f 6e79 2069 6d70 6f72 7420 2a2f 2076  mony import */ v
+00000440: 6172 205f 6a75 7079 7465 726c 6162 5f6e  ar _jupyterlab_n
+00000450: 6f74 6562 6f6f 6b5f 5f57 4542 5041 434b  otebook__WEBPACK
+00000460: 5f49 4d50 4f52 5445 445f 4d4f 4455 4c45  _IMPORTED_MODULE
+00000470: 5f31 5f5f 5f64 6566 6175 6c74 203d 202f  _1___default = /
+00000480: 2a23 5f5f 5055 5245 5f5f 2a2f 5f5f 7765  *#__PURE__*/__we
+00000490: 6270 6163 6b5f 7265 7175 6972 655f 5f2e  bpack_require__.
+000004a0: 6e28 5f6a 7570 7974 6572 6c61 625f 6e6f  n(_jupyterlab_no
+000004b0: 7465 626f 6f6b 5f5f 5745 4250 4143 4b5f  tebook__WEBPACK_
+000004c0: 494d 504f 5254 4544 5f4d 4f44 554c 455f  IMPORTED_MODULE_
+000004d0: 315f 5f29 3b0a 2f2a 2068 6172 6d6f 6e79  1__);./* harmony
+000004e0: 2069 6d70 6f72 7420 2a2f 2076 6172 205f   import */ var _
+000004f0: 6a75 7079 7465 726c 6162 5f73 6574 7469  jupyterlab_setti
+00000500: 6e67 7265 6769 7374 7279 5f5f 5745 4250  ngregistry__WEBP
+00000510: 4143 4b5f 494d 504f 5254 4544 5f4d 4f44  ACK_IMPORTED_MOD
+00000520: 554c 455f 325f 5f20 3d20 5f5f 7765 6270  ULE_2__ = __webp
+00000530: 6163 6b5f 7265 7175 6972 655f 5f28 2f2a  ack_require__(/*
+00000540: 2120 406a 7570 7974 6572 6c61 622f 7365  ! @jupyterlab/se
+00000550: 7474 696e 6772 6567 6973 7472 7920 2a2f  ttingregistry */
+00000560: 2022 7765 6270 6163 6b2f 7368 6172 696e   "webpack/sharin
+00000570: 672f 636f 6e73 756d 652f 6465 6661 756c  g/consume/defaul
+00000580: 742f 406a 7570 7974 6572 6c61 622f 7365  t/@jupyterlab/se
+00000590: 7474 696e 6772 6567 6973 7472 7922 293b  ttingregistry");
+000005a0: 0a2f 2a20 6861 726d 6f6e 7920 696d 706f  ./* harmony impo
+000005b0: 7274 202a 2f20 7661 7220 5f6a 7570 7974  rt */ var _jupyt
+000005c0: 6572 6c61 625f 7365 7474 696e 6772 6567  erlab_settingreg
+000005d0: 6973 7472 795f 5f57 4542 5041 434b 5f49  istry__WEBPACK_I
+000005e0: 4d50 4f52 5445 445f 4d4f 4455 4c45 5f32  MPORTED_MODULE_2
+000005f0: 5f5f 5f64 6566 6175 6c74 203d 202f 2a23  ___default = /*#
+00000600: 5f5f 5055 5245 5f5f 2a2f 5f5f 7765 6270  __PURE__*/__webp
+00000610: 6163 6b5f 7265 7175 6972 655f 5f2e 6e28  ack_require__.n(
+00000620: 5f6a 7570 7974 6572 6c61 625f 7365 7474  _jupyterlab_sett
+00000630: 696e 6772 6567 6973 7472 795f 5f57 4542  ingregistry__WEB
+00000640: 5041 434b 5f49 4d50 4f52 5445 445f 4d4f  PACK_IMPORTED_MO
+00000650: 4455 4c45 5f32 5f5f 293b 0a2f 2a20 6861  DULE_2__);./* ha
+00000660: 726d 6f6e 7920 696d 706f 7274 202a 2f20  rmony import */ 
+00000670: 7661 7220 5f6c 756d 696e 6f5f 6469 7370  var _lumino_disp
+00000680: 6f73 6162 6c65 5f5f 5745 4250 4143 4b5f  osable__WEBPACK_
+00000690: 494d 504f 5254 4544 5f4d 4f44 554c 455f  IMPORTED_MODULE_
+000006a0: 335f 5f20 3d20 5f5f 7765 6270 6163 6b5f  3__ = __webpack_
+000006b0: 7265 7175 6972 655f 5f28 2f2a 2120 406c  require__(/*! @l
+000006c0: 756d 696e 6f2f 6469 7370 6f73 6162 6c65  umino/disposable
+000006d0: 202a 2f20 2277 6562 7061 636b 2f73 6861   */ "webpack/sha
+000006e0: 7269 6e67 2f63 6f6e 7375 6d65 2f64 6566  ring/consume/def
+000006f0: 6175 6c74 2f40 6c75 6d69 6e6f 2f64 6973  ault/@lumino/dis
+00000700: 706f 7361 626c 6522 293b 0a2f 2a20 6861  posable");./* ha
+00000710: 726d 6f6e 7920 696d 706f 7274 202a 2f20  rmony import */ 
+00000720: 7661 7220 5f6c 756d 696e 6f5f 6469 7370  var _lumino_disp
+00000730: 6f73 6162 6c65 5f5f 5745 4250 4143 4b5f  osable__WEBPACK_
+00000740: 494d 504f 5254 4544 5f4d 4f44 554c 455f  IMPORTED_MODULE_
+00000750: 335f 5f5f 6465 6661 756c 7420 3d20 2f2a  3___default = /*
+00000760: 235f 5f50 5552 455f 5f2a 2f5f 5f77 6562  #__PURE__*/__web
+00000770: 7061 636b 5f72 6571 7569 7265 5f5f 2e6e  pack_require__.n
+00000780: 285f 6c75 6d69 6e6f 5f64 6973 706f 7361  (_lumino_disposa
+00000790: 626c 655f 5f57 4542 5041 434b 5f49 4d50  ble__WEBPACK_IMP
+000007a0: 4f52 5445 445f 4d4f 4455 4c45 5f33 5f5f  ORTED_MODULE_3__
+000007b0: 293b 0a2f 2a20 6861 726d 6f6e 7920 696d  );./* harmony im
+000007c0: 706f 7274 202a 2f20 7661 7220 6a75 7079  port */ var jupy
+000007d0: 7465 726c 6162 5f63 656c 6c74 6167 7363  terlab_celltagsc
+000007e0: 6c61 7373 6573 5f5f 5745 4250 4143 4b5f  lasses__WEBPACK_
+000007f0: 494d 504f 5254 4544 5f4d 4f44 554c 455f  IMPORTED_MODULE_
+00000800: 345f 5f20 3d20 5f5f 7765 6270 6163 6b5f  4__ = __webpack_
+00000810: 7265 7175 6972 655f 5f28 2f2a 2120 6a75  require__(/*! ju
+00000820: 7079 7465 726c 6162 2d63 656c 6c74 6167  pyterlab-celltag
+00000830: 7363 6c61 7373 6573 202a 2f20 2277 6562  sclasses */ "web
+00000840: 7061 636b 2f73 6861 7269 6e67 2f63 6f6e  pack/sharing/con
+00000850: 7375 6d65 2f64 6566 6175 6c74 2f6a 7570  sume/default/jup
+00000860: 7974 6572 6c61 622d 6365 6c6c 7461 6773  yterlab-celltags
+00000870: 636c 6173 7365 732f 6a75 7079 7465 726c  classes/jupyterl
+00000880: 6162 2d63 656c 6c74 6167 7363 6c61 7373  ab-celltagsclass
+00000890: 6573 2229 3b0a 2f2a 2068 6172 6d6f 6e79  es");./* harmony
+000008a0: 2069 6d70 6f72 7420 2a2f 2076 6172 206a   import */ var j
+000008b0: 7570 7974 6572 6c61 625f 6365 6c6c 7461  upyterlab_cellta
+000008c0: 6773 636c 6173 7365 735f 5f57 4542 5041  gsclasses__WEBPA
+000008d0: 434b 5f49 4d50 4f52 5445 445f 4d4f 4455  CK_IMPORTED_MODU
+000008e0: 4c45 5f34 5f5f 5f64 6566 6175 6c74 203d  LE_4___default =
+000008f0: 202f 2a23 5f5f 5055 5245 5f5f 2a2f 5f5f   /*#__PURE__*/__
+00000900: 7765 6270 6163 6b5f 7265 7175 6972 655f  webpack_require_
+00000910: 5f2e 6e28 6a75 7079 7465 726c 6162 5f63  _.n(jupyterlab_c
+00000920: 656c 6c74 6167 7363 6c61 7373 6573 5f5f  elltagsclasses__
+00000930: 5745 4250 4143 4b5f 494d 504f 5254 4544  WEBPACK_IMPORTED
+00000940: 5f4d 4f44 554c 455f 345f 5f29 3b0a 2f2a  _MODULE_4__);./*
+00000950: 0a20 2a20 666f 7220 6174 7461 6368 696e  . * for attachin
+00000960: 6720 6b65 7962 696e 6469 6e67 7320 6c61  g keybindings la
+00000970: 7465 7220 6f6e 2c20 7365 650a 202a 2068  ter on, see. * h
+00000980: 7474 7073 3a2f 2f74 6f77 6172 6473 6461  ttps://towardsda
+00000990: 7461 7363 6965 6e63 652e 636f 6d2f 686f  tascience.com/ho
+000009a0: 772d 746f 2d63 7573 746f 6d69 7a65 2d6a  w-to-customize-j
+000009b0: 7570 7974 6572 6c61 622d 6b65 7962 6f61  upyterlab-keyboa
+000009c0: 7264 2d73 686f 7274 6375 7473 2d37 3233  rd-shortcuts-723
+000009d0: 3231 6637 3337 3533 640a 202a 2f0a 0a0a  21f73753d. */...
+000009e0: 0a0a 0a0a 0a63 6f6e 7374 2050 4c55 4749  .....const PLUGI
+000009f0: 4e5f 4944 203d 2027 6a75 7079 7465 726c  N_ID = 'jupyterl
+00000a00: 6162 2d63 6f75 7273 656c 6576 656c 733a  ab-courselevels:
+00000a10: 706c 7567 696e 273b 0a63 6f6e 7374 2041  plugin';.const A
+00000a20: 4c4c 5f4c 4556 454c 5320 3d20 5b27 6261  LL_LEVELS = ['ba
+00000a30: 7369 6327 2c20 2769 6e74 6572 6d65 6469  sic', 'intermedi
+00000a40: 6174 6527 2c20 2761 6476 616e 6365 6427  ate', 'advanced'
+00000a50: 5d3b 0a63 6f6e 7374 2070 6c75 6769 6e20  ];.const plugin 
+00000a60: 3d20 7b0a 2020 2020 6964 3a20 504c 5547  = {.    id: PLUG
+00000a70: 494e 5f49 442c 0a20 2020 2061 7574 6f53  IN_ID,.    autoS
+00000a80: 7461 7274 3a20 7472 7565 2c0a 2020 2020  tart: true,.    
+00000a90: 7265 7175 6972 6573 3a20 5b5f 6a75 7079  requires: [_jupy
+00000aa0: 7465 726c 6162 5f61 7070 7574 696c 735f  terlab_apputils_
+00000ab0: 5f57 4542 5041 434b 5f49 4d50 4f52 5445  _WEBPACK_IMPORTE
+00000ac0: 445f 4d4f 4455 4c45 5f30 5f5f 2e49 436f  D_MODULE_0__.ICo
+00000ad0: 6d6d 616e 6450 616c 6574 7465 2c20 5f6a  mmandPalette, _j
+00000ae0: 7570 7974 6572 6c61 625f 6e6f 7465 626f  upyterlab_notebo
+00000af0: 6f6b 5f5f 5745 4250 4143 4b5f 494d 504f  ok__WEBPACK_IMPO
+00000b00: 5254 4544 5f4d 4f44 554c 455f 315f 5f2e  RTED_MODULE_1__.
+00000b10: 494e 6f74 6562 6f6f 6b54 7261 636b 6572  INotebookTracker
+00000b20: 2c20 5f6a 7570 7974 6572 6c61 625f 7365  , _jupyterlab_se
+00000b30: 7474 696e 6772 6567 6973 7472 795f 5f57  ttingregistry__W
+00000b40: 4542 5041 434b 5f49 4d50 4f52 5445 445f  EBPACK_IMPORTED_
+00000b50: 4d4f 4455 4c45 5f32 5f5f 2e49 5365 7474  MODULE_2__.ISett
+00000b60: 696e 6752 6567 6973 7472 795d 2c0a 2020  ingRegistry],.  
+00000b70: 2020 6163 7469 7661 7465 3a20 2861 7070    activate: (app
+00000b80: 2c20 7061 6c65 7474 652c 206e 6f74 6562  , palette, noteb
+00000b90: 6f6f 6b54 7261 636b 6572 2c20 7365 7474  ookTracker, sett
+00000ba0: 696e 6752 6567 6973 7472 7929 203d 3e20  ingRegistry) => 
+00000bb0: 7b0a 2020 2020 2020 2020 636f 6e73 6f6c  {.        consol
+00000bc0: 652e 6c6f 6728 2765 7874 656e 7369 6f6e  e.log('extension
+00000bd0: 206a 7570 7974 6572 6c61 622d 636f 7572   jupyterlab-cour
+00000be0: 7365 6c65 7665 6c73 2069 7320 6163 7469  selevels is acti
+00000bf0: 7661 7469 6e67 2729 3b0a 2020 2020 2020  vating');.      
+00000c00: 2020 2f2f 2068 7474 7073 3a2f 2f6c 756d    // https://lum
+00000c10: 696e 6f2e 7265 6164 7468 6564 6f63 732e  ino.readthedocs.
+00000c20: 696f 2f65 6e2f 312e 782f 6170 692f 636f  io/en/1.x/api/co
+00000c30: 6d6d 616e 6473 2f69 6e74 6572 6661 6365  mmands/interface
+00000c40: 732f 636f 6d6d 616e 6472 6567 6973 7472  s/commandregistr
+00000c50: 792e 696b 6579 6269 6e64 696e 676f 7074  y.ikeybindingopt
+00000c60: 696f 6e73 2e68 746d 6c0a 2020 2020 2020  ions.html.      
+00000c70: 2020 2f2f 2054 6865 2073 7570 706f 7274    // The support
+00000c80: 6564 206d 6f64 6966 6965 7273 2061 7265  ed modifiers are
+00000c90: 3a20 4163 6365 6c2c 2041 6c74 2c20 436d  : Accel, Alt, Cm
+00000ca0: 642c 2043 7472 6c2c 2061 6e64 2053 6869  d, Ctrl, and Shi
+00000cb0: 6674 2e20 5468 6520 4163 6365 6c0a 2020  ft. The Accel.  
+00000cc0: 2020 2020 2020 2f2f 206d 6f64 6966 6965        // modifie
+00000cd0: 7220 6973 2074 7261 6e73 6c61 7465 6420  r is translated 
+00000ce0: 746f 2043 6d64 206f 6e20 4d61 6320 616e  to Cmd on Mac an
+00000cf0: 6420 4374 726c 206f 6e20 616c 6c20 6f74  d Ctrl on all ot
+00000d00: 6865 7220 706c 6174 666f 726d 732e 2054  her platforms. T
+00000d10: 6865 0a20 2020 2020 2020 202f 2f20 436d  he.        // Cm
+00000d20: 6420 6d6f 6469 6669 6572 2069 7320 6967  d modifier is ig
+00000d30: 6e6f 7265 6420 6f6e 206e 6f6e 2d4d 6163  nored on non-Mac
+00000d40: 2070 6c61 7466 6f72 6d73 2e0a 2020 2020   platforms..    
+00000d50: 2020 2020 2f2f 2041 6c74 2069 7320 6f70      // Alt is op
+00000d60: 7469 6f6e 206f 6e20 6d61 630a 2020 2020  tion on mac.    
+00000d70: 2020 2020 6c65 7420 5b73 686f 775f 6c65      let [show_le
+00000d80: 7665 6c5f 6275 7474 6f6e 735d 203d 205b  vel_buttons] = [
+00000d90: 6661 6c73 655d 3b0a 2020 2020 2020 2020  false];.        
+00000da0: 636f 6e73 7420 414c 4c5f 4655 4c4c 5f4c  const ALL_FULL_L
+00000db0: 4556 454c 5320 3d20 414c 4c5f 4c45 5645  EVELS = ALL_LEVE
+00000dc0: 4c53 2e6d 6170 286c 6576 656c 203d 3e20  LS.map(level => 
+00000dd0: 606c 6576 656c 5f24 7b6c 6576 656c 7d60  `level_${level}`
+00000de0: 293b 0a20 2020 2020 2020 2063 6f6e 7374  );.        const
+00000df0: 2063 656c 6c5f 746f 6767 6c65 5f6c 6576   cell_toggle_lev
+00000e00: 656c 203d 2028 6365 6c6c 2c20 6c65 7665  el = (cell, leve
+00000e10: 6c29 203d 3e20 7b0a 2020 2020 2020 2020  l) => {.        
+00000e20: 2020 2020 636f 6e73 7420 6675 6c6c 5f6c      const full_l
+00000e30: 6576 656c 203d 2060 6c65 7665 6c5f 247b  evel = `level_${
+00000e40: 6c65 7665 6c7d 603b 0a20 2020 2020 2020  level}`;.       
+00000e50: 2020 2020 2072 6574 7572 6e20 2830 2c6a       return (0,j
+00000e60: 7570 7974 6572 6c61 625f 6365 6c6c 7461  upyterlab_cellta
+00000e70: 6773 636c 6173 7365 735f 5f57 4542 5041  gsclasses__WEBPA
+00000e80: 434b 5f49 4d50 4f52 5445 445f 4d4f 4455  CK_IMPORTED_MODU
+00000e90: 4c45 5f34 5f5f 2e6d 645f 746f 6767 6c65  LE_4__.md_toggle
+00000ea0: 5f6d 756c 7469 2928 6365 6c6c 2c20 2774  _multi)(cell, 't
+00000eb0: 6167 7327 2c20 6675 6c6c 5f6c 6576 656c  ags', full_level
+00000ec0: 2c20 414c 4c5f 4655 4c4c 5f4c 4556 454c  , ALL_FULL_LEVEL
+00000ed0: 5329 3b0a 2020 2020 2020 2020 7d3b 0a20  S);.        };. 
+00000ee0: 2020 2020 2020 2063 6f6e 7374 2074 6f67         const tog
+00000ef0: 676c 655f 6c65 7665 6c20 3d20 286c 6576  gle_level = (lev
+00000f00: 656c 2920 3d3e 207b 0a20 2020 2020 2020  el) => {.       
+00000f10: 2020 2020 2028 302c 6a75 7079 7465 726c       (0,jupyterl
+00000f20: 6162 5f63 656c 6c74 6167 7363 6c61 7373  ab_celltagsclass
+00000f30: 6573 5f5f 5745 4250 4143 4b5f 494d 504f  es__WEBPACK_IMPO
+00000f40: 5254 4544 5f4d 4f44 554c 455f 345f 5f2e  RTED_MODULE_4__.
+00000f50: 6170 706c 795f 6f6e 5f63 656c 6c73 2928  apply_on_cells)(
+00000f60: 6e6f 7465 626f 6f6b 5472 6163 6b65 722c  notebookTracker,
+00000f70: 206a 7570 7974 6572 6c61 625f 6365 6c6c   jupyterlab_cell
+00000f80: 7461 6773 636c 6173 7365 735f 5f57 4542  tagsclasses__WEB
+00000f90: 5041 434b 5f49 4d50 4f52 5445 445f 4d4f  PACK_IMPORTED_MO
+00000fa0: 4455 4c45 5f34 5f5f 2e53 636f 7065 2e4d  DULE_4__.Scope.M
+00000fb0: 756c 7469 706c 652c 2028 6365 6c6c 2920  ultiple, (cell) 
+00000fc0: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
+00000fd0: 2020 2020 2063 656c 6c5f 746f 6767 6c65       cell_toggle
+00000fe0: 5f6c 6576 656c 2863 656c 6c2c 206c 6576  _level(cell, lev
+00000ff0: 656c 293b 0a20 2020 2020 2020 2020 2020  el);.           
+00001000: 207d 293b 0a20 2020 2020 2020 207d 3b0a   });.        };.
+00001010: 2020 2020 2020 2020 6c65 7420 636f 6d6d          let comm
+00001020: 616e 643b 0a20 2020 2020 2020 2066 6f72  and;.        for
+00001030: 2028 636f 6e73 7420 5b6c 6576 656c 2c20   (const [level, 
+00001040: 6b65 795d 206f 6620 5b0a 2020 2020 2020  key] of [.      
+00001050: 2020 2020 2020 5b27 6261 7369 6327 2c20        ['basic', 
+00001060: 2743 7472 6c20 5827 5d2c 0a20 2020 2020  'Ctrl X'],.     
+00001070: 2020 2020 2020 205b 2769 6e74 6572 6d65         ['interme
+00001080: 6469 6174 6527 2c20 2743 7472 6c20 5927  diate', 'Ctrl Y'
+00001090: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+000010a0: 2761 6476 616e 6365 6427 2c20 2743 7472  'advanced', 'Ctr
+000010b0: 6c20 5a27 5d0a 2020 2020 2020 2020 5d29  l Z'].        ])
+000010c0: 207b 0a20 2020 2020 2020 2020 2020 2063   {.            c
+000010d0: 6f6d 6d61 6e64 203d 2060 636f 7572 7365  ommand = `course
+000010e0: 6c65 7665 6c73 3a74 6f67 676c 652d 6c65  levels:toggle-le
+000010f0: 7665 6c2d 247b 6c65 7665 6c7d 603b 0a20  vel-${level}`;. 
+00001100: 2020 2020 2020 2020 2020 2061 7070 2e63             app.c
+00001110: 6f6d 6d61 6e64 732e 6164 6443 6f6d 6d61  ommands.addComma
+00001120: 6e64 2863 6f6d 6d61 6e64 2c20 7b0a 2020  nd(command, {.  
+00001130: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00001140: 6265 6c3a 2060 746f 6767 6c65 2024 7b6c  bel: `toggle ${l
+00001150: 6576 656c 7d20 6c65 7665 6c60 2c0a 2020  evel} level`,.  
+00001160: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00001170: 6563 7574 653a 2028 2920 3d3e 2074 6f67  ecute: () => tog
+00001180: 676c 655f 6c65 7665 6c28 6c65 7665 6c29  gle_level(level)
+00001190: 0a20 2020 2020 2020 2020 2020 207d 293b  .            });
+000011a0: 0a20 2020 2020 2020 2020 2020 2070 616c  .            pal
+000011b0: 6574 7465 2e61 6464 4974 656d 287b 2063  ette.addItem({ c
+000011c0: 6f6d 6d61 6e64 2c20 6361 7465 676f 7279  ommand, category
+000011d0: 3a20 2763 6f75 7273 656c 6576 656c 7327  : 'courselevels'
+000011e0: 207d 293b 0a20 2020 2020 2020 2020 2020   });.           
+000011f0: 2061 7070 2e63 6f6d 6d61 6e64 732e 6164   app.commands.ad
+00001200: 644b 6579 4269 6e64 696e 6728 7b0a 2020  dKeyBinding({.  
+00001210: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00001220: 6d6d 616e 642c 0a20 2020 2020 2020 2020  mmand,.         
+00001230: 2020 2020 2020 206b 6579 733a 205b 2743         keys: ['C
+00001240: 7472 6c20 5c5c 272c 206b 6579 5d2c 0a20  trl \\', key],. 
+00001250: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001260: 656c 6563 746f 723a 2027 2e6a 702d 4e6f  elector: '.jp-No
+00001270: 7465 626f 6f6b 270a 2020 2020 2020 2020  tebook'.        
+00001280: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
+00001290: 7d0a 2020 2020 2020 2020 636f 6e73 7420  }.        const 
+000012a0: 746f 6767 6c65 5f66 7261 6d65 203d 2028  toggle_frame = (
+000012b0: 2920 3d3e 207b 0a20 2020 2020 2020 2020  ) => {.         
+000012c0: 2020 2028 302c 6a75 7079 7465 726c 6162     (0,jupyterlab
+000012d0: 5f63 656c 6c74 6167 7363 6c61 7373 6573  _celltagsclasses
+000012e0: 5f5f 5745 4250 4143 4b5f 494d 504f 5254  __WEBPACK_IMPORT
+000012f0: 4544 5f4d 4f44 554c 455f 345f 5f2e 6170  ED_MODULE_4__.ap
+00001300: 706c 795f 6f6e 5f63 656c 6c73 2928 6e6f  ply_on_cells)(no
+00001310: 7465 626f 6f6b 5472 6163 6b65 722c 206a  tebookTracker, j
+00001320: 7570 7974 6572 6c61 625f 6365 6c6c 7461  upyterlab_cellta
+00001330: 6773 636c 6173 7365 735f 5f57 4542 5041  gsclasses__WEBPA
+00001340: 434b 5f49 4d50 4f52 5445 445f 4d4f 4455  CK_IMPORTED_MODU
+00001350: 4c45 5f34 5f5f 2e53 636f 7065 2e41 6374  LE_4__.Scope.Act
+00001360: 6976 652c 2028 6365 6c6c 2920 3d3e 207b  ive, (cell) => {
+00001370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001380: 2028 302c 6a75 7079 7465 726c 6162 5f63   (0,jupyterlab_c
+00001390: 656c 6c74 6167 7363 6c61 7373 6573 5f5f  elltagsclasses__
+000013a0: 5745 4250 4143 4b5f 494d 504f 5254 4544  WEBPACK_IMPORTED
+000013b0: 5f4d 4f44 554c 455f 345f 5f2e 6d64 5f74  _MODULE_4__.md_t
+000013c0: 6f67 676c 6529 2863 656c 6c2c 2027 7461  oggle)(cell, 'ta
+000013d0: 6773 272c 2027 6672 616d 6564 5f63 656c  gs', 'framed_cel
+000013e0: 6c27 293b 0a20 2020 2020 2020 2020 2020  l');.           
+000013f0: 207d 293b 0a20 2020 2020 2020 207d 3b0a   });.        };.
+00001400: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+00001410: 3d20 2763 6f75 7273 656c 6576 656c 733a  = 'courselevels:
+00001420: 746f 6767 6c65 2d66 7261 6d65 273b 0a20  toggle-frame';. 
+00001430: 2020 2020 2020 2061 7070 2e63 6f6d 6d61         app.comma
+00001440: 6e64 732e 6164 6443 6f6d 6d61 6e64 2863  nds.addCommand(c
+00001450: 6f6d 6d61 6e64 2c20 7b0a 2020 2020 2020  ommand, {.      
+00001460: 2020 2020 2020 6c61 6265 6c3a 2027 746f        label: 'to
+00001470: 6767 6c65 2066 7261 6d65 272c 0a20 2020  ggle frame',.   
+00001480: 2020 2020 2020 2020 2065 7865 6375 7465           execute
+00001490: 3a20 2829 203d 3e20 746f 6767 6c65 5f66  : () => toggle_f
+000014a0: 7261 6d65 2829 0a20 2020 2020 2020 207d  rame().        }
+000014b0: 293b 0a20 2020 2020 2020 2070 616c 6574  );.        palet
+000014c0: 7465 2e61 6464 4974 656d 287b 2063 6f6d  te.addItem({ com
+000014d0: 6d61 6e64 2c20 6361 7465 676f 7279 3a20  mand, category: 
+000014e0: 2763 6f75 7273 656c 6576 656c 7327 207d  'courselevels' }
+000014f0: 293b 0a20 2020 2020 2020 2061 7070 2e63  );.        app.c
+00001500: 6f6d 6d61 6e64 732e 6164 644b 6579 4269  ommands.addKeyBi
+00001510: 6e64 696e 6728 7b0a 2020 2020 2020 2020  nding({.        
+00001520: 2020 2020 636f 6d6d 616e 642c 0a20 2020      command,.   
+00001530: 2020 2020 2020 2020 206b 6579 733a 205b           keys: [
+00001540: 2743 7472 6c20 5c5c 272c 2027 4374 726c  'Ctrl \\', 'Ctrl
+00001550: 204d 275d 2c0a 2020 2020 2020 2020 2020   M'],.          
+00001560: 2020 7365 6c65 6374 6f72 3a20 272e 6a70    selector: '.jp
+00001570: 2d4e 6f74 6562 6f6f 6b27 0a20 2020 2020  -Notebook'.     
+00001580: 2020 207d 293b 0a20 2020 2020 2020 2063     });.        c
+00001590: 6f6e 7374 2074 6f67 676c 655f 6c69 6365  onst toggle_lice
+000015a0: 6e63 6520 3d20 2829 203d 3e20 7b0a 2020  nce = () => {.  
+000015b0: 2020 2020 2020 2020 2020 2830 2c6a 7570            (0,jup
+000015c0: 7974 6572 6c61 625f 6365 6c6c 7461 6773  yterlab_celltags
+000015d0: 636c 6173 7365 735f 5f57 4542 5041 434b  classes__WEBPACK
+000015e0: 5f49 4d50 4f52 5445 445f 4d4f 4455 4c45  _IMPORTED_MODULE
+000015f0: 5f34 5f5f 2e61 7070 6c79 5f6f 6e5f 6365  _4__.apply_on_ce
+00001600: 6c6c 7329 286e 6f74 6562 6f6f 6b54 7261  lls)(notebookTra
+00001610: 636b 6572 2c20 6a75 7079 7465 726c 6162  cker, jupyterlab
+00001620: 5f63 656c 6c74 6167 7363 6c61 7373 6573  _celltagsclasses
+00001630: 5f5f 5745 4250 4143 4b5f 494d 504f 5254  __WEBPACK_IMPORT
+00001640: 4544 5f4d 4f44 554c 455f 345f 5f2e 5363  ED_MODULE_4__.Sc
+00001650: 6f70 652e 4163 7469 7665 2c20 2863 656c  ope.Active, (cel
+00001660: 6c29 203d 3e20 7b0a 2020 2020 2020 2020  l) => {.        
+00001670: 2020 2020 2020 2020 2830 2c6a 7570 7974          (0,jupyt
+00001680: 6572 6c61 625f 6365 6c6c 7461 6773 636c  erlab_celltagscl
+00001690: 6173 7365 735f 5f57 4542 5041 434b 5f49  asses__WEBPACK_I
+000016a0: 4d50 4f52 5445 445f 4d4f 4455 4c45 5f34  MPORTED_MODULE_4
+000016b0: 5f5f 2e6d 645f 746f 6767 6c65 2928 6365  __.md_toggle)(ce
+000016c0: 6c6c 2c20 2774 6167 7327 2c20 276c 6963  ll, 'tags', 'lic
+000016d0: 656e 6365 2729 3b0a 2020 2020 2020 2020  ence');.        
+000016e0: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
+000016f0: 7d3b 0a20 2020 2020 2020 2063 6f6d 6d61  };.        comma
+00001700: 6e64 203d 2027 636f 7572 7365 6c65 7665  nd = 'courseleve
+00001710: 6c73 3a74 6f67 676c 652d 6c69 6365 6e63  ls:toggle-licenc
+00001720: 6527 3b0a 2020 2020 2020 2020 6170 702e  e';.        app.
+00001730: 636f 6d6d 616e 6473 2e61 6464 436f 6d6d  commands.addComm
+00001740: 616e 6428 636f 6d6d 616e 642c 207b 0a20  and(command, {. 
+00001750: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00001760: 3a20 2774 6f67 676c 6520 6c69 6365 6e63  : 'toggle licenc
+00001770: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+00001780: 6578 6563 7574 653a 2028 2920 3d3e 2074  execute: () => t
+00001790: 6f67 676c 655f 6c69 6365 6e63 6528 290a  oggle_licence().
+000017a0: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
+000017b0: 2020 2020 7061 6c65 7474 652e 6164 6449      palette.addI
+000017c0: 7465 6d28 7b20 636f 6d6d 616e 642c 2063  tem({ command, c
+000017d0: 6174 6567 6f72 793a 2027 636f 7572 7365  ategory: 'course
+000017e0: 6c65 7665 6c73 2720 7d29 3b0a 2020 2020  levels' });.    
+000017f0: 2020 2020 6170 702e 636f 6d6d 616e 6473      app.commands
+00001800: 2e61 6464 4b65 7942 696e 6469 6e67 287b  .addKeyBinding({
+00001810: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+00001820: 6d61 6e64 2c0a 2020 2020 2020 2020 2020  mand,.          
+00001830: 2020 6b65 7973 3a20 5b27 4374 726c 205c    keys: ['Ctrl \
+00001840: 5c27 2c20 2743 7472 6c20 4c27 5d2c 0a20  \', 'Ctrl L'],. 
+00001850: 2020 2020 2020 2020 2020 2073 656c 6563             selec
+00001860: 746f 723a 2027 2e6a 702d 4e6f 7465 626f  tor: '.jp-Notebo
+00001870: 6f6b 270a 2020 2020 2020 2020 7d29 3b0a  ok'.        });.
+00001880: 2020 2020 2020 2020 2f2f 2074 6865 2062          // the b
+00001890: 7574 746f 6e73 2069 6e20 7468 6520 746f  uttons in the to
+000018a0: 6f6c 6261 720a 2020 2020 2020 2020 636f  olbar.        co
+000018b0: 6e73 7420 6372 6561 7465 5f6c 6576 656c  nst create_level
+000018c0: 5f62 7574 746f 6e73 203d 2028 2920 3d3e  _buttons = () =>
+000018d0: 207b 0a20 2020 2020 2020 2020 2020 2063   {.            c
+000018e0: 6f6e 7374 2066 696e 645f 7370 6163 6572  onst find_spacer
+000018f0: 203d 2028 7061 6e65 6c29 203d 3e20 7b0a   = (panel) => {.
+00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001910: 6c65 7420 696e 6465 7820 3d20 303b 0a20  let index = 0;. 
+00001920: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00001930: 6f72 2028 636f 6e73 7420 6368 696c 6420  or (const child 
+00001940: 6f66 2070 616e 656c 2e74 6f6f 6c62 6172  of panel.toolbar
+00001950: 2e63 6869 6c64 7265 6e28 2929 207b 0a20  .children()) {. 
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2069 6620 2863 6869 6c64 2e6e 6f64     if (child.nod
+00001980: 652e 636c 6173 734c 6973 742e 636f 6e74  e.classList.cont
+00001990: 6169 6e73 2827 6a70 2d54 6f6f 6c62 6172  ains('jp-Toolbar
+000019a0: 2d73 7061 6365 7227 2929 207b 0a20 2020  -spacer')) {.   
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 2020 2020 2072 6574 7572 6e20 696e 6465       return inde
+000019d0: 783b 0a20 2020 2020 2020 2020 2020 2020  x;.             
+000019e0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+000019f0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00001a00: 6520 7b0a 2020 2020 2020 2020 2020 2020  e {.            
+00001a10: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00001a20: 7820 2b3d 2031 3b0a 2020 2020 2020 2020  x += 1;.        
+00001a30: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00001a40: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 7265 7475 726e 2030 3b0a 2020 2020 2020  return 0;.      
+00001a70: 2020 2020 2020 7d3b 0a20 2020 2020 2020        };.       
+00001a80: 2020 2020 2063 6c61 7373 2042 6173 6963       class Basic
+00001a90: 4275 7474 6f6e 207b 0a20 2020 2020 2020  Button {.       
+00001aa0: 2020 2020 2020 2020 2063 7265 6174 654e           createN
+00001ab0: 6577 2870 616e 656c 2c20 636f 6e74 6578  ew(panel, contex
+00001ac0: 7429 207b 0a20 2020 2020 2020 2020 2020  t) {.           
+00001ad0: 2020 2020 2020 2020 2063 6f6e 7374 2062           const b
+00001ae0: 7574 746f 6e20 3d20 6e65 7720 5f6a 7570  utton = new _jup
+00001af0: 7974 6572 6c61 625f 6170 7075 7469 6c73  yterlab_apputils
+00001b00: 5f5f 5745 4250 4143 4b5f 494d 504f 5254  __WEBPACK_IMPORT
+00001b10: 4544 5f4d 4f44 554c 455f 305f 5f2e 546f  ED_MODULE_0__.To
+00001b20: 6f6c 6261 7242 7574 746f 6e28 7b0a 2020  olbarButton({.  
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b40: 2020 2020 2020 636c 6173 734e 616d 653a        className:
+00001b50: 2027 636f 7572 7365 6c65 7665 6c73 2d62   'courselevels-b
+00001b60: 7574 746f 6e27 2c0a 2020 2020 2020 2020  utton',.        
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 6963 6f6e 436c 6173 733a 2027 6661 7220  iconClass: 'far 
+00001b90: 6661 2d68 616e 642d 706f 696e 7465 7227  fa-hand-pointer'
+00001ba0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001bb0: 2020 2020 2020 2020 2020 6f6e 436c 6963            onClic
+00001bc0: 6b3a 2028 2920 3d3e 2074 6f67 676c 655f  k: () => toggle_
+00001bd0: 6c65 7665 6c28 2762 6173 6963 2729 2c0a  level('basic'),.
+00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bf0: 2020 2020 2020 2020 746f 6f6c 7469 703a          tooltip:
+00001c00: 2027 546f 6767 6c65 2062 6173 6963 206c   'Toggle basic l
+00001c10: 6576 656c 270a 2020 2020 2020 2020 2020  evel'.          
+00001c20: 2020 2020 2020 2020 2020 7d29 3b0a 2020            });.  
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 2020 2f2f 2063 6f6d 7075 7465 2077 6865    // compute whe
+00001c50: 7265 2074 6f20 696e 7365 7274 2069 740a  re to insert it.
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 636f 6e73 7420 696e 6465 7820      const index 
+00001c80: 3d20 6669 6e64 5f73 7061 6365 7228 7061  = find_spacer(pa
+00001c90: 6e65 6c29 3b0a 2020 2020 2020 2020 2020  nel);.          
+00001ca0: 2020 2020 2020 2020 2020 7061 6e65 6c2e            panel.
+00001cb0: 746f 6f6c 6261 722e 696e 7365 7274 4974  toolbar.insertIt
+00001cc0: 656d 2869 6e64 6578 2c20 2762 6173 6963  em(index, 'basic
+00001cd0: 4c65 7665 6c27 2c20 6275 7474 6f6e 293b  Level', button);
+00001ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001cf0: 2020 2020 2072 6574 7572 6e20 6e65 7720       return new 
+00001d00: 5f6c 756d 696e 6f5f 6469 7370 6f73 6162  _lumino_disposab
+00001d10: 6c65 5f5f 5745 4250 4143 4b5f 494d 504f  le__WEBPACK_IMPO
+00001d20: 5254 4544 5f4d 4f44 554c 455f 335f 5f2e  RTED_MODULE_3__.
+00001d30: 4469 7370 6f73 6162 6c65 4465 6c65 6761  DisposableDelega
+00001d40: 7465 2828 2920 3d3e 207b 0a20 2020 2020  te(() => {.     
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d60: 2020 2062 7574 746f 6e2e 6469 7370 6f73     button.dispos
+00001d70: 6528 293b 0a20 2020 2020 2020 2020 2020  e();.           
+00001d80: 2020 2020 2020 2020 207d 293b 0a20 2020           });.   
+00001d90: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00001da0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00001db0: 2020 2020 2020 2020 2061 7070 2e64 6f63           app.doc
+00001dc0: 5265 6769 7374 7279 2e61 6464 5769 6467  Registry.addWidg
+00001dd0: 6574 4578 7465 6e73 696f 6e28 274e 6f74  etExtension('Not
+00001de0: 6562 6f6f 6b27 2c20 6e65 7720 4261 7369  ebook', new Basi
+00001df0: 6342 7574 746f 6e28 2929 3b0a 2020 2020  cButton());.    
+00001e00: 2020 2020 2020 2020 636c 6173 7320 496e          class In
+00001e10: 7465 726d 6564 6961 7465 4275 7474 6f6e  termediateButton
+00001e20: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001e30: 2020 2063 7265 6174 654e 6577 2870 616e     createNew(pan
+00001e40: 656c 2c20 636f 6e74 6578 7429 207b 0a20  el, context) {. 
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 2020 2063 6f6e 7374 2062 7574 746f 6e20     const button 
+00001e70: 3d20 6e65 7720 5f6a 7570 7974 6572 6c61  = new _jupyterla
+00001e80: 625f 6170 7075 7469 6c73 5f5f 5745 4250  b_apputils__WEBP
+00001e90: 4143 4b5f 494d 504f 5254 4544 5f4d 4f44  ACK_IMPORTED_MOD
+00001ea0: 554c 455f 305f 5f2e 546f 6f6c 6261 7242  ULE_0__.ToolbarB
+00001eb0: 7574 746f 6e28 7b0a 2020 2020 2020 2020  utton({.        
+00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ed0: 636c 6173 734e 616d 653a 2027 636f 7572  className: 'cour
+00001ee0: 7365 6c65 7665 6c73 2d62 7574 746f 6e27  selevels-button'
+00001ef0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001f00: 2020 2020 2020 2020 2020 6963 6f6e 436c            iconCl
+00001f10: 6173 733a 2027 6661 7220 6661 2d68 616e  ass: 'far fa-han
+00001f20: 642d 7065 6163 6527 2c0a 2020 2020 2020  d-peace',.      
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2020 6f6e 436c 6963 6b3a 2028 2920 3d3e    onClick: () =>
+00001f50: 2074 6f67 676c 655f 6c65 7665 6c28 2769   toggle_level('i
+00001f60: 6e74 6572 6d65 6469 6174 6527 292c 0a20  ntermediate'),. 
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f80: 2020 2020 2020 2074 6f6f 6c74 6970 3a20         tooltip: 
+00001f90: 2754 6f67 676c 6520 696e 7465 726d 6564  'Toggle intermed
+00001fa0: 6961 7465 206c 6576 656c 270a 2020 2020  iate level'.    
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fc0: 7d29 3b0a 2020 2020 2020 2020 2020 2020  });.            
+00001fd0: 2020 2020 2020 2020 2f2f 2063 6f6d 7075          // compu
+00001fe0: 7465 2077 6865 7265 2074 6f20 696e 7365  te where to inse
+00001ff0: 7274 2069 740a 2020 2020 2020 2020 2020  rt it.          
+00002000: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
+00002010: 696e 6465 7820 3d20 6669 6e64 5f73 7061  index = find_spa
+00002020: 6365 7228 7061 6e65 6c29 3b0a 2020 2020  cer(panel);.    
+00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002040: 7061 6e65 6c2e 746f 6f6c 6261 722e 696e  panel.toolbar.in
+00002050: 7365 7274 4974 656d 2869 6e64 6578 2c20  sertItem(index, 
+00002060: 2769 6e74 6572 6d65 6469 6174 654c 6576  'intermediateLev
+00002070: 656c 272c 2062 7574 746f 6e29 3b0a 2020  el', button);.  
+00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002090: 2020 7265 7475 726e 206e 6577 205f 6c75    return new _lu
+000020a0: 6d69 6e6f 5f64 6973 706f 7361 626c 655f  mino_disposable_
+000020b0: 5f57 4542 5041 434b 5f49 4d50 4f52 5445  _WEBPACK_IMPORTE
+000020c0: 445f 4d4f 4455 4c45 5f33 5f5f 2e44 6973  D_MODULE_3__.Dis
+000020d0: 706f 7361 626c 6544 656c 6567 6174 6528  posableDelegate(
+000020e0: 2829 203d 3e20 7b0a 2020 2020 2020 2020  () => {.        
+000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002100: 6275 7474 6f6e 2e64 6973 706f 7365 2829  button.dispose()
+00002110: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00002120: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
+00002130: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00002140: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002150: 2020 2020 2020 6170 702e 646f 6352 6567        app.docReg
+00002160: 6973 7472 792e 6164 6457 6964 6765 7445  istry.addWidgetE
+00002170: 7874 656e 7369 6f6e 2827 4e6f 7465 626f  xtension('Notebo
+00002180: 6f6b 272c 206e 6577 2049 6e74 6572 6d65  ok', new Interme
+00002190: 6469 6174 6542 7574 746f 6e28 2929 3b0a  diateButton());.
+000021a0: 2020 2020 2020 2020 2020 2020 636c 6173              clas
+000021b0: 7320 4164 7661 6e63 6564 4275 7474 6f6e  s AdvancedButton
+000021c0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000021d0: 2020 2063 7265 6174 654e 6577 2870 616e     createNew(pan
+000021e0: 656c 2c20 636f 6e74 6578 7429 207b 0a20  el, context) {. 
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002200: 2020 2063 6f6e 7374 2062 7574 746f 6e20     const button 
+00002210: 3d20 6e65 7720 5f6a 7570 7974 6572 6c61  = new _jupyterla
+00002220: 625f 6170 7075 7469 6c73 5f5f 5745 4250  b_apputils__WEBP
+00002230: 4143 4b5f 494d 504f 5254 4544 5f4d 4f44  ACK_IMPORTED_MOD
+00002240: 554c 455f 305f 5f2e 546f 6f6c 6261 7242  ULE_0__.ToolbarB
+00002250: 7574 746f 6e28 7b0a 2020 2020 2020 2020  utton({.        
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 636c 6173 734e 616d 653a 2027 636f 7572  className: 'cour
+00002280: 7365 6c65 7665 6c73 2d62 7574 746f 6e27  selevels-button'
+00002290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000022a0: 2020 2020 2020 2020 2020 6963 6f6e 436c            iconCl
+000022b0: 6173 733a 2027 6661 7220 6661 2d68 616e  ass: 'far fa-han
+000022c0: 642d 7370 6f63 6b27 2c0a 2020 2020 2020  d-spock',.      
+000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022e0: 2020 6f6e 436c 6963 6b3a 2028 2920 3d3e    onClick: () =>
+000022f0: 2074 6f67 676c 655f 6c65 7665 6c28 2761   toggle_level('a
+00002300: 6476 616e 6365 6427 292c 0a20 2020 2020  dvanced'),.     
+00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002320: 2020 2074 6f6f 6c74 6970 3a20 2754 6f67     tooltip: 'Tog
+00002330: 676c 6520 6164 7661 6e63 6564 206c 6576  gle advanced lev
+00002340: 656c 270a 2020 2020 2020 2020 2020 2020  el'.            
+00002350: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 2f2f 2063 6f6d 7075 7465 2077 6865 7265  // compute where
+00002380: 2074 6f20 696e 7365 7274 2069 740a 2020   to insert it.  
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 636f 6e73 7420 696e 6465 7820 3d20    const index = 
+000023b0: 6669 6e64 5f73 7061 6365 7228 7061 6e65  find_spacer(pane
+000023c0: 6c29 3b0a 2020 2020 2020 2020 2020 2020  l);.            
+000023d0: 2020 2020 2020 2020 7061 6e65 6c2e 746f          panel.to
+000023e0: 6f6c 6261 722e 696e 7365 7274 4974 656d  olbar.insertItem
+000023f0: 2869 6e64 6578 2c20 2761 6476 616e 6365  (index, 'advance
+00002400: 644c 6576 656c 272c 2062 7574 746f 6e29  dLevel', button)
+00002410: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00002420: 2020 2020 2020 7265 7475 726e 206e 6577        return new
+00002430: 205f 6c75 6d69 6e6f 5f64 6973 706f 7361   _lumino_disposa
+00002440: 626c 655f 5f57 4542 5041 434b 5f49 4d50  ble__WEBPACK_IMP
+00002450: 4f52 5445 445f 4d4f 4455 4c45 5f33 5f5f  ORTED_MODULE_3__
+00002460: 2e44 6973 706f 7361 626c 6544 656c 6567  .DisposableDeleg
+00002470: 6174 6528 2829 203d 3e20 7b0a 2020 2020  ate(() => {.    
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2020 2020 6275 7474 6f6e 2e64 6973 706f      button.dispo
+000024a0: 7365 2829 3b0a 2020 2020 2020 2020 2020  se();.          
+000024b0: 2020 2020 2020 2020 2020 7d29 3b0a 2020            });.  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+000024d0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+000024e0: 2020 2020 2020 2020 2020 6170 702e 646f            app.do
+000024f0: 6352 6567 6973 7472 792e 6164 6457 6964  cRegistry.addWid
+00002500: 6765 7445 7874 656e 7369 6f6e 2827 4e6f  getExtension('No
+00002510: 7465 626f 6f6b 272c 206e 6577 2041 6476  tebook', new Adv
+00002520: 616e 6365 6442 7574 746f 6e28 2929 3b0a  ancedButton());.
+00002530: 2020 2020 2020 2020 2020 2020 636c 6173              clas
+00002540: 7320 4672 616d 6542 7574 746f 6e20 7b0a  s FrameButton {.
+00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002560: 6372 6561 7465 4e65 7728 7061 6e65 6c2c  createNew(panel,
+00002570: 2063 6f6e 7465 7874 2920 7b0a 2020 2020   context) {.    
+00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002590: 636f 6e73 7420 6275 7474 6f6e 203d 206e  const button = n
+000025a0: 6577 205f 6a75 7079 7465 726c 6162 5f61  ew _jupyterlab_a
+000025b0: 7070 7574 696c 735f 5f57 4542 5041 434b  pputils__WEBPACK
+000025c0: 5f49 4d50 4f52 5445 445f 4d4f 4455 4c45  _IMPORTED_MODULE
+000025d0: 5f30 5f5f 2e54 6f6f 6c62 6172 4275 7474  _0__.ToolbarButt
+000025e0: 6f6e 287b 0a20 2020 2020 2020 2020 2020  on({.           
+000025f0: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
+00002600: 7373 4e61 6d65 3a20 2763 6f75 7273 656c  ssName: 'coursel
+00002610: 6576 656c 732d 6275 7474 6f6e 272c 0a20  evels-button',. 
+00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002630: 2020 2020 2020 2069 636f 6e43 6c61 7373         iconClass
+00002640: 3a20 2766 6173 2066 612d 6372 6f70 2d61  : 'fas fa-crop-a
+00002650: 6c74 272c 0a20 2020 2020 2020 2020 2020  lt',.           
+00002660: 2020 2020 2020 2020 2020 2020 206f 6e43               onC
+00002670: 6c69 636b 3a20 2829 203d 3e20 746f 6767  lick: () => togg
+00002680: 6c65 5f66 7261 6d65 2829 2c0a 2020 2020  le_frame(),.    
+00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026a0: 2020 2020 746f 6f6c 7469 703a 2027 546f      tooltip: 'To
+000026b0: 6767 6c65 2066 7261 6d65 2061 726f 756e  ggle frame aroun
+000026c0: 6420 6365 6c6c 270a 2020 2020 2020 2020  d cell'.        
+000026d0: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
+000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026f0: 2020 2020 2f2f 2063 6f6d 7075 7465 2077      // compute w
+00002700: 6865 7265 2074 6f20 696e 7365 7274 2069  here to insert i
+00002710: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00002720: 2020 2020 2020 636f 6e73 7420 696e 6465        const inde
+00002730: 7820 3d20 6669 6e64 5f73 7061 6365 7228  x = find_spacer(
+00002740: 7061 6e65 6c29 3b0a 2020 2020 2020 2020  panel);.        
+00002750: 2020 2020 2020 2020 2020 2020 7061 6e65              pane
+00002760: 6c2e 746f 6f6c 6261 722e 696e 7365 7274  l.toolbar.insert
+00002770: 4974 656d 2869 6e64 6578 2c20 2766 7261  Item(index, 'fra
+00002780: 6d65 4c65 7665 6c27 2c20 6275 7474 6f6e  meLevel', button
+00002790: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+000027a0: 2020 2020 2020 2072 6574 7572 6e20 6e65         return ne
+000027b0: 7720 5f6c 756d 696e 6f5f 6469 7370 6f73  w _lumino_dispos
+000027c0: 6162 6c65 5f5f 5745 4250 4143 4b5f 494d  able__WEBPACK_IM
+000027d0: 504f 5254 4544 5f4d 4f44 554c 455f 335f  PORTED_MODULE_3_
+000027e0: 5f2e 4469 7370 6f73 6162 6c65 4465 6c65  _.DisposableDele
+000027f0: 6761 7465 2828 2920 3d3e 207b 0a20 2020  gate(() => {.   
+00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002810: 2020 2020 2062 7574 746f 6e2e 6469 7370       button.disp
+00002820: 6f73 6528 293b 0a20 2020 2020 2020 2020  ose();.         
+00002830: 2020 2020 2020 2020 2020 207d 293b 0a20             });. 
+00002840: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00002850: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00002860: 2020 2020 2020 2020 2020 2061 7070 2e64             app.d
+00002870: 6f63 5265 6769 7374 7279 2e61 6464 5769  ocRegistry.addWi
+00002880: 6467 6574 4578 7465 6e73 696f 6e28 274e  dgetExtension('N
+00002890: 6f74 6562 6f6f 6b27 2c20 6e65 7720 4672  otebook', new Fr
+000028a0: 616d 6542 7574 746f 6e28 2929 3b0a 2020  ameButton());.  
+000028b0: 2020 2020 2020 7d3b 0a20 2020 2020 2020        };.       
+000028c0: 202f 2f20 6c6f 6164 2073 6574 7469 6e67   // load setting
+000028d0: 7320 616e 6420 6372 6561 7465 2062 7574  s and create but
+000028e0: 746f 6e73 2069 6620 7265 7175 6573 7465  tons if requeste
+000028f0: 640a 2020 2020 2020 2020 6675 6e63 7469  d.        functi
+00002900: 6f6e 206c 6f61 6453 6574 7469 6e67 2873  on loadSetting(s
+00002910: 6574 7469 6e67 2920 7b0a 2020 2020 2020  etting) {.      
+00002920: 2020 2020 2020 2f2f 2052 6561 6420 7468        // Read th
+00002930: 6520 7365 7474 696e 6773 2061 6e64 2063  e settings and c
+00002940: 6f6e 7665 7274 2074 6f20 7468 6520 636f  onvert to the co
+00002950: 7272 6563 7420 7479 7065 0a20 2020 2020  rrect type.     
+00002960: 2020 2020 2020 2073 686f 775f 6c65 7665         show_leve
+00002970: 6c5f 6275 7474 6f6e 7320 3d20 7365 7474  l_buttons = sett
+00002980: 696e 672e 6765 7428 2773 686f 775f 6c65  ing.get('show_le
+00002990: 7665 6c5f 6275 7474 6f6e 7327 290a 2020  vel_buttons').  
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2e63                .c
+000029b0: 6f6d 706f 7369 7465 3b0a 2020 2020 2020  omposite;.      
+000029c0: 2020 2020 2020 636f 6e73 6f6c 652e 6c6f        console.lo
+000029d0: 6728 606a 7570 7974 6572 6c61 622d 636f  g(`jupyterlab-co
+000029e0: 7572 7365 6c65 7665 6c73 2065 7874 656e  urselevels exten
+000029f0: 7369 6f6e 3a20 7368 6f77 5f6c 6576 656c  sion: show_level
+00002a00: 5f62 7574 746f 6e73 2069 7320 7365 7420  _buttons is set 
+00002a10: 746f 2024 7b73 686f 775f 6c65 7665 6c5f  to ${show_level_
+00002a20: 6275 7474 6f6e 737d 6029 3b0a 2020 2020  buttons}`);.    
+00002a30: 2020 2020 2020 2020 6966 2028 7368 6f77          if (show
+00002a40: 5f6c 6576 656c 5f62 7574 746f 6e73 2920  _level_buttons) 
+00002a50: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002a60: 2020 6372 6561 7465 5f6c 6576 656c 5f62    create_level_b
+00002a70: 7574 746f 6e73 2829 3b0a 2020 2020 2020  uttons();.      
+00002a80: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00002a90: 7d0a 2020 2020 2020 2020 2f2f 2062 7574  }.        // but
+00002aa0: 2064 6f20 6974 206f 6e6c 7920 6166 7465   do it only afte
+00002ab0: 7220 7468 6520 6170 7020 6861 7320 7374  r the app has st
+00002ac0: 6172 7465 640a 2020 2020 2020 2020 5072  arted.        Pr
+00002ad0: 6f6d 6973 652e 616c 6c28 5b61 7070 2e72  omise.all([app.r
+00002ae0: 6573 746f 7265 642c 2073 6574 7469 6e67  estored, setting
+00002af0: 5265 6769 7374 7279 2e6c 6f61 6428 504c  Registry.load(PL
+00002b00: 5547 494e 5f49 4429 5d29 2e74 6865 6e28  UGIN_ID)]).then(
+00002b10: 285b 5f2c 2073 6574 7469 6e67 5d29 203d  ([_, setting]) =
+00002b20: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
+00002b30: 6c6f 6164 5365 7474 696e 6728 7365 7474  loadSetting(sett
+00002b40: 696e 6729 3b0a 2020 2020 2020 2020 2020  ing);.          
+00002b50: 2020 7365 7474 696e 672e 6368 616e 6765    setting.change
+00002b60: 642e 636f 6e6e 6563 7428 6c6f 6164 5365  d.connect(loadSe
+00002b70: 7474 696e 6729 3b0a 2020 2020 2020 2020  tting);.        
+00002b80: 7d29 3b0a 2020 2020 7d0a 7d3b 0a2f 2a20  });.    }.};./* 
+00002b90: 6861 726d 6f6e 7920 6465 6661 756c 7420  harmony default 
+00002ba0: 6578 706f 7274 202a 2f20 636f 6e73 7420  export */ const 
+00002bb0: 5f5f 5745 4250 4143 4b5f 4445 4641 554c  __WEBPACK_DEFAUL
+00002bc0: 545f 4558 504f 5254 5f5f 203d 2028 706c  T_EXPORT__ = (pl
+00002bd0: 7567 696e 293b 0a0a 0a2f 2a2a 2a2f 207d  ugin);.../***/ }
+00002be0: 290a 0a7d 5d29 3b0a 2f2f 2320 736f 7572  )..}]);.//# sour
+00002bf0: 6365 4d61 7070 696e 6755 524c 3d6c 6962  ceMappingURL=lib
+00002c00: 5f69 6e64 6578 5f6a 732e 3235 6662 6532  _index_js.25fbe2
+00002c10: 6636 3538 3164 3061 3737 3762 3166 2e6a  f6581d0a777b1f.j
+00002c20: 732e 6d61 70                             s.map
```

### Comparing `jupyterlab_courselevels-0.6.4/style/base.css` & `jupyterlab_courselevels-0.8.1/style/base.css`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 .courselevels-button {
   color: rgb(68, 36, 127);
   background-color: rgb(229, 228, 228) !important;
   border: 1px solid #400 !important;
   border-radius: 3px;
 }
 
-
 .jp-Notebook {
-
   & .cell-tag-level_basic {
     background-color: #c7e8c7 !important;
     border: 1px solid #040;
     border-radius: 10px;
     margin-bottom: 6px;
   }
```

### Comparing `jupyterlab_courselevels-0.6.4/.gitignore` & `jupyterlab_courselevels-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.6.4/LICENSE` & `jupyterlab_courselevels-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.6.4/README.md` & `jupyterlab_courselevels-0.8.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 
   - green : basic - all students should know that
   - blue : intermediate - if you want to dig a little more
   - red : advanced - for the geeks
 
 - in addition some cells may show up with a surrounding frame, to emphasize the course structure
 
-- the extension also comes with convenience tools to manage admonitions
-
 ## Important limitation
 
 because of the way MyST markdown is rendered, colors and frames are correctly
 rendered within Jupyter Lab, but they will **not render properly on code cells in
 the jupyter-book output**
 
-For this reason, colors and frames are no longer relevant on markdown cells,
+For this reason, colors and frames are **no longer relevant on markdown cells**,
 and we use admonition instead
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
@@ -51,30 +49,14 @@
 |   `courselevels:toggle-intermediate`   | `Ctrl-\ Ctrl-Y` |
 |     `courselevels:toggle-advanced`     | `Ctrl-\ Ctrl-Z` |
 |      `courselevels:toggle-frame`       | `Ctrl-\ Ctrl-M` |
 |     `courselevels:toggle-licence`      | `Ctrl-\ Ctrl-L` |
 | `courselevels:metadata-clean-selected` |   `Alt-Cmd-7`   | clean metadata on selected cells |
 |   `courselevels:metadata-clean-all`    |  `Ctrl-Alt-7`   | clean metadata on all cells      |
 
-as well as for adding/removing an admonition around a cell
-
-|                command                |   keybinding    |
-| :-----------------------------------: | :-------------: |
-|   `courselevels:toggle-admonition`    | `Ctrl-\ Ctrl-A` |
-| `courselevels:toggle-admonition-tip`  | `Ctrl-\ Ctrl-T` |
-| `courselevels:toggle-admonition-note` | `Ctrl-\ Ctrl-N` |
-|    `courselevels:toggle-attention`    |                 |
-|     `courselevels:toggle-caution`     |                 |
-|     `courselevels:toggle-danger`      |                 |
-|      `courselevels:toggle-error`      |                 |
-|      `courselevels:toggle-hint`       |                 |
-|    `courselevels:toggle-important`    |                 |
-|     `courselevels:toggle-seealso`     |                 |
-|     `courselevels:toggle-warning`     |                 |
-
 ### persistence
 
 this is done by adding the following tags in each cell
 
 - `level_basic`
 - `level_intermediate`
 - `level_advanced`
```

### Comparing `jupyterlab_courselevels-0.6.4/pyproject.toml` & `jupyterlab_courselevels-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.6.4/PKG-INFO` & `jupyterlab_courselevels-0.8.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab_courselevels
-Version: 0.6.4
+Version: 0.8.1
+Dynamic: Keywords
 Summary: Jlab extension for showing course levels and structure
 Project-URL: Homepage, https://github.com/parmentelat/jupyterlab-courselevels
 Project-URL: Bug Tracker, https://github.com/parmentelat/jupyterlab-courselevels/issues
 Project-URL: Repository, https://github.com/parmentelat/jupyterlab-courselevels.git
 Author-email: Thierry Parmentelat <thierry.parmentelat@inria.fr>
 License: BSD 3-Clause License
         
@@ -64,23 +65,21 @@
 
   - green : basic - all students should know that
   - blue : intermediate - if you want to dig a little more
   - red : advanced - for the geeks
 
 - in addition some cells may show up with a surrounding frame, to emphasize the course structure
 
-- the extension also comes with convenience tools to manage admonitions
-
 ## Important limitation
 
 because of the way MyST markdown is rendered, colors and frames are correctly
 rendered within Jupyter Lab, but they will **not render properly on code cells in
 the jupyter-book output**
 
-For this reason, colors and frames are no longer relevant on markdown cells,
+For this reason, colors and frames are **no longer relevant on markdown cells**,
 and we use admonition instead
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
@@ -107,30 +106,14 @@
 |   `courselevels:toggle-intermediate`   | `Ctrl-\ Ctrl-Y` |
 |     `courselevels:toggle-advanced`     | `Ctrl-\ Ctrl-Z` |
 |      `courselevels:toggle-frame`       | `Ctrl-\ Ctrl-M` |
 |     `courselevels:toggle-licence`      | `Ctrl-\ Ctrl-L` |
 | `courselevels:metadata-clean-selected` |   `Alt-Cmd-7`   | clean metadata on selected cells |
 |   `courselevels:metadata-clean-all`    |  `Ctrl-Alt-7`   | clean metadata on all cells      |
 
-as well as for adding/removing an admonition around a cell
-
-|                command                |   keybinding    |
-| :-----------------------------------: | :-------------: |
-|   `courselevels:toggle-admonition`    | `Ctrl-\ Ctrl-A` |
-| `courselevels:toggle-admonition-tip`  | `Ctrl-\ Ctrl-T` |
-| `courselevels:toggle-admonition-note` | `Ctrl-\ Ctrl-N` |
-|    `courselevels:toggle-attention`    |                 |
-|     `courselevels:toggle-caution`     |                 |
-|     `courselevels:toggle-danger`      |                 |
-|      `courselevels:toggle-error`      |                 |
-|      `courselevels:toggle-hint`       |                 |
-|    `courselevels:toggle-important`    |                 |
-|     `courselevels:toggle-seealso`     |                 |
-|     `courselevels:toggle-warning`     |                 |
-
 ### persistence
 
 this is done by adding the following tags in each cell
 
 - `level_basic`
 - `level_intermediate`
 - `level_advanced`
```

