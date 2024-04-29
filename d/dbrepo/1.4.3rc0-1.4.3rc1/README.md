# Comparing `tmp/dbrepo-1.4.3rc0.tar.gz` & `tmp/dbrepo-1.4.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbrepo-1.4.3rc0.tar", last modified: Sun Apr 28 16:09:12 2024, max compression
+gzip compressed data, was "dbrepo-1.4.3rc1.tar", last modified: Mon Apr 29 06:17:10 2024, max compression
```

## Comparing `dbrepo-1.4.3rc0.tar` & `dbrepo-1.4.3rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/LICENSE
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/README.md
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/dbrepo/
--rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/dbrepo/AmqpClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/dbrepo/RestClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/dbrepo/UploadClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/dbrepo/__init__.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/dbrepo/api/
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/dbrepo/api/__init__.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    21706 2024-04-28 16:07:17.000000 dbrepo-1.4.3rc0/dbrepo/api/dto.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.3rc0/dbrepo/api/encoder.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/dbrepo/api/exceptions.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/dbrepo.egg-info/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/SOURCES.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/dependency_links.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/requires.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/top_level.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1102 2024-04-28 16:09:09.000000 dbrepo-1.4.3rc0/pyproject.toml
--rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/setup.cfg
--rw-r--r--   0 mweise    (1000) mweise    (1000)      410 2024-04-28 16:09:09.000000 dbrepo-1.4.3rc0/setup.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/tests/
--rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_analyse.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_container.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_database.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_identifier.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_license.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_query.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/tests/test_rest_client.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_table.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_user.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_view.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 06:17:10.398779 dbrepo-1.4.3rc1/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc1/LICENSE
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-04-29 06:17:10.398779 dbrepo-1.4.3rc1/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/README.md
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 06:17:10.394779 dbrepo-1.4.3rc1/dbrepo/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/dbrepo/AmqpClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/dbrepo/RestClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/dbrepo/UploadClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc1/dbrepo/__init__.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 06:17:10.394779 dbrepo-1.4.3rc1/dbrepo/api/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc1/dbrepo/api/__init__.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    21438 2024-04-29 06:16:46.000000 dbrepo-1.4.3rc1/dbrepo/api/dto.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.3rc1/dbrepo/api/encoder.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc1/dbrepo/api/exceptions.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 06:17:10.398779 dbrepo-1.4.3rc1/dbrepo.egg-info/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-04-29 06:17:10.000000 dbrepo-1.4.3rc1/dbrepo.egg-info/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-04-29 06:17:10.000000 dbrepo-1.4.3rc1/dbrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-29 06:17:10.000000 dbrepo-1.4.3rc1/dbrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-29 06:17:10.000000 dbrepo-1.4.3rc1/dbrepo.egg-info/requires.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-29 06:17:10.000000 dbrepo-1.4.3rc1/dbrepo.egg-info/top_level.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1102 2024-04-29 06:17:06.000000 dbrepo-1.4.3rc1/pyproject.toml
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-29 06:17:10.398779 dbrepo-1.4.3rc1/setup.cfg
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      410 2024-04-29 06:17:06.000000 dbrepo-1.4.3rc1/setup.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 06:17:10.398779 dbrepo-1.4.3rc1/tests/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_analyse.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_container.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_database.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_identifier.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_license.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_query.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc1/tests/test_rest_client.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_table.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_user.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc1/tests/test_view.py
```

### Comparing `dbrepo-1.4.3rc0/LICENSE` & `dbrepo-1.4.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/PKG-INFO` & `dbrepo-1.4.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.3rc0
+Version: 1.4.3rc1
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.3rc0/README.md` & `dbrepo-1.4.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/dbrepo/AmqpClient.py` & `dbrepo-1.4.3rc1/dbrepo/AmqpClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/dbrepo/RestClient.py` & `dbrepo-1.4.3rc1/dbrepo/RestClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/dbrepo/UploadClient.py` & `dbrepo-1.4.3rc1/dbrepo/UploadClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/dbrepo/api/dto.py` & `dbrepo-1.4.3rc1/dbrepo/api/dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -554,25 +554,25 @@
 class CreateRelatedIdentifier(BaseModel):
     value: str
     type: RelatedIdentifierType
     relation: RelatedIdentifierRelation
 
 
 class CreateIdentifier(BaseModel):
+    database_id: int
     type: IdentifierType
     creators: List[CreateIdentifierCreator]
     publication_year: int
-    titles: Optional[List[CreateIdentifierTitle]] = field(default_factory=list)
-    descriptions: Optional[List[CreateIdentifierDescription]] = field(default_factory=list)
+    publisher: str
+    titles: List[CreateIdentifierTitle]
+    descriptions: List[CreateIdentifierDescription]
     funders: Optional[List[CreateIdentifierFunder]] = field(default_factory=list)
     doi: Optional[str] = None
-    publisher: Optional[str] = None
     language: Optional[str] = None
     licenses: Optional[List[License]] = field(default_factory=list)
-    database_id: Optional[int] = None
     query_id: Optional[int] = None
     table_id: Optional[int] = None
     view_id: Optional[int] = None
     query: Optional[str] = None
     query_normalized: Optional[str] = None
     execution: Optional[str] = None
     related_identifiers: Optional[List[CreateRelatedIdentifier]] = field(default_factory=list)
@@ -586,21 +586,21 @@
     id: int
     database_id: int
     type: IdentifierType
     creator: UserBrief
     status: IdentifierStatusType
     created: Timestamp
     last_modified: Timestamp
-    publication_year: Optional[int] = None
-    creators: Optional[List[IdentifierCreator]] = field(default_factory=list)
-    titles: Optional[List[IdentifierTitle]] = field(default_factory=list)
-    descriptions: Optional[List[IdentifierDescription]] = field(default_factory=list)
+    publication_year: int
+    publisher: str
+    creators: List[IdentifierCreator]
+    titles: List[IdentifierTitle]
+    descriptions: List[IdentifierDescription]
     funders: Optional[List[IdentifierFunder]] = field(default_factory=list)
     doi: Optional[str] = None
-    publisher: Optional[str] = None
     language: Optional[str] = None
     licenses: Optional[List[License]] = field(default_factory=list)
     query_id: Optional[int] = None
     table_id: Optional[int] = None
     view_id: Optional[int] = None
     query: Optional[str] = None
     query_normalized: Optional[str] = None
```

### Comparing `dbrepo-1.4.3rc0/dbrepo/api/exceptions.py` & `dbrepo-1.4.3rc1/dbrepo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/dbrepo.egg-info/PKG-INFO` & `dbrepo-1.4.3rc1/dbrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.3rc0
+Version: 1.4.3rc1
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.3rc0/dbrepo.egg-info/SOURCES.txt` & `dbrepo-1.4.3rc1/dbrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/pyproject.toml` & `dbrepo-1.4.3rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbrepo"
-version = "1.4.3rc0"
+version = "1.4.3rc1"
 description = "DBRepo Python Library"
 keywords = [
     "DBRepo",
     "Database Repository"
 ]
 authors = [
     { name = "Martin Weise, TU Wien", email = "martin.weise@tuwien.ac.at" }
```

### Comparing `dbrepo-1.4.3rc0/tests/test_analyse.py` & `dbrepo-1.4.3rc1/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_container.py` & `dbrepo-1.4.3rc1/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_database.py` & `dbrepo-1.4.3rc1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_identifier.py` & `dbrepo-1.4.3rc1/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_license.py` & `dbrepo-1.4.3rc1/tests/test_license.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_query.py` & `dbrepo-1.4.3rc1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_rest_client.py` & `dbrepo-1.4.3rc1/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_table.py` & `dbrepo-1.4.3rc1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_user.py` & `dbrepo-1.4.3rc1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc0/tests/test_view.py` & `dbrepo-1.4.3rc1/tests/test_view.py`

 * *Files identical despite different names*

