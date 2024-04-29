# Comparing `tmp/discord_data-0.2.1.tar.gz` & `tmp/discord_data-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_data-0.2.1.tar", last modified: Mon Sep 11 06:20:39 2023, max compression
+gzip compressed data, was "discord_data-0.2.2.tar", last modified: Mon Apr 29 02:41:12 2024, max compression
```

## Comparing `discord_data-0.2.1.tar` & `discord_data-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-09-11 06:20:39.346881 discord_data-0.2.1/
--rw-r--r--   0 sean      (1000) sean      (1000)    11358 2020-10-27 01:14:31.000000 discord_data-0.2.1/LICENSE
--rw-r--r--   0 sean      (1000) sean      (1000)       47 2020-10-27 01:14:31.000000 discord_data-0.2.1/MANIFEST.in
--rw-r--r--   0 sean      (1000) sean      (1000)     4692 2023-09-11 06:20:39.346881 discord_data-0.2.1/PKG-INFO
--rw-r--r--   0 sean      (1000) sean      (1000)     3894 2023-09-11 06:13:36.000000 discord_data-0.2.1/README.md
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-09-11 06:20:39.346881 discord_data-0.2.1/discord_data/
--rw-r--r--   0 sean      (1000) sean      (1000)      177 2021-03-24 06:41:39.000000 discord_data-0.2.1/discord_data/__init__.py
--rw-r--r--   0 sean      (1000) sean      (1000)     2310 2023-09-11 06:11:16.000000 discord_data-0.2.1/discord_data/__main__.py
--rw-r--r--   0 sean      (1000) sean      (1000)      216 2021-06-17 22:59:42.000000 discord_data-0.2.1/discord_data/common.py
--rw-r--r--   0 sean      (1000) sean      (1000)      132 2023-04-17 18:52:31.000000 discord_data-0.2.1/discord_data/error.py
--rw-r--r--   0 sean      (1000) sean      (1000)     2860 2023-04-17 18:58:47.000000 discord_data-0.2.1/discord_data/merge.py
--rw-r--r--   0 sean      (1000) sean      (1000)     2695 2023-09-11 06:18:59.000000 discord_data-0.2.1/discord_data/model.py
--rw-r--r--   0 sean      (1000) sean      (1000)     6161 2023-08-23 05:00:04.000000 discord_data-0.2.1/discord_data/parse.py
--rw-r--r--   0 sean      (1000) sean      (1000)        0 2021-03-15 08:07:44.000000 discord_data-0.2.1/discord_data/py.typed
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2023-09-11 06:20:39.346881 discord_data-0.2.1/discord_data.egg-info/
--rw-r--r--   0 sean      (1000) sean      (1000)     4692 2023-09-11 06:20:39.000000 discord_data-0.2.1/discord_data.egg-info/PKG-INFO
--rw-r--r--   0 sean      (1000) sean      (1000)      449 2023-09-11 06:20:39.000000 discord_data-0.2.1/discord_data.egg-info/SOURCES.txt
--rw-r--r--   0 sean      (1000) sean      (1000)        1 2023-09-11 06:20:39.000000 discord_data-0.2.1/discord_data.egg-info/dependency_links.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       60 2023-09-11 06:20:39.000000 discord_data-0.2.1/discord_data.egg-info/entry_points.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       24 2023-09-11 06:20:39.000000 discord_data-0.2.1/discord_data.egg-info/requires.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       13 2023-09-11 06:20:39.000000 discord_data-0.2.1/discord_data.egg-info/top_level.txt
--rw-r--r--   0 sean      (1000) sean      (1000)      461 2023-09-11 06:20:39.346881 discord_data-0.2.1/setup.cfg
--rw-r--r--   0 sean      (1000) sean      (1000)     1487 2023-09-11 06:16:17.000000 discord_data-0.2.1/setup.py
+drwxr-xr-x   0 sean      (1000) users      (984)        0 2024-04-29 02:41:12.903833 discord_data-0.2.2/
+-rw-r--r--   0 sean      (1000) users      (984)     1074 2024-04-19 04:59:19.000000 discord_data-0.2.2/LICENSE
+-rw-r--r--   0 sean      (1000) users      (984)       47 2024-04-19 04:59:19.000000 discord_data-0.2.2/MANIFEST.in
+-rw-r--r--   0 sean      (1000) users      (984)     4723 2024-04-29 02:41:12.903833 discord_data-0.2.2/PKG-INFO
+-rw-r--r--   0 sean      (1000) users      (984)     3961 2024-04-29 02:39:29.000000 discord_data-0.2.2/README.md
+drwxr-xr-x   0 sean      (1000) users      (984)        0 2024-04-29 02:41:12.900500 discord_data-0.2.2/discord_data/
+-rw-r--r--   0 sean      (1000) users      (984)      177 2024-04-19 04:59:19.000000 discord_data-0.2.2/discord_data/__init__.py
+-rw-r--r--   0 sean      (1000) users      (984)     2310 2024-04-19 04:59:19.000000 discord_data-0.2.2/discord_data/__main__.py
+-rw-r--r--   0 sean      (1000) users      (984)      216 2024-04-19 04:59:19.000000 discord_data-0.2.2/discord_data/common.py
+-rw-r--r--   0 sean      (1000) users      (984)      132 2024-04-19 04:59:19.000000 discord_data-0.2.2/discord_data/error.py
+-rw-r--r--   0 sean      (1000) users      (984)     2860 2024-04-19 04:59:19.000000 discord_data-0.2.2/discord_data/merge.py
+-rw-r--r--   0 sean      (1000) users      (984)     2695 2024-04-19 04:59:19.000000 discord_data-0.2.2/discord_data/model.py
+-rw-r--r--   0 sean      (1000) users      (984)     7151 2024-04-29 02:39:29.000000 discord_data-0.2.2/discord_data/parse.py
+-rw-r--r--   0 sean      (1000) users      (984)        0 2024-04-19 04:59:19.000000 discord_data-0.2.2/discord_data/py.typed
+drwxr-xr-x   0 sean      (1000) users      (984)        0 2024-04-29 02:41:12.903833 discord_data-0.2.2/discord_data.egg-info/
+-rw-r--r--   0 sean      (1000) users      (984)     4723 2024-04-29 02:41:12.000000 discord_data-0.2.2/discord_data.egg-info/PKG-INFO
+-rw-r--r--   0 sean      (1000) users      (984)      449 2024-04-29 02:41:12.000000 discord_data-0.2.2/discord_data.egg-info/SOURCES.txt
+-rw-r--r--   0 sean      (1000) users      (984)        1 2024-04-29 02:41:12.000000 discord_data-0.2.2/discord_data.egg-info/dependency_links.txt
+-rw-r--r--   0 sean      (1000) users      (984)       60 2024-04-29 02:41:12.000000 discord_data-0.2.2/discord_data.egg-info/entry_points.txt
+-rw-r--r--   0 sean      (1000) users      (984)       24 2024-04-29 02:41:12.000000 discord_data-0.2.2/discord_data.egg-info/requires.txt
+-rw-r--r--   0 sean      (1000) users      (984)       13 2024-04-29 02:41:12.000000 discord_data-0.2.2/discord_data.egg-info/top_level.txt
+-rw-r--r--   0 sean      (1000) users      (984)     1430 2024-04-29 02:41:12.903833 discord_data-0.2.2/setup.cfg
+-rw-r--r--   0 sean      (1000) users      (984)       69 2024-04-19 04:59:19.000000 discord_data-0.2.2/setup.py
```

### Comparing `discord_data-0.2.1/PKG-INFO` & `discord_data-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: discord_data
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library to parse the Discord GDPR export
 Home-page: https://github.com/seanbreckenridge/discord_data
 Author: Sean Breckenridge
-Author-email: seanbrecke@gmail.com
-License: http://www.apache.org/licenses/LICENSE-2.0
+Author-email: "seanbrecke@gmail.com"
+License: MIT
 Keywords: discord data
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,14 +22,16 @@
 
 ## discord_data
 
 Library to parse information from the discord data export, see more info [here](https://support.discord.com/hc/en-us/articles/360004027692).
 
 The request to process the data has to be done manually, and it can take a while for them to deliver it to you.
 
+This supports both the old CSV and new JSON formats for messages.
+
 ### Install:
 
 Requires `python3.8+`. To install with pip, run:
 
     pip install discord_data
 
 ## Single Export
```

### Comparing `discord_data-0.2.1/README.md` & `discord_data-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ## discord_data
 
 Library to parse information from the discord data export, see more info [here](https://support.discord.com/hc/en-us/articles/360004027692).
 
 The request to process the data has to be done manually, and it can take a while for them to deliver it to you.
 
+This supports both the old CSV and new JSON formats for messages.
+
 ### Install:
 
 Requires `python3.8+`. To install with pip, run:
 
     pip install discord_data
 
 ## Single Export
```

### Comparing `discord_data-0.2.1/discord_data/__main__.py` & `discord_data-0.2.2/discord_data/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                     "IPython not installed, falling back to standard REPL", fg="yellow"
                 )
 
                 code.interact(local=locals())
             else:
                 IPython.embed()  # type: ignore[no-untyped-call]
         else:
-            # backwards compatability, keep here
+            # backwards compatibility, keep here
             click.echo(f"Message count: {len(messages)}")
             click.echo(f"Activity count: {len(activity)}")
     elif output == "json":
         from .model import serialize
 
         click.echo(serialize({"messages": messages, "activity": activity}))
     elif output == "count":
```

### Comparing `discord_data-0.2.1/discord_data/merge.py` & `discord_data-0.2.2/discord_data/merge.py`

 * *Files identical despite different names*

### Comparing `discord_data-0.2.1/discord_data/model.py` & `discord_data-0.2.2/discord_data/model.py`

 * *Files identical despite different names*

### Comparing `discord_data-0.2.1/discord_data/parse.py` & `discord_data-0.2.2/discord_data/parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,28 +46,28 @@
 def parse_messages(messages_dir: PathIsh) -> Iterator[Res[Message]]:
     pmsg_dir: Path = expand_path(messages_dir)
     # get user id
 
     # parse index
     index_f = pmsg_dir / "index.json"
     if not index_f.exists():
-        yield RuntimeError(f"Message index 'index.json' doesnt exist at {index_f}")
+        yield RuntimeError(f"Message index 'index.json' doesn't exist at {index_f}")
         return
     index: Dict[str, Optional[str]] = json.loads(index_f.read_text())
 
     # get individual message directories
     msg_dirs: List[Path] = list(
         filter(lambda d: d.is_dir() and not d.name.startswith("."), pmsg_dir.iterdir())
     )
     for msg_chan in msg_dirs:
-        # chanel.json has some metadata about the channel/server
+        # channel.json has some metadata about the channel/server
         channel_info_f: Path = msg_chan / "channel.json"
         if not channel_info_f.exists():
             yield RuntimeError(
-                f"Channel info 'channel.json' doesnt exist at {channel_info_f}"
+                f"Channel info 'channel.json' doesn't exist at {channel_info_f}"
             )
             continue
         channel_json: Dict[str, Any] = json.loads(channel_info_f.read_text())
 
         # optionally, find server information
         server_info: Optional[Server] = None
 
@@ -89,28 +89,52 @@
             continue
         channel_obj: Channel = Channel(
             channel_id=int(channel_json["id"]),
             name=channel_name,
             server=server_info,
         )
 
-        # read CSV file to get messages
-        with (msg_chan / "messages.csv").open("r", encoding="utf-8", newline="") as f:
-            csv_reader = csv.reader(
-                f, delimiter=",", quotechar='"', quoting=csv.QUOTE_MINIMAL
-            )
-            next(csv_reader)  # ignore header row
-            for row in csv_reader:
+        channel_csv = msg_chan / "messages.csv"
+        if channel_csv.exists():
+            # read CSV file to get messages
+            with (msg_chan / "messages.csv").open(
+                "r", encoding="utf-8", newline=""
+            ) as f:
+                csv_reader = csv.reader(
+                    f, delimiter=",", quotechar='"', quoting=csv.QUOTE_MINIMAL
+                )
+                next(csv_reader)  # ignore header row
+                for row in csv_reader:
+                    try:
+                        yield Message(
+                            message_id=int(row[0]),
+                            timestamp=_parse_message_datetime(row[1]),
+                            channel=channel_obj,
+                            content=row[2],
+                            attachments=row[3],
+                        )
+                    except Exception as e:
+                        yield e
+        else:
+            json_file = msg_chan / "messages.json"
+            if not json_file.exists():
+                yield RuntimeError(f"No messages file found in in {msg_chan}")
+                continue
+
+            # read JSON file to get messages
+            messages_json: List[Dict[str, Any]] = json.loads(json_file.read_text())
+
+            for msg in messages_json:
                 try:
                     yield Message(
-                        message_id=int(row[0]),
-                        timestamp=_parse_message_datetime(row[1]),
+                        message_id=int(msg["ID"]),
+                        timestamp=_parse_message_datetime(msg["Timestamp"]),
                         channel=channel_obj,
-                        content=row[2],
-                        attachments=row[3],
+                        content=msg["Contents"],
+                        attachments=msg.get("Attachments", ""),
                     )
                 except Exception as e:
                     yield e
 
 
 def _parse_activity_blob(blob: Json) -> Activity:
     reginfo = None
```

### Comparing `discord_data-0.2.1/discord_data.egg-info/PKG-INFO` & `discord_data-0.2.2/discord_data.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: discord-data
-Version: 0.2.1
+Name: discord_data
+Version: 0.2.2
 Summary: Library to parse the Discord GDPR export
 Home-page: https://github.com/seanbreckenridge/discord_data
 Author: Sean Breckenridge
-Author-email: seanbrecke@gmail.com
-License: http://www.apache.org/licenses/LICENSE-2.0
+Author-email: "seanbrecke@gmail.com"
+License: MIT
 Keywords: discord data
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,14 +22,16 @@
 
 ## discord_data
 
 Library to parse information from the discord data export, see more info [here](https://support.discord.com/hc/en-us/articles/360004027692).
 
 The request to process the data has to be done manually, and it can take a while for them to deliver it to you.
 
+This supports both the old CSV and new JSON formats for messages.
+
 ### Install:
 
 Requires `python3.8+`. To install with pip, run:
 
     pip install discord_data
 
 ## Single Export
```

