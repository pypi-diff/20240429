# Comparing `tmp/imgio-1.4.1.tar.gz` & `tmp/imgio-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgio-1.4.1.tar", last modified: Fri Dec 29 13:43:46 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `imgio-1.4.1.tar` & `imgio-1.4.2.tar`

### file list

```diff
@@ -1,38 +1,27 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-12-29 13:43:46.466137 imgio-1.4.1/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-11-03 13:32:12.000000 imgio-1.4.1/LICENSE
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       87 2023-11-03 13:32:12.000000 imgio-1.4.1/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-12-29 13:43:46.466137 imgio-1.4.1/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      705 2023-11-03 13:32:12.000000 imgio-1.4.1/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-12-29 13:43:46.458137 imgio-1.4.1/imgio/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      303 2023-12-29 13:42:30.000000 imgio-1.4.1/imgio/__init__.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    40598 2023-12-29 13:42:30.000000 imgio-1.4.1/imgio/imgio.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4209 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/pfm.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4589 2023-12-29 13:42:30.000000 imgio-1.4.1/imgio/pnm.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-12-29 13:43:46.466137 imgio-1.4.1/imgio/test-images/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    62336 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/GrayRampsDiagonal.exr
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   139435 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/landscape_1.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   137359 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/landscape_2.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   140965 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/landscape_3.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   140588 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/landscape_4.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   137611 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/landscape_5.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   137628 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/landscape_6.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   140645 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/landscape_7.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   141286 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/landscape_8.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   129059 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/portrait_1.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   136072 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/portrait_2.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   135813 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/portrait_3.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   131520 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/portrait_4.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   133715 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/portrait_5.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   136257 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/portrait_6.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   135366 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/portrait_7.jpg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)   132543 2023-11-03 13:32:12.000000 imgio-1.4.1/imgio/test-images/portrait_8.jpg
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-12-29 13:43:46.462137 imgio-1.4.1/imgio.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-12-29 13:43:46.000000 imgio-1.4.1/imgio.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      872 2023-12-29 13:43:46.000000 imgio-1.4.1/imgio.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-12-29 13:43:46.000000 imgio-1.4.1/imgio.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-12-29 13:43:46.000000 imgio-1.4.1/imgio.egg-info/not-zip-safe
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       28 2023-12-29 13:43:46.000000 imgio-1.4.1/imgio.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        6 2023-12-29 13:43:46.000000 imgio-1.4.1/imgio.egg-info/top_level.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       32 2023-11-03 13:32:12.000000 imgio-1.4.1/requirements.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-12-29 13:43:46.466137 imgio-1.4.1/setup.cfg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      605 2023-11-03 13:32:12.000000 imgio-1.4.1/setup.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/__init__.py
+-rwxr-xr-x   0        0        0    40598 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/imgio.py
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/pfm.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/pnm.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/version.py
+-rw-r--r--   0        0        0    62336 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/GrayRampsDiagonal.exr
+-rw-r--r--   0        0        0   139435 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/landscape_1.jpg
+-rw-r--r--   0        0        0   137359 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/landscape_2.jpg
+-rw-r--r--   0        0        0   140965 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/landscape_3.jpg
+-rw-r--r--   0        0        0   140588 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/landscape_4.jpg
+-rw-r--r--   0        0        0   137611 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/landscape_5.jpg
+-rw-r--r--   0        0        0   137628 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/landscape_6.jpg
+-rw-r--r--   0        0        0   140645 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/landscape_7.jpg
+-rw-r--r--   0        0        0   141286 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/landscape_8.jpg
+-rw-r--r--   0        0        0   129059 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/portrait_1.jpg
+-rw-r--r--   0        0        0   136072 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/portrait_2.jpg
+-rw-r--r--   0        0        0   135813 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/portrait_3.jpg
+-rw-r--r--   0        0        0   131520 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/portrait_4.jpg
+-rw-r--r--   0        0        0   133715 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/portrait_5.jpg
+-rw-r--r--   0        0        0   136257 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/portrait_6.jpg
+-rw-r--r--   0        0        0   135366 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/portrait_7.jpg
+-rw-r--r--   0        0        0   132543 2020-02-02 00:00:00.000000 imgio-1.4.2/imgio/test-images/portrait_8.jpg
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 imgio-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 imgio-1.4.2/LICENSE
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 imgio-1.4.2/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 imgio-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 imgio-1.4.2/PKG-INFO
```

### Comparing `imgio-1.4.1/LICENSE` & `imgio-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/README.md` & `imgio-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # imgio
 
 [![Build Status](https://travis-ci.com/toaarnio/imgio.svg?branch=master)](https://travis-ci.com/github/toaarnio/imgio)
 
-Easy image file reading &amp; writing for Python. Tested on Python 3.8+.
+Easy image file reading &amp; writing for Python. Tested on Python 3.10.
 
 Supported file formats (read/write):
 
 ```
    .pnm
    .pgm
    .ppm
```

### Comparing `imgio-1.4.1/imgio/imgio.py` & `imgio-1.4.2/imgio/imgio.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
         o4 = ((b4 % 4) << 8) + b5
     unpacked = np.c_[o1, o2, o3, o4].ravel()
     return unpacked
 
 def _write_raw(filespec, image, _maxval, _pack=False, _verbose=False):
     # Warning: hardcoded endianness (x86)
     with open(filespec, "wb") as outfile:
-        image = image.copy(order='C')  # ensure x86 byte order
+        image = image.copy(order="C")  # ensure x86 byte order
         outfile.write(image)
 
 
 ######################################################################################
 #
 #  U N I T   T E S T S
 #
@@ -437,15 +437,15 @@
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", np.zeros((7, 7, 1), np.uint8))
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", np.zeros((7, 7, 2), np.uint8))
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", np.zeros((7, 7, 4), np.uint8))
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", np.zeros((7, 7, 3, 1), np.uint8))
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", pixels.astype(bool))
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", pixels.astype(np.float16))
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", pixels.astype(np.float64))
-        self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", pixels.astype('>f4'))
+        self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.ppm", pixels.astype(">f4"))
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.pfm", pixels, -1.0)
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "imgio.test.pfm", pixels, "255")
         self.assertRaisesRegex(ImageIOError, "^Failed to write.*shape", imwrite, "imgio.test.raw", pixels8b, 255)
         self.assertRaisesRegex(ImageIOError, "^Failed to write.*supported", imwrite, "imgio.test.raw", pixels8b, 255, packed=True)
         self.assertRaisesRegex(ImageIOError, "^Failed to write.*verbose", imwrite, "imgio.test.ppm", pixels8b, 255, verbose=0)
         os.remove("invalidformat.pfm")
         os.remove("invalidformat.jpg")
```

### Comparing `imgio-1.4.1/imgio/pfm.py` & `imgio-1.4.2/imgio/pfm.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def read(filename, verbose=False):
     """
     Reads in a PFM file by the given name and returns its contents in a new
     numpy ndarray with float32 elements. The absolute value of the 'scale
     factor' attribute is also returned. Both 1-channel and 3-channel images
     are supported, as well as both byte orders.
     """
-    with open(filename, 'rb') as f:
+    with open(filename, "rb") as f:
         buf = f.read()
         parsed = parse(buf)
         if parsed is not None:
             pixels, scale = parsed
             if verbose:
                 maxx = np.max(pixels)
                 h, w = pixels.shape[:2]
@@ -35,17 +35,17 @@
 def write(filename, pixels, scale=1.0, little_endian=True, verbose=False):
     """
     Writes the contents of the given float32 ndarray into a 1- or 3-channel
     PFM file by the given name. Both little-endian and big-endian files are
     supported. The shape of the given array must be (h, w) or (h, w, c),
     where c is either 1 or 3.
     """
-    with open(filename, 'wb') as f:
+    with open(filename, "wb") as f:
         if verbose:
-            print("Writing file %s "%(filename), end='')
+            print("Writing file %s "%(filename), end="")
         pfm_bytearray = generate(pixels, scale, little_endian, verbose)
         f.write(pfm_bytearray)
 
 def parse(pfm_bytearray):
     """
     Converts the given byte array, representing the contents of a PFM file, into
     a 1-channel or 3-channel numpy ndarray with float32 elements. Returns a tuple
@@ -88,10 +88,10 @@
         scale = -scale
         f32bs = f32
     else:
         byteorder = ">"
         f32bs = f32.byteswap()
     if verbose:
         print("(w=%d, h=%d, c=%d, scale=%.3f, byteorder='%s')"%(width, height, numchannels, abs(scale), byteorder))
-    pfm_bytearray = bytearray("%s %d %d %.3f\n"%(typestr, width, height, scale), 'utf-8')
+    pfm_bytearray = bytearray("%s %d %d %.3f\n"%(typestr, width, height, scale), "utf-8")
     pfm_bytearray.extend(f32bs.flatten())
     return bytes(pfm_bytearray)
```

### Comparing `imgio-1.4.1/imgio/pnm.py` & `imgio-1.4.2/imgio/pnm.py`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/GrayRampsDiagonal.exr` & `imgio-1.4.2/imgio/test-images/GrayRampsDiagonal.exr`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/landscape_1.jpg` & `imgio-1.4.2/imgio/test-images/landscape_1.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/landscape_2.jpg` & `imgio-1.4.2/imgio/test-images/landscape_2.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/landscape_3.jpg` & `imgio-1.4.2/imgio/test-images/landscape_3.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/landscape_4.jpg` & `imgio-1.4.2/imgio/test-images/landscape_4.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/landscape_5.jpg` & `imgio-1.4.2/imgio/test-images/landscape_5.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/landscape_6.jpg` & `imgio-1.4.2/imgio/test-images/landscape_6.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/landscape_7.jpg` & `imgio-1.4.2/imgio/test-images/landscape_7.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/landscape_8.jpg` & `imgio-1.4.2/imgio/test-images/landscape_8.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/portrait_1.jpg` & `imgio-1.4.2/imgio/test-images/portrait_1.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/portrait_2.jpg` & `imgio-1.4.2/imgio/test-images/portrait_2.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/portrait_3.jpg` & `imgio-1.4.2/imgio/test-images/portrait_3.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/portrait_4.jpg` & `imgio-1.4.2/imgio/test-images/portrait_4.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/portrait_5.jpg` & `imgio-1.4.2/imgio/test-images/portrait_5.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/portrait_6.jpg` & `imgio-1.4.2/imgio/test-images/portrait_6.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/portrait_7.jpg` & `imgio-1.4.2/imgio/test-images/portrait_7.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.4.1/imgio/test-images/portrait_8.jpg` & `imgio-1.4.2/imgio/test-images/portrait_8.jpg`

 * *Files identical despite different names*

