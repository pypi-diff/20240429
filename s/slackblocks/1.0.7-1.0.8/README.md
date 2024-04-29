# Comparing `tmp/slackblocks-1.0.7.tar.gz` & `tmp/slackblocks-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackblocks-1.0.7.tar", max compression
+gzip compressed data, was "slackblocks-1.0.8.tar", max compression
```

## Comparing `slackblocks-1.0.7.tar` & `slackblocks-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1065 2024-02-26 23:34:49.585947 slackblocks-1.0.7/LICENSE
--rw-r--r--   0        0        0     1526 2024-02-26 23:34:49.585947 slackblocks-1.0.7/LICENSE.BSD-3-Clause
--rw-r--r--   0        0        0     2554 2024-02-26 23:34:49.585947 slackblocks-1.0.7/README.md
--rw-r--r--   0        0        0     1753 2024-02-26 23:34:49.593947 slackblocks-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1505 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/__init__.py
--rw-r--r--   0        0        0     5834 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/attachments.py
--rw-r--r--   0        0        0    14918 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/blocks.py
--rw-r--r--   0        0        0    68769 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/elements.py
--rw-r--r--   0        0        0      455 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/errors.py
--rw-r--r--   0        0        0    10141 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/messages.py
--rw-r--r--   0        0        0      696 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/modals.py
--rw-r--r--   0        0        0    17987 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/objects.py
--rw-r--r--   0        0        0      669 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/rich_text/__init__.py
--rw-r--r--   0        0        0    11732 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/rich_text/elements.py
--rw-r--r--   0        0        0     7788 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/rich_text/objects.py
--rw-r--r--   0        0        0     6800 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/utils.py
--rw-r--r--   0        0        0     5902 2024-02-26 23:34:49.593947 slackblocks-1.0.7/slackblocks/views.py
--rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 slackblocks-1.0.7/setup.py
--rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 slackblocks-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-29 06:33:12.600847 slackblocks-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1526 2024-04-29 06:33:12.600847 slackblocks-1.0.8/LICENSE.BSD-3-Clause
+-rw-r--r--   0        0        0     2554 2024-04-29 06:33:12.600847 slackblocks-1.0.8/README.md
+-rw-r--r--   0        0        0     1753 2024-04-29 06:33:12.608847 slackblocks-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1505 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/__init__.py
+-rw-r--r--   0        0        0     5834 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/attachments.py
+-rw-r--r--   0        0        0    14958 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/blocks.py
+-rw-r--r--   0        0        0    68769 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/elements.py
+-rw-r--r--   0        0        0      455 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/errors.py
+-rw-r--r--   0        0        0    10141 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/messages.py
+-rw-r--r--   0        0        0      696 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/modals.py
+-rw-r--r--   0        0        0    17987 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/objects.py
+-rw-r--r--   0        0        0      669 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/rich_text/__init__.py
+-rw-r--r--   0        0        0    11732 2024-04-29 06:33:12.608847 slackblocks-1.0.8/slackblocks/rich_text/elements.py
+-rw-r--r--   0        0        0     7788 2024-04-29 06:33:12.612847 slackblocks-1.0.8/slackblocks/rich_text/objects.py
+-rw-r--r--   0        0        0     6800 2024-04-29 06:33:12.612847 slackblocks-1.0.8/slackblocks/utils.py
+-rw-r--r--   0        0        0     5902 2024-04-29 06:33:12.612847 slackblocks-1.0.8/slackblocks/views.py
+-rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 slackblocks-1.0.8/setup.py
+-rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 slackblocks-1.0.8/PKG-INFO
```

### Comparing `slackblocks-1.0.7/LICENSE` & `slackblocks-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/LICENSE.BSD-3-Clause` & `slackblocks-1.0.8/LICENSE.BSD-3-Clause`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/README.md` & `slackblocks-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/pyproject.toml` & `slackblocks-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slackblocks"
-version = "1.0.7"
+version = "1.0.8"
 description = "Python wrapper for the Slack Blocks API"
 authors = [
     "Nicholas Lambourne <dev@ndl.im>",
 ]
 maintainers = [
     "Nicholas Lambourne <dev@ndl.im>",
 ]
```

### Comparing `slackblocks-1.0.7/slackblocks/__init__.py` & `slackblocks-1.0.8/slackblocks/__init__.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/attachments.py` & `slackblocks-1.0.8/slackblocks/attachments.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/blocks.py` & `slackblocks-1.0.8/slackblocks/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,21 @@
     RadioButtonGroup,
     StaticMultiSelectMenu,
     StaticSelectMenu,
     UserMultiSelectMenu,
     UserSelectMenu,
 )
 from slackblocks.errors import InvalidUsageError
-from slackblocks.objects import CompositionObjectType, Text, TextLike, TextType
+from slackblocks.objects import (
+    CompositionObject,
+    CompositionObjectType,
+    Text,
+    TextLike,
+    TextType,
+)
 from slackblocks.rich_text import (
     RichTextCodeBlock,
     RichTextList,
     RichTextObject,
     RichTextQuote,
     RichTextSection,
 )
@@ -139,15 +145,15 @@
 
     Throws:
         InvalidUsageError: when items in `elements` are not `Text` or `Image` or exceed 10 items.
     """
 
     def __init__(
         self,
-        elements: Optional[List[Union[Element, CompositionObjectType]]] = None,
+        elements: Optional[List[Union[Element, CompositionObject]]] = None,
         block_id: Optional[str] = None,
     ) -> "ContextBlock":
         super().__init__(type_=BlockType.CONTEXT, block_id=block_id)
         self.elements = []
         for element in elements:
             if (
                 element.type == CompositionObjectType.TEXT
```

### Comparing `slackblocks-1.0.7/slackblocks/elements.py` & `slackblocks-1.0.8/slackblocks/elements.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/messages.py` & `slackblocks-1.0.8/slackblocks/messages.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/modals.py` & `slackblocks-1.0.8/slackblocks/modals.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/objects.py` & `slackblocks-1.0.8/slackblocks/objects.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/rich_text/__init__.py` & `slackblocks-1.0.8/slackblocks/rich_text/__init__.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/rich_text/elements.py` & `slackblocks-1.0.8/slackblocks/rich_text/elements.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/rich_text/objects.py` & `slackblocks-1.0.8/slackblocks/rich_text/objects.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/utils.py` & `slackblocks-1.0.8/slackblocks/utils.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/slackblocks/views.py` & `slackblocks-1.0.8/slackblocks/views.py`

 * *Files identical despite different names*

### Comparing `slackblocks-1.0.7/setup.py` & `slackblocks-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['slackblocks', 'slackblocks.rich_text']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'slackblocks',
-    'version': '1.0.7',
+    'version': '1.0.8',
     'description': 'Python wrapper for the Slack Blocks API',
     'long_description': '# slackblocks <img src="https://github.com/nicklambourne/slackblocks/raw/master/docs_src/img/sb.png" align="right" width="250px"/>\n\n![Licence: MIT](https://img.shields.io/badge/License-MIT-green.svg)\n![Licence: BSD-3-Clause](https://img.shields.io/badge/License-BSD_3_Clause-green.svg)\n![Python Versions](https://img.shields.io/pypi/pyversions/slackblocks)\n[![PyPI](https://img.shields.io/pypi/v/slackblocks?color=yellow&label=PyPI&logo=python&logoColor=white)](https://pypi.org/project/slackblocks/#history)\n[![Downloads](https://static.pepy.tech/badge/slackblocks)](https://pepy.tech/project/slackblocks)\n[![Build Status](https://github.com/nicklambourne/slackblocks/actions/workflows/unit-tests.yml/badge.svg?branch=master)](https://github.com/nicklambourne/slackblocks/actions)\n[![Docs](https://img.shields.io/badge/Docs-8A2BE2.svg)](https://nicklambourne.github.io/slackblocks)\n\n## What is it?\n`slackblocks` is a Python API for building messages in the fancy Slack [Block Kit API](https://api.slack.com/block-kit)\n\n## Documentation\nFull documentation is provided [here](https://nicklambourne.github.io/slackblocks/latest/).\n\n## Requirements\n`slackblocks` requires Python >= 3.8.\n\nAs of version 0.1.0 it has no dependencies outside the Python standard library.\n\n## Installation\n```bash\npip install slackblocks\n```\n\n## Basic Usage\n```python\nfrom slackblocks import Message, SectionBlock\n\n\nblock = SectionBlock("Hello, world!")\nmessage = Message(channel="#general", blocks=block)\nmessage.json()\n\n```\n\nWill produce the following JSON string:\n```json\n{\n    "channel": "#general",\n    "mrkdwn": true,\n    "blocks": [\n        {\n            "type": "section",\n            "block_id": "992ceb6b-9ad4-496b-b8e6-1bd8a632e8b3",\n            "text": {\n                "type": "mrkdwn",\n                "text": "Hello, world!"\n            }\n        }\n    ]\n}\n```\nWhich can be sent as payload to the Slack message API HTTP endpoints.\n\nOf more practical uses is the ability to unpack the objects directly into \nthe Python Slack Client in order to send messages:\n```python\nfrom os import environ\nfrom slack import WebClient\nfrom slackblocks import Message, SectionBlock\n\n\nclient = WebClient(token=environ["SLACK_API_TOKEN"])\nblock = SectionBlock("Hello, world!")\nmessage = Message(channel="#general", blocks=block)\n\nresponse = client.chat_postMessage(**message)\n```\n\nNote the `**` operator in front of the `message` object.\n\n## Can I use this in my project?\nYes, please do! The code is all open source and dual BSD-3.0 and MIT licensed\n    (use what suits you best).\n',
     'author': 'Nicholas Lambourne',
     'author_email': 'dev@ndl.im',
     'maintainer': 'Nicholas Lambourne',
     'maintainer_email': 'dev@ndl.im',
     'url': 'https://github.com/nicklambourne/slackblocks',
```

### Comparing `slackblocks-1.0.7/PKG-INFO` & `slackblocks-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackblocks
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python wrapper for the Slack Blocks API
 Home-page: https://github.com/nicklambourne/slackblocks
 License: MIT
 Keywords: slackblocks,slack,messaging,message generation,slack blocks,blocks
 Author: Nicholas Lambourne
 Author-email: dev@ndl.im
 Maintainer: Nicholas Lambourne
```

