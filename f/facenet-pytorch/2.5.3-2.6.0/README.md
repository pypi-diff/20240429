# Comparing `tmp/facenet-pytorch-2.5.3.tar.gz` & `tmp/facenet_pytorch-2.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facenet-pytorch-2.5.3.tar", last modified: Thu Apr  6 17:17:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

