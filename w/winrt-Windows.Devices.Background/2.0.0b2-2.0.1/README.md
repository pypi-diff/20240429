# Comparing `tmp/winrt-Windows.Devices.Background-2.0.0b2.tar.gz` & `tmp/winrt_Windows.Devices.Background-2.0.1-cp39-cp39-win_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winrt-Windows.Devices.Background-2.0.0b2.tar", last modified: Sat Dec  2 18:20:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

