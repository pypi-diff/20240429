# Comparing `tmp/winrt-Windows.Media.Capture.Core-2.0.0b2.tar.gz` & `tmp/winrt_Windows.Media.Capture.Core-2.0.1-cp39-cp39-win_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winrt-Windows.Media.Capture.Core-2.0.0b2.tar", last modified: Sat Dec  2 18:23:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

