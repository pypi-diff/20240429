# Comparing `tmp/selenium_form_killer-0.1.6.tar.gz` & `tmp/selenium_form_killer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_form_killer-0.1.6.tar", max compression
+gzip compressed data, was "selenium_form_killer-0.1.7.tar", max compression
```

## Comparing `selenium_form_killer-0.1.6.tar` & `selenium_form_killer-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1351 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/README.md
--rw-r--r--   0        0        0      709 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       65 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/__init__.py
--rw-r--r--   0        0        0       37 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/anti_captcha/__init__.py
--rw-r--r--   0        0        0     3402 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/anti_captcha/anti_captcha.py
--rw-r--r--   0        0        0       43 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/capmonster/__init__.py
--rw-r--r--   0        0        0      647 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/capmonster/captcha_breaker.py
--rw-r--r--   0        0        0      330 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/forms.py
--rw-r--r--   0        0        0    13991 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/killer.py
--rw-r--r--   0        0        0      748 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/log/logger.py
--rw-r--r--   0        0        0        0 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/util/__init__.py
--rw-r--r--   0        0        0      221 2024-03-27 15:20:29.132867 selenium_form_killer-0.1.6/selenium_form_killer/util/util.py
--rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 selenium_form_killer-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1351 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.7/README.md
+-rw-r--r--   0        0        0      709 2024-04-29 17:34:22.945601 selenium_form_killer-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.7/selenium_form_killer/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.7/selenium_form_killer/anti_captcha/__init__.py
+-rw-r--r--   0        0        0     3402 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.7/selenium_form_killer/anti_captcha/anti_captcha.py
+-rw-r--r--   0        0        0       43 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.7/selenium_form_killer/capmonster/__init__.py
+-rw-r--r--   0        0        0      648 2024-04-29 17:29:32.209655 selenium_form_killer-0.1.7/selenium_form_killer/capmonster/captcha_breaker.py
+-rw-r--r--   0        0        0      330 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.7/selenium_form_killer/forms.py
+-rw-r--r--   0        0        0    14877 2024-04-29 17:24:44.510072 selenium_form_killer-0.1.7/selenium_form_killer/killer.py
+-rw-r--r--   0        0        0      748 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.7/selenium_form_killer/log/logger.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:48:53.342634 selenium_form_killer-0.1.7/selenium_form_killer/util/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-29 14:48:53.342634 selenium_form_killer-0.1.7/selenium_form_killer/util/util.py
+-rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 selenium_form_killer-0.1.7/PKG-INFO
```

### Comparing `selenium_form_killer-0.1.6/README.md` & `selenium_form_killer-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `selenium_form_killer-0.1.6/pyproject.toml` & `selenium_form_killer-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selenium-form-killer"
-version = "0.1.6"
+version = "0.1.7"
 license = "MIT"
 description = ""
 authors = ["Rodrigoneal <rodrigho2006@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `selenium_form_killer-0.1.6/selenium_form_killer/anti_captcha/anti_captcha.py` & `selenium_form_killer-0.1.7/selenium_form_killer/anti_captcha/anti_captcha.py`

 * *Files identical despite different names*

### Comparing `selenium_form_killer-0.1.6/selenium_form_killer/capmonster/captcha_breaker.py` & `selenium_form_killer-0.1.7/selenium_form_killer/capmonster/captcha_breaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from capmonstercloudclient import CapMonsterClient, ClientOptions
 
 from capmonstercloudclient.requests.baseRequest import BaseRequest
 
+
 from selenium_form_killer.log.logger import get_logger
 
 logger = get_logger()
 
 
 async def captcha_token(
     request_captcha: BaseRequest, api_key: str, client_timeout: int = 30
```

### Comparing `selenium_form_killer-0.1.6/selenium_form_killer/killer.py` & `selenium_form_killer-0.1.7/selenium_form_killer/killer.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,17 @@
         self.data: Annotated[Optional[str], Doc("Dados da requisição")] = None
         self.cookies: Annotated[Optional[str], Doc("Cookies da requisição")] = None
         self._response = None
         self._forms: list[Form] = None
         self.status_code: Annotated[
             Optional[int], Doc("Status code da requisição")
         ] = None
-        self.session = httpx.AsyncClient(headers=headers)
+        self.session = httpx.AsyncClient(
+            headers=headers,
+        )
         self.logger = get_logger(verbose)
 
     def __call__(self, *args, **kwargs):
         return self.__class__(*args, **kwargs)
 
     def __soup(self, html: Optional[str] = None) -> BeautifulSoup:
         html = html or self._response.text
@@ -48,17 +50,20 @@
         return self.__soup(html_text)
 
     async def __aenter__(self):
         self.logger.info("Entering async context")
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        self.logger.info(
-            f"Exiting async context with exc_type:{exc_type}, exc_val:{exc_val}, exc_tb:{exc_tb}"
-        )
+        if not exc_type:
+            self.logger.info("Exiting async context")
+        else:
+            self.logger.critical(
+                f"Exiting async context with exc_type:{exc_type}, exc_val:{exc_val}, exc_tb:{exc_tb}"
+            )
         await self.session.aclose()
         self.logger.info("Session closed")
 
     def _forms_soup(self, html: Optional[str] = None) -> BeautifulSoup:
         html = html or self._response.text
         soup = BeautifulSoup(html, "html.parser")
         return soup.find_all("form")
@@ -206,44 +211,47 @@
             data=data,
             params=params,
             **httpx_options,
         )
         return self
 
     def extract_inputs(self, formulario: BeautifulSoup) -> list["FormInput"]:
-        self.logger.info(f"Extracting inputs from form: {formulario}")
         inputs = formulario.find_all(["input", "textarea"])
         _inputs = []
         for input_tag in inputs:
             nome = input_tag.get("name")
             valor = input_tag.get("value", "")
             if input_tag.get("type"):
                 _type = input_tag.get("type")
             else:
                 _type = "text"
-            _inputs.append(FormInput(name=nome, value=valor, type=_type))
+            form_input = FormInput(name=nome, value=valor, type=_type)
+            self.logger.info(f"Extracting inputs: {form_input}")
+            _inputs.append(form_input)
         return _inputs
 
     def extract_actions(self, formulario: BeautifulSoup) -> list[str]:
-        self.logger.info(f"Extracting actions from form:{formulario}")
         form_action = {"action": None, "id": None, "name": None, "method": None}
         form_action["action"] = formulario.get("action")
         form_action["id"] = formulario.get("id")
         form_action["name"] = formulario.get("name")
         form_action["method"] = formulario.get("method")
+        self.logger.info(f"Extracting actions from form:{form_action}")
         return form_action
 
     def extract_captcha(self, formulario: BeautifulSoup) -> str:
-        self.logger.info(f"Extracting captcha from form: {formulario}")
         captchas = formulario.find_all(
             class_=lambda value: value and "captcha" in value
         )
         for captcha in captchas:
-            if captcha.get("data-sitekey"):
-                return captcha.get("data-sitekey")
+            if data_site :=captcha.get("data-sitekey"):
+                self.logger.info(f"Extracting captcha from form: {captcha} data-sitekey: {data_site}")
+                return data_site
+            else:
+                self.logger.error(f"Extracting captcha from form: {captcha} not found data-sitekey")
 
     def extract_forms(self, html: Optional[str] = None) -> list["Form"]:
         self.logger.info("Extracting forms")
         forms = []
         for formulario in self._forms_soup(html):
             _captcha = self.extract_captcha(formulario)
             extract_actions = self.extract_actions(formulario)
@@ -256,19 +264,18 @@
                     button=None,
                     url_base=str(self.response.url),
                     **extract_actions,
                 )
             )
         return forms
 
-
     async def save_html(self, name: str) -> None:
         path = name
         if not name.endswith(".html"):
-            path = name+".html"        
+            path = name + ".html"
         await asyncio.to_thread(self._save_file, path)
 
     def _save_file(self, path: str) -> None:
         self.logger.info(f"Saving file to: {path}")
         with open(path, "wb") as f:
             f.write(self.response.content)
 
@@ -310,34 +317,47 @@
         self.id = id
         self.name = name
         self.button = button
         self.captcha = captcha
         self.url_base = url_base
         self.__killer = killer
 
+    def pretty_print(self) -> None:
+        for index, input in enumerate(self.inputs):
+            print(f"{index}: {input}")
+
     def __repr__(self) -> str:
+        if self.inputs:
+            if len(self.inputs) > 9:
+                 str_inputs = ", ".join([str(index) + ": " + str(input) for index, input in enumerate(self.inputs[:9])])
+                 str_inputs += ", ..."
+                 return str(f"<Form: {self.id=}, {str_inputs=}>")
+            else:
+                str_inputs = ", ".join([str(index) + ": " + str(input) for index, input in enumerate(self.inputs)])
+                return str(f"<Form: {self.id=}, {str_inputs=}>")
         return str(f"<Form: {self.id=}>")
 
     def add_input(self, name: str, value: str, type: str = "text") -> None:
         self.inputs.append(FormInput(name=name, value=value, type=type))
 
     def delete_input(self, name: str) -> None:
         self.inputs = [input for input in self.inputs if input.name != name]
-    
+
     def total_inputs(self) -> int:
         return len(self.inputs)
-    
+
     def get_input(self, name: str) -> "FormInput":
         for input in self.inputs:
             if input.name == name:
                 return input
 
+
     async def submit(
         self,
-        url: Optional[str] = None,        
+        url: Optional[str] = None,
         token: Optional[dict[str, str]] = {},
         method: str = None,
         input_data: str | list["FormInput"] | list[int] | None = "all",
         input_query_params: str | list["FormInput"] | list[int] | None = None,
         **kwargs,
     ) -> SeleniumKiller:
         self.__killer.logger.info(f"Submitting form: {self}")
@@ -367,15 +387,15 @@
                 self.inputs = input_data
         elif not input_data:
             self.inputs = []
         kwargs["data"] = {input.name: input.value for input in self.inputs}
 
         if token:
             kwargs["data"].update(token)
-        
+
         if not url:
             url = join_url_action(self.url_base, self.action)
         await self.__killer.send_request(method=self.method, url=url, **kwargs)
         return self.__killer
 
 
 class FormInput:
@@ -385,9 +405,8 @@
         self.value = value
 
     def __repr__(self) -> str:
         return str(f"<FormInput: name:{self.name} type:{self.type} value:{self.value}>")
 
     def to_dict(self) -> dict:
         return {self.name: self.value}
-
```

### Comparing `selenium_form_killer-0.1.6/selenium_form_killer/log/logger.py` & `selenium_form_killer-0.1.7/selenium_form_killer/log/logger.py`

 * *Files identical despite different names*

### Comparing `selenium_form_killer-0.1.6/PKG-INFO` & `selenium_form_killer-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-form-killer
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: MIT
 Author: Rodrigoneal
 Author-email: rodrigho2006@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

