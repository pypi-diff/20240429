# Comparing `tmp/get_holiday_cn-1.0.5.tar.gz` & `tmp/get_holiday_cn-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_holiday_cn-1.0.5.tar", last modified: Tue Dec 27 10:35:08 2022, max compression
+gzip compressed data, was "get_holiday_cn-1.0.6.tar", last modified: Mon Apr 29 11:26:16 2024, max compression
```

## Comparing `get_holiday_cn-1.0.5.tar` & `get_holiday_cn-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 10:35:08.310391 get_holiday_cn-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2022-12-27 10:35:08.310391 get_holiday_cn-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2022-12-27 10:34:54.000000 get_holiday_cn-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 10:35:08.306391 get_holiday_cn-1.0.5/get_holiday_cn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 10:34:54.000000 get_holiday_cn-1.0.5/get_holiday_cn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2022-12-27 10:34:54.000000 get_holiday_cn-1.0.5/get_holiday_cn/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 10:35:08.310391 get_holiday_cn-1.0.5/get_holiday_cn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2022-12-27 10:35:08.000000 get_holiday_cn-1.0.5/get_holiday_cn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-27 10:35:08.000000 get_holiday_cn-1.0.5/get_holiday_cn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 10:35:08.000000 get_holiday_cn-1.0.5/get_holiday_cn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-27 10:35:08.000000 get_holiday_cn-1.0.5/get_holiday_cn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 10:35:08.310391 get_holiday_cn-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2022-12-27 10:34:54.000000 get_holiday_cn-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:26:16.868271 get_holiday_cn-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-29 11:26:16.868271 get_holiday_cn-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-29 11:26:12.000000 get_holiday_cn-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:26:16.868271 get_holiday_cn-1.0.6/get_holiday_cn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:26:12.000000 get_holiday_cn-1.0.6/get_holiday_cn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-04-29 11:26:12.000000 get_holiday_cn-1.0.6/get_holiday_cn/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:26:16.868271 get_holiday_cn-1.0.6/get_holiday_cn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-29 11:26:16.000000 get_holiday_cn-1.0.6/get_holiday_cn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-29 11:26:16.000000 get_holiday_cn-1.0.6/get_holiday_cn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:26:16.000000 get_holiday_cn-1.0.6/get_holiday_cn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 11:26:16.000000 get_holiday_cn-1.0.6/get_holiday_cn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:26:16.868271 get_holiday_cn-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-29 11:26:12.000000 get_holiday_cn-1.0.6/setup.py
```

### Comparing `get_holiday_cn-1.0.5/PKG-INFO` & `get_holiday_cn-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_holiday_cn
-Version: 1.0.5
+Version: 1.0.6
 Summary: 获取中国法定节假日
 Home-page: https://github.com/longweiqiang/get_holiday_cn
 Author: Weiqiang.long
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -50,7 +50,14 @@
 
 client = getHoliday()
 # 获取今日数据
 print(client.assemble_holiday_data())
 # 指定日期获取数据
 print(client.assemble_holiday_data(today='2021-10-01'))
 ```
+
+### 2022/12/27 更新说明
+刚刚推送了v1.0.5版本，在此版本前可能会获取到空数组的2023年json文件，导致现在23年假期更新后还是无法查到；如出现下图所示，可以删除本地已缓存的`2023.json`文件，下次再请求时会自动获取最新的数据
+![企业微信截图_20221227160706](https://user-images.githubusercontent.com/22344864/209655031-1a3b4185-6b8c-436c-aaee-8371c6e2e1aa.png)
+
+### 2024/04/29 更新说明
+本次版本号v1.0.6，主要修复 [issues-4](https://github.com/longweiqiang/get_holiday_cn/issues/4) 的问题，在项目中增加了某个年份文件中返回空列表的情况判断
```

### Comparing `get_holiday_cn-1.0.5/get_holiday_cn/client.py` & `get_holiday_cn-1.0.6/get_holiday_cn/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # @Author  : Weiqiang.long
 # @Email   : 573925242@qq.com
 # @Site    : 
 # @File    : client.py
 # @Software: PyCharm
 # @Description: 获取github仓库的节假日json数据并存到本地文件中
 
+
 """
 https://github.com/NateScarlet/holiday-cn
 国内地址：
 https://ghproxy.com/https://raw.githubusercontent.com/NateScarlet/holiday-cn/master/{年份}.json
 https://cdn.jsdelivr.net/gh/NateScarlet/holiday-cn@master/{年份}.json
 数据格式：
 interface Holidays {
@@ -25,15 +26,15 @@
     /** 日期, ISO 8601 格式 */
     date: string;
     /** 是否为休息日 */
     isOffDay: boolean;
   }[]
 }
 """
-import datetime, requests, json, site
+import datetime, requests, json, site, os
 
 class YearKeyError(Exception):
     '''自定义异常：年份异常'''
     def __init__(self, message):
         self.msg = '年份异常，年份入参为：{0}，请检查入参'.format(message)
     def __str__(self):
         return self.msg
@@ -51,15 +52,21 @@
 
     def __init__(self):
         pass
 
     @staticmethod
     def get_get_holiday_cn_path():
         try:
-            return site.getsitepackages()[0] + '/get_holiday_cn' + '/'
+            sitepackages = site.getsitepackages()
+            for sitepackage in sitepackages:
+                get_holiday_cn_path = sitepackage + '/get_holiday_cn' + '/'
+                if os.path.exists(get_holiday_cn_path):
+                    return get_holiday_cn_path
+                else:
+                    return ""
         except Exception:
             return ""
 
     @staticmethod
     def get_current_year():
         '''获取当前的年份'''
         return datetime.datetime.now().year
@@ -68,72 +75,85 @@
     def get_current_isoweekday(today=None):
         '''获取当前的星期数（返回数字1-7代表周一到周日）'''
         if not today:
             return datetime.datetime.now().isoweekday()
         else:
             return datetime.datetime.strptime(today, "%Y-%m-%d").isoweekday()
 
+    def get_local_holiday_json(self, current_year=None):
+        """
+        查询本地对应年份的json数据
+        :param current_year: 要查询的年份
+        :return:
+        """
+        try:
+            with open(self.get_get_holiday_cn_path() + f"{current_year}.json", 'r', encoding='utf-8') as f:
+                list_data = json.load(f)['days']
+                # 针对本地已有年份，但年份文件中是空列表的情况做特殊处理==>重新获取一次远程仓库文件
+                # https://github.com/longweiqiang/get_holiday_cn/issues/4
+                if len(list_data) == 0:
+                    return self.get_holiday_json(current_year=current_year)
+                return list_data
+        except:
+            return self.get_holiday_json(current_year=current_year)
+
     def get_holiday_json(self, current_year=None):
         '''
         查询仓库中对应年份的json数据
         :param current_year: 要查询的年份
         :return:
         '''
         try:
-            with open(self.get_get_holiday_cn_path() + f"{current_year}.json", 'r', encoding='utf-8') as f:
-                return json.load(f)['days']
-        except:
-            try:
-                url = 'https://cdn.jsdelivr.net/gh/NateScarlet/holiday-cn@master/{year}.json'.format(year=current_year)
-                # url = 'https://raw.githubusercontent.com/NateScarlet/holiday-cn/master/{year}.json'.format(year=current_year)
+            url = 'https://cdn.jsdelivr.net/gh/NateScarlet/holiday-cn@master/{year}.json'.format(year=current_year)
+            # url = 'https://raw.githubusercontent.com/NateScarlet/holiday-cn/master/{year}.json'.format(year=current_year)
+            res = requests.get(url=url, timeout=5)
+            if res.status_code == 200:
+                try:
+                    with open(self.get_get_holiday_cn_path() + f"{current_year}.json", 'w', encoding='utf-8') as f:
+                        json.dump(res.json(), f, ensure_ascii=False, indent=4)
+                except FileNotFoundError:
+                    with open(f"{current_year}.json", 'w', encoding='utf-8') as f:
+                        json.dump(res.json(), f, ensure_ascii=False, indent=4)
+                return res.json()['days']
+            else:
+                print('主网址请求失败，正在发起重试！！！')
+                url = 'https://ghproxy.com/https://raw.githubusercontent.com/NateScarlet/holiday-cn/master/{year}.json'.format(
+                    year=current_year)
                 res = requests.get(url=url, timeout=5)
-                if res.status_code == 200:
+                if res.status_code == 404:
+                    raise YearKeyError(current_year)
+                else:
                     try:
-                        with open(self.get_get_holiday_cn_path() + f"{current_year}.json", 'w', encoding='utf-8') as f:
+                        with open(self.get_get_holiday_cn_path() + f"{current_year}.json", 'w',
+                                  encoding='utf-8') as f:
                             json.dump(res.json(), f, ensure_ascii=False, indent=4)
                     except FileNotFoundError:
                         with open(f"{current_year}.json", 'w', encoding='utf-8') as f:
                             json.dump(res.json(), f, ensure_ascii=False, indent=4)
-                    return res.json()['days']
+                return res.json()['days']
+        except (requests.exceptions.ConnectionError,requests.exceptions.ReadTimeout):
+            try:
+                print('主网址发生未知错误，正在请求备用站点！！！')
+                # 主站挂了直接except,并存储到本地
+                url = 'https://ghproxy.com/https://raw.githubusercontent.com/NateScarlet/holiday-cn/master/{year}.json'.format(
+                    year=current_year)
+                res = requests.get(url=url)
+                if res.status_code == 404:
+                    raise YearKeyError(current_year)
                 else:
-                    print('主网址请求失败，正在发起重试！！！')
-                    url = 'https://ghproxy.com/https://raw.githubusercontent.com/NateScarlet/holiday-cn/master/{year}.json'.format(
-                        year=current_year)
-                    res = requests.get(url=url, timeout=5)
-                    if res.status_code == 404:
-                        raise YearKeyError(current_year)
-                    else:
-                        try:
-                            with open(self.get_get_holiday_cn_path() + f"{current_year}.json", 'w',
-                                      encoding='utf-8') as f:
-                                json.dump(res.json(), f, ensure_ascii=False, indent=4)
-                        except FileNotFoundError:
-                            with open(f"{current_year}.json", 'w', encoding='utf-8') as f:
-                                json.dump(res.json(), f, ensure_ascii=False, indent=4)
-                    return res.json()['days']
-            except (requests.exceptions.ConnectionError,requests.exceptions.ReadTimeout):
-                try:
-                    print('主网址发生未知错误，正在请求备用站点！！！')
-                    # 主站挂了直接except,并存储到本地
-                    url = 'https://ghproxy.com/https://raw.githubusercontent.com/NateScarlet/holiday-cn/master/{year}.json'.format(
-                        year=current_year)
-                    res = requests.get(url=url)
-                    if res.status_code == 404:
-                        raise YearKeyError(current_year)
-                    else:
-                        try:
-                            with open(self.get_get_holiday_cn_path() + f"{current_year}.json", 'w',
-                                      encoding='utf-8') as f:
-                                json.dump(res.json(), f, ensure_ascii=False, indent=4)
-                        except FileNotFoundError:
-                            with open(f"{current_year}.json", 'w', encoding='utf-8') as f:
-                                json.dump(res.json(), f, ensure_ascii=False, indent=4)
-                    return res.json()['days']
-                except:
-                    raise HolidayError()
+                    try:
+                        with open(self.get_get_holiday_cn_path() + f"{current_year}.json", 'w',
+                                  encoding='utf-8') as f:
+                            json.dump(res.json(), f, ensure_ascii=False, indent=4)
+                    except FileNotFoundError:
+                        with open(f"{current_year}.json", 'w', encoding='utf-8') as f:
+                            json.dump(res.json(), f, ensure_ascii=False, indent=4)
+                return res.json()['days']
+            except:
+                raise HolidayError()
 
 
     def get_before_and_after_holiday_json(self, current_year=None):
         '''
         查询仓库中前后1年+当年的json数据
         :param current_year: 要查询的年份
         :return:
@@ -145,15 +165,15 @@
         # 防止大于当前年份+2，造成查询仓库json返回404（仓库中最多只会存在当前年份+1的数据）
         if int(current_year) >= int(self.get_current_year()) + 1:
             current_year = self.get_current_year()
         year_list = [int(current_year)-1, int(current_year), int(current_year)+1]
         # print(year_list)
         data_list = []
         for i in year_list:
-            res = self.get_holiday_json(current_year=i)
+            res = self.get_local_holiday_json(current_year=i)
             for n in res:
                 data_list.append(n)
         return data_list
 
     @staticmethod
     def get_weekday_enum_cn(week_day: int) -> str:
         '''获取中文的星期数枚举'''
@@ -253,17 +273,17 @@
     strptime, strftime = datetime.datetime.strptime, datetime.datetime.strftime
     days = (strptime(end, _format) - strptime(start, _format)).days
     return [strftime(strptime(start, _format) + datetime.timedelta(i), _format) for i in range(0, days, step)]
 
 if __name__ == '__main__':
     g = getHoliday()
     # print(getGithubHolidayJson.get_current_isoweekday())
-    # print(json.dumps(g.get_before_and_after_holiday_json()))
+    # print(json.dumps(g.get_before_and_after_holiday_json(current_year=2024), ensure_ascii=False))
     # print(getGithubHolidayJson.get_weekday_enum_cn(1))
     # print(g.get_get_holiday_cn_path())
     # 当天
-    print(g.assemble_holiday_data(today='2018-12-29'))
+    print(g.assemble_holiday_data(today='2025-05-01'))
     # print(g.assemble_holiday_data(today='2022-10-1'))
-    # print(g.get_holiday_json(current_year=2022))
+    # print(g.get_local_holiday_json(current_year=2022))
     # for i in dateRange('2021-12-17','2022-12-29'):
     #     print(g.assemble_holiday_data(i))
-    # print(g.get_today_data(today='2022-10-1', current_year=2022))
+    # print(g.get_today_data(today='2022-10-1', current_year=2022))
```

### Comparing `get_holiday_cn-1.0.5/get_holiday_cn.egg-info/PKG-INFO` & `get_holiday_cn-1.0.6/get_holiday_cn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: get-holiday-cn
-Version: 1.0.5
+Name: get_holiday_cn
+Version: 1.0.6
 Summary: 获取中国法定节假日
 Home-page: https://github.com/longweiqiang/get_holiday_cn
 Author: Weiqiang.long
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -50,7 +50,14 @@
 
 client = getHoliday()
 # 获取今日数据
 print(client.assemble_holiday_data())
 # 指定日期获取数据
 print(client.assemble_holiday_data(today='2021-10-01'))
 ```
+
+### 2022/12/27 更新说明
+刚刚推送了v1.0.5版本，在此版本前可能会获取到空数组的2023年json文件，导致现在23年假期更新后还是无法查到；如出现下图所示，可以删除本地已缓存的`2023.json`文件，下次再请求时会自动获取最新的数据
+![企业微信截图_20221227160706](https://user-images.githubusercontent.com/22344864/209655031-1a3b4185-6b8c-436c-aaee-8371c6e2e1aa.png)
+
+### 2024/04/29 更新说明
+本次版本号v1.0.6，主要修复 [issues-4](https://github.com/longweiqiang/get_holiday_cn/issues/4) 的问题，在项目中增加了某个年份文件中返回空列表的情况判断
```

### Comparing `get_holiday_cn-1.0.5/setup.py` & `get_holiday_cn-1.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "get_holiday_cn",
-    version = "1.0.5",
+    version = "1.0.6",
     author = "Weiqiang.long",
     description = "获取中国法定节假日",
     long_description = long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/longweiqiang/get_holiday_cn",
     packages = setuptools.find_packages(),
     classifiers=[
```

