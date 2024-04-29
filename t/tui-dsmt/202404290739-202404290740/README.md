# Comparing `tmp/tui_dsmt-202404290739.tar.gz` & `tmp/tui_dsmt-202404290740-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404290739.tar", last modified: Mon Apr 29 07:39:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

