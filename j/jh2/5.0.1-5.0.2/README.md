# Comparing `tmp/jh2-5.0.1.tar.gz` & `tmp/jh2-5.0.2-pp38-pypy38_pp73-macosx_10_12_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

