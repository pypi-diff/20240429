# Comparing `tmp/dbmaster-0.1.1-py3-none-any.whl.zip` & `tmp/dbmaster-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,24 @@
-Zip file size: 11916 bytes, number of entries: 17
+Zip file size: 18024 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat      178 b- defN 24-Apr-27 03:18 dbmaster/__init__.py
--rw-rw-rw-  2.0 fat      501 b- defN 24-Apr-27 03:18 dbmaster/__main__.py
--rw-rw-rw-  2.0 fat     1827 b- defN 24-Apr-27 03:18 dbmaster/command.py
--rw-rw-rw-  2.0 fat     2013 b- defN 24-Apr-27 03:18 dbmaster/config.py
--rw-rw-rw-  2.0 fat     1615 b- defN 24-Apr-27 03:18 dbmaster/util.py
--rw-rw-rw-  2.0 fat       43 b- defN 24-Apr-27 03:18 dbmaster/catalog/__init__.py
--rw-rw-rw-  2.0 fat     1475 b- defN 24-Apr-27 03:18 dbmaster/catalog/base.py
--rw-rw-rw-  2.0 fat     4356 b- defN 24-Apr-27 04:07 dbmaster/catalog/kline.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 24-Apr-28 21:55 dbmaster/__main__.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-Apr-28 21:55 dbmaster/_version.py
+-rw-rw-rw-  2.0 fat     4154 b- defN 24-Apr-28 21:55 dbmaster/command.py
+-rw-rw-rw-  2.0 fat     2002 b- defN 24-Apr-28 21:55 dbmaster/config.py
+-rw-rw-rw-  2.0 fat     1158 b- defN 24-Apr-27 03:18 dbmaster/config_example.toml
+-rw-rw-rw-  2.0 fat     4987 b- defN 24-Apr-28 21:55 dbmaster/util.py
+-rw-rw-rw-  2.0 fat       43 b- defN 24-Apr-28 02:40 dbmaster/catalog/__init__.py
+-rw-rw-rw-  2.0 fat      155 b- defN 24-Apr-28 21:55 dbmaster/catalog/base.py
+-rw-rw-rw-  2.0 fat     5176 b- defN 24-Apr-28 21:55 dbmaster/catalog/kline.py
+-rw-rw-rw-  2.0 fat       42 b- defN 24-Apr-28 21:55 dbmaster/derived/__init__.py
+-rw-rw-rw-  2.0 fat      288 b- defN 24-Apr-28 21:55 dbmaster/derived/base.py
+-rw-rw-rw-  2.0 fat     8862 b- defN 24-Apr-28 21:55 dbmaster/derived/pmom.py
 -rw-rw-rw-  2.0 fat       45 b- defN 24-Apr-27 03:18 dbmaster/vendor/__init__.py
--rw-rw-rw-  2.0 fat      797 b- defN 24-Apr-27 03:18 dbmaster/vendor/base.py
--rw-rw-rw-  2.0 fat     4523 b- defN 24-Apr-27 03:18 dbmaster/vendor/binance.py
--rw-rw-rw-  2.0 fat     1071 b- defN 24-Apr-27 04:16 dbmaster-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4207 b- defN 24-Apr-27 04:16 dbmaster-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 04:16 dbmaster-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       52 b- defN 24-Apr-27 04:16 dbmaster-0.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-27 04:16 dbmaster-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1352 b- defN 24-Apr-27 04:16 dbmaster-0.1.1.dist-info/RECORD
-17 files, 24156 bytes uncompressed, 9700 bytes compressed:  59.8%
+-rw-rw-rw-  2.0 fat     1268 b- defN 24-Apr-28 21:55 dbmaster/vendor/base.py
+-rw-rw-rw-  2.0 fat     4509 b- defN 24-Apr-28 21:55 dbmaster/vendor/binance.py
+-rw-rw-rw-  2.0 fat     1071 b- defN 24-Apr-28 21:55 dbmaster-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4207 b- defN 24-Apr-28 21:55 dbmaster-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 21:55 dbmaster-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       52 b- defN 24-Apr-28 21:55 dbmaster-0.2.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-28 21:55 dbmaster-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1758 b- defN 24-Apr-28 21:55 dbmaster-0.2.0.dist-info/RECORD
+22 files, 42306 bytes uncompressed, 15180 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,52 +1,67 @@
 Filename: dbmaster/__init__.py
 Comment: 
 
 Filename: dbmaster/__main__.py
 Comment: 
 
+Filename: dbmaster/_version.py
+Comment: 
+
 Filename: dbmaster/command.py
 Comment: 
 
 Filename: dbmaster/config.py
 Comment: 
 
+Filename: dbmaster/config_example.toml
+Comment: 
+
 Filename: dbmaster/util.py
 Comment: 
 
 Filename: dbmaster/catalog/__init__.py
 Comment: 
 
 Filename: dbmaster/catalog/base.py
 Comment: 
 
 Filename: dbmaster/catalog/kline.py
 Comment: 
 
+Filename: dbmaster/derived/__init__.py
+Comment: 
+
+Filename: dbmaster/derived/base.py
+Comment: 
+
+Filename: dbmaster/derived/pmom.py
+Comment: 
+
 Filename: dbmaster/vendor/__init__.py
 Comment: 
 
 Filename: dbmaster/vendor/base.py
 Comment: 
 
 Filename: dbmaster/vendor/binance.py
 Comment: 
 
-Filename: dbmaster-0.1.1.dist-info/LICENSE
+Filename: dbmaster-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: dbmaster-0.1.1.dist-info/METADATA
+Filename: dbmaster-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: dbmaster-0.1.1.dist-info/WHEEL
+Filename: dbmaster-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: dbmaster-0.1.1.dist-info/entry_points.txt
+Filename: dbmaster-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: dbmaster-0.1.1.dist-info/top_level.txt
+Filename: dbmaster-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dbmaster-0.1.1.dist-info/RECORD
+Filename: dbmaster-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dbmaster/__main__.py

```diff
@@ -1,21 +1,50 @@
+from collections import defaultdict
+import json
 import fire
 
-
-from dbmaster.command import Update
+from dbmaster.command import Update, Compute
 
 
 class Main:
     """DBMaster command line interface.
 
     Environment Variables:
         - DBMASTER_CONFIG_PATH: Path to config file
         - DBMASTER_MAX_WORKERS: Max number of workers, default is number of cpu cores
             set lower if you experience too frequent bans from vendor API or database locking.
     """
 
     def __init__(self):
         self.update = Update()
+        self.compute = Compute()
+
+    def list(self) -> None:
+        """List all available catalogs and vendors."""
+        from dbmaster.catalog import CatalogBase
+        from dbmaster.derived import DerivedBase
+        from dbmaster.vendor import VendorBase
+        from dbmaster.util import get_subclasses
+
+        vendor_clses = list(get_subclasses(VendorBase))
+
+        catelog_clses = list(get_subclasses(CatalogBase))
+        catalog_holder = defaultdict(list)
+        for catelog_cls in catelog_clses:
+            for vendor_cls in vendor_clses:
+                if catelog_cls.name in vendor_cls.has:
+                    catalog_holder[catelog_cls.name].append(vendor_cls.name)
+        print("Available catalog datasets:")
+        print(json.dumps(catalog_holder, sort_keys=True, indent=4))
+
+        derived_clses = list(get_subclasses(DerivedBase))
+        derived_holder = defaultdict(list)
+        for derived_cls in derived_clses:
+            for vendor_cls in vendor_clses:
+                if derived_cls.vendor in vendor_cls.name:
+                    derived_holder[derived_cls.name].append(vendor_cls.name)
+        print("Available derived datasets:")
+        print(json.dumps(derived_holder, sort_keys=True, indent=4))
 
 
 if __name__ == "__main__":
     fire.Fire(Main())
```

## dbmaster/command.py

```diff
@@ -1,16 +1,19 @@
 import threading
-from typing import Optional, Sequence
+from typing import Sequence
 from concurrent.futures import ThreadPoolExecutor
 import logging
 
+import pandas as pd
+
 from dbmaster import config
 from dbmaster.catalog import CatalogFactory
-from dbmaster.vendor import VendorFactory
+from dbmaster.derived import DerivedFactory
 from dbmaster.util import validate, DateTimeType, to_list
+from dbmaster.vendor.base import VendorFactory
 
 
 logger = logging.getLogger(__name__)
 
 
 class Update:
     """Update data catalog from vendor.
@@ -18,36 +21,95 @@
     Available Data Catalog:
         - kline: candlestick data (i.e. OHLCV)
     """
 
     @validate
     def kline(
         self,
-        symbol: Optional[str | Sequence[str]],
         vendor: str,
+        *,
+        symbol: str | Sequence[str] | None,
         freq: str,
-        datefrom: Optional[DateTimeType] = None,
-        dateto: Optional[DateTimeType] = None,
+        datefrom: DateTimeType | None = None,
+        dateto: DateTimeType | None = None,
         **kwargs,
     ):
         """Update kline from vendor."""
-        logger.info(f"Updating kline for {symbol=}, from {vendor=}, with: {freq=}, {datefrom=}, {dateto=}, {kwargs=}")
+        logger.info(f"Updating Kline for {symbol=}, from {vendor=}, with: {freq=}, {datefrom=}, {dateto=}, {kwargs=}")
         catalog_cls = CatalogFactory.get("kline", vendor)
         vendor_cls = VendorFactory.get(vendor)
-        vendor_hanlder = VendorFactory.get_handler(vendor, "kline")
         symbol = to_list(symbol or vendor_cls.universe)
 
         lock = threading.Lock()
 
         def task(symbol, freq=freq, datefrom=datefrom, dateto=dateto, kwargs=kwargs):
-            data = vendor_hanlder(symbol=symbol, freq=freq, datefrom=datefrom, dateto=dateto, **kwargs)
+            data = vendor_cls.get_kline(symbol=symbol, freq=freq, datefrom=datefrom, dateto=dateto, **kwargs)
             with lock:
-                return catalog_cls.set(symbol=symbol, freq=freq, df=data, **kwargs)
+                return catalog_cls.set(data, symbol=symbol, freq=freq, **kwargs)
 
         with ThreadPoolExecutor(max_workers=config.MAX_WORKERS) as executor:
             futures = []
             for sym in symbol:
                 future = executor.submit(task, symbol=sym)
                 futures.append(future)
 
             res = [future.result() for future in futures]
         print(f"Done. Returned: {res}")
+
+
+class Compute:
+    """Compute derived data from catalog.
+
+    Available Derived data:
+        - pmom: price momentum, price percentage change for BTCUSDT and the rest relative to BTC.
+    """
+
+    @validate
+    def pmom(
+        self,
+        vendor: str,
+        *,
+        symbol: Sequence[str] | None,
+        period: Sequence[str],
+        step: str,
+        datefrom: DateTimeType | None = None,
+        dateto: DateTimeType | None = None,
+        **kwargs,
+    ):
+        """Compute price momentum from catalog."""
+        logger.info(
+            f"Computing Price Momentum for {symbol=}, from {vendor=}, with: {period=}, {step=}, {datefrom=}, {dateto=}, {kwargs=}"
+        )
+        catalog_cls = CatalogFactory.get("kline", vendor)
+        derived_cls = DerivedFactory.get("pmom", vendor)
+        symbol = symbol or VendorFactory.get(vendor).universe
+
+        period = to_list(period)
+        period_td = [pd.Timedelta(prd) for prd in period]
+        period_min, period_max = min(period_td), max(period_td)
+        fetch_datefrom = datefrom + period_min
+        step_td = pd.Timedelta(step)
+
+        df = catalog_cls.get(symbol=symbol, freq=step, datefrom=fetch_datefrom, dateto=dateto)
+        df["Symbol"] = df["Symbol"].str.replace("USDT", "/USDT")
+        asof_start = df["OpenTime"].min() - pd.Timedelta(period_min)
+        asof_end = df["OpenTime"].max() - pd.Timedelta(period_max)
+        assert asof_start <= asof_end, f"{asof_start=} > {asof_end=}"
+        asofs = pd.date_range(asof_start, asof_end, freq=step_td)
+
+        lock = threading.Lock()
+
+        def task(asof, df=df):
+            logger.debug(f"Computing pmom {asof=} for {symbol=}, across {period=}")
+            window = df.loc[(df["OpenTime"] >= asof + period_min) & (df["OpenTime"] <= asof + period_max)]
+            df = derived_cls.compute(window, period=period, asof=asof)
+            with lock:
+                return derived_cls.set(df, **kwargs)
+
+        with ThreadPoolExecutor(max_workers=config.MAX_WORKERS) as executor:
+            futures = []
+            for asof in asofs:
+                future = executor.submit(task, asof=asof)
+                futures.append(future)
+
+            res = [future.result() for future in futures]
+        print(f"Done. Returned: {res}")
```

## dbmaster/config.py

```diff
@@ -1,56 +1,57 @@
 import os
-from typing import Optional, Sequence, Tuple, Type
+from typing import Sequence, Tuple, Type
 from pathlib import Path
 
 from pydantic import BaseModel, AfterValidator
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource, SettingsConfigDict, TomlConfigSettingsSource
 
 
 def _check_path(path: str) -> str:
     parent = str(Path(path).parent)
     assert os.path.exists(parent), f"{parent} not exist"
     return path
 
 
-class CatalogTypeConfig(BaseModel):
-    path: str
-
-
-class KlineCatalogTypeConfig(CatalogTypeConfig):
+class DatasetConfig(BaseModel):
     path: str = AfterValidator(_check_path)
 
 
 class CatalogConfig(BaseModel):
-    kline: KlineCatalogTypeConfig
+    kline: DatasetConfig
+
+
+class DerivedConfig(BaseModel):
+    pmom: DatasetConfig
 
 
 class BinanceConfig(BaseModel):
     api_key: str
     api_secret: str
-    http_proxy: Optional[str] = None
-    https_proxy: Optional[str] = None
+    http_proxy: str | None = None
+    https_proxy: str | None = None
 
 
 class VendorConfig(BaseModel):
-    binance: Optional[BinanceConfig]
+    binance: BinanceConfig | None
 
 
 class LoggingConfig(BaseModel):
     version: int = 1
     disable_existing_loggers: bool = False
 
     formatters: dict[str, dict[str, str]]
     handlers: dict[str, dict[str, str]]
     loggers: dict[str, dict[str, str | Sequence[str] | bool]]
     root: dict[str, str | Sequence[str]]
 
 
 class Config(BaseSettings):
     catalog: CatalogConfig
+    derived: DerivedConfig
     vendor: VendorConfig
     logging: LoggingConfig
 
     MAX_WORKERS: int = max(int(os.environ.get("DBMASTER_MAX_WORKERS", os.cpu_count())), 1)
 
     model_config = SettingsConfigDict(
         toml_file=Path(os.environ.get("DBMASTER_CONFIG_PATH", Path(__file__).parent / "config.toml")),
```

## dbmaster/util.py

```diff
@@ -1,12 +1,16 @@
 import datetime as dt
 from enum import Enum
-from typing import Any, Optional
+import functools
+from typing import Any, Sequence
 from typing_extensions import Annotated
+import re
+import abc
 
+import sqlalchemy as sa
 from pydantic import AfterValidator, validate_call
 
 import pandas as pd
 
 
 BINANCE_KLINE_FREQ = {"1m", "3m", "5m", "15m", "30m", "1h", "2h", "4h", "6h", "8h", "12h", "1d", "3d", "1w", "1M"}
 
@@ -15,40 +19,144 @@
 
 def to_list(x: Any):
     if x is None:
         return []
     return list(x) if isinstance(x, (list, set, tuple)) else [x]
 
 
-def check_binance_freq(freq: str):
+def to_camel_str(snake_str: str):
+    return "".join(x.capitalize() for x in snake_str.lower().split("_"))
+
+
+def to_snake_str(camel_str: str):
+    return re.sub(r"(?<!^)(?=[A-Z])", "_", camel_str).lower()
+
+
+def get_subclasses(cls: type):
+    for subclass in cls.__subclasses__():
+        yield from get_subclasses(subclass)
+        yield subclass
+
+
+def _check_binance_freq(freq: str):
     assert freq in BINANCE_KLINE_FREQ
     return freq
 
 
-def check_binance_symbol(symbol: str):
+def _check_binance_symbol(symbol: str):
     symbol = symbol.replace("/", "").replace("-", "")
     return symbol.upper()
 
 
+def _check_binance_currency(currency: str):
+    if currency.endswith("USDT") and "/" not in currency:
+        currency = currency.replace("USDT", "/USDT")
+    elif currency.endswith("BTC") and "/" not in currency:
+        currency = currency.replace("BTC", "/BTC")
+    assert "/" in currency and len(currency.split("/")) == 2, f"Invalid {currency=}"
+    return currency
+
+
+class VendorPurposeType(Enum):
+    RAW = "raw"
+    Catalog = "catalog"
+    Derived = "derived"
+
+
 class IfRowExistsType(Enum):
     RAISE = "raise"
     IGNORE = "ignore"
     INSERT = "insert"
     DROP = "drop"
 
 
-def check_datetime(datetime: Optional[str | dt.date | dt.datetime | pd.Timestamp]):
+def _check_datetime(datetime: str | dt.date | dt.datetime | pd.Timestamp | None):
     if datetime is None:
         datetime = pd.to_datetime("now")
     return pd.to_datetime(datetime).round("s")
 
 
-def check_date(date: Optional[str | dt.date | dt.datetime | pd.Timestamp]):
+def _check_date(date: str | dt.date | dt.datetime | pd.Timestamp | None):
     if date is None:
         date = pd.to_datetime("now")
     return pd.to_datetime(date).normalize()
 
 
-BinanceSymbolType = Annotated[str, AfterValidator(check_binance_symbol)]
-BinanceFreqType = Annotated[str, AfterValidator(check_binance_freq)]
-DateTimeType = Annotated[Optional[str | dt.date | dt.datetime | pd.Timestamp], AfterValidator(check_datetime)]
-DateType = Annotated[Optional[str | dt.date | dt.datetime | pd.Timestamp], AfterValidator(check_date)]
+def _check_period(period: str):
+    if not period.startswith("-") and not period.startswith("+"):
+        period = f"+{period}"
+    assert period.startswith("+") or period.startswith("-"), "period must start with + or -"
+    return period
+
+
+BinanceSymbolType = Annotated[str, AfterValidator(_check_binance_symbol)]
+BinanceCurrencyType = Annotated[str, AfterValidator(_check_binance_currency)]
+BinanceFreqType = Annotated[str, AfterValidator(_check_binance_freq)]
+DateTimeType = Annotated[str | dt.date | dt.datetime | pd.Timestamp | None, AfterValidator(_check_datetime)]
+DateType = Annotated[str | dt.date | dt.datetime | pd.Timestamp | None, AfterValidator(_check_date)]
+PeriodType = Annotated[str, AfterValidator(_check_period)]
+
+
+class DatasetBase(abc.ABC):
+    name: str = NotImplemented  # dataset name. e.g. kline
+    vendor: str = NotImplemented  # vendor that implemented the dataset. e.g. binance
+    table: sa.Table | Sequence[sa.Table] = NotImplemented  # table(s) in the dataset
+
+    names = set()
+
+    def __init_subclass__(cls, **kwargs) -> None:
+        super().__init_subclass__(**kwargs)
+
+        bypass = {"CatalogBase", "DerivedBase"}
+        if cls.__name__ in bypass:
+            return
+
+        catalog, vendor = to_snake_str(cls.__name__).split("_", maxsplit=1)
+
+        if cls.name is NotImplemented:
+            cls.name = catalog
+        if cls.vendor is NotImplemented:
+            cls.vendor = vendor
+        if cls.table is NotImplemented:
+            raise NotImplementedError("table is not implemented")
+
+        assert cls.name not in cls.names, f"{cls.name} already exists"
+        cls.names.add(cls.name)
+
+        cls.__initialize__()
+
+        for table in to_list(cls.table):
+            table.metadata = cls.metadata
+        cls.metadata.create_all(cls.engine, checkfirst=True)
+
+    @classmethod
+    @abc.abstractmethod
+    def __initialize__(cls, engine: sa.engine.Engine) -> None:
+        pass
+
+    @classmethod
+    @abc.abstractmethod
+    def get(cls, **kwargs) -> pd.DataFrame:
+        pass
+
+    @classmethod
+    @abc.abstractmethod
+    def set(cls, df: pd.DataFrame, **kwargs) -> Any:
+        pass
+
+    @classmethod
+    @functools.cache
+    def get_table(cls, name: str) -> sa.Table:
+        cls.metadata.reflect(cls.engine)
+        return cls.metadata.tables[name]
+
+
+class DatasetFactory:
+    @classmethod
+    def get(cls, name: str, vendor: str) -> DatasetBase:
+        from dbmaster.vendor import VendorFactory
+
+        vendor_name = VendorFactory.get(vendor).name
+        for sub_cls in get_subclasses(DatasetBase):
+            if sub_cls.name == name and sub_cls.vendor == vendor_name:
+                return sub_cls
+        raise ValueError(f"Dataset={name} not implemented for {vendor_name}")
```

## dbmaster/catalog/base.py

```diff
@@ -1,56 +1,9 @@
-import abc
-import functools
-from typing import Sequence
+from dbmaster.util import DatasetBase, DatasetFactory
 
-import pandas as pd
-import sqlalchemy as sa
 
-from dbmaster.util import to_list
+class CatalogBase(DatasetBase):
+    pass
 
 
-class CatalogBase(abc.ABC):
-    table: sa.Table | Sequence[sa.Table] = NotImplemented
-
-    def __init_subclass__(cls, **kwargs) -> None:
-        super().__init_subclass__(**kwargs)
-
-        cls.metadata = sa.MetaData()
-        if cls.table is NotImplemented:
-            raise NotImplementedError("table is not implemented")
-
-        cls.__initialize__()
-
-        for table in to_list(cls.table):
-            table.metadata = cls.metadata
-        cls.metadata.create_all(cls.engine, checkfirst=True)
-
-    @classmethod
-    @abc.abstractmethod
-    def __initialize__(cls, engine: sa.engine.Engine) -> None:
-        pass
-
-    @classmethod
-    @abc.abstractmethod
-    def get(cls, **kwargs) -> pd.DataFrame:
-        pass
-
-    @classmethod
-    @abc.abstractmethod
-    def set(cls, df: pd.DataFrame) -> bool:
-        pass
-
-    @classmethod
-    @functools.cache
-    def get_table(cls, name: str) -> sa.Table:
-        cls.metadata.reflect(cls.engine)
-        return cls.metadata.tables[name]
-
-
-class CatalogFactory:
-    @classmethod
-    def get(cls, name: str, vendor: str) -> CatalogBase:
-        import dbmaster.catalog as catalog
-
-        catalog_cls_name = f"{name.capitalize()}{vendor.capitalize()}"
-        catalog_cls = getattr(catalog, catalog_cls_name)
-        return catalog_cls
+class CatalogFactory(DatasetFactory):
+    pass
```

## dbmaster/catalog/kline.py

```diff
@@ -1,27 +1,31 @@
+"""
+Kline catalog implementation
+"""
+
 import logging
 import time
 from typing import Sequence
 
 import pandas as pd
 from retry import retry
 import sqlalchemy as sa
 from sqlalchemy import Column, DateTime, Float, String
 
 from dbmaster import config
+from dbmaster.catalog.base import CatalogBase
 from dbmaster.util import (
     validate,
     to_list,
     DateTimeType,
     BinanceSymbolType,
     BinanceFreqType,
     BINANCE_KLINE_FREQ,
     IfRowExistsType,
 )
-from dbmaster.catalog.base import CatalogBase
 
 logger = logging.getLogger(__name__)
 
 engine = sa.create_engine(f"sqlite:///{config.catalog.kline.path}")
 metadata = sa.MetaData()
 
 
@@ -40,26 +44,27 @@
             Column("BaseVolume", Float),
             Column("QuoteVolume", Float),
         )
         for freq in BINANCE_KLINE_FREQ
     ]
 
     @classmethod
-    def __initialize__(cls, engine=engine) -> None:
+    def __initialize__(cls, engine=engine, metadata=metadata) -> None:
         cls.engine = engine
+        cls.metadata = metadata
 
     @classmethod
     @validate
     def get(
         cls,
         symbol: BinanceSymbolType | Sequence[BinanceSymbolType],
         freq: BinanceFreqType,
         datefrom: DateTimeType | None = None,
         dateto: DateTimeType | None = None,
-        column: str | list[str] = None,
+        column: str | list[str] | None = None,
     ) -> pd.DataFrame:
         table = cls.get_table(f"kline_binance_{freq}")
 
         column = to_list(column) or [col.name for col in table.columns]
         sql = sa.select(*[table.c[col] for col in column])
         sql = sql.where(table.c.Symbol.in_(to_list(symbol))) if symbol else sql
         sql = sql.where(table.c.OpenTime >= datefrom.to_pydatetime()) if datefrom else sql
@@ -68,22 +73,24 @@
         return df
 
     @classmethod
     @validate
     @retry(sa.exc.OperationalError, tries=3, logger=logger)
     def set(
         cls,
+        df: pd.DataFrame,
         symbol: BinanceSymbolType,
         freq: BinanceFreqType,
-        df: pd.DataFrame,
         if_row_exists: IfRowExistsType = IfRowExistsType.INSERT,
         **kwargs,
     ) -> None:
-        logger.debug(f"KlineBinance.set({symbol=}, {freq=}, {df.shape=}, {if_row_exists=})")
+        logger.debug(f"{cls.__name__}.set({symbol=}, {freq=}, {df.shape=}, {if_row_exists=})")
         table_name = f"kline_binance_{freq}"
+        if df.empty:
+            return
         try:
             res = df.to_sql(table_name, con=engine, if_exists="append", index=False)
         except sa.exc.IntegrityError as e:
             logger.debug(f"{type(e)}({e})"[:80] + "...")
             if if_row_exists is IfRowExistsType.RAISE:
                 raise
             elif if_row_exists is IfRowExistsType.IGNORE:
@@ -104,15 +111,37 @@
                 table = cls.get_table(table_name)
                 sql = table.delete().where(table.c["Symbol"] == symbol).where(table.c["OpenTime"].in_(df["OpenTime"]))
                 with cls.engine.connect() as conn:
                     res_del = conn.execute(sql)
                     conn.commit()
                 res_inc = df.to_sql(table_name, con=engine, if_exists="append", index=False)
                 logger.info(f"Dropped {res_del.rowcount} rows from {table_name}, before inserting {res_inc} rows.")
+            else:
+                raise ValueError(f"Invalid {if_row_exists=}.")
         except sa.exc.OperationalError as e:
             time.sleep(5)
             raise Exception(str(e)[:80] + " ...") from e
         else:
             logger.info(f"Inserted {res} rows to {table_name}.")
 
 
-__all__ = ["KlineBinance"]
+class Kline:
+    @classmethod
+    @validate
+    def get(
+        cls,
+        vendor: str,
+        *,
+        symbol: str | Sequence[str],
+        freq: str,
+        datefrom: DateTimeType | None = None,
+        dateto: DateTimeType | None = None,
+        column: str | list[str] | None = None,
+    ) -> pd.DataFrame:
+        if vendor == "binance":
+            df = KlineBinance.get(symbol=symbol, freq=freq, datefrom=datefrom, dateto=dateto, column=column)
+        else:
+            raise NotImplementedError(f"{vendor} is not implemented")
+        return df
+
+
+__all__ = ["Kline", "KlineBinance"]
```

## dbmaster/vendor/base.py

```diff
@@ -1,31 +1,48 @@
+import abc
 from typing import Callable
 
+import pandas as pd
+
+from dbmaster.util import get_subclasses, to_snake_str
+
 
 class VendorBase:
-    pass
+    name: str = NotImplemented
+
+    def __init_subclass__(cls, **kwargs) -> None:
+        super().__init_subclass__(**kwargs)
+
+        cls.has = set()
+        if "name" not in cls.__dict__:
+            cls.name = to_snake_str(cls.__name__)
+
+    @classmethod
+    def get_catalog(cls, catalog: str) -> Callable:
+        func_name = f"get_{catalog}"
+        return getattr(cls.get(catalog), func_name)
 
 
-class KlineVendorBase(VendorBase):
+class KlineVendorBase(VendorBase, abc.ABC):
     def __init_subclass__(cls, **kwargs) -> None:
         super().__init_subclass__(**kwargs)
 
+        cls.has.add("kline")
+
         if "universe" not in cls.__dict__:  # abstract class property
             raise NotImplementedError("universe is not implemented")
 
-
-class VendorFactory:
     @classmethod
-    def get(cls, name: str) -> VendorBase:
-        import dbmaster.vendor as vendor
+    @abc.abstractmethod
+    def get_kline(cls, *args, **kwargs) -> pd.DataFrame:
+        pass
 
-        vendor_name = name.capitalize()
-        vendor_cls = getattr(vendor, vendor_name)
-        return vendor_cls
 
+class VendorFactory:
     @classmethod
-    def get_handler(cls, name: str, catalog: str) -> Callable:
-        func_name = f"get_{catalog}"
-        return getattr(cls.get(name), func_name)
+    def get(cls, name: str) -> Callable:
+        for sub_cls in get_subclasses(VendorBase):
+            if sub_cls.name == name:
+                return sub_cls
 
 
-__all__ = ["VendorFactory"]
+__all__ = ["VendorBase", "KlineVendorBase", "VendorFactory"]
```

## dbmaster/vendor/binance.py

```diff
@@ -1,10 +1,10 @@
 import functools
 from collections import defaultdict
-from typing import Optional
+from typing import Sequence
 import logging
 
 import pandas as pd
 import requests
 from retry import retry
 
 from dbmaster import config
@@ -34,15 +34,15 @@
             param.update({"https": https_proxy})
 
         return Client(config.vendor.binance.api_key, config.vendor.binance.api_secret, {"proxies": param})
 
     @classmethod
     @property
     @functools.cache
-    def universe(cls) -> tuple[BinanceSymbolType, ...]:
+    def universe(cls) -> Sequence[BinanceSymbolType]:
         all_usdt_symbols = [
             symbol["symbol"]
             for symbol in cls.client.get_exchange_info()["symbols"]
             if symbol["symbol"].endswith("USDT")
         ]
         return all_usdt_symbols
 
@@ -51,26 +51,26 @@
     @retry(
         (requests.exceptions.ReadTimeout, requests.exceptions.ProxyError, requests.exceptions.ConnectionError), tries=3
     )
     def get_kline(
         cls,
         symbol: BinanceSymbolType,
         freq: BinanceFreqType,
-        datefrom: Optional[DateTimeType] = None,
-        dateto: Optional[DateTimeType] = None,
+        datefrom: DateTimeType | None = None,
+        dateto: DateTimeType | None = None,
         closed_only: bool = True,
         klines_type: str | HistoricalKlinesType = HistoricalKlinesType.SPOT,
         **kwargs,
     ):
         """Get Kline data from Binance API.
         Args:
             symbol (str): Symbol name e.g. BTC/USDT.
             freq (str): Kline interval e.g. 1m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M.
-            datefrom (Optional[DateTimeType]): Date from. Defaults to None.
-            dateto (Optional[DateTimeType]): Date to. Defaults to None.
+            datefrom (DateTimeType | None): Date from. Defaults to None.
+            dateto (DateTimeType | None): Date to. Defaults to None.
             closed_only (bool): If True, only closed klines will be returned.
             klines_type (str | HistoricalKlinesType): Defaults to HistoricalKlinesType.SPOT
                 SPOT = 1; FUTURES = 2; FUTURES_COIN = 3
             **kwargs: igored
         Returns:
             pd.DataFrame: DataFrame of Kline data.
         """
```

## Comparing `dbmaster-0.1.1.dist-info/LICENSE` & `dbmaster-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dbmaster-0.1.1.dist-info/METADATA` & `dbmaster-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbmaster
-Version: 0.1.1
+Version: 0.2.0
 Summary: Personal Quant Research Database Manager
 Author-email: You Xie <xyshell@bu.edu>
 Maintainer-email: You Xie <xyshell@bu.edu>
 License: Copyright (c) 2024 You Xie
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

