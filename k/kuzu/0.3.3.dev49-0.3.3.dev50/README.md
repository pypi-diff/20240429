# Comparing `tmp/kuzu-0.3.3.dev49.tar.gz` & `tmp/kuzu-0.3.3.dev50-cp39-cp39-macosx_11_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.3.3.dev49.tar", last modified: Sun Apr 28 08:04:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

