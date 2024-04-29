# Comparing `tmp/xhs-0.2.8.tar.gz` & `tmp/xhs-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.2.8.tar", last modified: Fri Jan 12 11:26:45 2024, max compression
+gzip compressed data, was "xhs-0.2.9.tar", last modified: Fri Jan 12 12:26:33 2024, max compression
```

## Comparing `xhs-0.2.8.tar` & `xhs-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 11:26:45.904997 xhs-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-01-12 11:26:37.000000 xhs-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-12 11:26:37.000000 xhs-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-12 11:26:37.000000 xhs-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-01-12 11:26:45.904997 xhs-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-01-12 11:26:37.000000 xhs-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-12 11:26:37.000000 xhs-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-12 11:26:45.904997 xhs-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-01-12 11:26:37.000000 xhs-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 11:26:45.904997 xhs-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-01-12 11:26:37.000000 xhs-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-01-12 11:26:37.000000 xhs-0.2.8/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-01-12 11:26:37.000000 xhs-0.2.8/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-12 11:26:37.000000 xhs-0.2.8/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 11:26:45.904997 xhs-0.2.8/xhs/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-12 11:26:37.000000 xhs-0.2.8/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-12 11:26:37.000000 xhs-0.2.8/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34752 2024-01-12 11:26:37.000000 xhs-0.2.8/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-01-12 11:26:37.000000 xhs-0.2.8/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12595 2024-01-12 11:26:37.000000 xhs-0.2.8/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 11:26:45.904997 xhs-0.2.8/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-01-12 11:26:45.000000 xhs-0.2.8/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-12 11:26:45.000000 xhs-0.2.8/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 11:26:45.000000 xhs-0.2.8/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 11:26:45.000000 xhs-0.2.8/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-12 11:26:45.000000 xhs-0.2.8/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-12 11:26:45.000000 xhs-0.2.8/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 reajason   (501) staff       (20)        0 2024-01-12 12:26:33.265590 xhs-0.2.9/
+-rw-r--r--   0 reajason   (501) staff       (20)     2419 2024-01-12 11:25:39.000000 xhs-0.2.9/CHANGELOG.md
+-rw-r--r--   0 reajason   (501) staff       (20)     1065 2023-12-12 16:22:22.000000 xhs-0.2.9/LICENSE
+-rw-r--r--   0 reajason   (501) staff       (20)       85 2023-12-12 16:22:22.000000 xhs-0.2.9/MANIFEST.in
+-rw-r--r--   0 reajason   (501) staff       (20)     2359 2024-01-12 12:26:33.265550 xhs-0.2.9/PKG-INFO
+-rw-r--r--   0 reajason   (501) staff       (20)     1507 2023-12-12 16:22:22.000000 xhs-0.2.9/README.md
+-rw-r--r--   0 reajason   (501) staff       (20)       83 2023-12-13 13:25:47.000000 xhs-0.2.9/requirements.txt
+-rw-r--r--   0 reajason   (501) staff       (20)      283 2024-01-12 12:26:33.265760 xhs-0.2.9/setup.cfg
+-rw-r--r--   0 reajason   (501) staff       (20)     1346 2024-01-12 12:07:58.000000 xhs-0.2.9/setup.py
+drwxr-xr-x   0 reajason   (501) staff       (20)        0 2024-01-12 12:26:33.263440 xhs-0.2.9/tests/
+-rw-r--r--   0 reajason   (501) staff       (20)     1959 2023-12-28 09:16:38.000000 xhs-0.2.9/tests/__init__.py
+-rw-r--r--   0 reajason   (501) staff       (20)     3119 2023-12-12 16:22:22.000000 xhs-0.2.9/tests/test_help.py
+-rw-r--r--   0 reajason   (501) staff       (20)    11132 2023-12-28 09:16:38.000000 xhs-0.2.9/tests/test_xhs.py
+-rw-r--r--   0 reajason   (501) staff       (20)      102 2023-12-12 16:22:22.000000 xhs-0.2.9/tests/utils.py
+drwxr-xr-x   0 reajason   (501) staff       (20)        0 2024-01-12 12:26:33.264670 xhs-0.2.9/xhs/
+-rw-r--r--   0 reajason   (501) staff       (20)      427 2023-12-12 16:22:22.000000 xhs-0.2.9/xhs/__init__.py
+-rw-r--r--   0 reajason   (501) staff       (20)      448 2024-01-12 12:22:26.000000 xhs-0.2.9/xhs/__version__.py
+-rw-r--r--   0 reajason   (501) staff       (20)    34752 2023-12-28 09:16:38.000000 xhs-0.2.9/xhs/core.py
+-rw-r--r--   0 reajason   (501) staff       (20)      786 2023-12-12 16:22:22.000000 xhs-0.2.9/xhs/exception.py
+-rw-r--r--   0 reajason   (501) staff       (20)    12595 2024-01-12 11:19:51.000000 xhs-0.2.9/xhs/help.py
+drwxr-xr-x   0 reajason   (501) staff       (20)        0 2024-01-12 12:26:33.265411 xhs-0.2.9/xhs.egg-info/
+-rw-r--r--   0 reajason   (501) staff       (20)     2359 2024-01-12 12:26:33.000000 xhs-0.2.9/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 reajason   (501) staff       (20)      384 2024-01-12 12:26:33.000000 xhs-0.2.9/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 reajason   (501) staff       (20)        1 2024-01-12 12:26:33.000000 xhs-0.2.9/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 reajason   (501) staff       (20)        1 2024-01-12 12:26:33.000000 xhs-0.2.9/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 reajason   (501) staff       (20)       14 2024-01-12 12:26:33.000000 xhs-0.2.9/xhs.egg-info/requires.txt
+-rw-r--r--   0 reajason   (501) staff       (20)        4 2024-01-12 12:26:33.000000 xhs-0.2.9/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.2.8/CHANGELOG.md` & `xhs-0.2.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `xhs-0.2.8/LICENSE` & `xhs-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.2.8/PKG-INFO` & `xhs-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.2.8
+Version: 0.2.9
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: lxml
 
 <div align="center">
 
 <h1 align="center">
 🍰xhs
 </h1>
```

### Comparing `xhs-0.2.8/README.md` & `xhs-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `xhs-0.2.8/setup.py` & `xhs-0.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     author=about["__author__"],
     author_email=about["__author_email__"],
     url=about["__url__"],
     license=about["__license__"],
     packages=["xhs"],
-    install_requires=["requests"],
+    install_requires=["requests", "lxml"],
     keywords="xhs crawl",
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

### Comparing `xhs-0.2.8/tests/test_help.py` & `xhs-0.2.9/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.8/tests/test_xhs.py` & `xhs-0.2.9/tests/test_xhs.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,32 +259,37 @@
 def test_get_follow_notifications(xhs_client: XhsClient):
     mentions = xhs_client.get_follow_notifications()
     beauty_print(mentions)
     assert len(mentions["message_list"])
 
 
 def test_get_upload_image_ids(xhs_client: XhsClient):
-    count = 5
-    ids = xhs_client.get_upload_image_ids(count)
-    beauty_print(ids)
-    assert len(ids[0]["fileIds"]) == count
+    image_id, token = xhs_client.get_upload_files_permit("image")
+    upload_id = xhs_client.get_upload_id(image_id, token)
+    print(upload_id)
+    beauty_print(image_id)
+    assert image_id
 
 
 def test_upload_image(xhs_client: XhsClient):
-    ids = xhs_client.get_upload_image_ids(1)
-    file_info = ids[0]
-    file_id = file_info["fileIds"][0]
-    file_token = file_info["token"]
-    file_path = "/Users/reajason/Downloads/4538306CF3BDC215721FCC0532AF4D3D.jpg"
-    res = xhs_client.upload_image(file_id, file_token, file_path)
+    file_id, file_token = xhs_client.get_upload_files_permit("image")
+    file_path = "/Users/reajason/Downloads/wall/wallhaven-x6k21l.png"
+    res = xhs_client.upload_file(file_id, file_token, file_path)
     assert res.status_code == 200
     print(res.headers["X-Ros-Preview-Url"])
 
     with pytest.raises(DataFetchError, match="file already exists"):
-        xhs_client.upload_image(file_id, file_token, file_path)
+        xhs_client.upload_file(file_id, file_token, file_path)
+
+def test_upload_video(xhs_client: XhsClient):
+    file_id, file_token = xhs_client.get_upload_files_permit("video")
+    file_path = "/Users/reajason/Downloads/220114_01_Drone_4k_017.mp4"
+    res = xhs_client.upload_file(file_id, file_token, file_path, content_type="video/mp4")
+    assert res.status_code == 200
+    print(res.headers["X-Ros-Preview-Url"])
 
 
 def test_get_suggest_topic(xhs_client: XhsClient):
     topic_keyword = "Python"
     topics = xhs_client.get_suggest_topic(topic_keyword)
     beauty_print(topics)
     assert topic_keyword.upper() in topics[0]["name"].upper()
@@ -297,25 +302,25 @@
     assert ats_keyword.upper() in ats[0]["user_base_dto"]["user_nickname"].upper()
 
 
 def test_create_simple_note(xhs_client: XhsClient):
     title = "我是标题"
     desc = "下面我说两点 \n 1. 第一点 \n 2. 第二点"
     images = [
-        "/Users/reajason/Downloads/221686462282_.pic.png",
+        "/Users/reajason/Downloads/wall/wallhaven-x6k21l.png",
     ]
     note = xhs_client.create_image_note(title, desc, images, is_private=True, post_time="2023-07-25 23:59:59")
     beauty_print(note)
 
 
 def test_create_note_with_ats_topics(xhs_client: XhsClient):
     title = "我是通过自动发布脚本发送的笔记"
     desc = "deployed by GitHub xhs， #Python[话题]# @ReaJason"
     files = [
-        "/Users/reajason/Downloads/221686462282_.pic.png",
+        "/Users/reajason/Downloads/wall/wallhaven-x6k21l.png",
     ]
 
     # 可以通过 xhs_client.get_suggest_ats(ats_keyword) 接口获取用户数据
     ats = [
         {"nickname": "ReaJason", "user_id": "63273a77000000002303cc9b", "name": "ReaJason"}
     ]
 
@@ -328,17 +333,17 @@
     ]
     note = xhs_client.create_image_note(title, desc, files, ats=ats, topics=topics, is_private=True,
                                         post_time="2023-07-25 23:59:59")
     beauty_print(note)
 
 
 def test_create_video_note(xhs_client: XhsClient):
-    note = xhs_client.create_video_note(title="123123", video_path="/Users/reajason/Downloads/2.mp4", desc="",
+    note = xhs_client.create_video_note(title="123123", video_path="/Users/reajason/Downloads/1.mp4", desc="",
                                         is_private=True)
     beauty_print(note)
 
 
 def test_create_video_note_with_cover(xhs_client: XhsClient):
-    note = xhs_client.create_video_note(title="123123", video_path="/Users/reajason/Downloads/2.mp4", desc="",
-                                        cover_path="/Users/reajason/Downloads/221686462282_.pic.jpg",
+    note = xhs_client.create_video_note(title="123123", video_path="/Users/reajason/Downloads/1.mp4", desc="",
+                                        cover_path="/Users/reajason/Downloads/wall/wallhaven-x6k21l.png",
                                         is_private=True)
     beauty_print(note)
```

### Comparing `xhs-0.2.8/xhs/core.py` & `xhs-0.2.9/xhs/core.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.8/xhs/exception.py` & `xhs-0.2.9/xhs/exception.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.8/xhs/help.py` & `xhs-0.2.9/xhs/help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.8/xhs.egg-info/PKG-INFO` & `xhs-0.2.9/xhs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.2.8
+Version: 0.2.9
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: lxml
 
 <div align="center">
 
 <h1 align="center">
 🍰xhs
 </h1>
```

