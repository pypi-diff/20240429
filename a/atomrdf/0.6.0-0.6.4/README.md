# Comparing `tmp/atomrdf-0.6.0.tar.gz` & `tmp/atomrdf-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomrdf-0.6.0.tar", last modified: Fri Apr 19 14:49:53 2024, max compression
+gzip compressed data, was "atomrdf-0.6.4.tar", last modified: Mon Apr 29 20:45:59 2024, max compression
```

## Comparing `atomrdf-0.6.0.tar` & `atomrdf-0.6.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.227151 atomrdf-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 14:49:50.000000 atomrdf-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 14:49:50.000000 atomrdf-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-19 14:49:53.227151 atomrdf-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-19 14:49:50.000000 atomrdf-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.219151 atomrdf-0.6.0/atomrdf/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.223151 atomrdf-0.6.0/atomrdf/data/
--rw-r--r--   0 runner    (1001) docker     (127)    52930 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/asmo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/cmso.owl
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/dft_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/element.yml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/md_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/pldo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/podo.owl
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    38627 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/json_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.223151 atomrdf-0.6.0/atomrdf/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/term.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    59158 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.223151 atomrdf-0.6.0/atomrdf/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/workflow/pyiron.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.227151 atomrdf-0.6.0/atomrdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:49:53.227151 atomrdf-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 14:49:52.000000 atomrdf-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.227151 atomrdf-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_structuregraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_term.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_visualise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.375579 atomrdf-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 20:45:56.000000 atomrdf-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 20:45:56.000000 atomrdf-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-29 20:45:59.375579 atomrdf-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-29 20:45:56.000000 atomrdf-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.367579 atomrdf-0.6.4/atomrdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.371579 atomrdf-0.6.4/atomrdf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    52930 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/asmo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/cmso.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/dft_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/md_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/pldo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/podo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38763 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.371579 atomrdf-0.6.4/atomrdf/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59158 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.371579 atomrdf-0.6.4/atomrdf/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/workflow/pyiron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.375579 atomrdf-0.6.4/atomrdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:45:59.375579 atomrdf-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-29 20:45:59.000000 atomrdf-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.375579 atomrdf-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_structuregraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_visualise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_workflow.py
```

### Comparing `atomrdf-0.6.0/LICENSE` & `atomrdf-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/PKG-INFO` & `atomrdf-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomrdf
-Version: 0.6.0
+Version: 0.6.4
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/atomrdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `atomrdf-0.6.0/README.md` & `atomrdf-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/data/asmo.owl` & `atomrdf-0.6.4/atomrdf/data/asmo.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/data/cmso.owl` & `atomrdf-0.6.4/atomrdf/data/cmso.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/data/element.yml` & `atomrdf-0.6.4/atomrdf/data/element.yml`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/data/md_template.yml` & `atomrdf-0.6.4/atomrdf/data/md_template.yml`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/data/pldo.owl` & `atomrdf-0.6.4/atomrdf/data/pldo.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/data/podo.owl` & `atomrdf-0.6.4/atomrdf/data/podo.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/graph.py` & `atomrdf-0.6.4/atomrdf/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -906,127 +906,131 @@
         """
         if compress:
             package_base_name = ".".join(package_name.split(".")[:-2])
             with tarfile.open(package_name) as fin:
                 fin.extractall(".")
             # os.remove(package_name)
             # copy things out
+        else:
+            package_base_name = package_name
 
         return cls(
             store=store,
             store_file=store_file,
             identifier=identifier,
             graph_file=f"{package_base_name}/triples",
             structure_store=f"{package_base_name}/rdf_structure_store",
             ontology=ontology,
         )
 
-    def query(self, inquery):
+    def query(self, inquery, return_df=True):
         """
         Query the graph using SPARQL
 
         Parameters
         ----------
         inquery: string
             SPARQL query to be executed
 
+        return_df: bool, optional
+            if True, returns the results as a pandas DataFrame. Default is True.
         Returns
         -------
         res: pandas DataFrame
             pandas dataframe results
         """
         res = self.graph.query(inquery)
         if res is not None:
-            for line in inquery.split("\n"):
-                if "SELECT DISTINCT" in line:
-                    break
-            labels = [x[1:] for x in line.split()[2:]]
-            return pd.DataFrame(res, columns=labels)
+            if return_df:
+                for line in inquery.split("\n"):
+                    if "SELECT DISTINCT" in line:
+                        break
+                labels = [x[1:] for x in line.split()[2:]]
+                return pd.DataFrame(res, columns=labels)
+            else:
+                return res
         raise ValueError("SPARQL query returned None")
 
     def auto_query(
         self,
         source,
         destination,
-        condition=None,
         return_query=False,
         enforce_types=None,
+        return_df=True,
     ):
         """
         Automatically generates and executes a query based on the provided parameters.
 
         Parameters
         ----------
         source : OntoTerm
             The source of the query.
         destination : OntoTerm
             The destination of the query.
-        condition :str, optional
-            The condition to be applied in the query. Defaults to None.
         return_query : bool, optional
             If True, returns the generated query instead of executing it. Defaults to False.
         enforce_types : bool, optional
             If provided, enforces the specified type for the query. Defaults to None.
+        return_df: bool, optional
+            if True, returns the results as a pandas DataFrame. Default is True.
 
         Returns
         -------
         pandas DataFrame or str
             The result of the query execution. If `return_query` is True, returns the generated query as a string.
             Otherwise, returns the result of the query execution as a pandas DataFrame.
         """
         if enforce_types is None:
             for val in [True, False]:
                 query = self.ontology.create_query(
-                    source, destination, condition=condition, enforce_types=val
+                    source, destination, enforce_types=val
                 )
                 if return_query:
                     return query
-                res = self.query(query)
+                res = self.query(query, return_df=return_df)
                 if len(res) != 0:
                     return res
         else:
             query = self.ontology.create_query(
-                source, destination, condition=condition, enforce_types=enforce_types
+                source, destination, enforce_types=enforce_types
             )
             if return_query:
                 return query
-            res = self.query(query)
+            res = self.query(query, return_df=return_df)
 
         return res
 
     #################################
     # Methods to interact with sample
     #################################
     def query_sample(
-        self, destination, condition=None, return_query=False, enforce_types=None
+        self, destination, return_query=False, enforce_types=None
     ):
         """
         Query the knowledge graph for atomic scale samples.
 
         Parameters
         ----------
         destination : OntoTerm
             The destination of the query.
-        condition : str, optional
-            The condition to be applied in the query. Defaults to None.
         return_query : bool, optional
             If True, returns the generated query instead of executing it. Defaults to False.
         enforce_types : bool, optional
             If provided, enforces the specified type for the query. Defaults to None.
 
         Returns
         -------
         pandas DataFrame or str
             The result of the query execution. If `return_query` is True, returns the generated query as a string. Otherwise, returns the result of the query execution as a pandas DataFrame.
 
         """
         return self.auto_query(
             self.ontology.terms.cmso.AtomicScaleSample,
             destination,
-            condition=condition,
             return_query=return_query,
             enforce_types=enforce_types,
         )
 
     @property
     def n_samples(self):
         """
```

### Comparing `atomrdf-0.6.0/atomrdf/json_io.py` & `atomrdf-0.6.4/atomrdf/json_io.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/namespace.py` & `atomrdf-0.6.4/atomrdf/namespace.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/network/network.py` & `atomrdf-0.6.4/atomrdf/network/network.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,43 +78,14 @@
     @property
     def extra_namespaces(self):
         return self.onto.extra_namespaces
 
     def __radd__(self, ontonetwork):
         return self.__add__(ontonetwork)
 
-    def get_shortest_path(self, source, target, triples=False):
-        """
-        Compute the shortest path between two nodes in the graph.
-
-        Parameters:
-        -----------
-        source : node
-            The starting node for the path.
-        target : node
-            The target node for the path.
-        triples : bool, optional
-            If True, returns the path as a list of triples. Each triple consists of three consecutive nodes in the path.
-            If False, returns the path as a list of nodes.
-
-        Returns:
-        --------
-        path : list
-            The shortest path between the source and target nodes. If `triples` is True, the path is returned as a list of triples.
-            If `triples` is False, the path is returned as a list of nodes.
-
-        """
-        path = nx.shortest_path(self.g, source=source, target=target)
-        if triples:
-            triple_list = []
-            for x in range(len(path) // 2):
-                triple_list.append(path[2 * x : 2 * x + 3])
-            return triple_list
-        return path
-
     def _add_class_nodes(self):
         for key, val in self.onto.attributes["class"].items():
             self.g.add_node(val.name, node_type="class")
 
     def _add_object_properties(self):
         for key, val in self.onto.attributes["object_property"].items():
             self.g.add_node(val.name, node_type="object_property")
@@ -214,15 +185,14 @@
     def add_path(self, triple):
         """
         Add a triple as path.
 
         Note that all attributes of the triple should already exist in the graph.
         The ontology itself is not modified. Only the graph representation of it is.
         The expected use is to bridge between two (or more) different ontologies.
-        Therefore, mapping can only be between classes.
 
         Parameters
         ----------
         triple : tuple
         A tuple representing the triple to be added. The tuple should contain three elements:
         subject, predicate, and object.
 
@@ -301,123 +271,198 @@
             if node[1] is not None:
                 t = node[1]
                 dot.node(name, shape=styledict[t]["shape"], fontsize="6")
         for edge in edge_list:
             dot.edge(_replace_name(edge[0]), _replace_name(edge[1]))
         return dot
 
+    def _get_shortest_path(self, source, target):
+        #this function will be modified to take OntoTerms direcl as input; and use their names. 
+        path = nx.shortest_path(self.g, source=source.query_name, target=target.query_name)
+        #replace the start and end with thier corresponding variable names
+        path[0] = source.variable_name
+        path[-1] = target.variable_name
+        return path
+
+    def get_shortest_path(self, source, target, triples=False):
+        """
+        Compute the shortest path between two nodes in the graph.
+
+        Parameters:
+        -----------
+        source : node
+            The starting node for the path.
+        target : node
+            The target node for the path.
+        triples : bool, optional
+            If True, returns the path as a list of triples. Each triple consists of three consecutive nodes in the path.
+            If False, returns the path as a list of nodes.
+
+        Returns:
+        --------
+        path : list
+            The shortest path between the source and target nodes. If `triples` is True, the path is returned as a list of triples.
+            If `triples` is False, the path is returned as a list of nodes.
+
+        """
+        #this function should also check for stepped queries
+        path = []
+        if len(target._parents) > 0:
+            #this needs a stepped query
+            complete_list = [source, *target._parents, target]
+            #get path for first two terms
+            path = self._get_shortest_path(complete_list[0], complete_list[1])
+            for x in range(2, len(complete_list)):
+                temp_source = complete_list[x-1]
+                temp_dest = complete_list[x]
+                temp_path = self._get_shortest_path(temp_source, temp_dest)
+                path.extend(temp_path[1:])                
+        else:
+            path = self._get_shortest_path(source, target)
+
+        if triples:
+            triple_list = []
+            for x in range(len(path) // 2):
+                triple_list.append(path[2 * x : 2 * x + 3])
+            return triple_list
+        
+        return path
+    
     def get_path_from_sample(self, target):
         """
         Get the shortest path from the 'cmso:ComputationalSample' node to the target node.
 
         Parameters
         ----------
         target : OntoTerm
             The target node to find the shortest path to.
 
         Returns
         -------
         list
             A list of triples representing the shortest path from 'cmso:ComputationalSample' to the target node.
         """
+        #get the path
         path = self.get_shortest_path(
-            source="cmso:ComputationalSample", target=target, triples=True
+            source=self.terms.cmso.AtomicScaleSample, target=target, triples=True
         )
         return path
 
-    def create_query(self, source, destinations, condition=None, enforce_types=True):
+    def create_query(self, source, destinations, enforce_types=True):
         """
         Create a SPARQL query string based on the given source, destinations, condition, and enforce_types.
 
         Parameters
         ----------
         source : Node
             The source node from which the query starts.
         destinations : list or Node
             The destination node(s) to which the query should reach. If a single node is provided, it will be converted to a list.
-        condition : Condition, optional
-            The condition to be applied in the query. Defaults to None.
         enforce_types : bool, optional
             Whether to enforce the types of the source and destination nodes in the query. Defaults to True.
 
         Returns
         -------
         str
             The generated SPARQL query string.
 
         """
+        #if not list, convert to list
         if not isinstance(destinations, list):
             destinations = [destinations]
 
-        source_name = source.query_name
-        destination_names = [destination.query_name for destination in destinations]
-
-        # if condition is specified, and is not there, add it
-        if condition is not None:
-            if condition.query_name not in destination_names:
-                destination_names.append(condition.query_name)
-
-        # add source if not available
-        if source_name not in destination_names:
-            destination_names.append(source_name)
+        # check if more than one of them have an associated condition -> if so throw error
+        no_of_conditions = 0
+        for destination in destinations:
+            if destination._condition is not None:
+                no_of_conditions += 1
+        if no_of_conditions > 1:
+            raise ValueError("Only one condition is allowed")
+        
+        #iterate through the list, if they have condition parents, add them explicitely
+        for destination in destinations:
+            for parent in destination._condition_parents:
+                if parent.name not in [d.name for d in destinations]:
+                    destinations.append(parent)
 
+        #all names are now collected, in a list of lists
         # start prefix of query
         query = []
         for key, val in self.namespaces.items():
             query.append(f"PREFIX {key}: <{val}>")
         for key, val in self.extra_namespaces.items():
             query.append(f"PREFIX {key}: <{val}>")
 
-        # now for each destination, start adding the paths in the query
-        all_triplets = {}
-        for destination in destination_names:
-            triplets = self.get_shortest_path(source_name, destination, triples=True)
-            all_triplets[destination] = triplets
-
+        #construct the select distinct command:
+        #add source `variable_name`
+        #iterate over destinations, add their `variable_name`
         select_destinations = [
-            f"?{self.strip_name(destination)}" for destination in destination_names
+            "?"+destination.variable_name for destination in destinations
         ]
+        select_destinations = ["?"+source.variable_name] + select_destinations
         query.append(f'SELECT DISTINCT {" ".join(select_destinations)}')
         query.append("WHERE {")
-
-        # now add corresponding triples
-        for destination in destination_names:
-            for triple in all_triplets[destination]:
-                # print(triple)
-                query.append(
-                    "    ?%s %s ?%s ."
-                    % (
-                        self.strip_name(triple[0]),
+        
+        #constructing the spaql query path triples, by iterating over destinations
+        #for each destination:
+        #    - check if it has  parent by looking at `._parents`
+        #    - if it has `_parents`, called step path method
+        #    - else just get the path
+        #    - replace the ends of the path with `variable_name`
+        #    - if it deosnt exist in the collection of lines, add the lines
+        all_triplets = {}
+        for count, destination in enumerate(destinations):
+            #print(source, destination)
+            triplets = self.get_shortest_path(source, destination, triples=True)
+            for triple in triplets:
+                #print(triple)
+                line_text =  "    ?%s %s ?%s ."% ( triple[0].replace(":", "_"),
                         triple[1],
-                        self.strip_name(triple[2]),
+                        triple[2].replace(":", "_"),
                     )
-                )
+                if line_text not in query:
+                    query.append(line_text)                
+
 
         # we enforce types of the source and destination
         if enforce_types:
             if source.node_type == "class":
                 query.append(
                     "    ?%s rdf:type %s ."
-                    % (self.strip_name(source.query_name), source.query_name)
+                    % (self.strip_name(source.variable_name), source.query_name)
                 )
+            
             for destination in destinations:
                 if destination.node_type == "class":
                     query.append(
                         "    ?%s rdf:type %s ."
                         % (
-                            self.strip_name(destination.query_name),
+                            destination.variable_name,
                             destination.query_name,
                         )
                     )
-        # now we have to add filters
-        # filters are only needed if it is a dataproperty
+        #- formulate the condition, given by the `FILTER` command:
+        #    - extract the filter text from the term
+        #    - loop over destinations:
+        #        - call `replace(destination.query_name, destination.variable_name)`
         filter_text = ""
 
         # make filters; get all the unique filters from all the classes in destinations
-        if condition is not None:
-            if condition._condition is not None:
-                filter_text = condition._condition
-
+        for destination in destinations:
+            if destination._condition is not None:
+                filter_text = destination._condition
+                break
+        
+        #replace the query_name with variable_name
         if filter_text != "":
+            for destination in destinations:
+                filter_text = filter_text.replace(
+                    destination.query_name, destination.variable_name
+                )
             query.append(f"FILTER {filter_text}")
         query.append("}")
+
+        #finished, clean up the terms; 
+        for destination in destinations:
+            destination.refresh()
+            
         return "\n".join(query)
```

### Comparing `atomrdf-0.6.0/atomrdf/network/ontology.py` & `atomrdf-0.6.4/atomrdf/network/ontology.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,44 +44,58 @@
         "http://www.w3.org/ns/prov#actedOnBehalfOf", "object_property", delimiter="#"
     )
     combo.add_term(
         "http://www.w3.org/2000/01/rdf-schema#label",
         "data_property",
         delimiter="#",
         namespace="rdfs",
+        rn = ['str']
     )
     combo.add_term(
         "http://www.w3.org/1999/02/22-rdf-syntax-ns#type",
         "object_property",
         delimiter="#",
         namespace="rdf",
     )
 
     # add paths
 
     # General fixes
     combo.add_path(("cmso:CrystalStructure", "cmso:hasAltName", "string"))
-    combo.add_path(("cmso:ChemicalElement", "cmso:hasSymbol", "string"))
 
     # interontology paths
     combo.add_path(("cmso:Material", "cmso:hasDefect", "pldo:PlanarDefect"))
     combo.add_path(("cmso:Material", "cmso:hasDefect", "podo:Vacancy"))
     combo.add_path(("cmso:SimulationCell", "podo:hasVacancyConcentration", "float"))
     combo.add_path(("cmso:SimulationCell", "podo:hasNumberOfVacancies", "int"))
     combo.add_path(
         ("cmso:ComputationalSample", "prov:wasDerivedFrom", "cmso:ComputationalSample")
     )
     combo.add_path(("cmso:ComputationalSample", "rdf:type", "prov:Entity"))
+    combo.add_path(("cmso:AtomicScaleSample", "prov:wasGeneratedBy", "prov:Activity"))
     combo.add_path(("asmo:StructureOptimization", "rdf:type", "prov:Activity"))
     combo.add_path(
         ("asmo:StructureOptimization", "prov:wasAssociatedWith", "prov:SoftwareAgent")
     )
     combo.add_path(
         (
             "cmso:ComputationalSample",
             "prov:wasGeneratedBy",
             "asmo:StructureOptimization",
         )
     )
+    
+    combo.add_path(("cmso:CalculatedProperty", "asmo:hasValue", "float"))
+    combo.add_path(("cmso:CalculatedProperty", "rdfs:label", "string"))
+    #how to handle units?
+
+    #input parameters for ASMO
+    combo.add_path(("asmo:InputParameter", "rdfs:label", "string"))
+    combo.add_path(("asmo:InputParameter", "asmo:hasValue", "float"))
+
+    #software agent
+    combo.add_path(("prov:SoftwareAgent", "rdfs:label", "string"))
+    combo.add_path(("asmo:InteratomicPotential", "cmso:hasReference", "string"))
+    combo.add_path(("asmo:InteratomicPotential", "rdfs:label", "string"))
 
     # return
     return combo
```

### Comparing `atomrdf-0.6.0/atomrdf/network/parser.py` & `atomrdf-0.6.4/atomrdf/network/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             term.domain = dm
             term.range = rn
             term.node_type = "data_property"
             self.attributes["data_property"][term.name] = term
             # assign this data
             for d in dm:
                 if d != "owl:Thing":
-                    self.attributes["class"][d].is_range_of.append(term.name)
+                    self.attributes["class"][d].is_domain_of.append(term.name)
 
             # subproperties should be treated the same
 
     def _parse_object_property(self):
         for c in self.tree.object_properties():
             iri = c.iri
             dm = c.domain
@@ -162,19 +162,19 @@
             term.domain = dm
             term.range = rn
             term.node_type = "object_property"
             self.attributes["object_property"][term.name] = term
             for d in dm:
                 if d != "07:owl#Thing":
                     if d in self.attributes["class"]:
-                        self.attributes["class"][d].is_range_of.append(term.name)
+                        self.attributes["class"][d].is_domain_of.append(term.name)
             for r in rn:
                 if r != "07:owl#Thing":
-                    if d in self.attributes["class"]:
-                        self.attributes["class"][d].is_domain_of.append(term.name)
+                    if r in self.attributes["class"]:
+                        self.attributes["class"][r].is_range_of.append(term.name)
 
     def _parse_class_basic(self):
         classes = []
         for c in self.tree.classes():
             iri = c.iri
             # print(iri)
             # print(iri)
```

### Comparing `atomrdf-0.6.0/atomrdf/network/term.py` & `atomrdf-0.6.4/atomrdf/network/term.py`

 * *Files 25% similar despite different names*

```diff
@@ -71,14 +71,20 @@
         self.delimiter = delimiter
         self.is_domain_of = []
         self.is_range_of = []
         self._condition = None
         self._namespace = namespace
         # name of the class
         self._name = None
+        #parents for the class; these are accumulated
+        #when using the >> operator
+        self._parents = []
+        #condition parents are the parents that have conditions
+        #these are accumulated when using the & or || operators
+        self._condition_parents = []
 
     @property
     def uri(self):
         """
         Get the URI of the ontology term.
 
         Returns
@@ -185,17 +191,41 @@
         Notes
         -----
         If the term is a data property, the name will be appended with "value".
 
         """
         if self.node_type == "data_property":
             return self.name + "value"
+        elif self.node_type == "object_property":
+            if len(self.range) > 0:
+                #this has a domain
+                return self.range[0]
         return self.name
 
     @property
+    def variable_name(self):
+        """
+        Get the name of the term to use as a variable in a SPARQL query.
+
+        Returns
+        -------
+        str
+            The name of the term in a SPARQL query.
+
+        """
+        name_list = [x.name_without_prefix for x in self._parents]
+        name_list.append(self.name_without_prefix)
+        name =  "_".join(name_list) 
+        
+        if self.node_type == "data_property":
+            return name + "value"
+        
+        return name
+
+    @property
     def query_name_without_prefix(self):
         """
         Get the name of the term as it appears in a SPARQL query without prefix.
 
         Returns
         -------
         str
@@ -236,17 +266,19 @@
             raise TypeError("can only be performed with a number!")
 
     def _is_data_node(self):
         if not self.node_type == "data_property":
             raise TypeError(
                 "This operation can only be performed with a data property!"
             )
+    
+
 
     def _create_condition_string(self, condition, val):
-        return f'(?{self.query_name_without_prefix}{condition}"{val}"^^xsd:{self._clean_datatype(self.range[0])})'
+        return f'(?{self.query_name}{condition}"{val}"^^xsd:{self._clean_datatype(self.range[0])})'
 
     # overloading operators
     def __eq__(self, val):
         """
         =
         """
         # self._is_number(val)
@@ -288,24 +320,46 @@
         self._is_term(term)
         self._is_data_node()
         term._is_data_node()
         self._ensure_condition_exists()
         term._ensure_condition_exists()
         self._condition = "&&".join([self._condition, term._condition])
         self._condition = f"({self._condition})"
+        self._condition_parents.append(term)
+        #and clean up the inbound term
+        if self.name != term.name:
+            term.refresh_condition()
         return self
 
     def and_(self, term):
         self.__and__(term)
 
     def __or__(self, term):
         self._is_term(term)
         self._is_data_node()
         term._is_data_node()
         self._ensure_condition_exists()
         term._ensure_condition_exists()
         self._condition = "||".join([self._condition, term._condition])
         self._condition = f"({self._condition})"
+        self._condition_parents.append(term)
+        #and clean up the inbound term
+        if self.name != term.name:
+            term.refresh_condition()
         return self
 
     def or_(self, term):
         self.__or__(term)
+
+    def __rshift__(self, term):
+        term._parents.append(self)
+        return term
+    
+    def refresh_condition(self):
+        self._condition = None
+        self._condition_parents = []
+
+    def refresh(self):
+        self._condition = None
+        self._parents = []
+        self._condition_parents = []
+
```

### Comparing `atomrdf-0.6.0/atomrdf/properties.py` & `atomrdf-0.6.4/atomrdf/properties.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/stores.py` & `atomrdf-0.6.4/atomrdf/stores.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/structure.py` & `atomrdf-0.6.4/atomrdf/structure.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/visualize.py` & `atomrdf-0.6.4/atomrdf/visualize.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/workflow/pyiron.py` & `atomrdf-0.6.4/atomrdf/workflow/pyiron.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf/workflow/workflow.py` & `atomrdf-0.6.4/atomrdf/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/atomrdf.egg-info/PKG-INFO` & `atomrdf-0.6.4/atomrdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomrdf
-Version: 0.6.0
+Version: 0.6.4
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/atomrdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `atomrdf-0.6.0/atomrdf.egg-info/SOURCES.txt` & `atomrdf-0.6.4/atomrdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/setup.py` & `atomrdf-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='atomrdf',
-    version='0.6.0',
+    version='0.6.4',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['atomrdf', 'atomrdf.*']),
     zip_safe=False,
```

### Comparing `atomrdf-0.6.0/tests/test_encoder_and_write.py` & `atomrdf-0.6.4/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/tests/test_graph.py` & `atomrdf-0.6.4/tests/test_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -95,20 +95,18 @@
 	    ?structure cmso:hasSpaceGroup ?spgroup .
 	    ?spgroup cmso:hasSpaceGroupSymbol ?symbol .
 	FILTER (?number="4"^^xsd:integer)
 	}"""
 	res = kg.query(query)
 	assert res.symbol.values[0].toPython() == 'Pm-3m'
 
-	res = kg.query_sample(kg.ontology.terms.cmso.hasAltName, 
-	             condition=(kg.ontology.terms.cmso.hasAltName=='bcc'))
+	res = kg.query_sample(kg.ontology.terms.cmso.hasAltName=='bcc')
 	assert res.hasAltNamevalue.values[0].toPython() == 'bcc'
 
-	res = kg.query_sample(kg.ontology.terms.cmso.hasAltName, 
-	             condition=(kg.ontology.terms.cmso.hasAltName=='bcc'),
+	res = kg.query_sample(kg.ontology.terms.cmso.hasAltName=='bcc',
 	             enforce_types=True)
 	assert res.hasAltNamevalue.values[0].toPython() == 'bcc'
 
 def test_extract_sample():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 	sample_graph, no_atoms = kg.get_sample(struct_Fe.sample, no_atoms=True)
```

### Comparing `atomrdf-0.6.0/tests/test_structure.py` & `atomrdf-0.6.4/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/tests/test_structuregraph.py` & `atomrdf-0.6.4/tests/test_structuregraph.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/tests/test_term.py` & `atomrdf-0.6.4/tests/test_term.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,62 +6,62 @@
 
 def test_lt():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 
 	term = kg.ontology.terms.cmso.hasNumberOfAtoms
 	term < 2
-	assert term._condition == '(?hasNumberOfAtomsvalue<"2"^^xsd:int)'
+	assert term._condition == '(?cmso:hasNumberOfAtomsvalue<"2"^^xsd:int)'
 
 def test_eq():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 
 	term = kg.ontology.terms.cmso.hasNumberOfAtoms
 	term == 2
-	assert term._condition == '(?hasNumberOfAtomsvalue="2"^^xsd:int)'	
+	assert term._condition == '(?cmso:hasNumberOfAtomsvalue="2"^^xsd:int)'	
 
 def test_gt():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 
 	term = kg.ontology.terms.cmso.hasNumberOfAtoms
 	term > 2
-	assert term._condition == '(?hasNumberOfAtomsvalue>"2"^^xsd:int)'
+	assert term._condition == '(?cmso:hasNumberOfAtomsvalue>"2"^^xsd:int)'
 
 def test_lte():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 
 	term = kg.ontology.terms.cmso.hasNumberOfAtoms
 	term <= 2
-	assert term._condition == '(?hasNumberOfAtomsvalue<="2"^^xsd:int)'
+	assert term._condition == '(?cmso:hasNumberOfAtomsvalue<="2"^^xsd:int)'
 
 def test_gte():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 
 	term = kg.ontology.terms.cmso.hasNumberOfAtoms
 	term >= 2
-	assert term._condition == '(?hasNumberOfAtomsvalue>="2"^^xsd:int)'
+	assert term._condition == '(?cmso:hasNumberOfAtomsvalue>="2"^^xsd:int)'
 
 def test_ne():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 
 	term = kg.ontology.terms.cmso.hasNumberOfAtoms
 	term != 2
-	assert term._condition == '(?hasNumberOfAtomsvalue!="2"^^xsd:int)'
+	assert term._condition == '(?cmso:hasNumberOfAtomsvalue!="2"^^xsd:int)'
 
 def test_and():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 
 	term = (kg.ontology.terms.cmso.hasVolume > 2) & (kg.ontology.terms.cmso.hasVolume < 4)
-	assert term._condition == '((?hasVolumevalue<"4"^^xsd:float)&&(?hasVolumevalue<"4"^^xsd:float))'
+	assert term._condition == '((?cmso:hasVolumevalue<"4"^^xsd:float)&&(?cmso:hasVolumevalue<"4"^^xsd:float))'
 
 def test_or():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 
 	term = (kg.ontology.terms.cmso.hasVolume > 2) | (kg.ontology.terms.cmso.hasVolume < 4)
-	assert term._condition == '((?hasVolumevalue<"4"^^xsd:float)||(?hasVolumevalue<"4"^^xsd:float))'
+	assert term._condition == '((?cmso:hasVolumevalue<"4"^^xsd:float)||(?cmso:hasVolumevalue<"4"^^xsd:float))'
```

### Comparing `atomrdf-0.6.0/tests/test_visualise.py` & `atomrdf-0.6.4/tests/test_visualise.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.0/tests/test_workflow.py` & `atomrdf-0.6.4/tests/test_workflow.py`

 * *Files identical despite different names*

