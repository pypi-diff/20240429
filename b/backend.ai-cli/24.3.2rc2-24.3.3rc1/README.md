# Comparing `tmp/backend.ai-cli-24.3.2rc2.tar.gz` & `tmp/backend.ai_cli-24.3.3rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-cli-24.3.2rc2.tar", last modified: Wed Apr 17 05:19:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

