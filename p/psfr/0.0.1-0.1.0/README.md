# Comparing `tmp/psfr-0.0.1.tar.gz` & `tmp/psfr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psfr-0.0.1.tar", last modified: Wed Aug 10 21:19:54 2022, max compression
+gzip compressed data, was "psfr-0.1.0.tar", last modified: Mon Apr 29 19:15:01 2024, max compression
```

## Comparing `psfr-0.0.1.tar` & `psfr-0.1.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.963456 psfr-0.0.1/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.948742 psfr-0.0.1/.github/
--rw-r--r--   0 sibirrer   (501) staff       (20)      315 2022-07-17 18:42:34.000000 psfr-0.0.1/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.949098 psfr-0.0.1/.github/workflows/
--rw-r--r--   0 sibirrer   (501) staff       (20)     1941 2022-08-10 20:35:14.000000 psfr-0.0.1/.github/workflows/ci_test.yml
--rw-r--r--   0 sibirrer   (501) staff       (20)     1218 2022-07-17 22:10:53.000000 psfr-0.0.1/.gitignore
--rw-r--r--   0 sibirrer   (501) staff       (20)      170 2020-12-28 02:30:21.000000 psfr-0.0.1/.readthedocs.yml
--rw-r--r--   0 sibirrer   (501) staff       (20)      239 2022-08-10 17:39:12.000000 psfr-0.0.1/AUTHORS.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     3143 2022-07-17 18:47:00.000000 psfr-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       81 2022-08-10 20:59:32.000000 psfr-0.0.1/HISTORY.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1582 2022-07-28 16:34:29.000000 psfr-0.0.1/LICENSE
--rw-r--r--   0 sibirrer   (501) staff       (20)      262 2022-07-17 18:42:34.000000 psfr-0.0.1/MANIFEST.in
--rw-r--r--   0 sibirrer   (501) staff       (20)     2122 2022-08-10 21:05:54.000000 psfr-0.0.1/Makefile
--rw-r--r--   0 sibirrer   (501) staff       (20)     4112 2022-08-10 21:19:54.963582 psfr-0.0.1/PKG-INFO
--rw-r--r--   0 sibirrer   (501) staff       (20)     3414 2022-08-10 21:18:44.000000 psfr-0.0.1/README.rst
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.953203 psfr-0.0.1/docs/
--rw-r--r--   0 sibirrer   (501) staff       (20)      605 2022-07-17 18:42:34.000000 psfr-0.0.1/docs/Makefile
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.943740 psfr-0.0.1/docs/_build/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.943801 psfr-0.0.1/docs/_build/html/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.954310 psfr-0.0.1/docs/_build/html/_static/
--rw-r--r--   0 sibirrer   (501) staff       (20)      286 2021-12-07 21:51:58.000000 psfr-0.0.1/docs/_build/html/_static/file.png
--rw-r--r--   0 sibirrer   (501) staff       (20)       90 2021-12-07 21:51:58.000000 psfr-0.0.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 sibirrer   (501) staff       (20)       90 2021-12-07 21:51:58.000000 psfr-0.0.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 sibirrer   (501) staff       (20)   153972 2022-08-10 17:30:24.000000 psfr-0.0.1/docs/_build/html/_static/stacked_psf_animation.gif
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.954819 psfr-0.0.1/docs/_static/
--rw-r--r--   0 sibirrer   (501) staff       (20)   153972 2022-08-10 17:30:24.000000 psfr-0.0.1/docs/_static/stacked_psf_animation.gif
--rw-r--r--   0 sibirrer   (501) staff       (20)       28 2022-07-17 18:42:34.000000 psfr-0.0.1/docs/authors.rst
--rwxr-xr-x   0 sibirrer   (501) staff       (20)     4859 2022-08-10 20:55:46.000000 psfr-0.0.1/docs/conf.py
--rw-r--r--   0 sibirrer   (501) staff       (20)       33 2022-07-17 18:42:34.000000 psfr-0.0.1/docs/contributing.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       28 2022-07-17 18:42:34.000000 psfr-0.0.1/docs/history.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      257 2022-08-10 21:04:01.000000 psfr-0.0.1/docs/index.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1090 2022-07-17 18:42:34.000000 psfr-0.0.1/docs/installation.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      766 2022-07-17 18:42:34.000000 psfr-0.0.1/docs/make.bat
--rw-r--r--   0 sibirrer   (501) staff       (20)       49 2022-08-10 21:13:36.000000 psfr-0.0.1/docs/modules.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      523 2022-08-10 21:13:36.000000 psfr-0.0.1/docs/psfr.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       27 2022-07-17 18:42:34.000000 psfr-0.0.1/docs/readme.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       63 2022-07-17 18:42:34.000000 psfr-0.0.1/docs/usage.rst
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.955432 psfr-0.0.1/notebooks/
--rw-r--r--   0 sibirrer   (501) staff       (20)    13949 2022-08-10 20:29:44.000000 psfr-0.0.1/notebooks/JWST_PSF_reconstruction.ipynb
--rw-r--r--   0 sibirrer   (501) staff       (20)    18443 2022-07-21 21:24:51.000000 psfr-0.0.1/notebooks/testing.ipynb
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.956435 psfr-0.0.1/psfr/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.944425 psfr-0.0.1/psfr/Data/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.960320 psfr-0.0.1/psfr/Data/JWST/
--rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.0.1/psfr/Data/JWST/psf_f090w_star0.fits
--rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.0.1/psfr/Data/JWST/psf_f090w_star1.fits
--rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.0.1/psfr/Data/JWST/psf_f090w_star2.fits
--rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.0.1/psfr/Data/JWST/psf_f090w_star3.fits
--rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.0.1/psfr/Data/JWST/psf_f090w_star4.fits
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.960976 psfr-0.0.1/psfr/Data/JWST_mock/
--rw-r--r--   0 sibirrer   (501) staff       (20)   213120 2022-07-21 19:43:47.000000 psfr-0.0.1/psfr/Data/JWST_mock/psf_f090w_supersample5_crop.fits
--rw-r--r--   0 sibirrer   (501) staff       (20)      122 2022-07-17 18:42:34.000000 psfr-0.0.1/psfr/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1728 2022-07-20 18:14:44.000000 psfr-0.0.1/psfr/mask_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    26339 2022-08-10 21:13:35.000000 psfr-0.0.1/psfr/psfr.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3648 2022-08-10 19:25:57.000000 psfr-0.0.1/psfr/util.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.958488 psfr-0.0.1/psfr.egg-info/
--rw-r--r--   0 sibirrer   (501) staff       (20)     4112 2022-08-10 21:19:54.000000 psfr-0.0.1/psfr.egg-info/PKG-INFO
--rw-r--r--   0 sibirrer   (501) staff       (20)     1244 2022-08-10 21:19:54.000000 psfr-0.0.1/psfr.egg-info/SOURCES.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)        1 2022-08-10 21:19:54.000000 psfr-0.0.1/psfr.egg-info/dependency_links.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)        1 2022-08-10 21:15:22.000000 psfr-0.0.1/psfr.egg-info/not-zip-safe
--rw-r--r--   0 sibirrer   (501) staff       (20)        5 2022-08-10 21:19:54.000000 psfr-0.0.1/psfr.egg-info/top_level.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)       42 2022-08-10 19:26:02.000000 psfr-0.0.1/requirements.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      411 2022-08-10 21:19:54.964170 psfr-0.0.1/setup.cfg
--rw-r--r--   0 sibirrer   (501) staff       (20)     1238 2022-08-10 21:16:40.000000 psfr-0.0.1/setup.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.962508 psfr-0.0.1/tests/
--rw-r--r--   0 sibirrer   (501) staff       (20)       34 2022-07-17 18:42:34.000000 psfr-0.0.1/tests/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2022-08-10 21:19:54.963260 psfr-0.0.1/tests/test_Examples/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2022-07-21 17:57:38.000000 psfr-0.0.1/tests/test_Examples/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1683 2022-07-21 21:23:31.000000 psfr-0.0.1/tests/test_Examples/test_JWST.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3739 2022-07-21 19:43:48.000000 psfr-0.0.1/tests/test_Examples/test_gaussian.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11630 2022-07-28 13:25:50.000000 psfr-0.0.1/tests/test_psfr.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4172 2022-08-10 19:24:25.000000 psfr-0.0.1/tests/test_util.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.995717 psfr-0.1.0/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.975714 psfr-0.1.0/.github/
+-rw-r--r--   0 sibirrer   (501) staff       (20)      315 2022-07-17 18:42:34.000000 psfr-0.1.0/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.975849 psfr-0.1.0/.github/workflows/
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1941 2022-08-10 20:35:14.000000 psfr-0.1.0/.github/workflows/ci_test.yml
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1218 2022-07-17 22:10:53.000000 psfr-0.1.0/.gitignore
+-rw-r--r--   0 sibirrer   (501) staff       (20)      170 2020-12-28 02:30:21.000000 psfr-0.1.0/.readthedocs.yml
+-rw-r--r--   0 sibirrer   (501) staff       (20)      360 2023-01-31 19:39:09.000000 psfr-0.1.0/AUTHORS.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3143 2022-07-17 18:47:00.000000 psfr-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       81 2022-08-10 20:59:32.000000 psfr-0.1.0/HISTORY.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1582 2022-07-28 16:34:29.000000 psfr-0.1.0/LICENSE
+-rw-r--r--   0 sibirrer   (501) staff       (20)      262 2022-07-17 18:42:34.000000 psfr-0.1.0/MANIFEST.in
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2119 2024-04-29 19:09:55.000000 psfr-0.1.0/Makefile
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5560 2024-04-29 19:15:01.995820 psfr-0.1.0/PKG-INFO
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4898 2022-09-14 03:27:00.000000 psfr-0.1.0/README.rst
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.978005 psfr-0.1.0/docs/
+-rw-r--r--   0 sibirrer   (501) staff       (20)      605 2022-07-17 18:42:34.000000 psfr-0.1.0/docs/Makefile
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.973049 psfr-0.1.0/docs/_build/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.973094 psfr-0.1.0/docs/_build/html/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.978818 psfr-0.1.0/docs/_build/html/_static/
+-rw-r--r--   0 sibirrer   (501) staff       (20)      286 2021-12-07 21:51:58.000000 psfr-0.1.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 sibirrer   (501) staff       (20)       90 2021-12-07 21:51:58.000000 psfr-0.1.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sibirrer   (501) staff       (20)       90 2021-12-07 21:51:58.000000 psfr-0.1.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 sibirrer   (501) staff       (20)   153972 2022-08-10 17:30:24.000000 psfr-0.1.0/docs/_build/html/_static/stacked_psf_animation.gif
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.979518 psfr-0.1.0/docs/_static/
+-rw-r--r--   0 sibirrer   (501) staff       (20)   153972 2022-08-10 17:30:24.000000 psfr-0.1.0/docs/_static/stacked_psf_animation.gif
+-rw-r--r--   0 sibirrer   (501) staff       (20)       28 2022-07-17 18:42:34.000000 psfr-0.1.0/docs/authors.rst
+-rwxr-xr-x   0 sibirrer   (501) staff       (20)     4859 2022-08-10 20:55:46.000000 psfr-0.1.0/docs/conf.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)       33 2022-07-17 18:42:34.000000 psfr-0.1.0/docs/contributing.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       28 2022-07-17 18:42:34.000000 psfr-0.1.0/docs/history.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      156 2022-08-15 03:39:40.000000 psfr-0.1.0/docs/index.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      904 2022-08-10 21:31:22.000000 psfr-0.1.0/docs/installation.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      766 2022-07-17 18:42:34.000000 psfr-0.1.0/docs/make.bat
+-rw-r--r--   0 sibirrer   (501) staff       (20)       49 2024-04-29 19:09:57.000000 psfr-0.1.0/docs/modules.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      665 2024-04-29 19:09:57.000000 psfr-0.1.0/docs/psfr.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       27 2022-07-17 18:42:34.000000 psfr-0.1.0/docs/readme.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       63 2022-07-17 18:42:34.000000 psfr-0.1.0/docs/usage.rst
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.982569 psfr-0.1.0/notebooks/
+-rw-r--r--   0 sibirrer   (501) staff       (20)  1465250 2024-04-29 19:11:36.000000 psfr-0.1.0/notebooks/JWST_PSF_reconstruction.ipynb
+-rw-r--r--   0 sibirrer   (501) staff       (20)   978863 2024-04-29 19:11:36.000000 psfr-0.1.0/notebooks/testing.ipynb
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.988340 psfr-0.1.0/psfr/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.973496 psfr-0.1.0/psfr/Data/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.991217 psfr-0.1.0/psfr/Data/JWST/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.1.0/psfr/Data/JWST/psf_f090w_star0.fits
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.1.0/psfr/Data/JWST/psf_f090w_star1.fits
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.1.0/psfr/Data/JWST/psf_f090w_star2.fits
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.1.0/psfr/Data/JWST/psf_f090w_star3.fits
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40320 2022-07-15 04:34:52.000000 psfr-0.1.0/psfr/Data/JWST/psf_f090w_star4.fits
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.991426 psfr-0.1.0/psfr/Data/JWST_mock/
+-rw-r--r--   0 sibirrer   (501) staff       (20)   213120 2022-07-21 19:43:47.000000 psfr-0.1.0/psfr/Data/JWST_mock/psf_f090w_supersample5_crop.fits
+-rw-r--r--   0 sibirrer   (501) staff       (20)      122 2024-04-29 19:04:51.000000 psfr-0.1.0/psfr/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1988 2022-09-15 21:58:23.000000 psfr-0.1.0/psfr/mask_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    33430 2024-04-29 19:11:36.000000 psfr-0.1.0/psfr/psfr.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5198 2023-01-31 19:39:09.000000 psfr-0.1.0/psfr/util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2384 2022-08-12 18:57:22.000000 psfr-0.1.0/psfr/verbose_util.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.989027 psfr-0.1.0/psfr.egg-info/
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5560 2024-04-29 19:15:01.000000 psfr-0.1.0/psfr.egg-info/PKG-INFO
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1316 2024-04-29 19:15:01.000000 psfr-0.1.0/psfr.egg-info/SOURCES.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)        1 2024-04-29 19:15:01.000000 psfr-0.1.0/psfr.egg-info/dependency_links.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)        1 2024-04-29 19:15:01.000000 psfr-0.1.0/psfr.egg-info/not-zip-safe
+-rw-r--r--   0 sibirrer   (501) staff       (20)        5 2024-04-29 19:15:01.000000 psfr-0.1.0/psfr.egg-info/top_level.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)       42 2022-08-10 19:26:02.000000 psfr-0.1.0/requirements.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      411 2024-04-29 19:15:01.996637 psfr-0.1.0/setup.cfg
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1203 2024-04-29 19:11:17.000000 psfr-0.1.0/setup.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.995105 psfr-0.1.0/tests/
+-rw-r--r--   0 sibirrer   (501) staff       (20)       34 2022-07-17 18:42:34.000000 psfr-0.1.0/tests/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2024-04-29 19:15:01.995530 psfr-0.1.0/tests/test_Examples/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2022-07-21 17:57:38.000000 psfr-0.1.0/tests/test_Examples/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1698 2024-04-29 19:11:36.000000 psfr-0.1.0/tests/test_Examples/test_JWST.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3754 2024-04-29 19:11:36.000000 psfr-0.1.0/tests/test_Examples/test_gaussian.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1218 2022-09-15 21:59:30.000000 psfr-0.1.0/tests/test_mask_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19858 2024-04-29 19:11:36.000000 psfr-0.1.0/tests/test_psfr.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4599 2023-01-31 19:39:09.000000 psfr-0.1.0/tests/test_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      592 2022-08-12 17:37:54.000000 psfr-0.1.0/tests/test_verbose_util.py
```

### Comparing `psfr-0.0.1/.github/workflows/ci_test.yml` & `psfr-0.1.0/.github/workflows/ci_test.yml`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/.gitignore` & `psfr-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/CONTRIBUTING.rst` & `psfr-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/LICENSE` & `psfr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/Makefile` & `psfr-0.1.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 docs: ## generate Sphinx HTML documentation, including API docs
 	rm -f docs/psfr.rst
 	rm -f docs/modules.rst
 	sphinx-apidoc -o docs/ psfr
 	MAKE -C docs clean
 	MAKE -C docs html
-	BROWSER docs/_build/html/index.html
+	open docs/_build/html/index.html
 
 
 pypi-upload:
 	python setup.py sdist
 	twine upload --repository-url https://test.pypi.org/legacy/ dist/*
 	twine upload dist/*
```

### Comparing `psfr-0.0.1/PKG-INFO` & `psfr-0.1.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,26 @@
-Metadata-Version: 2.1
-Name: psfr
-Version: 0.0.1
-Summary: Telescope Images Point Spread Function Reconstruction
-Home-page: https://github.com/sibirrer/psfr
-Author: Simon Birrer
-Author-email: sibirrer@gmail.com
-License: BSD 3-Clause
-Keywords: psfr
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-
 ===========================================
 PSFr - Point Spread Function reconstruction
 ===========================================
 
-.. image:: https://github.com/sibirrer/psfr/workflows/Tests/badge.svg
+|PyPI| |CI| |Docs| |Coveralls|
+
+.. |CI| image:: https://github.com/sibirrer/psfr/workflows/Tests/badge.svg
     :target: https://github.com/sibirrer/psfr/actions
 
-.. image:: https://readthedocs.org/projects/psfr/badge/?version=latest
+.. |Docs| image:: https://readthedocs.org/projects/psfr/badge/?version=latest
         :target: http://psfr.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-.. image:: https://coveralls.io/repos/github/sibirrer/psfr/badge.svg?branch=main
+.. |Coveralls| image:: https://coveralls.io/repos/github/sibirrer/psfr/badge.svg?branch=main
     :target: https://coveralls.io/github/sibirrer/psfr?branch=main
 
+.. |PyPI| image:: https://img.shields.io/pypi/v/psfr?label=PyPI&logo=pypi
+    :target: https://pypi.python.org/pypi/psfr
+
 .. image:: https://github.com/sibirrer/psfr/blob/main/docs/_static/stacked_psf_animation.gif
 
 Point Spread Function reconstruction for astronomical
 ground- and space-based imaging data.
 
 
 Example
@@ -61,47 +47,64 @@
 --------
 
 * Iterative PSF reconstruction given cutouts of individual stars or other point-like sources.
 * Sub-pixel astrometric shifts calculated and accounted for while performing the PSF reconstruction.
 * PSF reconstruction available in super-sampling resolution.
 * Masking pixels, saturation levels and other options to deal with artifacts in the data.
 
+Algorithm
+---------
+The algorithm to iteratively propose a (optionally oversampled) PSF from a set of star cutouts goes as follow:
+
+
+(1) Stack all the stars for an initial guess of the PSF on the centroid pixel (ignoring sub-pixel offsets)
+
+(2) Fit the subpixel centroid with the PSF model estimate
+
+(3) Shift PSF with sub-pixel interpolation to the sub-pixel position of individual stars
+
+(4) Retrieve residuals of the shifted PSF model relative to the data of the cutouts
+
+(5) Apply an inverse sub-pixel shift of the residuals to be focused on the center of the pixel
+
+(6) Based on teh inverse shifted residuals of a set of fixed stars, propose a correction to the previous PSF model
+
+(7) Repeat step (3) - (6) multiple times with the option to repeat step (2)
+
+
+Details and options for the different steps can be found in the documentation and the source code.
+
+
 Used by
 -------
 PSFr is in use with James Webb Space Telescope imaging data (i.e., `Santini et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220711379S/abstract>`_,
 `Merlin et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220711701M/abstract>`_,
-`Yang et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220713101Y/abstract>`_).
+`Yang et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220713101Y/abstract>`_,
+`Ding et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220903359D/abstract>`_).
 The iterative PSF reconstruction procedure was originally developed and used for analyzing strongly lensed quasars
 (i.e., `Birrer et al. 2019 <https://ui.adsabs.harvard.edu/#abs/2018arXiv180901274B/abstract>`_
 , `Shajib et al. 2018 <https://ui.adsabs.harvard.edu/abs/2019MNRAS.483.5649S>`_ ,
 `Shajib et al. 2019 <https://ui.adsabs.harvard.edu/abs/2019arXiv191006306S/abstract>`_ ,
 `Schmidt et al. 2022 <https://arxiv.org/abs/2206.04696>`_).
 
 
 Other resources
 ---------------
 
 We also refer to the astropy core package
 `photutils <https://photutils.readthedocs.io/en/stable/index.html>`_
 and in particular to the empirical PSF module
 `ePSF <https://photutils.readthedocs.io/en/stable/epsf.html#build-epsf>`_ .
+PSF reconstructions are e.g. reported by
+`Anderson and King (2000; PASP 112, 1360) <https://ui.adsabs.harvard.edu/abs/2000PASP..112.1360A/abstract>`_
+and
+`Anderson (2016), ISR WFC3 2016-12 <https://www.stsci.edu/files/live/sites/www/files/home/hst/instrumentation/wfc3/documentation/instrument-science-reports-isrs/_documents/2016/WFC3-2016-12.pdf>`_.
+
 
 
 Credits
 -------
 
 The software is an off-spring of the iterative PSF reconstruction scheme of `lenstronomy <https://github.com/lenstronomy/lenstronomy>`_, in particular its `psf_fitting.py <https://github.com/lenstronomy/lenstronomy/blob/v1.10.4/lenstronomy/Workflow/psf_fitting.py>`_ functionalities.
 
 If you make use of this software, please cite: 'This code is using PSFr (Birrer et al. in prep) utilizing features of
 lenstronomy (`Birrer et al. 2021 <https://joss.theoj.org/papers/10.21105/joss.03283>`_)'.
-
-
-=======
-History
-=======
-
-0.0.1 (2022-08-10)
-------------------
-
-* First release.
-
-
```

### Comparing `psfr-0.0.1/docs/Makefile` & `psfr-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/docs/_build/html/_static/stacked_psf_animation.gif` & `psfr-0.1.0/docs/_build/html/_static/stacked_psf_animation.gif`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/docs/_static/stacked_psf_animation.gif` & `psfr-0.1.0/docs/_static/stacked_psf_animation.gif`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/docs/conf.py` & `psfr-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/docs/make.bat` & `psfr-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/docs/psfr.rst` & `psfr-0.1.0/docs/psfr.rst`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 ----------------
 
 .. automodule:: psfr.util
    :members:
    :undoc-members:
    :show-inheritance:
 
+psfr.verbose\_util module
+-------------------------
+
+.. automodule:: psfr.verbose_util
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Module contents
 ---------------
 
 .. automodule:: psfr
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `psfr-0.0.1/psfr/Data/JWST/psf_f090w_star0.fits` & `psfr-0.1.0/psfr/Data/JWST/psf_f090w_star0.fits`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/psfr/Data/JWST/psf_f090w_star1.fits` & `psfr-0.1.0/psfr/Data/JWST/psf_f090w_star1.fits`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/psfr/Data/JWST/psf_f090w_star2.fits` & `psfr-0.1.0/psfr/Data/JWST/psf_f090w_star2.fits`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/psfr/Data/JWST/psf_f090w_star3.fits` & `psfr-0.1.0/psfr/Data/JWST/psf_f090w_star3.fits`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/psfr/Data/JWST/psf_f090w_star4.fits` & `psfr-0.1.0/psfr/Data/JWST/psf_f090w_star4.fits`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/psfr/Data/JWST_mock/psf_f090w_supersample5_crop.fits` & `psfr-0.1.0/psfr/Data/JWST_mock/psf_f090w_supersample5_crop.fits`

 * *Files identical despite different names*

### Comparing `psfr-0.0.1/psfr/mask_util.py` & `psfr-0.1.0/psfr/mask_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,21 @@
     saturation_limit: None, float or list of floats with same length as star_list
         saturation limit of the pixels. Pixel values at and above this value will be masked
 
     Returns
     -------
     mask_list : list of 2d boolean or integer arrays, same shape as star_list
         an updated list of masks for each individual star taking into account saturation
+    use_mask : boolean
+        if True, indicates that the masks need to be used, otherwise calculations will ignore mask for speed-ups
     """
+    if saturation_limit is None and mask_list is None:
+        use_mask = False
+    else:
+        use_mask = True
     n_star = len(star_list)
     # define saturation masks
     if saturation_limit is not None:
         n_sat = len(np.atleast_1d(saturation_limit))
         if n_sat == 1:
             saturation_limit = [saturation_limit] * n_star
         else:
@@ -35,8 +41,8 @@
         for i, star in enumerate(star_list):
             mask = np.ones_like(star)
             mask_list.append(mask)
     # add threshold for saturation in mask
     if saturation_limit is not None:
         for i, mask in enumerate(mask_list):
             mask[star_list[i] > saturation_limit[i]] = 0
-    return mask_list
+    return mask_list, use_mask
```

### Comparing `psfr-0.0.1/psfr/psfr.py` & `psfr-0.1.0/psfr/psfr.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,114 +1,131 @@
 """Main module."""
 import numpy as np
 import scipy.optimize
-from scipy.ndimage import interpolation
+from scipy import ndimage
 import matplotlib.pylab as plt
 import matplotlib.animation as animation
 from lenstronomy.Util import util, kernel_util, image_util
-from psfr.util import regular2oversampled, oversampled2regular
+from psfr.util import regular2oversampled, oversampled2regular, median_with_mask
 from psfr import mask_util
+from psfr import verbose_util
 
-def stack_psf(star_list, oversampling=1, mask_list=None, saturation_limit=None, num_iteration=5, n_recenter=10,
-              verbose=False, kwargs_one_step=None, psf_initial_guess=None, kwargs_psf_stacking=None, **kwargs_animate):
+from lenstronomy.Sampling.Samplers.pso import ParticleSwarmOptimizer
+
+
+def stack_psf(star_list, oversampling=1, mask_list=None, error_map_list=None, saturation_limit=None, num_iteration=20,
+              n_recenter=5,
+              verbose=False, kwargs_one_step=None, psf_initial_guess=None, kwargs_psf_stacking=None,
+              centroid_optimizer='Nelder-Mead', **kwargs_animate):
     """
     Parameters
     ----------
     star_list: list of numpy arrays (2D) of stars. Odd square axis shape.
         Cutout stars from images with approximately centered on the center pixel. All stars need the same cutout size.
     oversampling : integer >=1
         higher-resolution PSF reconstruction and return
     mask_list : list of 2d boolean or integer arrays, same shape as star_list
         list of masks for each individual star's pixel to be included in the fit or not.
         0 means excluded, 1 means included
+    error_map_list : None, or list of 2d numpy array, same size as data
+        Variance in the uncorrelated uncertainties in the data for individual pixels.
+        If not set, assumes equal variances for all pixels.
     saturation_limit: float or list of floats of length of star_list
         pixel values above this threshold will not be considered in the reconstruction.
     num_iteration : integer >= 1
         number of iterative corrections applied on the PSF based on previous guess
     n_recenter: integer
         Every n_recenter iterations of the updated PSF, a re-centering of the centroids are performed with the updated
         PSF guess.
     verbose : boolean
         If True, provides plots of updated PSF during the iterative process
     kwargs_one_step : keyword arguments to be passed to one_step_psf_estimate() method
         See one_step_psf_estimate() method for options
     psf_initial_guess : None or 2d numpy array with square odd axis
         Initial guess PSF on oversampled scale. If not provided, estimates an initial guess with the stacked stars.
     kwargs_animate : keyword arguments for animation settings
-        Settings to display animation of interative process of psf reconstuction. The argument is organized as:
+        Settings to display animation of interactive process of psf reconstruction. The argument is organized as:
             {animate: bool, output_dir: str (directory to save animation in),
             duration: int (length of animation in milliseconds)}
     kwargs_psf_stacking: keyword argument list of arguments going into combine_psf()
-        stacking_option : option of stacking, 'mean' or 'median'
+        stacking_option : option of stacking, 'mean',  'median' or 'median_weight'
         symmetry: integer, imposed symmetry of PSF estimate
+    centroid_optimizer: 'Nelder-Mead' or 'PSO'
+        option for the optimizing algorithm used to find the center of each PSF in data.
+
 
     Returns
     -------
     psf_guess : 2d numpy array with square odd axis
         best guess PSF in the oversampled resolution
     mask_list : list of 2d boolean or integer arrays, same shape as star_list
         list of masks for each individual star's pixel to be included in the fit or not.
         0 means excluded, 1 means included.
         This list is updated with all the criteria applied on the fitting and might deviate from the input mask_list.
     center_list : list of 2d floats
         list of astrometric centers relative to the center pixel of the individual stars
 
     """
     # update the mask according to settings
-    mask_list = mask_util.mask_configuration(star_list, mask_list=mask_list, saturation_limit=saturation_limit)
+    mask_list, use_mask = mask_util.mask_configuration(star_list, mask_list=mask_list,
+                                                       saturation_limit=saturation_limit)
     if kwargs_one_step is None:
         kwargs_one_step = {}
     if kwargs_psf_stacking is None:
         kwargs_psf_stacking = {}
+    if error_map_list is None:
+        error_map_list = [np.ones_like(star_list[0])] * len(star_list)
 
     # update default options for animations
     animation_options = {'animate': False, 'output_dir': 'stacked_psf_animation.gif', 'duration': 5000}
     animation_options.update(kwargs_animate)
     # define base stacking without shift offset shifts
     # stacking with mask weight
-    star_stack_base = base_stacking(star_list, mask_list)
+    star_stack_base = base_stacking(star_list, mask_list, symmetry=4)
+    star_stack_base[star_stack_base < 0] = 0
     star_stack_base /= np.sum(star_stack_base)
 
     # estimate center offsets based on base stacking PSF estimate
     center_list = []
     for i, star in enumerate(star_list):
-        x_c, y_c = centroid_fit(star, star_stack_base, mask_list[i])
+        x_c, y_c = centroid_fit(star, star_stack_base, mask_list[i], optimizer_type=centroid_optimizer,
+                                variance=error_map_list[i])
         center_list.append([x_c, y_c])
 
-    # re-size initial guess to oversampled resolution
     if psf_initial_guess is None:
         psf_guess = regular2oversampled(star_stack_base, oversampling=oversampling)
     else:
         psf_guess = psf_initial_guess
-    if verbose:
-        f, axes = plt.subplots(1, 2, figsize=(4 * 2, 4))
 
-        ax = axes[0]
-        ax.imshow(np.log10(star_stack_base), origin='lower')
-        ax.set_title('star_stack_base')
-        plt.show()
-        ax = axes[1]
+    if verbose:
+        f, axes = plt.subplots(1, 1, figsize=(4 * 2, 4))
+        ax = axes
         ax.imshow(np.log10(psf_guess), origin='lower')
         ax.set_title('input first guess')
         plt.show()
 
     # simultaneous iterative correction of PSF starting with base stacking in oversampled resolution
     images_to_animate = []
+    if use_mask:
+        mask_list_one_step = mask_list
+    else:
+        mask_list_one_step = None
     for j in range(num_iteration):
-        psf_guess = one_step_psf_estimate(star_list, psf_guess, center_list, mask_list,
-                                          oversampling=oversampling, **kwargs_psf_stacking, **kwargs_one_step)
+        psf_guess, amplitude_list = one_step_psf_estimate(star_list, psf_guess, center_list, mask_list_one_step,
+                                          error_map_list=error_map_list, oversampling=oversampling,
+                                          **kwargs_psf_stacking, **kwargs_one_step)
         if j % n_recenter == 0 and j != 0:
             center_list = []
             for i, star in enumerate(star_list):
-                x_c, y_c = centroid_fit(star, psf_guess, mask_list[i], oversampling=oversampling)
+                x_c, y_c = centroid_fit(star, psf_guess, mask_list[i], oversampling=oversampling,
+                                        variance=error_map_list[i], optimizer_type=centroid_optimizer)
                 center_list.append([x_c, y_c])
         if animation_options['animate']:
             images_to_animate.append(psf_guess)
         if verbose:
-            # TODO: make a movie out of this
             plt.imshow(np.log(psf_guess), vmin=-5, vmax=-1)
             plt.title('iteration %s' % j)
             plt.colorbar()
             plt.show()
 
     # function that is called to update the image for the animation
     def _updatefig(i):
@@ -116,27 +133,27 @@
         return [img]
 
     if animation_options['animate']:
         global anim
         fig = plt.figure()
         img = plt.imshow(np.log10(images_to_animate[0]))
         cmap = plt.get_cmap('viridis')
-        cmap.set_bad(color = 'k', alpha = 1.)
+        cmap.set_bad(color='k', alpha=1.)
         cmap.set_under('k')
         # animate and display iterative psf reconstuction
-        anim = animation.FuncAnimation(fig, _updatefig, frames=len(images_to_animate), 
-                              interval=int(animation_options['duration']/len(images_to_animate)), blit=True)
+        anim = animation.FuncAnimation(fig, _updatefig, frames=len(images_to_animate),
+                                       interval=int(animation_options['duration'] / len(images_to_animate)), blit=True)
         anim.save(animation_options['output_dir'])
         plt.close()
 
-    return psf_guess, center_list, mask_list
+    return psf_guess, center_list, mask_list, amplitude_list
 
 
-def one_step_psf_estimate(star_list, psf_guess, center_list, mask_list, error_map_list=None, oversampling=1,
-                          step_factor=0.2, oversampled_residual_deshifting=False, deshift_order=1, verbose=False,
+def one_step_psf_estimate(star_list, psf_guess, center_list, mask_list=None, error_map_list=None, oversampling=1,
+                          step_factor=0.2, oversampled_residual_deshifting=True, deshift_order=1, verbose=False,
                           **kwargs_psf_stacking):
     """
 
     Parameters
     ----------
     star_list: list of numpy arrays (2D) of stars. Odd square axis shape.
         Cutout stars from images with approximately centered on the center pixel. All stars need the same cutout size.
@@ -159,114 +176,205 @@
     deshift_order : integer >= 0
         polynomial order of interpolation of the de-shifting of the residuals to the center to be interpreted as
         desired corrections for a given star
     step_factor : float or integer in (0, 1]
         weight of updated estimate based on new and old estimate;
         psf_update = step_factor * psf_new + (1 - step_factor) * psf_old
     kwargs_psf_stacking: keyword argument list of arguments going into combine_psf()
-        stacking_option : option of stacking, 'mean' or 'median'
+        stacking_option : option of stacking, 'mean',  'median' or 'median_weight'
         symmetry: integer, imposed symmetry of PSF estimate
     verbose : boolean
         If True, provides plots of intermediate products walking through one iteration process for each individual star
     """
+    # creating oversampled mask
     if mask_list is None:
-        mask_list = []
+        mask_list_ = []
         for i, star in enumerate(star_list):
-            mask_list.append(np.ones_like(star))
+            mask_list_.append(np.ones_like(star))
+        mask_list_oversampled = None
+    else:
+        mask_list_ = mask_list
+        mask_list_oversampled = []
+        for mask in mask_list_:
+            mask_ = regular2oversampled(mask, oversampling=oversampling)
+            mask_list_oversampled.append(mask_)
     if error_map_list is None:
-        error_map_list = [None] * len(star_list)
+        error_map_list = [np.ones_like(star_list[0]) * 10.0**(-50)] * len(star_list)  # * 10.0**(-50)
+    error_map_list_psf = []  # list of variances in the centroid position and super-sampled PSF estimate
     psf_list_new = []
-    weight_list = []
+    amplitude_list = []
     for i, star in enumerate(star_list):
         center = center_list[i]
         # shift PSF guess to estimated position of star
-
-        # shift PSF to position pre-determined to be the center of the point source, and degrate it to the image
+        # shift PSF to position pre-determined to be the center of the point source, and degrade it to the image
         psf_shifted = shift_psf(psf_guess, oversampling, shift=center_list[i], degrade=False, n_pix_star=len(star))
 
         # make data degraded version
         psf_shifted_data = oversampled2regular(psf_shifted, oversampling=oversampling)
         # make sure size is the same as the data and normalized to sum = 1
         psf_shifted_data = kernel_util.cut_psf(psf_shifted_data, len(star))
         # linear inversion in 1d
-        amp = _linear_amplitude(star, psf_shifted_data, variance=error_map_list[i], mask=mask_list[i])
-        weight_list.append(amp)
+        amp = _linear_amplitude(star, psf_shifted_data, variance=error_map_list[i], mask=mask_list_[i])
+        amplitude_list.append(amp)
+
+        # shift error_map_list to PSF position
+        error_map_shifted = ndimage.shift(error_map_list[i], shift=[-center[1], -center[0]], order=deshift_order,
+                                          mode='constant', cval=0)
+        error_map_shifted_oversampled = regular2oversampled(error_map_shifted, oversampling=oversampling)
+        error_map_list_psf.append(error_map_shifted_oversampled)
 
         # compute residuals on data
         if oversampled_residual_deshifting:  # directly in oversampled space
             star_super = regular2oversampled(star, oversampling=oversampling)  # TODO: needs only be calculated once!
-            mask_super = regular2oversampled(mask_list[i], oversampling=oversampling)
+            mask_super = regular2oversampled(mask_list_[i], oversampling=oversampling)
             # attention the routine is flux conserving and need to be changed for the mask,
             # in case of interpolation we block everything that has a tenth of a mask in there
-            mask_super[mask_super < 1./oversampling**2 / 10] = 0
-            mask_super[mask_super >= 1./oversampling**2 / 10] = 1
+            mask_super[mask_super < 1. / oversampling ** 2 / 10] = 0
+            mask_super[mask_super >= 1. / oversampling ** 2 / 10] = 1
             residuals = (star_super - amp * psf_shifted) * mask_super
             residuals /= amp
 
             # shift residuals back on higher res grid
             # inverse shift residuals
             shift_x = center[0] * oversampling
             shift_y = center[1] * oversampling
-            residuals_shifted = interpolation.shift(residuals, shift=[-shift_y, -shift_x], order=deshift_order)
+            residuals_shifted = ndimage.shift(residuals, shift=[-shift_y, -shift_x], order=deshift_order)
 
         else:  # in data space and then being oversampled
-            residuals = (star - amp * psf_shifted_data) * mask_list[i]
+            residuals = (star - amp * psf_shifted_data) * mask_list_[i]
             # re-normalize residuals
             residuals /= amp  # divide by amplitude of point source
             # high-res version of residuals
             residuals = residuals.repeat(oversampling, axis=0).repeat(oversampling, axis=1) / oversampling ** 2
             # shift residuals back on higher res grid
             # inverse shift residuals
             shift_x = center[0] * oversampling
             shift_y = center[1] * oversampling
 
             if oversampling % 2 == 1:  # for odd number super-sampling
-                residuals_shifted = interpolation.shift(residuals, shift=[-shift_y, -shift_x], order=deshift_order)
+                residuals_shifted = ndimage.shift(residuals, shift=[-shift_y, -shift_x], order=deshift_order)
 
             else:  # for even number super-sampling
                 # for even number super-sampling half a super-sampled pixel offset needs to be performed
                 # TODO: move them in all four directions (not only two)
-                residuals_shifted1 = interpolation.shift(residuals, shift=[-shift_y - 0.5, -shift_x - 0.5],
-                                                         order=deshift_order)
+                residuals_shifted1 = ndimage.shift(residuals, shift=[-shift_y - 0.5, -shift_x - 0.5],
+                                                   order=deshift_order)
                 # and the last column and row need to be removed
                 residuals_shifted1 = residuals_shifted1[:-1, :-1]
 
-                residuals_shifted2 = interpolation.shift(residuals, shift=[-shift_y + 0.5, -shift_x + 0.5],
-                                                         order=deshift_order)
+                residuals_shifted2 = ndimage.shift(residuals, shift=[-shift_y + 0.5, -shift_x + 0.5],
+                                                   order=deshift_order)
                 # and the last column and row need to be removed
                 residuals_shifted2 = residuals_shifted2[1:, 1:]
                 residuals_shifted = (residuals_shifted1 + residuals_shifted2) / 2
 
         # re-size shift residuals
         psf_size = len(psf_guess)
         residuals_shifted = image_util.cut_edges(residuals_shifted, psf_size)
         # normalize residuals
-        correction = residuals_shifted - np.mean(residuals_shifted)
+        # remove noise from corrections
+        # TODO: normalization correction
+        # TODO: make sure without error_map that no correction is performed
+        correction = residuals_shifted  # - np.sign(residuals_shifted) * np.minimum(np.sqrt(error_map_shifted_oversampled)/amp, np.abs(residuals_shifted)) # - np.mean(residuals_shifted)
         psf_new = psf_guess + correction
-        psf_new[psf_new < 0] = 0
-        psf_new /= np.sum(psf_new)
+        # TODO: for negative pixels, apply an average correction with its neighboring pixels
+        # psf_new[psf_new < 0] = 0
+        # re-normalization can bias the PSF for low S/N ratios
+        # psf_new /= np.sum(psf_new)
         if verbose:
-            _verbose_one_step(star, psf_shifted, psf_shifted_data, residuals, residuals_shifted, correction, psf_new)
+            fig = verbose_util.verbose_one_step(star, psf_shifted, psf_shifted_data, residuals, residuals_shifted,
+                                                correction, psf_new)
+            fig.show()
         psf_list_new.append(psf_new)
 
     # stack all residuals and update the psf guess
-    # TODO: make combine_psf remember the masks and relative brightness in the weighting scheme (for later)
     psf_stacking_options = {'stacking_option': 'median', 'symmetry': 1}
     psf_stacking_options.update(kwargs_psf_stacking)
-    weight_list = np.array(weight_list)
-    weight_list[weight_list < 0] = 0
-    # the weights are supposed to be Poisson noise dominated, which scales as the square root of the brightness
-    weights_psf_combined = np.sqrt(weight_list)
-    kernel_new = combine_psf(psf_list_new, psf_guess, factor=step_factor, mask_list=mask_list,
-                             weight_list=weights_psf_combined, **psf_stacking_options)
+    amplitude_list = np.array(amplitude_list)
+    amplitude_list[amplitude_list < 0] = 0
+
+    # TODO: None as input for mask_list if mask are irrelevant
+    kernel_new = combine_psf(psf_list_new, psf_guess, factor=step_factor, mask_list=mask_list_oversampled,
+                             amplitude_list=amplitude_list, error_map_list=error_map_list_psf,
+                             **psf_stacking_options)
     kernel_new = kernel_util.cut_psf(kernel_new, psf_size=len(psf_guess))
-    return kernel_new
+    return kernel_new, amplitude_list
+
+
+def psf_error_map(star_list, psf_kernel, center_list, mask_list=None, error_map_list=None, oversampling=1):
+    """
+    computes the excess variance in the normalized residuals.
+    This quantity can be interpreted as a linearly scaled variance term proportional to the flux of the PSF
+    <point source variance>(i, j) = error_map(i, j) * <integrated point source flux>
+
+    Parameters
+    ----------
+    star_list: list of numpy arrays (2D) of stars. Odd square axis shape.
+        Cutout stars from images with approximately centered on the center pixel. All stars need the same cutout size.
+    psf_kernel : 2d numpy array with square odd axis normalized to sum = 1
+        PSF model in the oversampled resolution prior to this iteration step
+    center_list : list of 2d floats
+        list of astrometric centers relative to the center pixel of the individual stars
+    mask_list : list of 2d boolean or integer arrays, same shape as star_list
+        list of masks for each individual star's pixel to be included in the fit or not.
+        0 means excluded, 1 means included
+    oversampling : integer >=1
+        higher-resolution PSF reconstruction and return
+    error_map_list : None, or list of 2d numpy array, same size as data
+        Variance in the uncorrelated uncertainties in the data for individual pixels.
+        If not set, assumes equal variances for all pixels.
+
+    Returns
+    -------
+    psf_error_map : 2d numpy array of the size of the pixel grid
+        variance in the normalized PSF such that
+        <point source variance>(i, j) = error_map(i, j) * <integrated point source flux>
 
 
-def shift_psf(psf_center, oversampling, shift, degrade=True, n_pix_star=None):
+    """
+    # creating oversampled mask
+    if mask_list is None:
+        mask_list_ = []
+        for i, star in enumerate(star_list):
+            mask_list_.append(np.ones_like(star))
+    else:
+        mask_list_ = mask_list
+    if error_map_list is None:
+        error_map_list = [None] * len(star_list)
+    norm_residual_list = np.zeros((len(star_list), len(star_list[0]), len(star_list[0])))
+
+    for i, star in enumerate(star_list):
+        center = center_list[i]
+        # shift PSF guess to estimated position of star
+        # shift PSF to position pre-determined to be the center of the point source, and degrade it to the image
+        psf_shifted = shift_psf(psf_kernel, oversampling, shift=center, degrade=False, n_pix_star=len(star))
+
+        # make data degraded version
+        psf_shifted_data = oversampled2regular(psf_shifted, oversampling=oversampling)
+        # make sure size is the same as the data and normalized to sum = 1
+        psf_shifted_data = kernel_util.cut_psf(psf_shifted_data, len(star))
+        # linear inversion in 1d
+        amp = _linear_amplitude(star, psf_shifted_data, variance=error_map_list[i], mask=mask_list_[i])
+        residuals = np.abs(star - amp * psf_shifted_data) * mask_list_[i]
+        # subtract expected noise level
+        if error_map_list[i] is not None:
+            residuals -= np.sqrt(error_map_list[i])
+        # make sure absolute residuals are none-negative
+        residuals[residuals < 0] = 0
+        # estimate relative error per star
+        residuals /= amp
+        norm_residual_list[i, :, :] = residuals ** 2
+    error_map_psf = median_with_mask(norm_residual_list, mask_list_)
+    # error_map_psf[psf_kernel > 0] /= psf_kernel[psf_kernel > 0] ** 2
+    error_map_psf = np.nan_to_num(error_map_psf)
+    error_map_psf[error_map_psf > 1] = 1  # cap on error to be the same
+    return error_map_psf
+
+
+def shift_psf(psf_center, oversampling, shift, degrade=True, n_pix_star=None, order=1):
     """
     shift PSF to the star position. Optionally degrades to the image resolution afterwards
 
     Parameters
     ----------
     psf_center : 2d numpy array with odd square length
         Centered PSF in the oversampling space of the input
@@ -274,61 +382,97 @@
         oversampling factor per axis of the psf_center relative to the data and coordinate shift
     shift : [x, y], 2d floats
         off-center shift in the units of the data
     degrade : boolean
         if True degrades the shifted PSF to the data resolution and cuts the resulting size to n_pix_star
     n_pix_star : odd integer
         size per axis of the data, used when degrading the shifted {SF
+    order : integer >=0
+        polynomial order of the ndimage.shift interpolation
 
     Returns
     -------
     psf_shifted : 2d numpy array, odd axis number
         shifted PSF, optionally degraded to the data resolution
 
     """
     shift_x = shift[0] * oversampling
     shift_y = shift[1] * oversampling
     # shift psf
     # TODO: what is optimal interpolation in the shift, or doing it in Fourier space instead?
     # Partial answer: interpolation in order=1 is better than order=0 (order=2 is even better for Gaussian PSF's)
-    psf_shifted = interpolation.shift(psf_center, shift=[shift_y, shift_x], order=2)
+    psf_shifted = ndimage.shift(psf_center, shift=[shift_y, shift_x], order=order)
 
     # resize to pixel scale (making sure the grid definition with the center in the central pixel is preserved)
     if degrade is True:
         psf_shifted = oversampled2regular(psf_shifted, oversampling=oversampling)
         psf_shifted = image_util.cut_edges(psf_shifted, n_pix_star)
         # psf_shifted = kernel_util.cut_psf(psf_shifted, n_pix_star)
     return psf_shifted
 
 
-def base_stacking(star_list, mask_list):
+def luminosity_centring(star):
+    """
+    computes luminosity center and shifts star such that the luminosity is centered at the central pixel
+
+    Parameters
+    ----------
+    star : 2d numpy array with square odd number
+        cutout of a star
+
+    Returns
+    -------
+    star_shift : luminosity centered star
+    """
+    x_grid, y_grid = util.make_grid(numPix=len(star), deltapix=1, left_lower=False)
+    x_grid, y_grid = util.array2image(x_grid), util.array2image(y_grid)
+    x_c, y_c = np.sum(star * x_grid) / np.sum(star), np.sum(star * y_grid) / np.sum(star)
+    # c_ = (len(star) - 1) / 2
+    # x_s, y_s = 2 * c_ - y_c, 2 * c_ - x_c
+    star_shift = shift_psf(star, oversampling=1, shift=[-x_c, -y_c], degrade=False, n_pix_star=len(star))
+    return star_shift
+
+
+def base_stacking(star_list, mask_list, symmetry=1):
     """
     Basic stacking of stars in luminosity-weighted and mask-excluded regime.
     The method ignores sub-pixel off-centering of individual stars nor does it provide an oversampled solution.
     This method is intended as a baseline comparison and as an initial guess version for the full PSF-r features.
 
     Parameters
     ----------
     star_list : list of 2d numpy arrays
         list of cutout stars (to be included in the fitting)
     mask_list : list of 2d boolean or integer arrays, same shape as star_list
         list of masks for each individual star's pixel to be included in the fit or not.
         0 means excluded, 1 means included
+    symmetry: integer >= 1
+        imposed symmetry of PSF estimate
 
     Returns
     -------
     star_stack_base : 2d numpy array of size of the stars in star_list
         luminosity weighted and mask-excluded stacked stars
     """
     star_stack_base = np.zeros_like(star_list[0])
     weight_map = np.zeros_like(star_list[0])
+    angle = 360. / symmetry
     for i, star in enumerate(star_list):
-        star_stack_base += star * mask_list[i]
-        weight_map += mask_list[i] * np.sum(star)
+        for k in range(symmetry):
+            star_shift = luminosity_centring(star)
+            star_rotated = image_util.rotateImage(star_shift, angle * k)
+            mask_rotated = image_util.rotateImage(mask_list[i], angle * k)
+            star_stack_base += star_rotated * mask_rotated
+            weight_map += mask_rotated * np.sum(star)
+
+    # code can't handle situations where there is never a non-zero pixel
+    weight_map[weight_map == 0] = 1e-12
+
     star_stack_base = star_stack_base / weight_map
+
     return star_stack_base
 
 
 def _linear_amplitude(data, model, variance=None, mask=None):
     """
     computes linear least square amplitude to minimize
     min[(data - amp * model)^2 / variance]
@@ -353,29 +497,31 @@
     """
     y = util.image2array(data)
     x = util.image2array(model)
     if mask is not None:
         mask_ = util.image2array(mask)
         x = x[mask_ == 1]
         y = y[mask_ == 1]
+    else:
+        mask_ = None
 
     if variance is None:
         w = 1  # we simply give equal weight to all data points
     else:
         w = util.image2array(1. / variance)
-        if mask is not None:
-            w = w[mask == 1]
+        if mask_ is not None:  # mask is not None:
+            w = w[mask_ == 1]
     wsum = np.sum(w)
     xw = np.sum(w * x) / wsum
     yw = np.sum(w * y) / wsum
     amp = np.sum(w * (x - xw) * (y - yw)) / np.sum(w * (x - xw) ** 2)
     return amp
 
 
-def centroid_fit(data, model, mask=None, variance=None, oversampling=1):
+def centroid_fit(data, model, mask=None, variance=None, oversampling=1, optimizer_type='Nelder-Mead'):
     """
     fit the centroid of the model to the image by shifting and scaling the model to best match the data
     This is done in a non-linear minimizer in the positions (x, y) and linear amplitude minimization on the fly.
     The model is interpolated to match the data. The starting point of the model is to be aligned with the image.
 
     Parameters
     ----------
@@ -386,180 +532,162 @@
     mask : None, or 2d integer or boolean array, same size as data
         Masking pixels not to be considered in fitting the linear amplitude;
         zeros are ignored, ones are taken into account. None as input takes all pixels into account (default)
     variance : None, or 2d numpy array, same size as data
         Variance in the uncorrelated uncertainties in the data for individual pixels
     oversampling : integer >= 1
         oversampling factor per axis of the model relative to the data and coordinate shift
+    optimizer_type: string
+        'Nelder-Mead' or 'PSO'
 
     Returns
     -------
     center_shift : 2d array (delta_x, delta_y)
         required shift in units of pixels in the data such that the model matches best the data
     """
 
-    def _minimize(x, data, model, variance=None, mask=None, oversampling=1):
+    def _minimize(x, data, model, mask, variance, oversampling=1, negative=1):
         # shift model to proposed astrometric position
         model_shifted = shift_psf(psf_center=model, oversampling=oversampling, shift=x, degrade=True,
                                   n_pix_star=len(data))
         # linear amplitude
-        if mask is None:
-            mask = np.ones_like(data)
         amp = _linear_amplitude(data, model_shifted, variance=variance, mask=mask)
 
-        if variance is None:
-            variance = 1
-        # compute chi2
-        chi2 = np.sum((data - model_shifted * amp) ** 2 / variance * mask)
+        chi2 = negative * np.sum((data - model_shifted * amp) ** 2 / variance * mask)
+
         return chi2
 
     init = np.array([0, 0])
-    x = scipy.optimize.minimize(_minimize, init, args=(data, model, variance, mask, oversampling),
-                                bounds=((-5, 5), (-5, 5)), method='Nelder-Mead')
-    return x.x
+    bounds = ((-10, 10), (-10, 10))
+    if mask is None:
+        mask = np.ones_like(data)
+    if variance is None:
+        variance = np.ones_like(data)
 
+    if optimizer_type == 'Nelder-Mead':
+        x = scipy.optimize.minimize(_minimize, init, args=(data, model, mask, variance, oversampling),
+                                    bounds=bounds, method='Nelder-Mead')
+        return x.x
+
+    elif optimizer_type == 'PSO':
+        lowerLims = np.array([bounds[0][0], bounds[1][0]])
+        upperLims = np.array([bounds[0][1], bounds[1][1]])
+
+        n_particles = 50
+        n_iterations = 100
+        pool = None
+        pso = ParticleSwarmOptimizer(_minimize,
+                                     lowerLims, upperLims, n_particles,
+                                     pool=pool, args=[data, model, mask, variance],
+                                     kwargs={'oversampling': oversampling,
+                                             'negative': -1})
 
-def combine_psf(kernel_list_new, kernel_old, mask_list=None, weight_list=None, factor=1., stacking_option='median',
-                symmetry=1, combine_with_old=False):
+        result, [log_likelihood_list, pos_list, vel_list] = pso.optimize(n_iterations, verbose=False)
+        return result
+
+    else:
+        raise ValueError('optimization type %s is not supported. Please use Nelder-Mead or PSO' % optimizer_type)
+
+
+def combine_psf(kernel_list_new, kernel_old, mask_list=None, amplitude_list=None, factor=1., stacking_option='median',
+                symmetry=1, combine_with_old=False, error_map_list=None):
     """
     updates psf estimate based on old kernel and several new estimates
 
     Parameters
     ----------
     kernel_list_new : list of 2d numpy arrays
         new PSF kernels estimated from the point sources in the image (un-normalized)
     kernel_old : 2d numpy array of shape of the oversampled kernel
         old PSF kernel
     mask_list : None or list of booleans of shape of kernel_list_new
         masks used in the 'kernel_list_new' determination. These regions will not be considered in the combined PSF.
-    weight_list : None or list of floats with positive semi-definite values
-        weights of the different new kernel estimates (i.e. brightness of the stars, etc)
+    amplitude_list : None or list of floats with positive semi-definite values
+        pre-normalized amplitude of the different new kernel estimates (i.e. brightness of the stars, etc)
     factor : weight of updated estimate based on new and old estimate, factor=1 means new estimate,
         factor=0 means old estimate
     stacking_option : string
         option of stacking, mean or median
     symmetry: integer >= 1
         imposed symmetry of PSF estimate
     combine_with_old : boolean
         if True, adds the previous PSF as one of the proposals for the new PSFs
+    error_map_list : None, or list of 2d numpy array, same size as data
+        Variance in the uncorrelated uncertainties in the data for individual pixels.
+        If not set, assumes equal variances for all pixels.
 
     Returns
     -------
     kernel_return : updated PSF estimate and error_map associated with it
     """
 
     n = int(len(kernel_list_new) * symmetry)
-    if weight_list is None:
-        weight_list = np.ones(len(kernel_list_new))
+
+    if amplitude_list is None:
+        amplitude_list = np.ones(len(kernel_list_new))
+    if error_map_list is None:
+        error_map_list = [np.ones_like(kernel_old)] * len(kernel_list_new)
+
     angle = 360. / symmetry
     kernelsize = len(kernel_old)
     kernel_list = np.zeros((n, kernelsize, kernelsize))
-    weights = np.zeros(n)
+    weights = np.zeros((n, kernelsize, kernelsize))
     i = 0
     for j, kernel_new in enumerate(kernel_list_new):
+        if mask_list is None:
+            mask = np.ones_like(kernel_new, dtype='int')
+        else:
+            mask = mask_list[j]
+        error_map_list[j][error_map_list[j] < 10 ** (-10)] = 10 ** (-10)
         for k in range(symmetry):
             kernel_rotated = image_util.rotateImage(kernel_new, angle * k)
+            error_map = image_util.rotateImage(error_map_list[j], angle * k)
+            mask_rot = image_util.rotateImage(mask, angle * k)
             kernel_norm = kernel_util.kernel_norm(kernel_rotated)
             kernel_list[i, :, :] = kernel_norm
-            weights[i] = weight_list[j]
+            # weight according to surface brightness, inverse variance map, and mask
+            weights[i, :, :] = amplitude_list[j] * 1 / error_map * mask_rot
             i += 1
 
     if combine_with_old is True:
         kernel_old_rotated = np.zeros((symmetry, kernelsize, kernelsize))
         for i in range(symmetry):
-            kernel_old_rotated[i, :, :] = kernel_old/np.sum(kernel_old)
+            kernel_old_rotated[i, :, :] = kernel_old / np.sum(kernel_old)
             kernel_list = np.append(kernel_list, kernel_old_rotated, axis=0)
-            weights = np.append(weights, 1)
+            # TODO: this next line is ambiguous about what weight being used for the old kernel estimate
+            weights = np.append(weights, kernel_old)
 
-    # TODO: add mask_list
     # TODO: outlier detection?
     if stacking_option == 'median_weight':
         # TODO: this is rather slow as it needs to loop through all the pixels
-        # adapted from this thread: https://stackoverflow.com/questions/26102867/python-weighted-median-algorithm-with-pandas
+        # adapted from this thread:
+        # https://stackoverflow.com/questions/26102867/python-weighted-median-algorithm-with-pandas
         flattened_psfs = np.array([y.flatten() for y in kernel_list])
+        flattened_weights = np.array([y.flatten() for y in weights])
         x_dim, y_dim = kernel_list[0].shape
         new_img = []
         for i in range(x_dim * y_dim):
             pixels = flattened_psfs[:, i]
-            cumsum = np.cumsum(weights)
-            cutoff = np.sum(weights) / 2.0
+            cumsum = np.cumsum(flattened_weights[:, i])  # weights
+            cutoff = np.sum(flattened_weights[:, i]) / 2.0  # weights
             pixels = np.sort(pixels)
             median = pixels[cumsum >= cutoff][0]
             new_img.append(median)
         kernel_new = np.array(new_img).reshape(x_dim, y_dim)
+
     elif stacking_option == 'mean':
-        kernel_new = np.average(kernel_list, weights = weights, axis=0)
+        kernel_new = np.average(kernel_list, weights=weights, axis=0)
+
     elif stacking_option == 'median':
-        kernel_new = np.median(kernel_list, axis = 0)
+        if mask_list is None:
+            kernel_new = np.median(kernel_list, axis=0)
+        else:
+            # ignore masked pixels instead of over-writing with old one
+            kernel_new = median_with_mask(kernel_list, mask_list)
     else:
-        raise ValueError(" stack_option must be 'median', 'median_weight' or 'mean', %s is not supported." % stacking_option)
+        raise ValueError(" stack_option must be 'median', 'median_weight' or 'mean', %s is not supported."
+                         % stacking_option)
     kernel_new = np.nan_to_num(kernel_new)
-    kernel_new[kernel_new < 0] = 0
+    # kernel_new[kernel_new < 0] = 0
     kernel_new = kernel_util.kernel_norm(kernel_new)
-    kernel_return = factor * kernel_new + (1.-factor) * kernel_old
+    kernel_return = factor * kernel_new + (1. - factor) * kernel_old
     return kernel_return
-
-
-def _verbose_one_step(star, psf_shifted, psf_shifted_data, residuals, residuals_shifted, correction, psf_new):
-    """
-    plotting of intermediate products happening during one step
-    """
-    from mpl_toolkits.axes_grid1 import make_axes_locatable
-    f, axes = plt.subplots(1, 7, figsize=(4 * 7, 4))
-    vmin, vmax = -5, -1
-
-    ax = axes[0]
-    im = ax.imshow(np.log10(star / np.sum(star)), origin='lower', vmin=vmin, vmax=vmax)
-    # ax.autoscale(False)
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    plt.colorbar(im, cax=cax)
-    ax.set_title('star normalized')
-
-    ax = axes[1]
-    im = ax.imshow(np.log10(psf_shifted), origin='lower', vmin=vmin, vmax=vmax)
-    # ax.autoscale(False)
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    plt.colorbar(im, cax=cax)
-    ax.set_title('psf shifted (oversampled)')
-
-    ax = axes[2]
-    im = ax.imshow(np.log10(psf_shifted_data), origin='lower', vmin=vmin, vmax=vmax)
-    # ax.autoscale(False)
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    plt.colorbar(im, cax=cax)
-    ax.set_title('psf shifted (regular)')
-
-    ax = axes[3]
-    im = ax.imshow(residuals, origin='lower')
-    # ax.autoscale(False)
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    plt.colorbar(im, cax=cax)
-    ax.set_title('residuals on data')
-
-    ax = axes[4]
-    im = ax.imshow(residuals_shifted, origin='lower')
-    # ax.autoscale(False)
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    plt.colorbar(im, cax=cax)
-    ax.set_title('residuals re-centered')
-
-    ax = axes[5]
-    im = ax.imshow(correction, origin='lower')
-    # ax.autoscale(False)
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    plt.colorbar(im, cax=cax)
-    ax.set_title('corrections on previous PSF')
-
-    ax = axes[6]
-    im = ax.imshow(np.log10(psf_new), origin='lower', vmin=vmin, vmax=vmax)
-    # ax.autoscale(False)
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    plt.colorbar(im, cax=cax)
-    ax.set_title('new proposed PSF')
-    plt.show()
```

### Comparing `psfr-0.0.1/psfr.egg-info/PKG-INFO` & `psfr-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: psfr
-Version: 0.0.1
+Version: 0.1.0
 Summary: Telescope Images Point Spread Function Reconstruction
 Home-page: https://github.com/sibirrer/psfr
 Author: Simon Birrer
 Author-email: sibirrer@gmail.com
 License: BSD 3-Clause
 Keywords: psfr
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 
 ===========================================
 PSFr - Point Spread Function reconstruction
 ===========================================
 
-.. image:: https://github.com/sibirrer/psfr/workflows/Tests/badge.svg
+|PyPI| |CI| |Docs| |Coveralls|
+
+.. |CI| image:: https://github.com/sibirrer/psfr/workflows/Tests/badge.svg
     :target: https://github.com/sibirrer/psfr/actions
 
-.. image:: https://readthedocs.org/projects/psfr/badge/?version=latest
+.. |Docs| image:: https://readthedocs.org/projects/psfr/badge/?version=latest
         :target: http://psfr.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-.. image:: https://coveralls.io/repos/github/sibirrer/psfr/badge.svg?branch=main
+.. |Coveralls| image:: https://coveralls.io/repos/github/sibirrer/psfr/badge.svg?branch=main
     :target: https://coveralls.io/github/sibirrer/psfr?branch=main
 
+.. |PyPI| image:: https://img.shields.io/pypi/v/psfr?label=PyPI&logo=pypi
+    :target: https://pypi.python.org/pypi/psfr
+
 .. image:: https://github.com/sibirrer/psfr/blob/main/docs/_static/stacked_psf_animation.gif
 
 Point Spread Function reconstruction for astronomical
 ground- and space-based imaging data.
 
 
 Example
@@ -61,33 +65,62 @@
 --------
 
 * Iterative PSF reconstruction given cutouts of individual stars or other point-like sources.
 * Sub-pixel astrometric shifts calculated and accounted for while performing the PSF reconstruction.
 * PSF reconstruction available in super-sampling resolution.
 * Masking pixels, saturation levels and other options to deal with artifacts in the data.
 
+Algorithm
+---------
+The algorithm to iteratively propose a (optionally oversampled) PSF from a set of star cutouts goes as follow:
+
+
+(1) Stack all the stars for an initial guess of the PSF on the centroid pixel (ignoring sub-pixel offsets)
+
+(2) Fit the subpixel centroid with the PSF model estimate
+
+(3) Shift PSF with sub-pixel interpolation to the sub-pixel position of individual stars
+
+(4) Retrieve residuals of the shifted PSF model relative to the data of the cutouts
+
+(5) Apply an inverse sub-pixel shift of the residuals to be focused on the center of the pixel
+
+(6) Based on teh inverse shifted residuals of a set of fixed stars, propose a correction to the previous PSF model
+
+(7) Repeat step (3) - (6) multiple times with the option to repeat step (2)
+
+
+Details and options for the different steps can be found in the documentation and the source code.
+
+
 Used by
 -------
 PSFr is in use with James Webb Space Telescope imaging data (i.e., `Santini et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220711379S/abstract>`_,
 `Merlin et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220711701M/abstract>`_,
-`Yang et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220713101Y/abstract>`_).
+`Yang et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220713101Y/abstract>`_,
+`Ding et al. 2022  <https://ui.adsabs.harvard.edu/abs/2022arXiv220903359D/abstract>`_).
 The iterative PSF reconstruction procedure was originally developed and used for analyzing strongly lensed quasars
 (i.e., `Birrer et al. 2019 <https://ui.adsabs.harvard.edu/#abs/2018arXiv180901274B/abstract>`_
 , `Shajib et al. 2018 <https://ui.adsabs.harvard.edu/abs/2019MNRAS.483.5649S>`_ ,
 `Shajib et al. 2019 <https://ui.adsabs.harvard.edu/abs/2019arXiv191006306S/abstract>`_ ,
 `Schmidt et al. 2022 <https://arxiv.org/abs/2206.04696>`_).
 
 
 Other resources
 ---------------
 
 We also refer to the astropy core package
 `photutils <https://photutils.readthedocs.io/en/stable/index.html>`_
 and in particular to the empirical PSF module
 `ePSF <https://photutils.readthedocs.io/en/stable/epsf.html#build-epsf>`_ .
+PSF reconstructions are e.g. reported by
+`Anderson and King (2000; PASP 112, 1360) <https://ui.adsabs.harvard.edu/abs/2000PASP..112.1360A/abstract>`_
+and
+`Anderson (2016), ISR WFC3 2016-12 <https://www.stsci.edu/files/live/sites/www/files/home/hst/instrumentation/wfc3/documentation/instrument-science-reports-isrs/_documents/2016/WFC3-2016-12.pdf>`_.
+
 
 
 Credits
 -------
 
 The software is an off-spring of the iterative PSF reconstruction scheme of `lenstronomy <https://github.com/lenstronomy/lenstronomy>`_, in particular its `psf_fitting.py <https://github.com/lenstronomy/lenstronomy/blob/v1.10.4/lenstronomy/Workflow/psf_fitting.py>`_ functionalities.
```

### Comparing `psfr-0.0.1/psfr.egg-info/SOURCES.txt` & `psfr-0.1.0/psfr.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -31,24 +31,27 @@
 docs/_static/stacked_psf_animation.gif
 notebooks/JWST_PSF_reconstruction.ipynb
 notebooks/testing.ipynb
 psfr/__init__.py
 psfr/mask_util.py
 psfr/psfr.py
 psfr/util.py
+psfr/verbose_util.py
 psfr.egg-info/PKG-INFO
 psfr.egg-info/SOURCES.txt
 psfr.egg-info/dependency_links.txt
 psfr.egg-info/not-zip-safe
 psfr.egg-info/top_level.txt
 psfr/Data/JWST/psf_f090w_star0.fits
 psfr/Data/JWST/psf_f090w_star1.fits
 psfr/Data/JWST/psf_f090w_star2.fits
 psfr/Data/JWST/psf_f090w_star3.fits
 psfr/Data/JWST/psf_f090w_star4.fits
 psfr/Data/JWST_mock/psf_f090w_supersample5_crop.fits
 tests/__init__.py
+tests/test_mask_util.py
 tests/test_psfr.py
 tests/test_util.py
+tests/test_verbose_util.py
 tests/test_Examples/__init__.py
 tests/test_Examples/test_JWST.py
 tests/test_Examples/test_gaussian.py
```

### Comparing `psfr-0.0.1/setup.py` & `psfr-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,30 +15,29 @@
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Simon Birrer",
     author_email='sibirrer@gmail.com',
     python_requires='>=3.6',
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.11',
     ],
     description="Telescope Images Point Spread Function Reconstruction",
     install_requires=requirements,
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     license = 'BSD 3-Clause',
     license_file = 'LICENSE.rst',
     keywords='psfr',
     name='psfr',
     packages=find_packages(include=['psfr', 'psfr.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/sibirrer/psfr',
-    version='0.0.1',
+    version='0.1.0',
     zip_safe=False,
 )
```

### Comparing `psfr-0.0.1/tests/test_Examples/test_JWST.py` & `psfr-0.1.0/tests/test_Examples/test_JWST.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     star_list_webb = []
     np.random.seed(42)
     for i in range(5):
         x_shift, y_shift = np.random.uniform(-0.5, 0.5), np.random.uniform(-0.5, 0.5)
         star = psfr.shift_psf(psf_center=kernel, oversampling=5, shift=[x_shift, y_shift], degrade=True, n_pix_star=kernel.shape[0]/oversampling)
         star_list_webb.append(star)
 
-    psf_psfr_super, center_list_psfr_super, mask_list = psfr.stack_psf(star_list_webb, oversampling=oversampling, 
+    psf_psfr_super, center_list_psfr_super, mask_list, amplitude_list = psfr.stack_psf(star_list_webb, oversampling=oversampling,
                                                   saturation_limit=None, num_iteration=10, 
                                                   n_recenter=20)
                                                 
     kernel_degraded = util.degrade_kernel(kernel, oversampling)
     psf_guess = star_list_webb[0]
     stacked_psf_degraded = psfr.oversampled2regular(psf_psfr_super, oversampling)
```

### Comparing `psfr-0.0.1/tests/test_Examples/test_gaussian.py` & `psfr-0.1.0/tests/test_Examples/test_gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         amp = np.random.uniform([0.1, 10])
         kwargs_model = [{'amp': 1, 'sigma': sigma, 'center_x': x_c, 'center_y': y_c}]
         flux_model = gauss.surface_brightness(x_grid, y_grid, kwargs_model)
         star = util.array2image(flux_model)
         star = oversampled2regular(star, oversampling=oversampling_compute)
         star_list.append(star)
 
-    psf_after, center_list_after, mask_list = stack_psf(star_list, oversampling=oversampling,
+    psf_after, center_list_after, mask_list,amplitude_list = stack_psf(star_list, oversampling=oversampling,
                                                         saturation_limit=None, num_iteration=num_iteration,
                                                         n_recenter=n_recenter, verbose=False, kwargs_one_step=kwargs_one_step)
 
     psf_true = kernel_util.cut_psf(psf_true, len(psf_after))
     psf_guess = kernel_util.cut_psf(psf_guess, len(psf_after))
     assert np.sum((psf_after - psf_true) ** 2) < np.sum((psf_guess - psf_true) ** 2)
```

### Comparing `psfr-0.0.1/tests/test_util.py` & `psfr-0.1.0/tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,7 +95,22 @@
             else:
                 npt.assert_almost_equal(image_degraded - image, 0, decimal=3)
 
 
 def test_jwst_example_stars():
     star_list_jwst = util.jwst_example_stars()
     assert len(star_list_jwst) == 5
+
+
+def test_median_with_mask():
+    np.random.seed(2)
+    mask_list = []
+    data_list = []
+    for i in range(5):
+        mask = np.random.randint(2, size=(3, 3))
+        data = np.ones((3, 3))
+        data[mask == 0] = 2
+        mask_list.append(mask)
+        data_list.append(data)
+    median_stack = util.median_with_mask(np.array(data_list), np.array(mask_list))
+    npt.assert_almost_equal(median_stack, np.ones((3, 3)))
+
```

