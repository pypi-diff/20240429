# Comparing `tmp/rina_pp_pyb-0.9.9.tar.gz` & `tmp/rina_pp_pyb-1.0.0-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

