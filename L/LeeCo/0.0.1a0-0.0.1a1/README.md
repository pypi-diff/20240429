# Comparing `tmp/LeeCo-0.0.1a0.tar.gz` & `tmp/LeeCo-0.0.1a1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\N27321\PycharmProjects\LeetCodeTestcaseHelper\dist\.tmp-ijmbwsua\LeeCo-0.0.1a0.tar", last modified: Tue Apr 23 10:29:45 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

