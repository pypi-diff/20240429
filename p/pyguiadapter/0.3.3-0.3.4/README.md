# Comparing `tmp/pyguiadapter-0.3.3.tar.gz` & `tmp/pyguiadapter-0.3.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyguiadapter-0.3.3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

