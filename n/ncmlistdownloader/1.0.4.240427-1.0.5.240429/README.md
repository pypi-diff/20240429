# Comparing `tmp/ncmlistdownloader-1.0.4.240427.tar.gz` & `tmp/ncmlistdownloader-1.0.5.240429-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.4.240427.tar", last modified: Sat Apr 27 08:17:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

