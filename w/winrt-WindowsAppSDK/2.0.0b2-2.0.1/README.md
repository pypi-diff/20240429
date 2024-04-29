# Comparing `tmp/winrt-WindowsAppSDK-2.0.0b2.tar.gz` & `tmp/winrt_WindowsAppSDK-2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winrt-WindowsAppSDK-2.0.0b2.tar", last modified: Sat Dec  2 18:28:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

