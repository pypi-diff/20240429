# Comparing `tmp/yxr_atcoder_core-0.0.3.4.tar.gz` & `tmp/yxr_atcoder_core-0.0.3.5.tar.gz`

## Comparing `yxr_atcoder_core-0.0.3.4.tar` & `yxr_atcoder_core-0.0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/__init__.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/auth.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/constant.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/language.py
--rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/problem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/py.typed
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/result.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/submit.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/url.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/contest/__init__.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/contest/listpage.py
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/contest/standing.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/contest/tasks.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/interfaces/HttpUtil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/modal/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/modal/problem_test_case.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/utils/__init__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/ac_core/utils/html_parse_helper.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/LICENSE
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/README.md
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/auth.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/constant.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/language.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/problem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/py.typed
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/result.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/submit.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/url.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/contest/__init__.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/contest/listpage.py
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/contest/standing.py
+-rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/contest/tasks.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/interfaces/HttpUtil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/modal/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/modal/problem_test_case.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/utils/__init__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/ac_core/utils/html_parse_helper.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/LICENSE
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/README.md
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 yxr_atcoder_core-0.0.3.5/PKG-INFO
```

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/auth.py` & `yxr_atcoder_core-0.0.3.5/ac_core/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from logging import getLogger
 from typing import cast
 from bs4 import BeautifulSoup
 import bs4
 
-from ac_core.constant import _SITE_URL
+from ac_core.constant import SITE_URL
 from ac_core.interfaces.HttpUtil import HttpUtilInterface
 from ac_core.utils import HTML_PARSER
 
-logger = getLogger(__name__)
+logger = getLogger('yxr-atcoder-core')
 
 
 def is_logged_in(http_util: HttpUtilInterface) -> bool:
   """This method will use ``http_util`` for login check by visit atcoder site and parse html
 
     :param HttpUtilInterface http_util: a http instance, for example ``requests.session()``
 
@@ -25,15 +25,15 @@
       import requests
       h = requests.session()
       #h = Helper(requests.session())
       print(is_logged_in(h))
       print(fetch_login(h, 'username', 'password'))
       print(is_logged_in(h))
   """
-  html = http_util.get(f"{_SITE_URL}/home").text
+  html = http_util.get(f"{SITE_URL}/home").text
   soup = BeautifulSoup(html, HTML_PARSER)
   dropdown_menus = soup.find_all('ul', class_="dropdown-menu")
   found_user_link = False
   for menu in dropdown_menus:
     a_s = menu.find_all('a')
     for a in a_s:
       if a['href'].startswith('/users/'):
@@ -60,15 +60,15 @@
       h = requests.session()
       #h = Helper(requests.session())
       print(is_logged_in(h))
       print(fetch_login(h, 'username', 'password'))
       print(is_logged_in(h))
   """
   try:
-    res = http_util.get(_SITE_URL + '/login')
+    res = http_util.get(SITE_URL + '/login')
     soup = BeautifulSoup(res.text, HTML_PARSER)
     csrf_token = cast(bs4.Tag, soup.find(attrs={'name': 'csrf_token'})).get('value')
     post_data = {
         'csrf_token': csrf_token,
         'username': username,
         'password': password,
     }
@@ -80,19 +80,8 @@
       logger.error(ret.text)
   except Exception as e:
     logger.exception(e)
     return False
   return is_logged_in(http_util)
 
 
-class InvalidSessionError(Exception):
-  """
-    :meta private:
-  """
-  # not use, hide in doc now
-  DEFAULT_MESSAGE = "Your login session is invalid. please relogin."
-
-  def __init__(self, message: str = DEFAULT_MESSAGE) -> None:
-    super().__init__(message)
-
-
 # TODO logout support
```

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/language.py` & `yxr_atcoder_core-0.0.3.5/ac_core/language.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import List
 
 from bs4 import BeautifulSoup, Tag
 
-from ac_core.constant import _SITE_URL
+from ac_core.constant import SITE_URL
 from ac_core.interfaces.HttpUtil import HttpUtilInterface
 
 
 @dataclass
 class LanguageKV:
   value: str
   text: str
@@ -26,15 +26,15 @@
         from ac_core.auth import fetch_login, is_logged_in
         from ac_core.language import fetch_language
         h = requests.session()
         fetch_login(h, 'username', 'password')
         assert(is_logged_in(h))
         print(fetch_language(h))
   """
-  url = _SITE_URL + '/contests/practice/submit'
+  url = SITE_URL + '/contests/practice/submit'
   resp = http_util.get(url)
   assert resp.status_code == 200
   soup = BeautifulSoup(resp.text, 'lxml')
   result: List[LanguageKV] = []
   tag = soup.find('div', attrs={'id': 'select-lang-practice_1'}).find('select')
   if isinstance(tag, Tag):
     options = tag.find_all('option')
```

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/problem.py` & `yxr_atcoder_core-0.0.3.5/ac_core/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from logging import getLogger
 import re
 from typing import Dict, Iterator, List, Optional, Tuple
 
 from bs4 import BeautifulSoup
 import bs4
-from ac_core.constant import _SITE_URL
+from ac_core.constant import SITE_URL
 from ac_core.modal.problem_test_case import ProblemTestCase
 from ac_core.utils import HTML_PARSER, get_direct_children_text, remove_prefix, remove_suffix
 from ac_core.utils.html_parse_helper import parse_start_end, parse_url
 
 logger = getLogger(__name__)
 
 
@@ -191,15 +191,15 @@
     logger.error(str(e))
 
   score = _parse_score(soup)
   url = parse_url(soup)
   contest_info = soup.find(class_="contest-title")
   assert isinstance(contest_info, bs4.Tag)
   contest_name = contest_info.text
-  contest_url = _SITE_URL + contest_info.attrs["href"]
+  contest_url = SITE_URL + contest_info.attrs["href"]
   start_time, end_time = parse_start_end(soup)
 
   return ProblemResult(
       id=alphabet,
       url=url,
       name=name,
       time_limit_msec=time_limit_msec,
```

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/result.py` & `yxr_atcoder_core-0.0.3.5/ac_core/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from enum import Enum
 import json
 import os
 import re
 
 from bs4 import BeautifulSoup
-from ac_core.constant import _SITE_URL
+from ac_core.constant import SITE_URL
 from ac_core.interfaces.HttpUtil import HttpUtilInterface
 
 
 @dataclass
 class SubmissionResult:
 
   class Status(Enum):
@@ -17,14 +17,15 @@
     PENDING: str = 'Waiting for Judging'
     RUNNING: str = 'Judging'
     RE: str = 'Runtime Error'
     AC: str = 'Accepted'
     WA: str = 'Wrong Answer'
     CE: str = 'Compilation Error'
     TLE: str = 'Time Limit Exceeded'
+    MLE: str = 'Memory Limit Exceeded'
 
   id: str = ''
   url: str = ''  # json url for refetch
   score: int = 500
   status: Status = Status.INIT
   time_cost_ms: int = 0
   mem_cost_kb: int = 0
@@ -38,15 +39,15 @@
 # title=\"Compilation Error\"\u003eCE\u003c/span\u003e\u003c/td\u003e","Score":"0"
 def parse_result(resp: str) -> SubmissionResult:
   """parse submit result get from json result
     :param resp: the json result get from ``https://atcoder.jp/contests/{contest_id}/submissions/me/status/json?sids[]={submision id}``
 
     :examples:
 
-    .. code-block:: 
+    .. code-block::
 
         import requests
         from ac_core.result import parse_result
 
         r = requests.get('https://atcoder.jp/contests/abc101/submissions/me/status/json?sids[]=5371077')
         if r.status_code == 200:
             print(parse_result(r.text)) # pass html
@@ -81,29 +82,29 @@
       mem_cost_kb=mem_cost_kb,
       msg_txt=msg_txt,
   )
 
 
 def fetch_result_by_url(http_util: HttpUtilInterface, json_url: str) -> SubmissionResult:
   """parse submit result by *http_util* with submission *json_url*.
-  
+
     :param http_util: e.g. ``requests.session()``
     :param json_url: e.g. ``https://atcoder.jp/contests/abc101/submissions/me/status/json?sids[]=5371077``
 
     :examples:
 
-    .. code-block:: 
+    .. code-block::
 
         import requests
         from ac_core.result import fetch_result_by_url
         print(fetch_result_by_url(requests.session(),'https://atcoder.jp/contests/abc101/submissions/me/status/json?sids[]=5371077'))
 
     the structured data returned by :py:func:`fetch_result` has the submission json url
 
-    .. code-block:: 
+    .. code-block::
 
         import requests
         from ac_core.auth import fetch_login, is_logged_in
         from ac_core.result import fetch_result, fetch_result_by_url
 
         h = requests.session()
         fetch_login(h, 'username', 'password')
@@ -129,28 +130,28 @@
 
 def _parse_json_url(html: str):
   soup = BeautifulSoup(html, 'lxml')
   # <a href='/contests/abc101/submissions/5371227'>Detail</a>
   r = re.search('<td class="text-center">.*?"/contests/(.*?)/submissions/([0-9]*?)\">Detail</a>', str(soup),
                 re.DOTALL | re.MULTILINE)
   assert r is not None  # no submission
-  return os.path.join(_SITE_URL, f"contests/{r.group(1)}/submissions/me/status/json?sids[]={r.group(2)}")
+  return os.path.join(SITE_URL, f"contests/{r.group(1)}/submissions/me/status/json?sids[]={r.group(2)}")
 
 
 def fetch_result(http_util: HttpUtilInterface, problem_url: str) -> SubmissionResult:
   """parse submit result by *http_util* with *problem_url*.
-    
+
     You need logged in before using this method. This function will find your last submission for the problem.
-  
+
     :param http_util: e.g. ``requests.session()``
     :param problem_url: e.g. ``https://atcoder.jp/contests/abc275/tasks/abc275_f``
 
     :examples:
 
-    .. code-block:: 
+    .. code-block::
 
         import requests
         from ac_core.auth import fetch_login, is_logged_in
         from ac_core.result import fetch_result
 
         h = requests.session()
         fetch_login(h, 'username', 'password')
```

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/submit.py` & `yxr_atcoder_core-0.0.3.5/ac_core/submit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Dict, cast
 
 from bs4 import BeautifulSoup
 import bs4
 
-from ac_core.constant import _SITE_URL
+from ac_core.constant import SITE_URL
 from ac_core.interfaces.HttpUtil import HttpUtilInterface, HttpRespInterface
 from ac_core.url import url_2_contest_id
 from ac_core.utils import HTML_PARSER
 
 
 @dataclass
 class SubmitResult:
@@ -34,15 +34,15 @@
 
     .. code-block::
 
         from ac_core.submit import problem_url_2_submit_url
         print(problem_url_2_submit_url('https://atcoder.jp/contests/abc285/tasks/abc285_a'))
   """
   contest_id = url_2_contest_id(problem_url)
-  return _SITE_URL + '/contests/' + contest_id + '/submit'
+  return SITE_URL + '/contests/' + contest_id + '/submit'
 
 
 def fetch_submit(http_util: HttpUtilInterface, problem_url: str, lang_id: str, source_code: str) -> HttpRespInterface:
   """Submit code. You need logged in before using this method.
 
     :param http_util: e.g. requests.session()
     :param problem_url: e.g. ``'https://atcoder.jp/contests/abc285/tasks/abc285_a'``
```

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/url.py` & `yxr_atcoder_core-0.0.3.5/ac_core/url.py`

 * *Files identical despite different names*

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/contest/listpage.py` & `yxr_atcoder_core-0.0.3.5/ac_core/contest/listpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import List, cast
 from bs4 import BeautifulSoup
 import bs4
 from dataclasses_json import dataclass_json
-from ac_core.constant import _SITE_URL
+from ac_core.constant import SITE_URL
 from ac_core.interfaces.HttpUtil import HttpUtilInterface
 
 from ac_core.utils import HTML_PARSER, time_str_2_timestamp
 
 
 @dataclass_json
 @dataclass
@@ -65,11 +65,11 @@
 
     .. code-block::
 
         import requests
         from ac_core.contest import fetch_list
         print(fetch_list(requests.session()))
   """
-  url = _SITE_URL + '/contests/'
+  url = SITE_URL + '/contests/'
   resp = http_util.get(url)
   assert resp.status_code == 200
   return parse_list(resp.text)
```

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/contest/standing.py` & `yxr_atcoder_core-0.0.3.5/ac_core/contest/standing.py`

 * *Files identical despite different names*

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/contest/tasks.py` & `yxr_atcoder_core-0.0.3.5/ac_core/contest/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bs4 import BeautifulSoup
 import bs4
 
 from ac_core.modal.problem_test_case import ProblemTestCase
 from ac_core.interfaces.HttpUtil import HttpUtilInterface
 from ac_core.problem import parse_task
 from ac_core.utils import HTML_PARSER, remove_suffix
-from ac_core.constant import _SITE_URL
+from ac_core.constant import SITE_URL
 from ac_core.utils.html_parse_helper import parse_start_end, parse_url
 
 
 @dataclass
 class ParserProblemResult:
   id: str
   url: str
@@ -70,15 +70,15 @@
   problems: List[ParserProblemResult] = []
 
   tbody = cast(bs4.Tag, soup.find('tbody'))
   trs = tbody.find_all('tr')
   for tr in trs:
     tds = tr.find_all('td')
     assert len(tds) > 0
-    url = _SITE_URL + tds[1].find('a')['href']
+    url = SITE_URL + tds[1].find('a')['href']
     alphabet = tds[0].text
     name = tds[1].text
     if tds[2].text.endswith(' msec'):
       time_limit_msec = int(remove_suffix(tds[2].text, ' msec'))
     elif tds[2].text.endswith(' sec'):
       time_limit_msec = int(float(remove_suffix(tds[2].text, ' sec')) * 1000)
     else:
@@ -122,15 +122,15 @@
 
     .. code-block::
 
         import requests
         from ac_core.contest import fetch_tasks
         print(fetch_tasks(requests.session(), 'abc259')) # pass contest id
   """
-  contest_url = _SITE_URL + '/contests/' + contest_id + '/tasks'
+  contest_url = SITE_URL + '/contests/' + contest_id + '/tasks'
   contest_resp = http_util.get(contest_url)
   assert contest_resp.status_code == 200
   contest_result = contest_resp.text
   contest_parser_result = parse_tasks(contest_result)
   problems_meta = contest_parser_result.problems
   urls = list(map(lambda p: p.url, problems_meta))
 
@@ -170,11 +170,11 @@
 
     .. code-block::
 
         import requests
         from ac_core.contest import fetch_tasks_meta
         print(fetch_tasks_meta(requests.session(), 'abc260'))
   """
-  url = os.path.join(_SITE_URL, 'contests', contest_id, 'tasks')
+  url = os.path.join(SITE_URL, 'contests', contest_id, 'tasks')
   resp = http_util.get(url)
   assert resp.status_code == 200
   return parse_tasks(resp.text)
```

### Comparing `yxr_atcoder_core-0.0.3.4/ac_core/utils/__init__.py` & `yxr_atcoder_core-0.0.3.5/ac_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yxr_atcoder_core-0.0.3.4/.gitignore` & `yxr_atcoder_core-0.0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `yxr_atcoder_core-0.0.3.4/LICENSE` & `yxr_atcoder_core-0.0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yxr_atcoder_core-0.0.3.4/README.md` & `yxr_atcoder_core-0.0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `yxr_atcoder_core-0.0.3.4/pyproject.toml` & `yxr_atcoder_core-0.0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yxr_atcoder_core-0.0.3.4/PKG-INFO` & `yxr_atcoder_core-0.0.3.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: yxr-atcoder-core
-Version: 0.0.3.4
+Version: 0.0.3.5
 Summary: Simple Atcoder core api
 Project-URL: Homepage, https://github.com/CroMarmot/yxr-atcoder-core
 Project-URL: Bug Tracker, https://github.com/CroMarmot/yxr-atcoder-core/issues
 Author-email: YeXiaoRain <yexiaorain@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 陈鼫RWHTYFZ
@@ -35,16 +35,21 @@
 Requires-Dist: dataclasses-json
 Requires-Dist: lxml>=4
 Requires-Dist: requests>=2
 Requires-Dist: toml
 Requires-Dist: types-beautifulsoup4
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
+Requires-Dist: coverage>=6; extra == 'dev'
+Requires-Dist: furo; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: myst-parser; extra == 'dev'
+Requires-Dist: pytest>=7; extra == 'dev'
+Requires-Dist: sphinx>=5; extra == 'dev'
 Requires-Dist: yapf>=0.32; extra == 'dev'
-Requires-Dist: yxr-atcoder-core[doc,test]; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: furo; extra == 'doc'
 Requires-Dist: myst-parser; extra == 'doc'
 Requires-Dist: sphinx>=5; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: coverage>=6; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
```

