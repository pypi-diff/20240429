# Comparing `tmp/Fr1997v011-1.4.2.tar.gz` & `tmp/Fr1997v011-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.4.2.tar", last modified: Mon Apr 29 05:35:00 2024, max compression
+gzip compressed data, was "Fr1997v011-1.4.3.tar", last modified: Mon Apr 29 17:06:07 2024, max compression
```

## Comparing `Fr1997v011-1.4.2.tar` & `Fr1997v011-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.095495 Fr1997v011-1.4.2/
-drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.053181 Fr1997v011-1.4.2/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-29 05:34:59.000000 Fr1997v011-1.4.2/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.2/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-29 05:35:00.092495 Fr1997v011-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-29 05:34:14.000000 Fr1997v011-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.078494 Fr1997v011-1.4.2/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.2/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.084494 Fr1997v011-1.4.2/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.2/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   173053 2024-04-29 02:56:03.000000 Fr1997v011-1.4.2/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:35:00.088495 Fr1997v011-1.4.2/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.2/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-29 05:35:00.095495 Fr1997v011-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-29 05:34:22.000000 Fr1997v011-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.375366 Fr1997v011-1.4.3/
+drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.365354 Fr1997v011-1.4.3/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-29 17:06:07.373367 Fr1997v011-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-29 09:24:56.000000 Fr1997v011-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.367360 Fr1997v011-1.4.3/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.3/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.370366 Fr1997v011-1.4.3/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.3/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   173742 2024-04-29 09:28:37.000000 Fr1997v011-1.4.3/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.372366 Fr1997v011-1.4.3/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.3/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:06:07.375366 Fr1997v011-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-29 09:24:52.000000 Fr1997v011-1.4.3/setup.py
```

### Comparing `Fr1997v011-1.4.2/LICENSE` & `Fr1997v011-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.2/README.md` & `Fr1997v011-1.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.4.2.tar.gz
+pip install dist/Fr1997v011-1.4.3.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.4.2/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.4.3/fr1997_mode/mode_func/all_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -3861,26 +3861,42 @@
             if response.status_code == 200:
                 data_data = response.json()
                 code = data_data['code']
                 if code == 200:
                     return data_data
         return {'code': 500}
 
-    # 应用 创建
+    # 应用 创建key
     def app_chat_key(self, member_id, appId):
         data = {"name": member_id, "limit": {"maxUsagePoints": -1}, "appId": appId}
         response = requests.post(f'{self.base_url}/support/openapi/create', headers=self.get_token_header(),
                                  json=data)
         if response.status_code == 200:
             data_data = response.json()
             code = data_data['code']
             if code == 200:
                 return data_data
         return {'code': 500}
 
+    # 应用 创建key
+    def app_log(self, member_id, appId):
+        url = f'{self.base_url}/core/chat/init?appId={appId}&chatId={member_id}&loadCustomFeedbacks=true'
+        params = (
+            ('appId', appId),
+            ('chatId', member_id),
+            ('loadCustomFeedbacks', 'true'),
+        )
+        response = requests.get(url, headers=self.get_token_header(), params=params)
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
@@ -4357,8 +4373,9 @@
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
 
-# FastGptAuto(run_path=2).api_1()
+# data_data = FastGptAuto(run_path=2).app_log('12419','662f0e6d9cc568621d02d0fb')
+# print(data_data)
```

