# Comparing `tmp/melting_schemas-1.0.7.tar.gz` & `tmp/melting_schemas-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melting_schemas-1.0.7.tar", last modified: Wed Mar  6 16:44:54 2024, max compression
+gzip compressed data, was "melting_schemas-1.0.8.tar", last modified: Mon Apr 29 18:26:10 2024, max compression
```

## Comparing `melting_schemas-1.0.7.tar` & `melting_schemas-1.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:54.569711 melting_schemas-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-06 16:44:54.569711 melting_schemas-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:54.565711 melting_schemas-1.0.7/melting_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:54.565711 melting_schemas-1.0.7/melting_schemas/completion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/completion/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/completion/fcall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/completion/tcall.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/completion/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:54.569711 melting_schemas-1.0.7/melting_schemas/encoding/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/encoding/text_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:54.569711 melting_schemas-1.0.7/melting_schemas/historian/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/historian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/historian/chat_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/historian/text_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:54.569711 melting_schemas-1.0.7/melting_schemas/templating/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/templating/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/melting_schemas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:44:54.569711 melting_schemas-1.0.7/melting_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-06 16:44:54.000000 melting_schemas-1.0.7/melting_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-06 16:44:54.000000 melting_schemas-1.0.7/melting_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 16:44:54.000000 melting_schemas-1.0.7/melting_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-06 16:44:54.000000 melting_schemas-1.0.7/melting_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-06 16:44:54.000000 melting_schemas-1.0.7/melting_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 16:44:54.569711 melting_schemas-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-06 16:44:44.000000 melting_schemas-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.552070 melting_schemas-1.0.8/melting_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/fcall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/tcall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas/encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/encoding/text_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas/historian/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/historian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/historian/chat_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/historian/text_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/templating/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/setup.py
```

### Comparing `melting_schemas-1.0.7/melting_schemas/completion/chat.py` & `melting_schemas-1.0.8/melting_schemas/completion/chat.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.7/melting_schemas/completion/fcall.py` & `melting_schemas-1.0.8/melting_schemas/completion/fcall.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,17 @@
     usage: TokenUsage
 
     class Config:
         smart_unions = True
 
 
 class PluginStreamedResponse(BaseModel):
-    op_type: Literal["step", "result", "start", "stop", "execution_id"]
+    op_type: Literal[
+        "step", "result", "start", "stop", "execution_id", "error", "selection"
+    ]
     plugin_name: Optional[str] = None
     method: Optional[str] = None
     content: str
 
 
 class StartPluginStreamedResponse(PluginStreamedResponse):
     params: dict
```

### Comparing `melting_schemas-1.0.7/melting_schemas/completion/tcall.py` & `melting_schemas-1.0.8/melting_schemas/completion/tcall.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.7/melting_schemas/completion/text.py` & `melting_schemas-1.0.8/melting_schemas/completion/text.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.7/melting_schemas/encoding/text_encoding.py` & `melting_schemas-1.0.8/melting_schemas/encoding/text_encoding.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.7/melting_schemas/historian/text_completions.py` & `melting_schemas-1.0.8/melting_schemas/historian/text_completions.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.7/melting_schemas.egg-info/SOURCES.txt` & `melting_schemas-1.0.8/melting_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.7/setup.py` & `melting_schemas-1.0.8/setup.py`

 * *Files identical despite different names*

