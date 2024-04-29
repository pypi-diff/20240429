# Comparing `tmp/PyGenStability-0.2.3.tar.gz` & `tmp/PyGenStability-0.2.4-cp39-cp39-macosx_10_13_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGenStability-0.2.3.tar", last modified: Mon Nov  6 07:40:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

