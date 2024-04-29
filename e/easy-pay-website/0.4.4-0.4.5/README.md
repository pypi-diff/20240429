# Comparing `tmp/easy_pay_website-0.4.4.tar.gz` & `tmp/easy_pay_website-0.4.5.tar.gz`

## Comparing `easy_pay_website-0.4.4.tar` & `easy_pay_website-0.4.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/mkdocs.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/src/easy_pay_website/__init__.py
--rw-r--r--   0        0        0    17004 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/src/easy_pay_website/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/src/easy_pay_website/py.typed
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/LICENSE
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/README.md
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easy_pay_website-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/mkdocs.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/src/easy_pay_website/__init__.py
+-rw-r--r--   0        0        0    15688 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/src/easy_pay_website/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/src/easy_pay_website/py.typed
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/LICENSE
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/README.md
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/PKG-INFO
```

### Comparing `easy_pay_website-0.4.4/mkdocs.yml` & `easy_pay_website-0.4.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `easy_pay_website-0.4.4/src/easy_pay_website/core.py` & `easy_pay_website-0.4.5/src/easy_pay_website/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -423,51 +423,8 @@
             }
             
     else:
         return {
                 "result": False,
                 "message": "failed",
                 "data" : []
-        }
-    
-if __name__ == '__main__':
-    url = "http://beidou.6688732.com"
-    username = "beidou"
-    password = "dhdhqwt77!!92A11"
-    quary_key = "tianmasetsail"
-    query_value = "20230788"
-    admin_name = "beidou"
-    admin_id = "17"
-
-    # login_result = login(url, username, password, quary_key, query_value)
-    # print(login_result)
-    # http://beidou.6688732.com/manage/dingdan/index.html?userid=&ordernum=&ordermd5=&tz=&pzid=36&jkstyle=&status=1&bdstatus=&start=2024-02-13+00%3A00%3A00&end=2024-02-16+23%3A59%3A59
-    path= "/manage/dingdan/index.html"
-    query = {
-        "userid": "",
-        "ordernum": "",
-        "ordermd5": "",
-        "tz": "",
-        "pzid": "36",
-        "jkstyle": "",
-        "status": "1",
-        "bdstatus": "",
-        "start": "2024-02-13 00:00:00",
-        "end": "2024-02-16 23:59:59"
-    }
-
-    # http://beidou.6688732.com/manage/api/user.html
-    # path = "/manage/http/index.html"
-    # query = {}
-
-    # http://beidou.6688732.com/manage/pay/index/status/1.html
-    # path = "/manage/pay/index/status/1.html"
-    # query = {}
-
-    # result = main(url, path, query, admin_name, admin_id)
-    # print(result)
-
-    # result = check_login_status(url, admin_name, admin_id)
-    # print(result)
-
-    r = login(url, username, password, quary_key, query_value)
-    print(r)
+        }
```

### Comparing `easy_pay_website-0.4.4/.gitignore` & `easy_pay_website-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `easy_pay_website-0.4.4/LICENSE` & `easy_pay_website-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_pay_website-0.4.4/pyproject.toml` & `easy_pay_website-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easy_pay_website-0.4.4/PKG-INFO` & `easy_pay_website-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: easy_pay_website
-Version: 0.4.4
+Version: 0.4.5
 Summary: easy pay website
 Project-URL: Documentation, https://asmitul.github.io/easy_pay_website
 Project-URL: Issues, https://github.com/asmitul/easy_pay_website/issues
 Project-URL: Source, https://github.com/asmitul/easy_pay_website
 Author: asmitul
 License-Expression: MIT
 License-File: LICENSE
```

