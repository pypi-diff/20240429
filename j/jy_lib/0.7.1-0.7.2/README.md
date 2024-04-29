# Comparing `tmp/jy_lib-0.7.1.tar.gz` & `tmp/jy_lib-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.7.1.tar` & `jy_lib-0.7.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2083 2024-01-01 02:29:02.554641 jy_lib-0.7.1/.gitignore
--rw-r--r--   0        0        0      285 2024-01-01 02:29:02.554755 jy_lib-0.7.1/.pypirc
--rw-r--r--   0        0        0     1073 2024-01-01 02:29:02.555085 jy_lib-0.7.1/LICENSE
--rw-r--r--   0        0        0      573 2024-04-21 14:22:14.414420 jy_lib-0.7.1/Pipfile
--rw-r--r--   0        0        0    40838 2024-01-01 02:29:02.555480 jy_lib-0.7.1/Pipfile.lock
--rw-r--r--   0        0        0       10 2024-01-01 02:29:02.555572 jy_lib-0.7.1/README.md
--rw-r--r--   0        0        0      469 2024-01-01 02:29:02.555665 jy_lib-0.7.1/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-27 14:14:23.202665 jy_lib-0.7.1/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2024-01-01 02:29:02.555927 jy_lib-0.7.1/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2024-01-01 02:29:02.556043 jy_lib-0.7.1/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2024-01-01 02:29:02.556135 jy_lib-0.7.1/jy_lib/base.py
--rw-r--r--   0        0        0    11460 2024-04-26 13:44:43.888654 jy_lib-0.7.1/jy_lib/cache.py
--rw-r--r--   0        0        0     8541 2024-04-27 14:14:12.824322 jy_lib-0.7.1/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-27 14:14:12.824508 jy_lib-0.7.1/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2024-01-01 02:29:02.556414 jy_lib-0.7.1/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2024-01-01 02:29:02.556554 jy_lib-0.7.1/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-04-21 14:22:14.416027 jy_lib-0.7.1/jy_lib/date.py
--rw-r--r--   0        0        0      931 2024-01-01 02:29:02.556726 jy_lib-0.7.1/jy_lib/decorator.py
--rw-r--r--   0        0        0     5916 2024-04-26 13:44:43.889079 jy_lib-0.7.1/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-04-21 14:22:14.416177 jy_lib-0.7.1/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2024-01-01 02:29:02.556936 jy_lib-0.7.1/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-04-21 14:22:14.416596 jy_lib-0.7.1/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2024-01-01 02:29:02.557127 jy_lib-0.7.1/jy_lib/nav.py
--rw-r--r--   0        0        0     1702 2024-04-27 14:14:12.824614 jy_lib-0.7.1/jy_lib/reader.py
--rw-r--r--   0        0        0    18478 2024-04-21 14:22:14.416811 jy_lib-0.7.1/jy_lib/smb_client.py
--rw-r--r--   0        0        0    22173 2024-04-26 13:44:43.889377 jy_lib-0.7.1/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-04-21 14:22:14.417332 jy_lib-0.7.1/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2024-01-01 02:29:02.557631 jy_lib-0.7.1/jy_lib/time.py
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557712 jy_lib-0.7.1/publish-jypi.sh
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557791 jy_lib-0.7.1/publish-pypi.sh
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557873 jy_lib-0.7.1/publish-test.sh
--rw-r--r--   0        0        0      639 2024-04-21 14:22:14.417488 jy_lib-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-21 14:22:14.417721 jy_lib-0.7.1/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2083 2024-01-01 02:29:02.554641 jy_lib-0.7.2/.gitignore
+-rw-r--r--   0        0        0      285 2024-01-01 02:29:02.554755 jy_lib-0.7.2/.pypirc
+-rw-r--r--   0        0        0     1073 2024-01-01 02:29:02.555085 jy_lib-0.7.2/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-21 14:22:14.414420 jy_lib-0.7.2/Pipfile
+-rw-r--r--   0        0        0    40838 2024-01-01 02:29:02.555480 jy_lib-0.7.2/Pipfile.lock
+-rw-r--r--   0        0        0       10 2024-01-01 02:29:02.555572 jy_lib-0.7.2/README.md
+-rw-r--r--   0        0        0      469 2024-01-01 02:29:02.555665 jy_lib-0.7.2/README_Project.md
+-rw-r--r--   0        0        0      518 2024-04-29 13:37:38.658367 jy_lib-0.7.2/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2024-01-01 02:29:02.555927 jy_lib-0.7.2/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2024-01-01 02:29:02.556043 jy_lib-0.7.2/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2024-01-01 02:29:02.556135 jy_lib-0.7.2/jy_lib/base.py
+-rw-r--r--   0        0        0    11460 2024-04-26 13:44:43.888654 jy_lib-0.7.2/jy_lib/cache.py
+-rw-r--r--   0        0        0    11967 2024-04-29 13:37:23.357311 jy_lib-0.7.2/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-27 14:14:12.824508 jy_lib-0.7.2/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2024-01-01 02:29:02.556414 jy_lib-0.7.2/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2024-01-01 02:29:02.556554 jy_lib-0.7.2/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-04-21 14:22:14.416027 jy_lib-0.7.2/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2024-01-01 02:29:02.556726 jy_lib-0.7.2/jy_lib/decorator.py
+-rw-r--r--   0        0        0     5916 2024-04-26 13:44:43.889079 jy_lib-0.7.2/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-04-21 14:22:14.416177 jy_lib-0.7.2/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2024-01-01 02:29:02.556936 jy_lib-0.7.2/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-04-21 14:22:14.416596 jy_lib-0.7.2/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2024-01-01 02:29:02.557127 jy_lib-0.7.2/jy_lib/nav.py
+-rw-r--r--   0        0        0     2194 2024-04-29 13:37:23.357463 jy_lib-0.7.2/jy_lib/reader.py
+-rw-r--r--   0        0        0    18478 2024-04-21 14:22:14.416811 jy_lib-0.7.2/jy_lib/smb_client.py
+-rw-r--r--   0        0        0    22173 2024-04-26 13:44:43.889377 jy_lib-0.7.2/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-04-21 14:22:14.417332 jy_lib-0.7.2/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2024-01-01 02:29:02.557631 jy_lib-0.7.2/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557712 jy_lib-0.7.2/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557791 jy_lib-0.7.2/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557873 jy_lib-0.7.2/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-21 14:22:14.417488 jy_lib-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-21 14:22:14.417721 jy_lib-0.7.2/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.7.2/PKG-INFO
```

### Comparing `jy_lib-0.7.1/.gitignore` & `jy_lib-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/LICENSE` & `jy_lib-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/Pipfile` & `jy_lib-0.7.2/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/Pipfile.lock` & `jy_lib-0.7.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/__init__.py` & `jy_lib-0.7.2/jy_lib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     SymbolFlag,
     SymbolSubType,
     SymbolType,
     WarrantsType,
 )
 from .symbol_em import EMParser, KLineRecord, TrendRecord
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
```

### Comparing `jy_lib-0.7.1/jy_lib/auth_client.py` & `jy_lib-0.7.2/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/bank.py` & `jy_lib-0.7.2/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/base.py` & `jy_lib-0.7.2/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/cache.py` & `jy_lib-0.7.2/jy_lib/cache.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/clickhouse.py` & `jy_lib-0.7.2/jy_lib/clickhouse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # -*- coding: utf-8 -*-
+import collections
+import datetime
+import threading
 from abc import abstractmethod
 import clickhouse_driver
 import io
 import os
 import polars as pl
 import requests
 import time
 import urllib.parse
 import zstandard
-from typing import Dict, Type, List, Any
+from typing import Dict, Type, List, Any, Tuple, DefaultDict
 from loguru import logger
 from jy_lib.compressor import ZstdStreamCompressor
 from jy_lib.interrupt_protect import KeyboardInterruptProtect
 
 
 class FieldDetail:
-    def __init__(self, name: str, read_dtype: Type = pl.Float64, dtype: Any = None,
+    def __init__(self, name: str, read_dtype: Any = pl.Float64, dtype: Any = None,
                  convertor: pl.Expr = None, comment: str = '', drop: bool = False):
         self.name: str = name                           # 字段名
-        self.read_dtype: Type = read_dtype              # 从csv读入pl的数据类型
+        self.read_dtype: Any = read_dtype              # 从csv读入pl的数据类型
         self.dtype: Type | pl.Datetime = dtype or self.read_dtype     # 从csv读入pl的数据类型
         if convertor is not None:
             self.convertor: pl.Expr = convertor
         elif read_dtype != self.dtype:
             self.convertor = pl.col(name).cast(self.dtype)
         else:
             self.convertor = None
@@ -57,15 +60,36 @@
 
     def ch_column(self, nullable: bool = True) -> str:
         """clickhouse中对应列的创建语句"""
         ch_type: str = f'Nullable({self.ch_type})' if nullable else self.ch_type
         return f"`{self.name}` {ch_type} {self.ch_comment} {self.ch_codec}"
 
 
+class DefaultFieldDetails:
+    def __init__(self):
+        self.fds: Dict[str, FieldDetail] = {}
+
+    def add(self, fd: FieldDetail | List[FieldDetail]):
+        if isinstance(fd, FieldDetail):
+            fd = [fd]
+        assert isinstance(fd, list)
+        for _fd in fd:
+            assert isinstance(_fd, FieldDetail)
+            assert _fd.name not in self.fds
+            self.fds[_fd.name] = _fd
+
+    def get(self, name: str) -> FieldDetail:
+        return self.fds.get(name)
+
+    def __getitem__(self, item):
+        return self.fds[item]
+
+
 class QuoteStruct:
+    subclasses: List = []
     fields: List[FieldDetail] = []
     priority_cols: List[str] = []
 
     def __class_getitem__(cls, item) -> FieldDetail:
         for fd in cls.fields:
             if fd.name == item:
                 return fd
@@ -120,14 +144,38 @@
     def pk1(cls) -> str:
         return cls.priority_cols[0]
 
     @classmethod
     def pk2(cls) -> str:
         return cls.priority_cols[1]
 
+    @classmethod
+    def sql_create_table(cls, fds: DefaultFieldDetails, period: str = None):
+        """建表语句"""
+        cols: List[str] = []
+        for i, name in enumerate(cls.cols()):
+            fd: FieldDetail | None = fds.get(name) or cls.get(name)
+            if not fd:
+                assert i == 0, '非主键列不能为空'
+                fd = FieldDetail(name=cls.pk1(), read_dtype=pl.String, dtype=pl.String)
+            if i == 0:
+                assert fd.dtype == pl.String
+            elif i == 1:
+                assert fd.dtype.is_integer() or fd.dtype.base_type() == pl.Datetime
+            if not fd.drop:
+                cols.append(fd.ch_column(nullable=name not in cls.priority_cols))
+        tb: str = '\n' + ',\n'.join(cols)
+        sql: str = f"""
+            CREATE TABLE IF NOT EXISTS `{cls.table_name(period=period)}` ({tb})
+            ENGINE = ReplacingMergeTree()
+            PARTITION BY sipHash64(`{cls.pk1()}`) % 256
+            PRIMARY KEY (`{cls.pk1()}`, `{cls.pk2()}`)
+            ORDER BY (`{cls.pk1()}`, `{cls.pk2()}`)"""
+        return sql
+
 
 class KlinesStruct(QuoteStruct):
     """K线数据"""
     fields: List[FieldDetail] = []
     priority_cols: List[str] = ['symbol', 'datetime']
 
     @classmethod
@@ -152,58 +200,38 @@
     priority_cols: List[str] = ['symbol', 'id']
 
     @classmethod
     def table_name(cls, period: str | None = None) -> str:
         return cls.__name__
 
 
-class DefaultFieldDetails:
-    def __init__(self):
-        self.fds: Dict[str, FieldDetail] = {}
-
-    def add(self, fd: FieldDetail | List[FieldDetail]):
-        if isinstance(fd, FieldDetail):
-            fd = [fd]
-        assert isinstance(fd, list)
-        for _fd in fd:
-            assert isinstance(_fd, FieldDetail)
-            assert _fd.name not in self.fds
-            self.fds[_fd.name] = _fd
-
-    def get(self, name: str) -> FieldDetail:
-        return self.fds.get(name)
-
-    def __getitem__(self, item):
-        return self.fds[item]
-
-
 class ClickHouse:
-
     def __init__(self, url: str, http_port: int = 8123):
         self.client = clickhouse_driver.Client.from_url(url=url)
         self.http_port: int = http_port
         sp = urllib.parse.urlsplit(url)
         self.database_name: str = os.path.basename(sp.path)
         assert not sp.path or sp.path == f'/{self.database_name}'
         self.url_http: str = f'http://{sp.hostname}:{http_port}'
         self.credential: Dict = {
             'user': sp.username,
             'password': sp.password,
         }
+        self.table_locks: DefaultDict[str, threading.Lock] = collections.defaultdict(threading.Lock)
         self.execute = self.client.execute
 
     def bulk_insert(self, table_name: str, df: pl.DataFrame):
         columns: str = ', '.join([f'`{column}`' for column in df.columns])
-        sql: str = f'INSERT INTO `{self.database_name}`.`{table_name}`({columns}) VALUES'
+        sql: str = f'INSERT INTO `{table_name}`({columns}) VALUES'
         with KeyboardInterruptProtect():
-            logger.debug(f'[{self.database_name}.{table_name}]准备插入{df.height:12,d}条数据')
+            logger.debug(f'[{table_name}]准备插入{df.height:12,d}条数据')
             t1: float = time.time()
             self.client.execute(query=sql, params=df.to_dicts())
             t2: float = time.time()
-            logger.success(f'[{self.database_name}.{table_name}]成功插入{df.height:12,d}条数据 耗时{t2 - t1:0.0f}秒')
+            logger.success(f'[{table_name}]成功插入{df.height:12,d}条数据 耗时{t2 - t1:0.0f}秒')
 
     def import_csv(self, table_name: str, csv: str, height: int = None):
         sql: str = f'INSERT INTO `{self.database_name}`.`{table_name}` FORMAT CSVWithNames'
         params: Dict = {
             'query': sql,
             **self.credential,
             'enable_http_compression': 1,
@@ -219,30 +247,78 @@
             return
         assert height >= 0
         csv: bytes = csv.encode('utf-8')
         with ZstdStreamCompressor(size=len(csv), level=zstandard.STRATEGY_FAST) as sc:
             sc.update(data=csv)
             stream: io.BytesIO = sc.stream
         with KeyboardInterruptProtect():
-            logger.debug(f'[{self.database_name}.{table_name}]准备插入{height:12,d}条数据')
+            logger.debug(f'[{table_name}]准备插入{height:12,d}条数据')
             r = requests.post(
                 url=self.url_http,
                 params=params,
                 data=stream.getvalue(),
                 headers={
                     'Content-Encoding': 'zstd',
                     'Accept-Encoding': 'zstd',
                 },
             )
             t2: float = time.time()
         assert r.status_code == 200, f'[{r.status_code}]{r.text}'
         if r.text:
             logger.info(r.text)
-        logger.success(f'[{self.database_name}.{table_name}]成功插入{height:12,d}条数据 耗时{t2 - t1:0.0f}秒')
+        logger.success(f'[{table_name}]成功插入{height:12,d}条数据 耗时{t2 - t1:0.0f}秒')
 
-    def import_df(self, table_name: str, df: pl.DataFrame, datetime_format='%Y-%m-%d %H:%M:%S%.f'):
+    def import_df(self, table_name: str, df: pl.DataFrame, pks: Tuple):
+        """将polars.DataFrame导入ClickHouse,约束列为pks"""
+        datetime_format: str = '%Y-%m-%d %H:%M:%S.%f'
         assert self.database_name
-        return self.import_csv(
-            table_name=table_name,
-            csv=df.write_csv(include_header=True, datetime_format=datetime_format),
-            height=df.height
-        )
+        assert pks and set(df.columns).issuperset(pks)
+        # 按主键去重
+        df = df.unique(subset=pks)
+        # 通常第1主键为symbol
+        pk1: str = pks[0]
+        idx1: int = df.columns.index(pk1)
+        assert df.dtypes[idx1] == pl.String
+        pk1_vs = df[pk1].unique()
+        outputs: str = ', '.join([f'`{pk}`' for pk in pks])
+        sql = f"SELECT {outputs} FROM `{table_name}` WHERE "
+        if pk1_vs.len() == 1:
+            sql += f"`{pk1}` = '{pk1_vs.to_list()[0]}' "
+        else:
+            sql += f"`{pk1}` IN {pk1_vs.to_list()} "
+        if len(pks) == 2:
+            # 通常第2主键为id或datetime
+            pk2: str = pks[1]
+            idx2: int = df.columns.index(pk2)
+            if df.dtypes[idx2].is_integer():
+                pk2_min: int = df[pk2].min()
+                pk2_max: int = df[pk2].max()
+                sql += f"AND `{pk2}` BETWEEN {pk2_min} AND {pk2_max}"
+            elif df.dtypes[idx2].base_type() == pl.Datetime:
+                pk2_min: datetime.datetime = df[pk2].min()
+                pk2_min: str = pk2_min.strftime(f'{datetime_format}')
+                pk2_max: datetime.datetime = df[pk2].max()
+                pk2_max: str = pk2_max.strftime(f'{datetime_format}')
+                sql += f"AND `{pk2}` BETWEEN '{pk2_min}' AND '{pk2_max}'"
+            elif df.dtypes[idx2] == pl.String:
+                sql += f"AND `{pk2}` IN {df[pk2].unique().to_list()}"
+            else:
+                raise TypeError(df.dtypes[idx2])
+
+        with self.table_locks[table_name]:
+            rs: List[Tuple] = self.execute(sql, columnar=True)
+            if rs:
+                # 多列反选
+                exists: pl.DataFrame = pl.DataFrame(dict(zip(pks, rs)))
+                converts = []
+                for pk in pks:
+                    if exists[pk].dtype != df[pk].dtype:
+                        converts.append(pl.col(pk).cast(df[pk].dtype))
+                if converts:
+                    exists = exists.with_columns(converts)
+                df = df.join(exists, on=pks, how='anti')
+            # 确定df转换为csv时候的时间格式
+            return self.import_csv(
+                table_name=table_name,
+                csv=df.write_csv(include_header=True, datetime_format='%Y-%m-%d %H:%M:%S%.9f'),
+                height=df.height
+            )
```

### Comparing `jy_lib-0.7.1/jy_lib/compressor.py` & `jy_lib-0.7.2/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/country.py` & `jy_lib-0.7.2/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/currency.py` & `jy_lib-0.7.2/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/date.py` & `jy_lib-0.7.2/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/decorator.py` & `jy_lib-0.7.2/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/exchange.py` & `jy_lib-0.7.2/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/interrupt_protect.py` & `jy_lib-0.7.2/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/lock.py` & `jy_lib-0.7.2/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/math.py` & `jy_lib-0.7.2/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/nav.py` & `jy_lib-0.7.2/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/reader.py` & `jy_lib-0.7.2/jy_lib/reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import os
 import zipfile
 import zstandard
-from typing import IO, AnyStr, Iterator, Tuple
+from typing import IO, AnyStr, Iterator, Tuple, List
 
 
 class TextReader:
     """多行文本分块读取器"""
 
     @classmethod
     def iter_zst_text(cls, f: AnyStr | IO, size: int = 64 * 1024 ** 2) -> Iterator[Tuple[str, str | None]]:
@@ -33,17 +33,28 @@
                 if zi.is_dir():
                     continue
                 with zf.open(zi) as stream:
                     for text in cls.iter_stream_text(stream=stream, size=size):
                         yield text, zi.filename
 
     @classmethod
-    def iter_stream_text(cls, stream: IO, size: int = 64 * 1024 ** 2) -> Iterator[str]:
+    def iter_stream_text(cls, stream: IO, size: int = 64 * 1024 ** 2, encodings: Tuple = ('utf-8', 'gbk')) -> Iterator[str]:
+        for payload in cls.iter_stream_bytes(stream=stream, size=size):
+            for i, encoding in enumerate(encodings):
+                try:
+                    text: str = payload.decode(encoding)
+                    yield text
+                    break
+                except Exception as e:
+                    if i == len(encodings) - 1:
+                        raise e
+
+    @classmethod
+    def iter_stream_bytes(cls, stream: IO, size: int = 64 * 1024 ** 2) -> Iterator[bytes]:
         tail: bytes = b''
         i: int = 0
         while segment := stream.read(size):  # 每次处理size大小的多行文本
             idx: int = segment.rfind(b'\n')
-            text: bytes = tail + segment[:idx + 1]
+            payload: bytes = tail + segment[:idx + 1]
             tail: bytes = segment[idx + 1:]
-            text: str = text.decode('utf-8')
-            yield text
+            yield payload
             i += 1
```

### Comparing `jy_lib-0.7.1/jy_lib/smb_client.py` & `jy_lib-0.7.2/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/symbol.py` & `jy_lib-0.7.2/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/symbol_em.py` & `jy_lib-0.7.2/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/jy_lib/time.py` & `jy_lib-0.7.2/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.1/pyproject.toml` & `jy_lib-0.7.2/pyproject.toml`

 * *Files identical despite different names*

