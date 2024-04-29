# Comparing `tmp/classy-community-23.1.0.tar.gz` & `tmp/classy_community-23.2.0-cp312-cp312-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classy-community-23.1.0.tar", last modified: Tue Sep  5 17:16:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

