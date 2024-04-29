# Comparing `tmp/databend_sqlalchemy-0.4.5.tar.gz` & `tmp/databend_sqlalchemy-0.4.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databend_sqlalchemy-0.4.5.tar", last modified: Thu Feb  1 11:50:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

