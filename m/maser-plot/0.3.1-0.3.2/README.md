# Comparing `tmp/maser_plot-0.3.1.tar.gz` & `tmp/maser_plot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maser_plot-0.3.1.tar", max compression
+gzip compressed data, was "maser_plot-0.3.2.tar", max compression
```

## Comparing `maser_plot-0.3.1.tar` & `maser_plot-0.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     2582 2024-03-14 14:17:35.235126 maser_plot-0.3.1/README.md
--rw-r--r--   0        0        0       80 2024-03-14 14:17:35.227635 maser_plot-0.3.1/maser/__init__.py
--rw-r--r--   0        0        0     1797 2024-03-14 14:17:35.227496 maser_plot-0.3.1/maser/plot/__init__.py
--rw-r--r--   0        0        0      533 2024-03-14 14:17:35.227883 maser_plot-0.3.1/maser/plot/base/__init__.py
--rw-r--r--   0        0        0    13234 2024-03-14 14:17:35.228025 maser_plot-0.3.1/maser/plot/base/base.py
--rw-r--r--   0        0        0     1306 2024-03-14 14:17:35.227948 maser_plot-0.3.1/maser/plot/base/dataset_filename_regex.json
--rw-r--r--   0        0        0      673 2024-03-14 14:17:35.228228 maser_plot-0.3.1/maser/plot/cdpp/__init__.py
--rw-r--r--   0        0        0       89 2024-03-14 14:17:35.228316 maser_plot-0.3.1/maser/plot/cdpp/interball/__init__.py
--rw-r--r--   0        0        0      501 2024-03-14 14:17:35.228400 maser_plot-0.3.1/maser/plot/cdpp/interball/plot.py
--rw-r--r--   0        0        0      208 2024-03-14 14:17:35.228600 maser_plot-0.3.1/maser/plot/cdpp/stereo/__init__.py
--rw-r--r--   0        0        0     2406 2024-03-14 14:17:35.228699 maser_plot-0.3.1/maser/plot/cdpp/stereo/plot.py
--rw-r--r--   0        0        0       75 2024-03-14 14:17:35.230607 maser_plot-0.3.1/maser/plot/cdpp/viking/__init__.py
--rw-r--r--   0        0        0      198 2024-03-14 14:17:35.228944 maser_plot-0.3.1/maser/plot/cdpp/viking/plot.py
--rw-r--r--   0        0        0      346 2024-03-14 14:17:35.229023 maser_plot-0.3.1/maser/plot/cdpp/wind/__init__.py
--rw-r--r--   0        0        0     2198 2024-03-14 14:17:35.229128 maser_plot-0.3.1/maser/plot/cdpp/wind/plot.py
--rw-r--r--   0        0        0      403 2024-03-14 14:17:35.228841 maser_plot-0.3.1/maser/plot/ecallisto/__init__.py
--rw-r--r--   0        0        0      622 2024-03-14 14:17:35.229349 maser_plot-0.3.1/maser/plot/ecallisto/plot.py
--rw-r--r--   0        0        0      826 2024-03-14 14:17:35.229499 maser_plot-0.3.1/maser/plot/nancay/__init__.py
--rw-r--r--   0        0        0      273 2024-03-14 14:17:35.229696 maser_plot-0.3.1/maser/plot/nancay/nda/__init__.py
--rw-r--r--   0        0        0     2511 2024-03-14 14:17:35.230612 maser_plot-0.3.1/maser/plot/nancay/nda/plot.py
--rw-r--r--   0        0        0      128 2024-03-14 14:17:35.230535 maser_plot-0.3.1/maser/plot/nancay/nenufar/__init__.py
--rw-r--r--   0        0        0      525 2024-03-14 14:17:35.230577 maser_plot-0.3.1/maser/plot/nancay/nenufar/plot.py
--rw-r--r--   0        0        0      690 2024-03-14 14:17:35.230576 maser_plot-0.3.1/maser/plot/padc/__init__.py
--rw-r--r--   0        0        0       73 2024-03-14 14:17:35.230668 maser_plot-0.3.1/maser/plot/padc/bepi/__init__.py
--rw-r--r--   0        0        0      118 2024-03-14 14:17:35.230774 maser_plot-0.3.1/maser/plot/padc/bepi/sorbet/__init__.py
--rw-r--r--   0        0        0      633 2024-03-14 14:17:35.230886 maser_plot-0.3.1/maser/plot/padc/bepi/sorbet/plot.py
--rw-r--r--   0        0        0      114 2024-03-14 14:17:35.231567 maser_plot-0.3.1/maser/plot/padc/cassini/__init__.py
--rw-r--r--   0        0        0     2295 2024-03-14 14:17:35.231214 maser_plot-0.3.1/maser/plot/padc/cassini/plot.py
--rw-r--r--   0        0        0     1243 2024-03-14 14:17:35.231020 maser_plot-0.3.1/maser/plot/padc/expres/__init__.py
--rw-r--r--   0        0        0     1562 2024-03-14 14:17:35.231710 maser_plot-0.3.1/maser/plot/padc/expres/plot.py
--rw-r--r--   0        0        0       87 2024-03-14 14:17:35.231868 maser_plot-0.3.1/maser/plot/padc/juno/__init__.py
--rw-r--r--   0        0        0     2321 2024-03-14 14:17:35.232010 maser_plot-0.3.1/maser/plot/padc/juno/plot.py
--rw-r--r--   0        0        0      260 2024-03-14 14:17:35.232104 maser_plot-0.3.1/maser/plot/padc/stereo/__init__.py
--rw-r--r--   0        0        0     2112 2024-03-14 14:17:35.232208 maser_plot-0.3.1/maser/plot/padc/stereo/plot.py
--rw-r--r--   0        0        0      148 2024-03-14 14:17:35.232291 maser_plot-0.3.1/maser/plot/padc/wind/__init__.py
--rw-r--r--   0        0        0     1376 2024-03-14 14:17:35.232377 maser_plot-0.3.1/maser/plot/padc/wind/plot.py
--rw-r--r--   0        0        0      524 2024-03-14 14:17:35.232632 maser_plot-0.3.1/maser/plot/pds/__init__.py
--rw-r--r--   0        0        0      131 2024-03-14 14:17:35.232773 maser_plot-0.3.1/maser/plot/pds/co/__init__.py
--rw-r--r--   0        0        0      544 2024-03-14 14:17:35.232910 maser_plot-0.3.1/maser/plot/pds/co/plot.py
--rw-r--r--   0        0        0     2555 2024-03-14 14:17:35.232989 maser_plot-0.3.1/maser/plot/pds/plot.py
--rw-r--r--   0        0        0      371 2024-03-14 14:17:35.233078 maser_plot-0.3.1/maser/plot/pds/vg/__init__.py
--rw-r--r--   0        0        0     4510 2024-03-14 14:17:35.233170 maser_plot-0.3.1/maser/plot/pds/vg/plot.py
--rw-r--r--   0        0        0      286 2024-03-14 14:17:35.233253 maser_plot-0.3.1/maser/plot/psa/__init__.py
--rw-r--r--   0        0        0      287 2024-03-14 14:17:35.233347 maser_plot-0.3.1/maser/plot/psa/mex/__init__.py
--rw-r--r--   0        0        0     1221 2024-03-14 14:17:35.233431 maser_plot-0.3.1/maser/plot/psa/mex/plot.py
--rw-r--r--   0        0        0      443 2024-03-14 14:17:35.233648 maser_plot-0.3.1/maser/plot/rpw/__init__.py
--rw-r--r--   0        0        0     3629 2024-03-14 14:17:35.233813 maser_plot-0.3.1/maser/plot/rpw/cross_section.py
--rw-r--r--   0        0        0     4565 2024-03-14 14:17:35.233993 maser_plot-0.3.1/maser/plot/rpw/lfr.py
--rw-r--r--   0        0        0     2733 2024-03-14 14:17:35.234489 maser_plot-0.3.1/maser/plot/rpw/plot.py
--rw-r--r--   0        0        0     5339 2024-03-14 14:17:35.233719 maser_plot-0.3.1/maser/plot/rpw/plot_mean.py
--rw-r--r--   0        0        0     5518 2024-03-14 14:17:35.234796 maser_plot-0.3.1/maser/plot/rpw/quick_look.py
--rw-r--r--   0        0        0     2360 2024-03-14 14:17:35.234898 maser_plot-0.3.1/maser/plot/rpw/tnr.py
--rw-r--r--   0        0        0      527 2024-03-14 14:17:35.234969 maser_plot-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 maser_plot-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2582 2024-03-15 09:04:50.806732 maser_plot-0.3.2/README.md
+-rw-r--r--   0        0        0       80 2024-03-14 14:17:35.227635 maser_plot-0.3.2/maser/__init__.py
+-rw-r--r--   0        0        0     1797 2024-03-15 09:04:50.797860 maser_plot-0.3.2/maser/plot/__init__.py
+-rw-r--r--   0        0        0      533 2024-03-15 09:04:50.798014 maser_plot-0.3.2/maser/plot/base/__init__.py
+-rw-r--r--   0        0        0    13234 2024-03-15 09:04:50.798169 maser_plot-0.3.2/maser/plot/base/base.py
+-rw-r--r--   0        0        0     1306 2024-03-15 09:04:50.798380 maser_plot-0.3.2/maser/plot/base/dataset_filename_regex.json
+-rw-r--r--   0        0        0      673 2024-03-15 09:04:50.798506 maser_plot-0.3.2/maser/plot/cdpp/__init__.py
+-rw-r--r--   0        0        0       89 2024-03-15 09:04:50.798737 maser_plot-0.3.2/maser/plot/cdpp/interball/__init__.py
+-rw-r--r--   0        0        0      501 2024-03-15 09:04:50.798852 maser_plot-0.3.2/maser/plot/cdpp/interball/plot.py
+-rw-r--r--   0        0        0      208 2024-03-15 09:04:50.798965 maser_plot-0.3.2/maser/plot/cdpp/stereo/__init__.py
+-rw-r--r--   0        0        0     2406 2024-03-15 09:04:50.799094 maser_plot-0.3.2/maser/plot/cdpp/stereo/plot.py
+-rw-r--r--   0        0        0       75 2024-03-15 09:04:50.799252 maser_plot-0.3.2/maser/plot/cdpp/viking/__init__.py
+-rw-r--r--   0        0        0      198 2024-03-15 09:04:50.799392 maser_plot-0.3.2/maser/plot/cdpp/viking/plot.py
+-rw-r--r--   0        0        0      346 2024-03-15 09:04:50.799562 maser_plot-0.3.2/maser/plot/cdpp/wind/__init__.py
+-rw-r--r--   0        0        0     2198 2024-03-15 09:04:50.799743 maser_plot-0.3.2/maser/plot/cdpp/wind/plot.py
+-rw-r--r--   0        0        0      403 2024-03-15 09:04:50.799949 maser_plot-0.3.2/maser/plot/ecallisto/__init__.py
+-rw-r--r--   0        0        0      622 2024-03-15 09:04:50.800086 maser_plot-0.3.2/maser/plot/ecallisto/plot.py
+-rw-r--r--   0        0        0      826 2024-03-15 09:04:50.800296 maser_plot-0.3.2/maser/plot/nancay/__init__.py
+-rw-r--r--   0        0        0      273 2024-03-15 09:04:50.800431 maser_plot-0.3.2/maser/plot/nancay/nda/__init__.py
+-rw-r--r--   0        0        0     2511 2024-03-15 09:04:50.800571 maser_plot-0.3.2/maser/plot/nancay/nda/plot.py
+-rw-r--r--   0        0        0      128 2024-03-15 09:04:50.800808 maser_plot-0.3.2/maser/plot/nancay/nenufar/__init__.py
+-rw-r--r--   0        0        0      525 2024-03-15 09:04:50.801039 maser_plot-0.3.2/maser/plot/nancay/nenufar/plot.py
+-rw-r--r--   0        0        0      690 2024-03-15 09:04:50.801191 maser_plot-0.3.2/maser/plot/padc/__init__.py
+-rw-r--r--   0        0        0       73 2024-03-15 09:04:50.801341 maser_plot-0.3.2/maser/plot/padc/bepi/__init__.py
+-rw-r--r--   0        0        0      118 2024-03-15 09:04:50.801504 maser_plot-0.3.2/maser/plot/padc/bepi/sorbet/__init__.py
+-rw-r--r--   0        0        0      633 2024-03-15 09:04:50.801719 maser_plot-0.3.2/maser/plot/padc/bepi/sorbet/plot.py
+-rw-r--r--   0        0        0      114 2024-03-15 09:04:50.801873 maser_plot-0.3.2/maser/plot/padc/cassini/__init__.py
+-rw-r--r--   0        0        0     2295 2024-03-15 09:04:50.802083 maser_plot-0.3.2/maser/plot/padc/cassini/plot.py
+-rw-r--r--   0        0        0     1243 2024-03-15 09:04:50.802221 maser_plot-0.3.2/maser/plot/padc/expres/__init__.py
+-rw-r--r--   0        0        0     1562 2024-03-15 09:04:50.802400 maser_plot-0.3.2/maser/plot/padc/expres/plot.py
+-rw-r--r--   0        0        0       87 2024-03-15 09:04:50.802630 maser_plot-0.3.2/maser/plot/padc/juno/__init__.py
+-rw-r--r--   0        0        0     2321 2024-03-15 09:04:50.802835 maser_plot-0.3.2/maser/plot/padc/juno/plot.py
+-rw-r--r--   0        0        0      260 2024-03-15 09:04:50.803049 maser_plot-0.3.2/maser/plot/padc/stereo/__init__.py
+-rw-r--r--   0        0        0     2112 2024-03-15 09:04:50.803383 maser_plot-0.3.2/maser/plot/padc/stereo/plot.py
+-rw-r--r--   0        0        0      148 2024-03-15 09:04:50.803237 maser_plot-0.3.2/maser/plot/padc/wind/__init__.py
+-rw-r--r--   0        0        0     1376 2024-03-15 09:04:50.803906 maser_plot-0.3.2/maser/plot/padc/wind/plot.py
+-rw-r--r--   0        0        0      524 2024-03-15 09:04:50.803647 maser_plot-0.3.2/maser/plot/pds/__init__.py
+-rw-r--r--   0        0        0      131 2024-03-15 09:04:50.804105 maser_plot-0.3.2/maser/plot/pds/co/__init__.py
+-rw-r--r--   0        0        0      544 2024-03-15 09:04:50.804287 maser_plot-0.3.2/maser/plot/pds/co/plot.py
+-rw-r--r--   0        0        0     2555 2024-03-15 09:04:50.804485 maser_plot-0.3.2/maser/plot/pds/plot.py
+-rw-r--r--   0        0        0      371 2024-03-15 09:04:50.804649 maser_plot-0.3.2/maser/plot/pds/vg/__init__.py
+-rw-r--r--   0        0        0     4510 2024-03-15 09:04:50.804939 maser_plot-0.3.2/maser/plot/pds/vg/plot.py
+-rw-r--r--   0        0        0      286 2024-03-15 09:04:50.804788 maser_plot-0.3.2/maser/plot/psa/__init__.py
+-rw-r--r--   0        0        0      287 2024-03-15 09:04:50.805078 maser_plot-0.3.2/maser/plot/psa/mex/__init__.py
+-rw-r--r--   0        0        0     1221 2024-03-15 09:04:50.805226 maser_plot-0.3.2/maser/plot/psa/mex/plot.py
+-rw-r--r--   0        0        0      443 2024-03-15 09:04:50.806115 maser_plot-0.3.2/maser/plot/rpw/__init__.py
+-rw-r--r--   0        0        0     3629 2024-03-14 14:17:35.233813 maser_plot-0.3.2/maser/plot/rpw/cross_section.py
+-rw-r--r--   0        0        0     4565 2024-03-14 14:17:35.233993 maser_plot-0.3.2/maser/plot/rpw/lfr.py
+-rw-r--r--   0        0        0     2733 2024-03-15 09:04:50.806557 maser_plot-0.3.2/maser/plot/rpw/plot.py
+-rw-r--r--   0        0        0     5339 2024-03-14 14:17:35.233719 maser_plot-0.3.2/maser/plot/rpw/plot_mean.py
+-rw-r--r--   0        0        0     5518 2024-03-14 14:17:35.234796 maser_plot-0.3.2/maser/plot/rpw/quick_look.py
+-rw-r--r--   0        0        0     1920 2024-04-29 08:34:17.733548 maser_plot-0.3.2/maser/plot/rpw/tnr.py
+-rw-r--r--   0        0        0      440 2024-04-29 08:41:52.604978 maser_plot-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 maser_plot-0.3.2/PKG-INFO
```

### Comparing `maser_plot-0.3.1/README.md` & `maser_plot-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/__init__.py` & `maser_plot-0.3.2/maser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/base/__init__.py` & `maser_plot-0.3.2/maser/plot/base/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/base/base.py` & `maser_plot-0.3.2/maser/plot/base/base.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/base/dataset_filename_regex.json` & `maser_plot-0.3.2/maser/plot/base/dataset_filename_regex.json`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/cdpp/__init__.py` & `maser_plot-0.3.2/maser/plot/cdpp/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/cdpp/stereo/plot.py` & `maser_plot-0.3.2/maser/plot/cdpp/stereo/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/cdpp/wind/plot.py` & `maser_plot-0.3.2/maser/plot/cdpp/wind/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/ecallisto/plot.py` & `maser_plot-0.3.2/maser/plot/ecallisto/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/nancay/__init__.py` & `maser_plot-0.3.2/maser/plot/nancay/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/nancay/nda/plot.py` & `maser_plot-0.3.2/maser/plot/nancay/nda/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/nancay/nenufar/plot.py` & `maser_plot-0.3.2/maser/plot/nancay/nenufar/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/padc/__init__.py` & `maser_plot-0.3.2/maser/plot/padc/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/padc/bepi/sorbet/plot.py` & `maser_plot-0.3.2/maser/plot/padc/bepi/sorbet/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/padc/cassini/plot.py` & `maser_plot-0.3.2/maser/plot/padc/cassini/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/padc/expres/__init__.py` & `maser_plot-0.3.2/maser/plot/padc/expres/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/padc/expres/plot.py` & `maser_plot-0.3.2/maser/plot/padc/expres/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/padc/juno/plot.py` & `maser_plot-0.3.2/maser/plot/padc/juno/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/padc/stereo/plot.py` & `maser_plot-0.3.2/maser/plot/padc/stereo/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/padc/wind/plot.py` & `maser_plot-0.3.2/maser/plot/padc/wind/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/pds/__init__.py` & `maser_plot-0.3.2/maser/plot/pds/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/pds/co/plot.py` & `maser_plot-0.3.2/maser/plot/pds/co/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/pds/plot.py` & `maser_plot-0.3.2/maser/plot/pds/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/pds/vg/plot.py` & `maser_plot-0.3.2/maser/plot/pds/vg/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/psa/mex/plot.py` & `maser_plot-0.3.2/maser/plot/psa/mex/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/rpw/cross_section.py` & `maser_plot-0.3.2/maser/plot/rpw/cross_section.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/rpw/lfr.py` & `maser_plot-0.3.2/maser/plot/rpw/lfr.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/rpw/plot.py` & `maser_plot-0.3.2/maser/plot/rpw/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/rpw/plot_mean.py` & `maser_plot-0.3.2/maser/plot/rpw/plot_mean.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/rpw/quick_look.py` & `maser_plot-0.3.2/maser/plot/rpw/quick_look.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.1/maser/plot/rpw/tnr.py` & `maser_plot-0.3.2/maser/plot/rpw/tnr.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,20 @@
     from matplotlib import colors
     import matplotlib.colorbar as cbar
 
     # create a colorbar axis
     if cbar_ax is None:
         cbar_ax, kw = cbar.make_axes(ax)
 
-    auto = data_wrapper.as_xarray()["VOLTAGE_SPECTRAL_POWER"]
-
-    # keep only V1-V2 sensor
-    v1_v2_auto = auto.where(auto.sensor == sensor, drop=True)
+    auto = data_wrapper.as_xarray()[sensor]
 
     # determine min/max for the colorbar
     # use q5 and q95 for vmin and vmax to avoid outliers
-    positive_v1_v2_auto = v1_v2_auto.where(v1_v2_auto > 0)
-    vmin, vmax = positive_v1_v2_auto.quantile([0.05, 0.95])
+    positive_auto = auto.where(auto > 0)
+    vmin, vmax = positive_auto.quantile([0.05, 0.95])
 
     plot_kwargs = {
         "cmap": "plasma",
         "norm": "log",
         "vmin": vmin,
         "vmax": vmax,
         "cbar_ax": cbar_ax,
@@ -40,32 +37,25 @@
     # create a new norm object to display the colorbar in log scale
     if "norm" in plot_kwargs and plot_kwargs["norm"] == "log":
         plot_kwargs["norm"] = colors.LogNorm()
 
     meshes = []
 
     # group data by band and plot each channel
-    for band, data_array in v1_v2_auto.groupby("band"):
-        if band not in bands:
-            # skip bands not in the list
-            continue
-
-        for channel in data_wrapper.channel_labels:
-            # create a new mesh for each band/channel
-            mesh = data_array.sel(channel=channel).plot.pcolormesh(
+    mesh = auto.plot.pcolormesh(
                 ax=ax,
                 x="time",
                 y="frequency",
                 yscale="log",
                 add_colorbar=True,
                 **plot_kwargs,
             )
 
-            # store the mesh for future use
-            meshes.append(mesh)
+    # store the mesh for future use
+    meshes.append(mesh)
 
     return {
         "ax": ax,
         "cbar_ax": cbar_ax,
         "vmin": vmin,
         "vmax": vmax,
         "meshes": meshes,
```

### Comparing `maser_plot-0.3.1/PKG-INFO` & `maser_plot-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: maser-plot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Maser4py submodule to plot radio data
 License: CeCILL
-Author: Baptiste Cecconi
-Author-email: baptiste.cecconi@obspm.fr
+Author: MASER team
+Author-email: contact.maser@obspm.fr
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

