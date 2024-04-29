# Comparing `tmp/Fr1997v011-1.4.1.tar.gz` & `tmp/Fr1997v011-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.4.1.tar", last modified: Sun Apr 28 08:52:37 2024, max compression
+gzip compressed data, was "Fr1997v011-1.4.2.tar", last modified: Mon Apr 29 05:35:00 2024, max compression
```

## Comparing `Fr1997v011-1.4.1.tar` & `Fr1997v011-1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.595714 Fr1997v011-1.4.1/
-drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.586516 Fr1997v011-1.4.1/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-28 08:52:37.594615 Fr1997v011-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.587615 Fr1997v011-1.4.1/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.1/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.590616 Fr1997v011-1.4.1/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.1/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   172506 2024-04-28 08:51:02.000000 Fr1997v011-1.4.1/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.592616 Fr1997v011-1.4.1/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.1/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-28 08:52:37.595714 Fr1997v011-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-28 08:52:34.000000 Fr1997v011-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.095495 Fr1997v011-1.4.2/
+drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.053181 Fr1997v011-1.4.2/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-29 05:35:00.092495 Fr1997v011-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-29 05:34:14.000000 Fr1997v011-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.078494 Fr1997v011-1.4.2/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.2/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.084494 Fr1997v011-1.4.2/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.2/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   173053 2024-04-29 02:56:03.000000 Fr1997v011-1.4.2/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.088495 Fr1997v011-1.4.2/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.2/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 05:35:00.095495 Fr1997v011-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-29 05:34:22.000000 Fr1997v011-1.4.2/setup.py
```

### Comparing `Fr1997v011-1.4.1/LICENSE` & `Fr1997v011-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.1/README.md` & `Fr1997v011-1.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.4.1.tar.gz
+pip install dist/Fr1997v011-1.4.2.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.4.1/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.4.2/fr1997_mode/mode_func/all_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -3861,14 +3861,26 @@
             if response.status_code == 200:
                 data_data = response.json()
                 code = data_data['code']
                 if code == 200:
                     return data_data
         return {'code': 500}
 
+    # 应用 创建
+    def app_chat_key(self, member_id, appId):
+        data = {"name": member_id, "limit": {"maxUsagePoints": -1}, "appId": appId}
+        response = requests.post(f'{self.base_url}/support/openapi/create', headers=self.get_token_header(),
+                                 json=data)
+        if response.status_code == 200:
+            data_data = response.json()
+            code = data_data['code']
+            if code == 200:
+                return data_data
+        return {'code': 500}
+
     # 应用 修改 【知识库】 【提示词】
     def app_update(self, app_id, up_data):
         response = requests.post(
             f'{self.base_url}/core/app/update?appId={app_id}',
             headers=self.get_token_header(),
             json=up_data)
         if response.status_code == 200:
@@ -4099,30 +4111,30 @@
             "fileId": "662380773f901b42fce7f6e7"
         }
         response = requests.post(url, headers=self.get_header(), json=data)
         print(response.text)
 
     def api_1(self):
         headers = {
-            'Authorization': 'Bearer fastgpt-Qas3mebW6La0aYczKyoFWMPMM36oG7OMZVMZnq9cnMwfU2Y79FcQ4s',
+            'Authorization': 'Bearer fastgpt-DPOEvxkScPWHI3G3T442ZXTS6KWy9oyMxmttl1obEgyOhOW22RYcjBlfi',
             'Content-Type': 'application/json',
         }
 
         data = {
-            "chatId": "662394053f901b42fce8005a",
+            "chatId": "12419",
             "stream": False,
             "detail": False,
             "messages": [
                 {
-                    "content": "导演是谁",
+                    "content": "如何快速提升",
                     "role": "user"
                 }
             ]
         }
-        response = requests.post('https://aitest.dso100.com/api/v1/chat/completions', headers=headers, json=data)
+        response = requests.post('http://101.35.29.36:3020/api/v1/chat/completions', headers=headers, json=data)
         print(response.text)
 
         # headers = {
         #     'Authorization': 'Bearer fastgpt-MdBia1If20J3gKnrHHzHOnNUg4a53FQU8dGEure6QaVK8gJXa5d9VB2Dy',
         #     'Content-Type': 'application/json',
         # }
         #
@@ -4345,7 +4357,8 @@
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
 
+# FastGptAuto(run_path=2).api_1()
```

