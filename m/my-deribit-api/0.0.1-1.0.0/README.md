# Comparing `tmp/my_deribit_api-0.0.1.tar.gz` & `tmp/my_deribit_api-1.0.0.tar.gz`

## Comparing `my_deribit_api-0.0.1.tar` & `my_deribit_api-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/requirements.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/src/my_deribit_api/__about__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/src/my_deribit_api/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/src/my_deribit_api/constant.py
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/src/my_deribit_api/deribit_api.py
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/src/my_deribit_api/deribit_websocket.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/README.md
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 my_deribit_api-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/requirements.txt
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/src/my_deribit_api/__about__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/src/my_deribit_api/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/src/my_deribit_api/constant.py
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/src/my_deribit_api/deribit_api.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/src/my_deribit_api/deribit_websocket.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/tests/test_http_client.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/tests/test_websocket_client.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/README.md
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 my_deribit_api-1.0.0/PKG-INFO
```

### Comparing `my_deribit_api-0.0.1/src/my_deribit_api/deribit_api.py` & `my_deribit_api-1.0.0/src/my_deribit_api/deribit_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import requests
 import multitasking
 from time import sleep
 
 from binance.error import ClientError, ServerError
 
-from .constant import GrantType, RetCode
+from .constant import GrantType, RetCode, OrderType, TimeInForce
 
 class DeribitAPI(API):
     """API base class
 
     Keyword Args:
         base_url (str, optional): the API base url, useful to switch to testnet, etc. By default it's https://api.binance.com
         timeout (int, optional): the time waiting for server response, number of seconds. https://docs.python-requests.org/en/master/user/advanced/#timeouts
@@ -22,28 +22,30 @@
         private_key (str, optional): RSA private key for RSA authentication
         private_key_pass(str, optional): Password for PSA private key
     """
     
     running: bool = True
     refresh_token: str = ''
     expires_in: int = 0
+    
 
     def __init__(
         self,
         api_key=None,
         api_secret=None,
         base_url='https://test.deribit.com/api/v2',
         timeout=None,
         proxies=None,
         show_limit_usage=False,
         show_header=False,
         private_key=None,
         private_key_pass=None,
         client_id=None,
-        client_secret=None
+        client_secret=None,
+        auto_refresh=True
     ):
         self.api_key = api_key
         self.api_secret = api_secret
         self.base_url = base_url
         self.timeout = timeout
         self.proxies = None
         self.show_limit_usage = False
@@ -65,15 +67,15 @@
         if show_header is True:
             self.show_header = True
 
         if type(proxies) is dict:
             self.proxies = proxies
 
         self._logger = logging.getLogger(__name__)
-        self.auth()
+        self.auth(auto_refresh=auto_refresh)
     
     def _handle_exception(self, response):
         status_code = response.status_code
         if status_code < 400:
             return
         if 400 <= status_code < 500:
             try:
@@ -130,31 +132,58 @@
         
         return RetCode.OK, reuslt 
     
     def get_instrument(self, instrument_name):
         url_path = '/public/get_instrument'
         return self.request_path('GET', url_path, {'instrument_name': instrument_name})
 
-    def get_open_orders(self, instrument_name):
+    def get_open_orders_by_instrument(self, instrument_name):
         url_path = '/private/get_open_orders_by_instrument'
         return self.request_path('GET', url_path, {'instrument_name': instrument_name})
     
+    def get_open_orders_by_currency(self, currency):
+        url_path = '/private/get_open_orders_by_currency'
+        return self.request_path('GET', url_path, {'currency': currency})
+    
     def get_position(self, instrument_name):
         url_path = '/private/get_position'
         return self.request_path('GET', url_path, {'instrument_name': instrument_name})
     
+    def get_positions(self, currency='BTC', kind='option'):
+        url_path = '/private/get_positions'
+        return self.request_path('GET', url_path, {'currency': currency, 'kind': kind})
+    
+    def get_account(self, currency='BTC', extended=False):
+        url_path = '/private/get_account_summary'
+        return self.request_path('GET', url_path, {'currency': currency, 'extended': 'true' if extended else 'false'})
+    
+    def get_order_book(self, instrument_name, depth=5):
+        url_path = '/public/get_order_book'
+        return self.request_path('GET', url_path, {'instrument_name': instrument_name, 'depth': depth})
+    
+    def buy(self, instrument_name, price, amount, type=OrderType.LIMIT, time_in_force=TimeInForce.GTC, label=''):
+        url_path = '/private/buy'
+        return self.request_path('GET', url_path, {
+            'instrument_name': instrument_name,
+            'price':price, 'amount': amount,
+            'type': type.value,
+            'time_in_force': time_in_force.value,
+            'label': label
+        })
+    
+    def sell(self, instrument_name, price, amount, type=OrderType.LIMIT, time_in_force=TimeInForce.GTC, label=''):
+        url_path = '/private/sell'
+        return self.request_path('GET', url_path, {
+            'instrument_name': instrument_name,
+            'price':price, 'amount': amount,
+            'type': type.value,
+            'time_in_force': time_in_force.value,
+            'label': label
+        })
+    
+    def cancel(self, order_id):
+        url_path = '/private/cancel'
+        return self.request_path('GET', url_path, {
+            'order_id': order_id,
+        })
     
-
-if __name__ == '__main__':
-    import json
-    with open('config.json') as fs:
-        config = json.load(fs)
-    api = DeribitAPI(base_url='https://test.deribit.com/api/v2', client_id=config['client_id'], client_secret=config['client_secret'])
-    instrument_name = "BTC-26APR24-66000-C"
-    # ret_code, data = api.get_open_orders(instrument_name)
-    # print(ret_code, data)
-    ret_code, data = api.get_instrument(instrument_name)
-    print(ret_code, data)
-    # ret_code, data = api.get_position(instrument_name)
-    # print(ret_code, data)
-
```

### Comparing `my_deribit_api-0.0.1/src/my_deribit_api/deribit_websocket.py` & `my_deribit_api-1.0.0/src/my_deribit_api/deribit_websocket.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ABNF,
     create_connection,
     WebSocketException,
     WebSocketConnectionClosedException,
     WebSocketTimeoutException,
 )
 
-from .constant import SubType, TimeInForce
+from .constant import SubscribeType, TimeInForce
 
 class DeribitSocketManager(BinanceSocketManager):
     running: bool = True
 
     def _handle_heartbeat(self, op_code, frame):
         data = json.loads(frame.data)
         if data.get('method') == 'heartbeat' and data['params']['type'] == 'test_request':
@@ -161,23 +161,29 @@
             "method" : "private/get_open_orders_by_instrument",
             "params" : {
                 "instrument_name" : instrument_name
             }
         }
         self.send(msg)
 
-    def subscribe(self, instrument_name, interval='raw', sub_types = [SubType.BOOK, SubType.TICKER, SubType.USER_TRADES]):
+    def subscribe(self, instrument_name, interval='raw', types = [SubscribeType.TICK, SubscribeType.BOOK, SubscribeType.USER_ORDER , SubscribeType.USER_TRADE]):
         channels = []
-        for sub_type in sub_types:
-            if sub_type == SubType.TICKER:
+        for type in types:
+            if type == SubscribeType.TICK:
                 channels.append(f'ticker.{instrument_name}.{interval}')
-            elif sub_type == SubType.BOOK:
+            elif type == SubscribeType.BOOK:
                 channels.append(f'book.{instrument_name}.{interval}')
-            elif sub_type == SubType.USER_TRADES:
+            elif type == SubscribeType.TRADE:
+                channels.append(f'trades.{instrument_name}.{interval}')
+            elif type == SubscribeType.USER_ORDER:
+                channels.append(f'user.orders.any.any.{interval}')
+            elif type == SubscribeType.USER_TRADE:
                 channels.append(f'user.trades.any.any.{interval}')
+            elif type == SubscribeType.USER_CHANGE:
+                channels.append(f'user.changes.any.any.{interval}')
 
         msg = {
             "method" : "public/subscribe",
             "params": {
                 "channels": channels
             },
             "jsonrpc" : "2.0"
@@ -208,33 +214,11 @@
                 "type": "limit",
                 "time_in_force": time_in_force.value,
                 "label": label
             }
         }
         self.send(msg)
 
-if __name__ == '__main__':
-    import json
-    with open('config.json') as fs:
-        config = json.load(fs)
-
-    def on_message(x, y):
-        print(f'on_message:{y}')
-
-    def on_ping(x):
-        print(f'on_message:{x}')
-
-    def on_pong(x):
-        print(f'on_message:{x}')
-    
-    ws = DeribitWebsocketStreamClient(client_id=config['client_id'], client_secret=config['client_secret'], on_message=on_message, on_ping=on_ping, on_pong=on_pong)
-    # ws.auth('l3gSQPH-', 'v1c4QjbNxwhiTTHooXCjg61bhO_KB_69FJWTdBdwUSo')
-    # ws.subscribe("BTC-26APR24-66000-C")
-    # ws.get_instrument('BTC-26APR24-66000-C')
-    instrument_name = "BTC-26APR24-66000-C"
-    # ws.subscribe(instrument_name, sub_types=[SubType.USER_TRADES])
-    # ws.order(instrument_name, 0.033, 39, label='test_order', time_in_force=TimeInForce.IOC)
-    ws.get_open_orders(instrument_name)
```

### Comparing `my_deribit_api-0.0.1/LICENSE.txt` & `my_deribit_api-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `my_deribit_api-0.0.1/README.md` & `my_deribit_api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `my_deribit_api-0.0.1/pyproject.toml` & `my_deribit_api-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,21 @@
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
+[tool.pytest.ini_options]
+addopts = [
+  "--strict-config",
+  "--strict-markers",
+  "--ignore=docs_src",
+]
+
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.types]
 dependencies = [
   "mypy>=1.0.0",
 ]
```

### Comparing `my_deribit_api-0.0.1/PKG-INFO` & `my_deribit_api-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: my-deribit-api
-Version: 0.0.1
+Version: 1.0.0
 Project-URL: Documentation, https://github.com/unknown/my-deribit-api#readme
 Project-URL: Issues, https://github.com/unknown/my-deribit-api/issues
 Project-URL: Source, https://github.com/unknown/my-deribit-api
 Author-email: liuyanzhi08 <702368372@qq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

