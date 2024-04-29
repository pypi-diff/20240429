# Comparing `tmp/asyncTwitterClient-0.5.0.tar.gz` & `tmp/asyncTwitterClient-0.6.0.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncTwitterClient-0.5.0.tar", last modified: Sun Apr 28 21:44:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

