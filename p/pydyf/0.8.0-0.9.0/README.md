# Comparing `tmp/pydyf-0.8.0.tar.gz` & `tmp/pydyf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydyf-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pydyf-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pydyf-0.8.0.tar` & `pydyf-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1521 2020-10-23 10:08:11.789280 pydyf-0.8.0/LICENSE
--rw-r--r--   0        0        0      866 2022-04-24 06:04:00.881657 pydyf-0.8.0/README.rst
--rw-r--r--   0        0        0      312 2023-03-29 18:08:19.213027 pydyf-0.8.0/docs/api_reference.rst
--rw-r--r--   0        0        0     6157 2023-09-25 10:51:48.241293 pydyf-0.8.0/docs/changelog.rst
--rw-r--r--   0        0        0     4389 2023-03-29 18:08:19.214027 pydyf-0.8.0/docs/common_use_cases.rst
--rw-r--r--   0        0        0     2748 2023-07-13 15:48:39.082171 pydyf-0.8.0/docs/conf.py
--rw-r--r--   0        0        0     2086 2022-09-19 07:09:14.775515 pydyf-0.8.0/docs/contribute.rst
--rw-r--r--   0        0        0      758 2020-12-06 18:47:25.897394 pydyf-0.8.0/docs/first_steps.rst
--rw-r--r--   0        0        0     1032 2022-04-25 11:13:06.410209 pydyf-0.8.0/docs/going_further.rst
--rw-r--r--   0        0        0      296 2020-12-06 18:47:25.897394 pydyf-0.8.0/docs/index.rst
--rw-r--r--   0        0        0      884 2020-12-06 18:47:25.897394 pydyf-0.8.0/docs/support.rst
--rwxr-xr-x   0        0        0    21049 2023-09-25 08:21:44.465171 pydyf-0.8.0/pydyf/__init__.py
--rw-r--r--   0        0        0     1870 2023-07-02 16:38:04.888622 pydyf-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2945 2022-04-23 22:14:02.282916 pydyf-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0    15742 2022-05-22 16:50:31.356023 pydyf-0.8.0/tests/test_pydyf.py
--rw-r--r--   0        0        0     2551 1970-01-01 00:00:00.000000 pydyf-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2020-04-13 15:26:09.000000 pydyf-0.9.0/LICENSE
+-rw-r--r--   0        0        0      866 2022-09-01 13:51:34.003264 pydyf-0.9.0/README.rst
+-rw-r--r--   0        0        0      312 2024-02-26 13:03:37.086921 pydyf-0.9.0/docs/api_reference.rst
+-rw-r--r--   0        0        0     6815 2024-02-26 13:21:41.238674 pydyf-0.9.0/docs/changelog.rst
+-rw-r--r--   0        0        0     6610 2024-02-26 13:03:37.086921 pydyf-0.9.0/docs/common_use_cases.rst
+-rw-r--r--   0        0        0     2748 2024-02-26 13:03:37.086921 pydyf-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0     2086 2024-02-26 13:03:37.090255 pydyf-0.9.0/docs/contribute.rst
+-rw-r--r--   0        0        0      758 2021-02-10 11:12:31.000000 pydyf-0.9.0/docs/first_steps.rst
+-rw-r--r--   0        0        0     1032 2022-09-01 13:51:34.003264 pydyf-0.9.0/docs/going_further.rst
+-rw-r--r--   0        0        0      296 2020-11-29 21:40:31.000000 pydyf-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0      884 2020-11-29 21:40:31.000000 pydyf-0.9.0/docs/support.rst
+-rwxr-xr-x   0        0        0    22270 2024-02-26 13:22:26.869224 pydyf-0.9.0/pydyf/__init__.py
+-rw-r--r--   0        0        0     1871 2024-02-26 13:21:32.794636 pydyf-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2945 2021-08-22 13:18:43.000000 pydyf-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    15742 2022-09-01 13:51:34.003264 pydyf-0.9.0/tests/test_pydyf.py
+-rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 pydyf-0.9.0/PKG-INFO
```

### Comparing `pydyf-0.8.0/LICENSE` & `pydyf-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/README.rst` & `pydyf-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/docs/changelog.rst` & `pydyf-0.9.0/docs/changelog.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,60 @@
 Changelog
 =========
 
 
+Version 0.9.0
+-------------
+
+Released on 2024-02-26.
+
+Dependencies:
+
+* Python 3.12 is supported and tested
+* Python 3.8+ is now needed, Python 3.7 is not supported anymore
+
+New features:
+
+* Add inline images support
+
+Performance:
+
+* Simplify `_to_bytes()`
+
+Documentation:
+
+* Add sample to create a PDF with metadata
+
+Contributors:
+
+* Panagiotis H.M. Issaris
+* Guillaume Ayoub
+* Lucie Anglade
+
+Backers and sponsors:
+
+* Spacinov
+* Kobalt
+* Grip Angebotssoftware
+* Manuel Barkhau
+* SimonSoft
+* Menutech
+* KontextWork
+* René Fritz
+* Simon Sapin
+* Arcanite
+* TrainingSparkle
+* Healthchecks.io
+* Hammerbacher
+* Docraptor
+* Yanal-Yvez Fargialla
+* Morntag
+* NBCO
+
+
 Version 0.8.0
 -------------
 
 Released on 2023-09-25.
 
 New features:
```

### Comparing `pydyf-0.8.0/docs/common_use_cases.rst` & `pydyf-0.9.0/docs/common_use_cases.rst`

 * *Files 27% similar despite different names*

```diff
@@ -175,7 +175,91 @@
           'ProcSet': pydyf.Array(['/PDF', '/Text']),
           'Font': pydyf.Dictionary({'F1': font.reference}),
       })
   }))
 
   with open('document.pdf', 'wb') as f:
       document.write(f)
+
+
+Add metadata
+------------
+
+.. code-block:: python
+
+    import datetime
+
+    import pydyf
+
+    document = pydyf.PDF()
+    document.info['Author'] = pydyf.String('Jane Doe')
+    document.info['Creator'] = pydyf.String('pydyf')
+    document.info['Keywords'] = pydyf.String('some keywords')
+    document.info['Producer'] = pydyf.String('The producer')
+    document.info['Subject'] = pydyf.String('An example PDF')
+    document.info['Title'] = pydyf.String('A PDF containing metadata')
+    now = datetime.datetime.now()
+    document.info['CreationDate'] = pydyf.String(now.strftime('D:%Y%m%d%H%M%S'))
+
+    document.add_page(
+        pydyf.Dictionary(
+            {
+                'Type': '/Page',
+                'Parent': document.pages.reference,
+                'MediaBox': pydyf.Array([0, 0, 200, 200]),
+            }
+        )
+    )
+
+    # 550 bytes PDF
+    with open('metadata.pdf', 'wb') as f:
+        document.write(f)
+
+
+Display inline QR-code image
+----------------------------
+
+.. code-block:: python
+
+    import pydyf
+    import qrcode
+
+    # Create a QR code image
+    image = qrcode.make('Some data here')
+    raw_data = image.tobytes()
+    width = image.size[0]
+    height = image.size[1]
+
+    document = pydyf.PDF()
+    stream = pydyf.Stream(compress=True)
+    stream.push_state()
+    x = 0
+    y = 0
+    stream.transform(width, 0, 0, height, x, y)
+    # Add the 1-bit grayscale image inline in the PDF
+    stream.inline_image(width, height, 'Gray', 1, raw_data)
+    stream.pop_state()
+    document.add_object(stream)
+
+    # Put the image in the resources of the PDF
+    document.add_page(
+        pydyf.Dictionary(
+            {
+                'Type': '/Page',
+                'Parent': document.pages.reference,
+                'MediaBox': pydyf.Array([0, 0, 400, 400]),
+                'Resources': pydyf.Dictionary(
+                    {
+                        'ProcSet': pydyf.Array(
+                            ['/PDF', '/ImageB', '/ImageC', '/ImageI']
+                        ),
+                    }
+                ),
+                'Contents': stream.reference,
+            }
+        )
+    )
+
+    # 909 bytes PDF
+    with open('qrcode.pdf', 'wb') as f:
+        document.write(f, compress=True)
+
```

### Comparing `pydyf-0.8.0/docs/conf.py` & `pydyf-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/docs/contribute.rst` & `pydyf-0.9.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/docs/first_steps.rst` & `pydyf-0.9.0/docs/first_steps.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/docs/going_further.rst` & `pydyf-0.9.0/docs/going_further.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/docs/support.rst` & `pydyf-0.9.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/pydyf/__init__.py` & `pydyf-0.9.0/pydyf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """
 A low-level PDF generator.
 
 """
 
+import base64
 import re
 import zlib
 from codecs import BOM_UTF16_BE
 from hashlib import md5
 from math import ceil, log
 
-VERSION = __version__ = '0.8.0'
+VERSION = __version__ = '0.9.0'
 
 
 def _to_bytes(item):
     """Convert item to bytes."""
     if isinstance(item, bytes):
         return item
-    elif isinstance(item, Object):
-        return item.data
     elif isinstance(item, float):
         if item.is_integer():
-            return f'{int(item):d}'.encode('ascii')
+            return str(int(item)).encode('ascii')
         else:
             return f'{item:f}'.rstrip('0').encode('ascii')
-    elif isinstance(item, int):
-        return f'{item:d}'.encode('ascii')
+    elif isinstance(item, Object):
+        return item.data
     return str(item).encode('ascii')
 
 
 class Object:
     """Base class for PDF objects."""
     def __init__(self):
         #: Number of the object.
@@ -362,14 +361,52 @@
         :type f: :obj:`int` or :obj:`float`
 
         """
         self.stream.append(b' '.join((
             _to_bytes(a), _to_bytes(b), _to_bytes(c),
             _to_bytes(d), _to_bytes(e), _to_bytes(f), b'cm')))
 
+    def inline_image(self, width, height, color_space, bpc, raw_data):
+        """Add an inline image.
+
+        :param width: The width of the image.
+        :type width: :obj:`int`
+        :param height: The height of the image.
+        :type height: :obj:`int`
+        :param colorspace: The color space of the image, f.e. RGB, Gray.
+        :type colorspace: :obj:`str`
+        :param bpc: The bits per component. 1 for BW, 8 for grayscale.
+        :type bpc: :obj:`int`
+        :param raw_data: The raw pixel data.
+
+        """
+        if self.compress:
+            data = zlib.compress(raw_data)
+        else:
+            data = raw_data
+        enc_data = base64.a85encode(data)
+        self.stream.append(
+            b' '.join(
+                (
+                    b'BI',
+                    b'/W', _to_bytes(width),
+                    b'/H', _to_bytes(height),
+                    b'/BPC', _to_bytes(bpc),
+                    b'/CS',
+                    b'/Device' + color_space.encode(),
+                    b'/F',
+                    b'[/A85 /Fl]' if self.compress else b'/A85',
+                    b'/L', _to_bytes(len(enc_data) + 2),
+                    b'ID',
+                    enc_data + b'~>',
+                    b'EI',
+                )
+            )
+        )
+
     @property
     def data(self):
         stream = b'\n'.join(_to_bytes(item) for item in self.stream)
         extra = Dictionary(self.extra.copy())
         if self.compress:
             extra['Filter'] = '/FlateDecode'
             compressobj = zlib.compressobj(level=9)
```

### Comparing `pydyf-0.8.0/pyproject.toml` & `pydyf-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,19 @@
   'Development Status :: 4 - Beta',
   'Intended Audience :: Developers',
   'License :: OSI Approved :: BSD License',
   'Operating System :: OS Independent',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
-  'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
+  'Programming Language :: Python :: 3.12',
   'Programming Language :: Python :: Implementation :: CPython',
   'Programming Language :: Python :: Implementation :: PyPy',
 ]
 dynamic = ['version']
 
 [project.urls]
 Homepage = 'https://www.courtbouillon.org/pydyf'
```

### Comparing `pydyf-0.8.0/tests/__init__.py` & `pydyf-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/tests/test_pydyf.py` & `pydyf-0.9.0/tests/test_pydyf.py`

 * *Files identical despite different names*

### Comparing `pydyf-0.8.0/PKG-INFO` & `pydyf-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pydyf
-Version: 0.8.0
+Version: 0.9.0
 Summary: A low-level PDF generator.
 Keywords: pdf,generator
 Author-email: CourtBouillon <contact@courtbouillon.org>
 Maintainer-email: CourtBouillon <contact@courtbouillon.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: isort ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
```

