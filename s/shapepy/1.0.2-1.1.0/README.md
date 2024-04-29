# Comparing `tmp/shapepy-1.0.2.tar.gz` & `tmp/shapepy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapepy-1.0.2.tar", max compression
+gzip compressed data, was "shapepy-1.1.0.tar", max compression
```

## Comparing `shapepy-1.0.2.tar` & `shapepy-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2024-04-14 11:06:15.762523 shapepy-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     1930 2024-04-14 11:06:15.762523 shapepy-1.0.2/README.md
--rw-r--r--   0        0        0      810 2024-04-14 11:06:15.770522 shapepy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      691 2024-04-14 11:06:15.770522 shapepy-1.0.2/src/shapepy/__init__.py
--rw-r--r--   0        0        0    24691 2024-04-14 11:06:15.770522 shapepy-1.0.2/src/shapepy/curve.py
--rw-r--r--   0        0        0    27619 2024-04-14 11:06:15.770522 shapepy-1.0.2/src/shapepy/jordancurve.py
--rw-r--r--   0        0        0     4677 2024-04-14 11:06:15.770522 shapepy-1.0.2/src/shapepy/plot.py
--rw-r--r--   0        0        0     7941 2024-04-14 11:06:15.770522 shapepy-1.0.2/src/shapepy/polygon.py
--rw-r--r--   0        0        0     7411 2024-04-14 11:06:15.770522 shapepy-1.0.2/src/shapepy/primitive.py
--rw-r--r--   0        0        0    37537 2024-04-14 11:06:15.770522 shapepy-1.0.2/src/shapepy/shape.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 shapepy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-29 19:40:24.667681 shapepy-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1930 2024-04-29 19:40:24.667681 shapepy-1.1.0/README.md
+-rw-r--r--   0        0        0      810 2024-04-29 19:40:24.675681 shapepy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      691 2024-04-29 19:40:24.675681 shapepy-1.1.0/src/shapepy/__init__.py
+-rw-r--r--   0        0        0    24691 2024-04-29 19:40:24.675681 shapepy-1.1.0/src/shapepy/curve.py
+-rw-r--r--   0        0        0    27619 2024-04-29 19:40:24.675681 shapepy-1.1.0/src/shapepy/jordancurve.py
+-rw-r--r--   0        0        0     4677 2024-04-29 19:40:24.675681 shapepy-1.1.0/src/shapepy/plot.py
+-rw-r--r--   0        0        0     7941 2024-04-29 19:40:24.675681 shapepy-1.1.0/src/shapepy/polygon.py
+-rw-r--r--   0        0        0     7411 2024-04-29 19:40:24.675681 shapepy-1.1.0/src/shapepy/primitive.py
+-rw-r--r--   0        0        0    37537 2024-04-29 19:40:24.675681 shapepy-1.1.0/src/shapepy/shape.py
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 shapepy-1.1.0/PKG-INFO
```

### Comparing `shapepy-1.0.2/LICENSE.md` & `shapepy-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shapepy-1.0.2/README.md` & `shapepy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `shapepy-1.0.2/pyproject.toml` & `shapepy-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shapepy"
-version = "1.0.2"
+version = "1.1.0"
 description = "Geometric 2D library"
 authors = ["Carlos Adir <carlos.adir.leite@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "shapepy", from = "src" }]
 
 [tool.poetry.dependencies]
 numpy = "^1.0.0"
```

### Comparing `shapepy-1.0.2/src/shapepy/__init__.py` & `shapepy-1.1.0/src/shapepy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     DisjointShape,
     EmptyShape,
     IntegrateShape,
     SimpleShape,
     WholeShape,
 )
 
-__version__ = "1.0.2"
+__version__ = "1.1.0"
 
 if __name__ == "__main__":
     pass
```

### Comparing `shapepy-1.0.2/src/shapepy/curve.py` & `shapepy-1.1.0/src/shapepy/curve.py`

 * *Files identical despite different names*

### Comparing `shapepy-1.0.2/src/shapepy/jordancurve.py` & `shapepy-1.1.0/src/shapepy/jordancurve.py`

 * *Files identical despite different names*

### Comparing `shapepy-1.0.2/src/shapepy/plot.py` & `shapepy-1.1.0/src/shapepy/plot.py`

 * *Files identical despite different names*

### Comparing `shapepy-1.0.2/src/shapepy/polygon.py` & `shapepy-1.1.0/src/shapepy/polygon.py`

 * *Files identical despite different names*

### Comparing `shapepy-1.0.2/src/shapepy/primitive.py` & `shapepy-1.1.0/src/shapepy/primitive.py`

 * *Files identical despite different names*

### Comparing `shapepy-1.0.2/src/shapepy/shape.py` & `shapepy-1.1.0/src/shapepy/shape.py`

 * *Files identical despite different names*

### Comparing `shapepy-1.0.2/PKG-INFO` & `shapepy-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapepy
-Version: 1.0.2
+Version: 1.1.0
 Summary: Geometric 2D library
 Author: Carlos Adir
 Author-email: carlos.adir.leite@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

