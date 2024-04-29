# Comparing `tmp/coll-filter-1.2.2.tar.gz` & `tmp/coll-filter-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coll-filter-1.2.2.tar", last modified: Sun Apr 28 11:37:41 2024, max compression
+gzip compressed data, was "coll-filter-1.2.3.tar", last modified: Mon Apr 29 01:45:37 2024, max compression
```

## Comparing `coll-filter-1.2.2.tar` & `coll-filter-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:37:41.374529 coll-filter-1.2.2/
--rw-r--r--   0 summy      (501) staff       (20)      956 2024-04-28 11:37:41.373755 coll-filter-1.2.2/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      601 2024-04-28 11:37:37.000000 coll-filter-1.2.2/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:37:41.367150 coll-filter-1.2.2/cf/
--rw-r--r--   0 summy      (501) staff       (20)     6680 2024-04-28 11:16:57.000000 coll-filter-1.2.2/cf/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     9727 2024-04-28 11:25:00.000000 coll-filter-1.2.2/cf/base.py
--rw-r--r--   0 summy      (501) staff       (20)     5143 2024-04-28 10:05:34.000000 coll-filter-1.2.2/cf/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)      867 2023-11-27 02:09:24.000000 coll-filter-1.2.2/cf/utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:37:41.371737 coll-filter-1.2.2/coll_filter.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      956 2024-04-28 11:37:41.000000 coll-filter-1.2.2/coll_filter.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-04-28 11:37:41.000000 coll-filter-1.2.2/coll_filter.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-28 11:37:41.000000 coll-filter-1.2.2/coll_filter.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-28 11:32:15.000000 coll-filter-1.2.2/coll_filter.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        3 2024-04-28 11:37:41.000000 coll-filter-1.2.2/coll_filter.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-28 11:37:41.374799 coll-filter-1.2.2/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      846 2024-04-28 11:37:37.000000 coll-filter-1.2.2/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:37:41.372631 coll-filter-1.2.2/test/
--rw-r--r--   0 summy      (501) staff       (20)      277 2024-01-05 03:59:08.000000 coll-filter-1.2.2/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-29 01:45:37.606146 coll-filter-1.2.3/
+-rw-r--r--   0 summy      (501) staff       (20)      959 2024-04-29 01:45:37.605651 coll-filter-1.2.3/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      604 2024-04-29 01:45:27.000000 coll-filter-1.2.3/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-29 01:45:37.594087 coll-filter-1.2.3/cf/
+-rw-r--r--   0 summy      (501) staff       (20)     7545 2024-04-29 01:13:18.000000 coll-filter-1.2.3/cf/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    10125 2024-04-29 01:13:18.000000 coll-filter-1.2.3/cf/base.py
+-rw-r--r--   0 summy      (501) staff       (20)     5350 2024-04-29 01:13:18.000000 coll-filter-1.2.3/cf/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)      867 2023-11-27 02:09:24.000000 coll-filter-1.2.3/cf/utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-29 01:45:37.601377 coll-filter-1.2.3/coll_filter.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      959 2024-04-29 01:45:37.000000 coll-filter-1.2.3/coll_filter.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-04-29 01:45:37.000000 coll-filter-1.2.3/coll_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-29 01:45:37.000000 coll-filter-1.2.3/coll_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-28 11:32:15.000000 coll-filter-1.2.3/coll_filter.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        3 2024-04-29 01:45:37.000000 coll-filter-1.2.3/coll_filter.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-29 01:45:37.606441 coll-filter-1.2.3/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      846 2024-04-28 16:55:56.000000 coll-filter-1.2.3/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-29 01:45:37.603357 coll-filter-1.2.3/test/
+-rw-r--r--   0 summy      (501) staff       (20)      277 2024-01-05 03:59:08.000000 coll-filter-1.2.3/test/test.py
```

### Comparing `coll-filter-1.2.2/PKG-INFO` & `coll-filter-1.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coll-filter
-Version: 1.2.2
+Version: 1.2.3
 Summary: Collaborative Filtering with multi-process parallelism.
 Home-page: https://gitee.com/summry/myai
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: Collaborative Filtering,recommend
 Platform: UNKNOWN
@@ -18,15 +18,18 @@
 
     from cf import CollFilter
 
     if __name__ == '__main__':
         data = read_data(train_path)
         data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
         cf = CollFilter(data)
+
         ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
         icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
-        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+
         recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
+        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+
         cf.release()
```

### Comparing `coll-filter-1.2.2/README.rst` & `coll-filter-1.2.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -5,13 +5,16 @@
 
     from cf import CollFilter
 
     if __name__ == '__main__':
         data = read_data(train_path)
         data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
         cf = CollFilter(data)
+
         ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
         icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
-        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+
         recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
+        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+
         cf.release()
```

### Comparing `coll-filter-1.2.2/cf/__init__.py` & `coll-filter-1.2.3/cf/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,21 +37,22 @@
 def sqrt_similar_func(items: List, other: List) -> float:
     """两个item数相乘开根"""
     return 1.0 / math.sqrt(len(items) * len(other))
 
 
 class CollFilter(Generic[U, T]):
 
-    def __init__(self, data: Iterable[Tuple[U, T, float]], parallel_num=2 * os.cpu_count(), similar_fn=default_similar_func):
+    def __init__(self, data: Iterable[Tuple[U, T, float]], parallel_num=2 * os.cpu_count(),
+                 similar_fn=default_similar_func, cache_similar=False):
         if parallel_num > 1:
             from cf.pooling import PoolCollFilter
-            self.coll_filter = PoolCollFilter(data, parallel_num, similar_fn)
+            self._coll_filter = PoolCollFilter(data, parallel_num, similar_fn, cache_similar)
         else:
             from cf.base import BaseCollFilter
-            self.coll_filter = BaseCollFilter(data, similar_fn)
+            self._coll_filter = BaseCollFilter(data, similar_fn, cache_similar)
 
     def user_cf(self,
                 recall_num=64,
                 similar_num=256,
                 user_ids: Collection[U] = None,
                 user_similar: Mapping[U, Mapping[U, float]] = None,
                 similar_fn=None
@@ -62,15 +63,15 @@
         @param similar_num  每个用户最大相似用户个数
         @param user_ids  要推荐的用户列表
         @param user_similar  用户相似矩阵
         @param similar_fn  相似度计算函数
         @return {user_id: [(item_id, score),],}
         """
         assert recall_num > 0, "'recall_num' should be a positive number."
-        return self.coll_filter.user_cf(recall_num, similar_num, user_ids, user_similar, similar_fn)
+        return self._coll_filter.user_cf(recall_num, similar_num, user_ids, user_similar, similar_fn)
 
     def item_cf(self,
                 recall_num=64,
                 similar_num=256,
                 user_ids: Collection[U] = None,
                 item_similar: Mapping[T, Mapping[T, float]] = None,
                 similar_fn=None
@@ -81,94 +82,104 @@
         @param similar_num  每个物品最大相似物品个数
         @param user_ids  要推荐的用户列表
         @param item_similar  物品相似矩阵
         @param similar_fn  相似度计算函数
         @return {user_id: [(item_id, score),],}
         """
         assert recall_num > 0, "'recall_num' should be a positive number."
-        return self.coll_filter.item_cf(recall_num, similar_num, user_ids, item_similar, similar_fn)
+        return self._coll_filter.item_cf(recall_num, similar_num, user_ids, item_similar, similar_fn)
 
-    def recommend(self, user_id: U, recall_num=64, similar_num=8, similar_fn=None) -> List[Tuple[T, float]]:
+    def recommend(self, user_id: U, recall_num=64, similar_num=8, similar_fn=None, ratio=0.5) -> List[Tuple[T, float]]:
         """
         给一个用户推荐
         @param user_id  要推荐的用户
         @param recall_num  每个用户最大召回个数
         @param similar_num  每个物品最大相似物品个数
         @param similar_fn  相似度计算函数
+        @param ratio  推荐结果中item_cf所占比例
         @return [(item_id, score),]
         """
         icf = self.item_cf(recall_num, similar_num, [user_id], None, similar_fn)
-        items = icf[user_id]
+        icf_items = icf[user_id]
         if recall_num == 1:
-            if items:
-                return items
+            if icf_items:
+                return icf_items
             else:
                 return self.user_cf(recall_num, similar_num, [user_id], None, similar_fn)[user_id]
         else:
-            half = round(recall_num / 2)
             ucf_items = self.user_cf(recall_num, similar_num, [user_id], None, similar_fn)[user_id]
-            if len(items) > half and len(ucf_items) > (recall_num - half):
-                tmp = items[:half]
-                tmp.extend(ucf_items[:(recall_num - half)])
-                return tmp
-            elif len(items) < half:
-                items.extend(ucf_items[:(recall_num - half)])
-                return items
-            elif len(ucf_items) < (1-half):
-                tmp = items[:(recall_num - len(ucf_items))]
-                tmp.extend(ucf_items)
-                return tmp
-
-            return items
+            return self._fusion(icf_items, ucf_items, recall_num, ratio)
 
     def recommends(self,
                    user_ids: Collection[U],
                    recall_num=64,
                    similar_num=8,
-                   similar_fn=None
+                   similar_fn=None,
+                   ratio=0.5
                    ) -> Mapping[U, List[Tuple[T, float]]]:
         """
         给一批用户推荐
         @param user_ids  要推荐的用户列表
         @param recall_num  每个用户最大召回个数
         @param similar_num  每个物品最大相似物品个数
         @param similar_fn  相似度计算函数
+        @param ratio  推荐结果中item_cf所占比例
         @return {user_id: [(item_id, score),],}
         """
         icf = self.item_cf(recall_num, similar_num, user_ids, None, similar_fn)
         if recall_num == 1:
             user_similar = self.get_user_similar(similar_num, similar_fn)
             for user_id, items in icf.items():
                 if not items:
-                    items = self.user_cf(recall_num, similar_num, [user_id], user_similar, similar_fn)[user_id]
+                    icf[user_id] = self.user_cf(recall_num, similar_num, [user_id], user_similar, similar_fn)[user_id]
         else:
-            half = round(recall_num / 2)
             ucf = self.user_cf(recall_num, similar_num, user_ids, None, similar_fn)
-            for user_id, items in icf.items():
+            for user_id, icf_items in icf.items():
                 ucf_items = ucf[user_id]
-                if len(items) >= half and len(ucf_items) >= (recall_num - half):
-                    tmp = items[:half]
-                    tmp.extend(ucf_items[:(recall_num - half)])
-                    items = tmp
-                elif len(items) < half:
-                    items.extend(ucf_items[:(recall_num - half)])
-                elif len(ucf_items) < (1-half):
-                    tmp = items[:(recall_num - len(ucf_items))]
-                    tmp.extend(ucf_items)
-                    items = tmp
+                icf[user_id] = self._fusion(icf_items, ucf_items, recall_num, ratio)
 
         return icf
 
     def get_user_similar(self, similar_num=256, similar_fn=None) -> Mapping[U, Mapping[U, float]]:
         """
         用户相似矩阵
         """
-        return self.coll_filter.cal_similar(CFType.UCF, similar_num, similar_fn)
+        return self._coll_filter.cal_similar(CFType.UCF, similar_num, similar_fn)
 
     def get_item_similar(self, similar_num=256, similar_fn=None) -> Mapping[T, Mapping[T, float]]:
         """
         物品相似矩阵
         """
-        return self.coll_filter.cal_similar(CFType.ICF, similar_num, similar_fn)
+        return self._coll_filter.cal_similar(CFType.ICF, similar_num, similar_fn)
 
     def release(self):
-        self.coll_filter.release()
+        self._coll_filter.release()
+
+    @staticmethod
+    def _fusion(icf_items, ucf_items, recall_num, ratio):
+        ucf_items_dict = dict(ucf_items)
+        # item_cf和user_cf共同出现的先放进result_items里
+        result_items = [(item[0], item[1] + ucf_items_dict[item[0]]) for item in icf_items if item[0] in ucf_items_dict]
+        result_items_len = len(result_items)
+        if result_items_len >= recall_num:
+            return result_items[:recall_num]
+
+        leave_num = recall_num - result_items_len
+        half = round(leave_num * ratio + 0.01)  # 加0.01避免*.5是四舍五入向下取整
+        result_item_ids = [item[0] for item in result_items]
+        leave_icf_items = [item for item in icf_items if item[0] not in result_item_ids]
+        leave_ucf_items = [item for item in ucf_items if item[0] not in result_item_ids]
+        if len(leave_icf_items) > half and len(leave_ucf_items) > (leave_num - half):
+            result_items.extend(icf_items[:half])
+            result_items.extend(leave_ucf_items[:(leave_num - half)])
+            return result_items
+        elif len(leave_icf_items) < half:
+            result_items.extend(leave_icf_items)
+            result_items.extend(leave_ucf_items[:(leave_num - half)])
+            return result_items
+        elif len(leave_ucf_items) < (leave_num - half):
+            result_items.extend(leave_icf_items[:(leave_num - len(leave_ucf_items))])
+            result_items.extend(leave_ucf_items)
+            return result_items
+
+        result_items.extend(leave_icf_items[:leave_num])
+        return result_items
```

### Comparing `coll-filter-1.2.2/cf/base.py` & `coll-filter-1.2.3/cf/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -54,25 +54,29 @@
 
         print_cost_time(f"\t进程: {os.getpid()}, 处理 {len(user_items_list)} 条记录, 生成 {len(result)} 条记录, 耗时", start_time)
         return result
 
 
 class BaseCollFilter(CollFilterHelper, Generic[U, T]):
 
-    def __init__(self, data: Iterable[Tuple[U, T, float]], similar_fn=default_similar_func):
+    def __init__(self, data: Iterable[Tuple[U, T, float]], similar_fn=default_similar_func, cache_similar=False):
         self.similar_fn = similar_fn
         # {user_id: {item_id: rating},}  {item_id: {user_id: rating},}
         self.user_item_ratings, self.item_users = {}, {}
         start_time = time.perf_counter()
         cnt = 0
-        for user_id, item_id, score in data:
+        for user_id, item_id, rating in data:
             cnt += 1
-            self._data_process(user_id, item_id, score)
+            self._data_process(user_id, item_id, rating)
 
         self.item_users = {item_id: list(set(users)) for item_id, users in self.item_users.items()}
+        self._cache_similar = cache_similar
+        if cache_similar:
+            self._user_similar_cache, self._item_similar_cache = None, None
+
         print_cost_time(f"数据处理, 当前进程: {os.getpid()}, 处理 {cnt} 条记录, "
                         f"user数: {len(self.user_item_ratings)}, item数: {len(self.item_users)}, 耗时", start_time)
 
     def user_cf(self, recall_num=10, similar_num=256, user_ids=None, user_similar=None, similar_fn=None):
         """
         用户协同过滤
 
@@ -83,60 +87,81 @@
         @param similar_fn  相似度计算函数
         @return {user_id: [(item, score),],}
         """
         if user_similar is None:
             user_similar = self.cal_similar(CFType.UCF, similar_num, similar_fn)
         return self._cf(user_ids, user_similar, recall_num, CFType.UCF)
 
-    def item_cf(self, size_per_user=10, similar_num=256, user_ids=None, item_similar=None, similar_fn=None):
+    def item_cf(self, recall_num=10, similar_num=256, user_ids=None, item_similar=None, similar_fn=None):
         """
         物品协同过滤
 
-        @param size_per_user  每个用户推荐结果数目
+        @param recall_num  每个用户推荐结果数目
         @param similar_num  物品相似矩阵最大个数
         @param user_ids  要推荐的用户列表
         @param item_similar  物品相似矩阵
         @param similar_fn  相似度计算函数
         @return {user_id: [(item, score),],}
         """
         if item_similar is None:
             item_similar = self.cal_similar(CFType.ICF, similar_num, similar_fn)
-        return self._cf(user_ids, item_similar, size_per_user, CFType.ICF)
+        return self._cf(user_ids, item_similar, recall_num, CFType.ICF)
 
     def cal_similar(self, cf_type: CFType, similar_num=256, similar_fn=None):
         """
         计算相似度
 
         @return dict{:List()}    {user1: {user2: similar}}
         """
+        if self._cache_similar:
+            if CFType.UCF == cf_type:
+                if not self._user_similar_cache:
+                    self._user_similar_cache = self._cal_similar(cf_type, similar_num, similar_fn)
+                return self._user_similar_cache
+            else:
+                if not self._item_similar_cache:
+                    self._item_similar_cache = self._cal_similar(cf_type, similar_num, similar_fn)
+                return self._item_similar_cache
+        else:
+            return self._cal_similar(cf_type, similar_num, similar_fn)
+
+    def release(self):
+        del self.user_item_ratings
+        del self.item_users
+        if self._cache_similar:
+            del self._user_similar_cache
+            del self._item_similar_cache
+
+    def _cal_similar(self, cf_type: CFType, similar_num, similar_fn):
+        """
+        计算相似度
+
+        @return dict{:List()}    {user1: {user2: similar}}
+        """
         print(f'开始{cf_type.value}相似度计算, similar_num = {similar_num}')
         func_start_time = time.perf_counter()
         dict1, items_list, cal_similar_func = self._get_cal_similar_inputs(cf_type)
         similar_fn = similar_fn if similar_fn else self.similar_fn
         similar = cal_similar_func(dict1, items_list, similar_fn)
         similar = sort_similar(similar, similar_num)
         print_cost_time(f"完成{cf_type.value}相似度计算, 当前进程: {os.getpid()}, 总生成 {len(similar)} 条记录, 总耗时", func_start_time)
         return similar
 
-    def release(self):
-        del self.user_item_ratings
-        del self.item_users
-
-    def _data_process(self, user_id: U, item_id: T, score: float):
+    def _data_process(self, user_id: U, item_id: T, rating: float):
         user_item_rating = self.user_item_ratings.get(user_id)
         if user_item_rating:
-            user_item_rating[item_id] = user_item_rating.get(item_id, 0) + score
+            user_item_rating[item_id] = user_item_rating.get(item_id, 0) + rating
         else:
-            self.user_item_ratings[user_id] = {item_id: score}
+            self.user_item_ratings[user_id] = {item_id: rating}
 
         item_user_rating = self.item_users.get(item_id)
         if item_user_rating:
-            item_user_rating[user_id] = item_user_rating.get(user_id, 0) + score
+            item_user_rating[user_id] = item_user_rating.get(user_id, 0) + rating
         else:
-            self.item_users[item_id] = {user_id: score}
+            self.item_users[item_id] = {user_id: rating}
 
     def _get_cal_similar_inputs(self, cf_type: CFType):
         if cf_type == CFType.UCF:
             return self.user_item_ratings, self.item_users.values(), self._cal_ucf_similar
         else:
             return self.item_users, self.user_item_ratings.values(), self._cal_icf_similar
 
@@ -180,43 +205,22 @@
                                                                                           dict1.get(item2, []))
         print_cost_time(f"\t进程: {os.getpid()}, 生成 {len(similar)} 条记录, 耗时", start_time)
         return similar
 
     def _cf(self, user_ids, similar_dict, recall_num, cf_type: CFType):
         print(f'开始{cf_type.value}推理, recall_num = {recall_num}')
         func_start_time = time.perf_counter()
-        user_items_list = list(map(lambda x: (x, self.user_item_ratings.get(x, {})), user_ids)) if user_ids else self.user_item_ratings.items()
+        if user_ids:
+            if not set(user_ids).intersection(self.user_item_ratings.keys()):
+                return {user_id: [] for user_id in user_ids}
+
+            user_items_list = [(user_id, self.user_item_ratings.get(user_id, {})) for user_id in user_ids]
+        else:
+            user_items_list = self.user_item_ratings.items()
 
         if cf_type == CFType.UCF:
             cf_result = self._rating_user_cf(self.user_item_ratings, similar_dict, user_items_list, recall_num)
         else:
             cf_result = self._rating_item_cf(self.user_item_ratings, similar_dict, user_items_list, recall_num)
         print_cost_time(f"完成{cf_type.value}推理, 当前进程: {os.getpid()}, 生成{len(cf_result)}条记录, 总耗时", func_start_time)
         return cf_result
 
-
-if __name__ == '__main__':
-    import json
-    from cf.utils import read_data, pre_process
-    # train_path = '/Users/summy/project/rust/ai/train.csv'
-    # data = read_data(train_path)
-    # data = pre_process(data)
-    # cf = BaseCollFilter(data)
-    # ucf = cf.user_cf()
-    # with open('ucf_pool', 'w') as f:
-    #     json.dump(ucf, f)
-    # icf = cf.item_cf()
-    # with open('icf_pool', 'w') as f:
-    #     json.dump(icf, f)
-
-    def handle(line) -> (int, str, float):
-        user_id, item_id, _, _, _ = line.strip().split(",")
-        return int(user_id), item_id, 1
-
-    train_path = '/Users/summy/project/python/work/video_rec_recall/data/V0002_20_25.csv'
-    data = read_data(train_path)[:50000]
-    data = pre_process(data, handle)
-    cf = BaseCollFilter(data)
-    ucf = cf.user_cf()
-    icf = cf.item_cf()
-
-
```

### Comparing `coll-filter-1.2.2/cf/pooling.py` & `coll-filter-1.2.3/cf/pooling.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,43 +59,50 @@
 
     def release(self):
         self.pool.close()
 
 
 class PoolCollFilter(BaseCollFilter):
 
-    def __init__(self, data: Iterable[Tuple[U, T, float]], parallel_num=0, similar_fn=default_similar_func):
-        super().__init__(data, similar_fn)
+    def __init__(self, data: Iterable[Tuple[U, T, float]], parallel_num=0, similar_fn=default_similar_func,
+                 cache_similar=False):
+        super().__init__(data, similar_fn, cache_similar)
         self.processor = PoolMultiProcessor(parallel_num)
 
-    def cal_similar(self, cf_type: CFType, similar_num=256, similar_fn=None):
+    def release(self):
+        super().release()
+
+    def _cal_similar(self, cf_type: CFType, similar_num, similar_fn):
         """
         计算相似度
 
         @return dict{:dict}    {user1: {user2: similar}}
         """
         print(f'开始{cf_type.value}相似度计算, similar_num: {similar_num}')
         func_start_time = time.perf_counter()
         dict1, items_list, cal_similar_func = self._get_cal_similar_inputs(cf_type)
         items_list = list(items_list)
         similar_fn = similar_fn if similar_fn else self.similar_fn
         similar = self.processor.cal_similar(dict1, items_list, cal_similar_func, similar_fn)
         similar = sort_similar(similar, similar_num)
         print_cost_time(f"完成{cf_type.value}相似度计算, 当前进程: {os.getpid()}, 总生成 {len(similar)} 条记录, 总耗时", func_start_time)
         return similar
-
-    def release(self):
-        super().release()
         self.processor.release()
 
     def _cf(self, user_ids, similar_dict, recall_num, cf_type: CFType):
         print(f'开始{cf_type.value}推理, recall_num: {recall_num}')
         func_start_time = time.perf_counter()
-        user_items_list = list(map(lambda x: (x, self.user_item_ratings.get(x, [])), user_ids) if user_ids
-                               else self.user_item_ratings.items())
+        if user_ids:
+            if not set(user_ids).intersection(self.user_item_ratings.keys()):
+                return {user_id: [] for user_id in user_ids}
+
+            user_items_list = list(map(lambda x: (x, self.user_item_ratings.get(x, [])), user_ids))
+        else:
+            user_items_list = self.user_item_ratings.items()
+
         cf_func = self._rating_user_cf if cf_type == CFType.UCF else self._rating_item_cf
         if len(user_items_list) > 4096:
             cf_result = self.processor.cf(self.user_item_ratings, user_items_list, similar_dict, recall_num, cf_func)
         else:
             cf_result = cf_func(self.user_item_ratings, similar_dict, user_items_list, recall_num)
         print_cost_time(f"完成{cf_type.value}推理, 当前进程: {os.getpid()}, 生成{len(cf_result)}条记录, 总耗时", func_start_time)
         return cf_result
```

### Comparing `coll-filter-1.2.2/cf/utils.py` & `coll-filter-1.2.3/cf/utils.py`

 * *Files identical despite different names*

### Comparing `coll-filter-1.2.2/coll_filter.egg-info/PKG-INFO` & `coll-filter-1.2.3/coll_filter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coll-filter
-Version: 1.2.2
+Version: 1.2.3
 Summary: Collaborative Filtering with multi-process parallelism.
 Home-page: https://gitee.com/summry/myai
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: Collaborative Filtering,recommend
 Platform: UNKNOWN
@@ -18,15 +18,18 @@
 
     from cf import CollFilter
 
     if __name__ == '__main__':
         data = read_data(train_path)
         data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
         cf = CollFilter(data)
+
         ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
         icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
-        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+
         recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
+        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+
         cf.release()
```

### Comparing `coll-filter-1.2.2/setup.py` & `coll-filter-1.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='coll-filter',
     packages=['cf'],
     description="Collaborative Filtering with multi-process parallelism.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.2',
+    version='1.2.3',
     url='https://gitee.com/summry/myai',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['Collaborative Filtering', 'recommend'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

