# Comparing `tmp/artistools-2024.4.23.tar.gz` & `tmp/artistools-2024.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artistools-2024.4.23.tar", last modified: Tue Apr 23 11:24:48 2024, max compression
+gzip compressed data, was "artistools-2024.4.29.tar", last modified: Mon Apr 29 13:35:07 2024, max compression
```

## Comparing `artistools-2024.4.23.tar` & `artistools-2024.4.29.tar`

### file list

```diff
@@ -1,354 +1,354 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.174853 artistools-2024.4.23/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 11:24:42.000000 artistools-2024.4.23/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 11:24:42.000000 artistools-2024.4.23/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 11:24:42.000000 artistools-2024.4.23/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-23 11:24:42.000000 artistools-2024.4.23/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-23 11:24:42.000000 artistools-2024.4.23/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 11:24:42.000000 artistools-2024.4.23/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-23 11:24:42.000000 artistools-2024.4.23/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 11:24:42.000000 artistools-2024.4.23/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-23 11:24:42.000000 artistools-2024.4.23/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 11:24:42.000000 artistools-2024.4.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-23 11:24:48.170853 artistools-2024.4.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-23 11:24:42.000000 artistools-2024.4.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.110853 artistools-2024.4.23/artistools/
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.110853 artistools-2024.4.23/artistools/atomic/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/atomic/_atomic_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/codecomparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.114853 artistools-2024.4.23/artistools/data/
--rw-r--r--   0 runner    (1001) docker     (127)    70935 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/ElBiEn_2007.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/atomic_properties.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/betaminusdecays.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/binding_energies.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/collion-AR1985.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/collion-reference.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/collion.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/elements.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.118853 artistools-2024.4.23/artistools/data/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/400.txt
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/520.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.118853 artistools-2024.4.23/artistools/data/filters/ASIAGO/
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17947 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/zs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    48059 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/FUV.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/H.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/H_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)    55262 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/J.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/J_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/K.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/K_ab.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.122853 artistools-2024.4.23/artistools/data/filters/LCOGT/
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/R.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.122853 artistools-2024.4.23/artistools/data/filters/LSQ/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LSQ/rs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.122853 artistools-2024.4.23/artistools/data/filters/LT/
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24161 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.122853 artistools-2024.4.23/artistools/data/filters/NOT/
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/R.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.126853 artistools-2024.4.23/artistools/data/filters/NTT/
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/R.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/zs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NUV.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.126853 artistools-2024.4.23/artistools/data/filters/OGLE/
--rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/OGLE/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/OGLE/V.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.126853 artistools-2024.4.23/artistools/data/filters/PS1/
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/ws.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/zs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    84060 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/R.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.126853 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/zs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)    55259 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvm2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvm2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvw1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvw1_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvw2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvw2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.134853 artistools-2024.4.23/artistools/data/lightcurves/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN1991T.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN1999by.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN1999dq.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2005cf.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2011fe.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2012cg.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2012dn.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2012fr.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2014J.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2015F.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2018byg.dat.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.134853 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.158853 artistools-2024.4.23/artistools/data/refspectra/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    75182 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)    73950 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2010lp_20110928_fors2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   787320 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   713500 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   713176 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   664004 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   708656 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   712196 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   709200 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   552728 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   707384 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   705880 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   257680 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   104189 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   210900 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   122618 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/nero-nebspec.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   103168 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/solar_r_abundance_pattern.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/splitmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/deposition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.162853 artistools-2024.4.23/artistools/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17106 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/estimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2270 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/exportmassfractions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/plot3destimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    48660 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/plotestimators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/test_estimators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26288 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/gsinetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/hesma_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.166853 artistools-2024.4.23/artistools/inputmodel/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6406 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/1dslicefrom3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3984 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/botyanski2017.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11072 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/describeinputmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/downscale3dgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/energyinputfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/from_alcar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.166853 artistools-2024.4.23/artistools/inputmodel/fromcmfgen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/fromcmfgen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10699 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2701 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/fullymixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    54779 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/inputmodel_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5146 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/makeartismodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/map_1d_to_3d_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17178 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/maptogrid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16419 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/modelfromhydro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/opacityinputfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3801 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/plotdensity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17379 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/plotinitialcomposition.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8257 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/recombinationenergy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23731 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/rprocess_from_trajectory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5325 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/rprocess_solar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2636 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/scalevelocity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3586 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/shen2018.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9548 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/slice1dfromconein3dmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14048 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/test_inputmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4064 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/to_tardis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.166853 artistools-2024.4.23/artistools/lightcurve/
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23668 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)    65520 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/plotlightcurve.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2953 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/test_lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)    32172 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/viewingangleanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/writebollightcurvedata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    38118 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/linefluxes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4887 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/logfiles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5914 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/macroatom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/make_vpkt_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    40374 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (127)    57242 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.166853 artistools-2024.4.23/artistools/nltepops/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nltepops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nltepops/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nltepops/nltepops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32642 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nltepops/plotnltepops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.170853 artistools-2024.4.23/artistools/nonthermal/
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    58560 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/_nonthermal_core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5022 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/leptontransport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11735 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/plotnonthermal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14149 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/solvespencerfanocmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/test_nonthermal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.170853 artistools-2024.4.23/artistools/packets/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36685 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/packets/packets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/packets/packetsplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/packets/test_packets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17298 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/plotspherical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/plottools.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (127)    41390 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/radfield.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.170853 artistools-2024.4.23/artistools/spectra/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    56091 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/plotspectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/sampleblackbodyfrompacket_tr.py
--rw-r--r--   0 runner    (1001) docker     (127)    55326 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8618 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/test_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3443 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/test_vspectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/writespectra.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4717 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/test_artistools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23013 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6858 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/viewing_angles_visualization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11238 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/writecomparisondata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.170853 artistools-2024.4.23/artistools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-23 11:24:48.000000 artistools-2024.4.23/artistools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistoolscompletions.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-23 11:24:42.000000 artistools-2024.4.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-23 11:24:42.000000 artistools-2024.4.23/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:24:48.174853 artistools-2024.4.23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.768051 artistools-2024.4.29/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-29 13:35:01.000000 artistools-2024.4.29/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-29 13:35:01.000000 artistools-2024.4.29/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-29 13:35:01.000000 artistools-2024.4.29/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-29 13:35:01.000000 artistools-2024.4.29/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-29 13:35:01.000000 artistools-2024.4.29/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 13:35:01.000000 artistools-2024.4.29/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-29 13:35:01.000000 artistools-2024.4.29/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-29 13:35:01.000000 artistools-2024.4.29/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 13:35:01.000000 artistools-2024.4.29/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-29 13:35:01.000000 artistools-2024.4.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-29 13:35:07.768051 artistools-2024.4.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-29 13:35:01.000000 artistools-2024.4.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.700051 artistools-2024.4.29/artistools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.700051 artistools-2024.4.29/artistools/atomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/atomic/_atomic_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/codecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.704051 artistools-2024.4.29/artistools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    70935 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/ElBiEn_2007.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/atomic_properties.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/betaminusdecays.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/binding_energies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/collion-AR1985.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/collion-reference.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/collion.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.708051 artistools-2024.4.29/artistools/data/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/400.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/520.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.708051 artistools-2024.4.29/artistools/data/filters/ASIAGO/
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/ASIAGO/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/ASIAGO/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17947 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/ASIAGO/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/ASIAGO/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/ASIAGO/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/ASIAGO/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/ASIAGO/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    48059 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/FUV.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/H_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    55262 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/J.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/J_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/K_ab.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.712051 artistools-2024.4.29/artistools/data/filters/LCOGT/
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LCOGT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.712051 artistools-2024.4.29/artistools/data/filters/LSQ/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LSQ/rs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.712051 artistools-2024.4.29/artistools/data/filters/LT/
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24161 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/LT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.712051 artistools-2024.4.29/artistools/data/filters/NOT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NOT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.716051 artistools-2024.4.29/artistools/data/filters/NTT/
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NTT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NTT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NTT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NTT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NTT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NTT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NTT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NTT/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/NUV.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.716051 artistools-2024.4.29/artistools/data/filters/OGLE/
+-rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/OGLE/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/OGLE/V.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.716051 artistools-2024.4.29/artistools/data/filters/PS1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/PS1/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/PS1/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/PS1/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/PS1/ws.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/PS1/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    84060 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/R.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.716051 artistools-2024.4.29/artistools/data/filters/SKYMAPPER/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/SKYMAPPER/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/SKYMAPPER/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/SKYMAPPER/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/SKYMAPPER/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/SKYMAPPER/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    55259 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/uvm2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/uvm2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/uvw1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/uvw1_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/uvw2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/uvw2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/filters/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.724051 artistools-2024.4.29/artistools/data/lightcurves/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN1991T.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN1999by.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN1999dq.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2005cf.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2011fe.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2012cg.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2012dn.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2012fr.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2014J.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2015F.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/SN2018byg.dat.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.724051 artistools-2024.4.29/artistools/data/lightcurves/bollightcurves/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.752051 artistools-2024.4.29/artistools/data/refspectra/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    75182 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    73950 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2010lp_20110928_fors2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   787320 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 13:35:01.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   713500 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   713176 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   664004 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   708656 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   712196 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   709200 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   552728 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   707384 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   705880 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   257680 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   104189 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   210900 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   122618 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/nero-nebspec.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   103168 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/solar_r_abundance_pattern.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/data/splitmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/deposition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.756051 artistools-2024.4.29/artistools/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/estimators/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17106 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/estimators/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/estimators/estimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2270 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/estimators/exportmassfractions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/estimators/plot3destimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48624 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/estimators/plotestimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/estimators/test_estimators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26288 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/gsinetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/hesma_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.760051 artistools-2024.4.29/artistools/inputmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3984 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/botyanski2017.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11056 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/describeinputmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/downscale3dgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/energyinputfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/from_alcar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.760051 artistools-2024.4.29/artistools/inputmodel/fromcmfgen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/fromcmfgen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10699 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2701 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/fullymixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54910 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/inputmodel_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6406 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/make1dslicefrom3d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5146 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/makeartismodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/map_1d_to_3d_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17178 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/maptogrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16419 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/modelfromhydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/opacityinputfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3801 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/plotdensity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17379 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/plotinitialcomposition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8257 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/recombinationenergy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23778 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/rprocess_from_trajectory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5325 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/rprocess_solar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2636 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/scalevelocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3586 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/shen2018.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9548 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/slice1dfromconein3dmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/test_inputmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4064 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/inputmodel/to_tardis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.760051 artistools-2024.4.29/artistools/lightcurve/
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/lightcurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/lightcurve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/lightcurve/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65684 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/lightcurve/plotlightcurve.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2953 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/lightcurve/test_lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32172 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/lightcurve/viewingangleanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/lightcurve/writebollightcurvedata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38118 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/linefluxes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4828 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/logfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5914 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/macroatom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/make_vpkt_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40374 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)    58094 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.760051 artistools-2024.4.29/artistools/nltepops/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nltepops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nltepops/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nltepops/nltepops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32658 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nltepops/plotnltepops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.764051 artistools-2024.4.29/artistools/nonthermal/
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nonthermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nonthermal/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58560 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nonthermal/_nonthermal_core.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5022 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nonthermal/leptontransport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11735 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nonthermal/plotnonthermal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14149 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nonthermal/solvespencerfanocmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/nonthermal/test_nonthermal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.764051 artistools-2024.4.29/artistools/packets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36627 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/packets/packets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/packets/packetsplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/packets/test_packets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17280 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/plotspherical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/plottools.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41372 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/radfield.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.764051 artistools-2024.4.29/artistools/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/spectra/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/spectra/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57545 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/spectra/plotspectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/spectra/sampleblackbodyfrompacket_tr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56300 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/spectra/spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8618 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/spectra/test_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3443 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/spectra/test_vspectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/spectra/writespectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4717 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/test_artistools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23013 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6854 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/viewing_angles_visualization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11241 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistools/writecomparisondata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:07.764051 artistools-2024.4.29/artistools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-29 13:35:07.000000 artistools-2024.4.29/artistools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-04-29 13:35:02.000000 artistools-2024.4.29/artistoolscompletions.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-29 13:35:02.000000 artistools-2024.4.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-29 13:35:02.000000 artistools-2024.4.29/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:35:07.768051 artistools-2024.4.29/setup.cfg
```

### Comparing `artistools-2024.4.23/.codecov.yml` & `artistools-2024.4.29/.codecov.yml`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/.gitignore` & `artistools-2024.4.29/.gitignore`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/.pre-commit-config.yaml` & `artistools-2024.4.29/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 
     # - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
     #   rev: 0.2.3
     #   hooks:
     #       - id: yamlfmt
 
     - repo: https://github.com/astral-sh/ruff-pre-commit
-      rev: v0.4.1
+      rev: v0.4.2
       hooks:
           - id: ruff
             args: [--fix, --exit-non-zero-on-fix]
 
     - repo: https://github.com/astral-sh/ruff-pre-commit
-      rev: v0.4.1
+      rev: v0.4.2
       hooks:
           - id: ruff-format
 
     # - repo: https://github.com/pre-commit/mirrors-mypy
     #   rev: v1.6.1
     #   hooks:
     #       - id: mypy
```

### Comparing `artistools-2024.4.23/.sourcery.yaml` & `artistools-2024.4.29/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/CITATION.cff` & `artistools-2024.4.29/CITATION.cff`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/LICENSE.txt` & `artistools-2024.4.29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/PKG-INFO` & `artistools-2024.4.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artistools
-Version: 2024.4.23
+Version: 2024.4.29
 Summary: Plotting and analysis tools for the ARTIS 3D radiative transfer code for supernovae and kilonovae.
 Author-email: "Luke J. Shingles" <luke.shingles@gmail.com>, "Christine E. Collins" <c.collins@gsi.de>, Alexander Holas <alexander.holas@h-its.org>, Fionntan Callan <fcallan02@qub.ac.uk>, Stuart Sim <s.sim@qub.ac.uk>
 License: MIT
 Project-URL: Repository, https://www.github.com/artis-mcrt/artistools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
@@ -13,42 +13,42 @@
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: argcomplete>=3.3.0
 Requires-Dist: astropy>=6.0.1
-Requires-Dist: coverage>=7.4.4
+Requires-Dist: coverage>=7.5.0
 Requires-Dist: extinction>=0.4.6
 Requires-Dist: imageio>=2.34.1
 Requires-Dist: matplotlib>=3.8.4
-Requires-Dist: mypy>=1.9.0
+Requires-Dist: mypy>=1.10.0
 Requires-Dist: numexpr>=2.10.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas[compression,parquet,pyarrow]>=2.2.2
-Requires-Dist: polars>=0.20.22
+Requires-Dist: polars>=0.20.23
 Requires-Dist: pre-commit>=3.7.0
 Requires-Dist: pyarrow>=16.0.0
 Requires-Dist: pynonthermal>=2024.2.17
 Requires-Dist: pypdf2>=3.0.1
-Requires-Dist: pytest>=8.1.1
+Requires-Dist: pytest>=8.2.0
 Requires-Dist: pytest-cov>=5.0.0
-Requires-Dist: pytest-xdist[psutil]>=3.5.0
+Requires-Dist: pytest-xdist[psutil]>=3.6.1
 Requires-Dist: python-xz>=0.5
-Requires-Dist: pyvista>=0.43.5
+Requires-Dist: pyvista>=0.43.6
 Requires-Dist: PyYAML>=6.0.1
-Requires-Dist: pyzstd>=0.15.10
-Requires-Dist: ruff>=0.4.1
+Requires-Dist: ruff>=0.4.2
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: setuptools_scm[toml]>=8.0.4
 Requires-Dist: tabulate>=0.9
 Requires-Dist: typeguard>=4.2.1
 Requires-Dist: types-PyYAML>=6.0.12.20240311
 Requires-Dist: types-tabulate>=0.9.0.20240106
 Requires-Dist: wheel>=0.43.0
+Requires-Dist: zstandard>=0.22.0
 
 # Artistools
 
 > Artistools is collection of plotting, analysis, and file format conversion tools for the [ARTIS](https://github.com/artis-mcrt/artis) radiative transfer code.
 
 [![DOI](https://zenodo.org/badge/53433932.svg)](https://zenodo.org/badge/latestdoi/53433932)
 [![Installation and pytest](https://github.com/artis-mcrt/artistools/actions/workflows/pytest.yml/badge.svg)](https://github.com/artis-mcrt/artistools/actions/workflows/pytest.yml)
```

### Comparing `artistools-2024.4.23/README.md` & `artistools-2024.4.29/README.md`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/__init__.py` & `artistools-2024.4.29/artistools/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/__main__.py` & `artistools-2024.4.29/artistools/__main__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/atomic/_atomic_core.py` & `artistools-2024.4.29/artistools/atomic/_atomic_core.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/codecomparison.py` & `artistools-2024.4.29/artistools/codecomparison.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/commands.py` & `artistools-2024.4.29/artistools/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     "writecodecomparisondata": ("writecomparisondata", "main"),
     "writespectra": ("spectra.writespectra", "main"),
     "inputmodel": {
         "describe": ("inputmodel.describeinputmodel", "main"),
         "maptogrid": ("inputmodel.maptogrid", "main"),
         "makeartismodelfromparticlegridmap": ("inputmodel.modelfromhydro", "main"),
         "makeartismodel": ("inputmodel.makeartismodel", "main"),
-        "make1dslicefrom3dmodel": ("inputmodel.1dslicefrom3d", "main"),
+        "make1dslicefrom3dmodel": ("inputmodel.make1dslicefrom3d", "main"),
         "makeartismodel1dslicefromcone": ("inputmodel.slice1dfromconein3dmodel", "main"),
         "makeartismodelbotyanski2017": ("inputmodel.botyanski2017", "main"),
         "makeartismodelfromshen2018": ("inputmodel.shen2018", "main"),
         "makeartismodelscalevelocity": ("inputmodel.scalevelocity", "main"),
         "makeartismodelfullymixed": ("inputmodel.fullymixed", "main"),
         "makeartismodelsolar_rprocess": ("inputmodel.rprocess_solar", "main"),
         "makeartismodelfromsingletrajectory": ("inputmodel.rprocess_from_trajectory", "main"),
```

### Comparing `artistools-2024.4.23/artistools/configuration.py` & `artistools-2024.4.29/artistools/configuration.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/ElBiEn_2007.txt` & `artistools-2024.4.29/artistools/data/ElBiEn_2007.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/atomic_properties.txt` & `artistools-2024.4.29/artistools/data/atomic_properties.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/betaminusdecays.txt` & `artistools-2024.4.29/artistools/data/betaminusdecays.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/binding_energies.txt` & `artistools-2024.4.29/artistools/data/binding_energies.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/collion-AR1985.txt` & `artistools-2024.4.29/artistools/data/collion-AR1985.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/collion-reference.txt` & `artistools-2024.4.29/artistools/data/collion-reference.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/collion.txt` & `artistools-2024.4.29/artistools/data/collion.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/elements.csv` & `artistools-2024.4.29/artistools/data/elements.csv`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/400.txt` & `artistools-2024.4.29/artistools/data/filters/400.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/520.txt` & `artistools-2024.4.29/artistools/data/filters/520.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/ASIAGO/B.txt` & `artistools-2024.4.29/artistools/data/filters/ASIAGO/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/ASIAGO/U.txt` & `artistools-2024.4.29/artistools/data/filters/ASIAGO/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/ASIAGO/V.txt` & `artistools-2024.4.29/artistools/data/filters/ASIAGO/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/ASIAGO/gs.txt` & `artistools-2024.4.29/artistools/data/filters/ASIAGO/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/ASIAGO/is.txt` & `artistools-2024.4.29/artistools/data/filters/ASIAGO/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/ASIAGO/rs.txt` & `artistools-2024.4.29/artistools/data/filters/ASIAGO/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/ASIAGO/zs.txt` & `artistools-2024.4.29/artistools/data/filters/ASIAGO/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/B.txt` & `artistools-2024.4.29/artistools/data/filters/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/FUV.txt` & `artistools-2024.4.29/artistools/data/filters/FUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/H.txt` & `artistools-2024.4.29/artistools/data/filters/H.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/H_ab.txt` & `artistools-2024.4.29/artistools/data/filters/H_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/I.txt` & `artistools-2024.4.29/artistools/data/filters/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/J.txt` & `artistools-2024.4.29/artistools/data/filters/J.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/J_ab.txt` & `artistools-2024.4.29/artistools/data/filters/J_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/K.txt` & `artistools-2024.4.29/artistools/data/filters/K.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/K_ab.txt` & `artistools-2024.4.29/artistools/data/filters/K_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/B.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/I.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/R.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/U.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/V.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/gs.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/is.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/rs.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/us.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LCOGT/zs.txt` & `artistools-2024.4.29/artistools/data/filters/LCOGT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LSQ/rs.txt` & `artistools-2024.4.29/artistools/data/filters/LSQ/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LT/gs.txt` & `artistools-2024.4.29/artistools/data/filters/LT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LT/is.txt` & `artistools-2024.4.29/artistools/data/filters/LT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LT/rs.txt` & `artistools-2024.4.29/artistools/data/filters/LT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LT/us.txt` & `artistools-2024.4.29/artistools/data/filters/LT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/LT/zs.txt` & `artistools-2024.4.29/artistools/data/filters/LT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/B.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/I.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/R.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/U.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/V.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/gs.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/is.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/rs.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/us.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NOT/zs.txt` & `artistools-2024.4.29/artistools/data/filters/NOT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NTT/B.txt` & `artistools-2024.4.29/artistools/data/filters/NTT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NTT/I.txt` & `artistools-2024.4.29/artistools/data/filters/NTT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NTT/R.txt` & `artistools-2024.4.29/artistools/data/filters/NTT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NTT/U.txt` & `artistools-2024.4.29/artistools/data/filters/NTT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NTT/V.txt` & `artistools-2024.4.29/artistools/data/filters/NTT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NTT/gs.txt` & `artistools-2024.4.29/artistools/data/filters/NTT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NTT/rs.txt` & `artistools-2024.4.29/artistools/data/filters/NTT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NTT/zs.txt` & `artistools-2024.4.29/artistools/data/filters/NTT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/NUV.txt` & `artistools-2024.4.29/artistools/data/filters/NUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/OGLE/I.txt` & `artistools-2024.4.29/artistools/data/filters/OGLE/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/OGLE/V.txt` & `artistools-2024.4.29/artistools/data/filters/OGLE/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/PS1/gs.txt` & `artistools-2024.4.29/artistools/data/filters/PS1/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/PS1/is.txt` & `artistools-2024.4.29/artistools/data/filters/PS1/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/PS1/rs.txt` & `artistools-2024.4.29/artistools/data/filters/PS1/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/PS1/ws.txt` & `artistools-2024.4.29/artistools/data/filters/PS1/ws.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/PS1/zs.txt` & `artistools-2024.4.29/artistools/data/filters/PS1/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/R.txt` & `artistools-2024.4.29/artistools/data/filters/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/gs.txt` & `artistools-2024.4.29/artistools/data/filters/SKYMAPPER/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/is.txt` & `artistools-2024.4.29/artistools/data/filters/SKYMAPPER/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/rs.txt` & `artistools-2024.4.29/artistools/data/filters/SKYMAPPER/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/us.txt` & `artistools-2024.4.29/artistools/data/filters/SKYMAPPER/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/zs.txt` & `artistools-2024.4.29/artistools/data/filters/SKYMAPPER/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/U.txt` & `artistools-2024.4.29/artistools/data/filters/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/V.txt` & `artistools-2024.4.29/artistools/data/filters/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/gs.txt` & `artistools-2024.4.29/artistools/data/filters/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/is.txt` & `artistools-2024.4.29/artistools/data/filters/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/rs.txt` & `artistools-2024.4.29/artistools/data/filters/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/us.txt` & `artistools-2024.4.29/artistools/data/filters/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/uvm2.txt` & `artistools-2024.4.29/artistools/data/filters/uvm2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/uvm2_ab.txt` & `artistools-2024.4.29/artistools/data/filters/uvm2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/uvw1.txt` & `artistools-2024.4.29/artistools/data/filters/uvw1.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/uvw1_ab.txt` & `artistools-2024.4.29/artistools/data/filters/uvw1_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/uvw2.txt` & `artistools-2024.4.29/artistools/data/filters/uvw2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/uvw2_ab.txt` & `artistools-2024.4.29/artistools/data/filters/uvw2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/filters/zs.txt` & `artistools-2024.4.29/artistools/data/filters/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt` & `artistools-2024.4.29/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt` & `artistools-2024.4.29/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt` & `artistools-2024.4.29/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/2010lp_20110928_fors2.txt` & `artistools-2024.4.29/artistools/data/refspectra/2010lp_20110928_fors2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz` & `artistools-2024.4.29/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt` & `artistools-2024.4.29/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt` & `artistools-2024.4.29/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt` & `artistools-2024.4.29/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt` & `artistools-2024.4.29/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt` & `artistools-2024.4.29/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt` & `artistools-2024.4.29/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt` & `artistools-2024.4.29/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt` & `artistools-2024.4.29/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt` & `artistools-2024.4.29/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/data/solar_r_abundance_pattern.txt` & `artistools-2024.4.29/artistools/data/solar_r_abundance_pattern.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/deposition.py` & `artistools-2024.4.29/artistools/deposition.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/estimators/__init__.py` & `artistools-2024.4.29/artistools/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/estimators/estimators.py` & `artistools-2024.4.29/artistools/estimators/estimators.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/estimators/estimators_classic.py` & `artistools-2024.4.29/artistools/estimators/estimators_classic.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/estimators/exportmassfractions.py` & `artistools-2024.4.29/artistools/estimators/exportmassfractions.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/estimators/plot3destimators_classic.py` & `artistools-2024.4.29/artistools/estimators/plot3destimators_classic.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/estimators/plotestimators.py` & `artistools-2024.4.29/artistools/estimators/plotestimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,18 +248,18 @@
     estimators: pl.LazyFrame | pl.DataFrame,
     modelpath: str | Path,
     args: argparse.Namespace,
     **plotkwargs: t.Any,
 ) -> None:
     if seriestype == "levelpopulation_dn_on_dvel":
         ax.set_ylabel("dN/dV [{}km$^{{-1}}$ s]")
-        ax.yaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(ax.get_ylabel(), useMathText=True))
+        ax.yaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(ax.get_ylabel()))
     elif seriestype == "levelpopulation":
         ax.set_ylabel("X$_{{i}}$ [{}/cm3]")
-        ax.yaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(ax.get_ylabel(), useMathText=True))
+        ax.yaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(ax.get_ylabel()))
     else:
         raise ValueError
 
     modeldata, _ = at.inputmodel.get_modeldata(modelpath, derived_cols=["mass_g", "volume"])
 
     adata = at.atomic.get_levels(modelpath)
```

### Comparing `artistools-2024.4.23/artistools/estimators/test_estimators.py` & `artistools-2024.4.29/artistools/estimators/test_estimators.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/gsinetwork.py` & `artistools-2024.4.29/artistools/gsinetwork.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/hesma_scripts.py` & `artistools-2024.4.29/artistools/hesma_scripts.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/1dslicefrom3d.py` & `artistools-2024.4.29/artistools/inputmodel/make1dslicefrom3d.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/__init__.py` & `artistools-2024.4.29/artistools/inputmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/botyanski2017.py` & `artistools-2024.4.29/artistools/inputmodel/botyanski2017.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/describeinputmodel.py` & `artistools-2024.4.29/artistools/inputmodel/describeinputmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,17 +55,15 @@
     dfmodel, modelmeta = at.inputmodel.get_modeldata_polars(
         args.inputfile,
         get_elemabundances=True,
         printwarningsonly=False,
         derived_cols=["mass_g", "vel_r_mid", "rho"],
     )
 
-    dfmodel = (
-        dfmodel.filter(pl.col("rho") > 0.0).drop("X_n")  # don't confuse neutrons with Nitrogen
-    )
+    dfmodel = dfmodel.filter(pl.col("rho") > 0.0).drop("X_n")  # don't confuse neutrons with Nitrogen
 
     if args.noabund:
         dfmodel = dfmodel.drop(cs.starts_with("X_"))
 
     if not args.isotopes:
         dfmodel = dfmodel.drop(cs.matches("X_[A-z]+[0-9]"))
```

### Comparing `artistools-2024.4.23/artistools/inputmodel/downscale3dgrid.py` & `artistools-2024.4.29/artistools/inputmodel/downscale3dgrid.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 @typechecked
 def make_downscaled_3d_grid(
     modelpath: str | Path, outputgridsize: int = 50, plot: bool = False, outputfolder: Path | str | None = None
 ) -> Path:
     """Get a 3D model with smallgrid^3 cells from a 3D model with grid^3 cells.
+
     Should be same as downscale_3d_grid.pro.
     """
     modelpath = Path(modelpath)
 
     dfmodel, modelmeta = at.get_modeldata(modelpath)
     dfelemabund = at.inputmodel.get_initelemabundances(modelpath)
 
@@ -88,15 +89,15 @@
     print("writing abundance file")
     i = 0
     with (modelpath / smallabundancefile).open("w") as newabundancefile:
         for z, y, x in itertools.product(range(smallgrid), range(smallgrid), range(smallgrid)):
             line = abund_small[x, y, z, :].tolist()  # index 1:30 are abundances
             line[0] = i + 1  # replace index 0 with index id
             i += 1
-            newabundancefile.writelines("%g " % item for item in line)
+            newabundancefile.writelines(f"{item:g} " for item in line)
             newabundancefile.writelines("\n")
 
     print("writing model file")
     xmax = vmax * t_model_days * 3600 * 24
     cellindex = 0
     with (modelpath / smallmodelfile).open("w") as newmodelfile:
         gridsize = smallgrid**3
@@ -109,17 +110,17 @@
                 cellindex + 1,
                 -xmax + 2 * x * xmax / smallgrid,
                 -xmax + 2 * y * xmax / smallgrid,
                 -xmax + 2 * z * xmax / smallgrid,
                 rho_small[x, y, z],
             ]
             line2 = radioabunds_small[x, y, z, :]
-            newmodelfile.writelines("%g " % item for item in line1)
+            newmodelfile.writelines(f"{item:g} " for item in line1)
             newmodelfile.writelines("\n")
-            newmodelfile.writelines("%g " % item for item in line2)
+            newmodelfile.writelines(f"{item:g} " for item in line2)
             newmodelfile.writelines("\n")
             cellindex += 1
 
     if plot:
         print("making diagnostic plot")
         try:
             import matplotlib.pyplot as plt
```

### Comparing `artistools-2024.4.23/artistools/inputmodel/energyinputfiles.py` & `artistools-2024.4.29/artistools/inputmodel/energyinputfiles.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/from_alcar.py` & `artistools-2024.4.29/artistools/inputmodel/from_alcar.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py` & `artistools-2024.4.29/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/fromcmfgen/rd_cmfgen.py` & `artistools-2024.4.29/artistools/inputmodel/fromcmfgen/rd_cmfgen.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/fullymixed.py` & `artistools-2024.4.29/artistools/inputmodel/fullymixed.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/inputmodel_misc.py` & `artistools-2024.4.29/artistools/inputmodel/inputmodel_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,14 +422,16 @@
         "ncoordgrid": ncoordgrid,
         "ncoordgridx": ncoordgrid,
         "ncoordgridy": ncoordgrid,
         "ncoordgridz": ncoordgrid,
         "headercommentlines": [],
     }
 
+    fncoordgrid = float(ncoordgrid)  # fixes an issue with polars 0.20.23 https://github.com/pola-rs/polars/issues/15952
+
     dfmodel = (
         pl.DataFrame(
             {"modelgridindex": range(ncoordgrid**3), "inputcellid": range(1, 1 + ncoordgrid**3)},
             schema={"modelgridindex": pl.Int32, "inputcellid": pl.Int32},
         )
         .lazy()
         .with_columns(
@@ -437,17 +439,17 @@
                 pl.col("modelgridindex").mod(ncoordgrid).alias("n_x"),
                 (pl.col("modelgridindex") // ncoordgrid).mod(ncoordgrid).alias("n_y"),
                 (pl.col("modelgridindex") // (ncoordgrid**2)).mod(ncoordgrid).alias("n_z"),
             ]
         )
         .with_columns(
             [
-                (-xmax + 2 * pl.col("n_x") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_x_min"),
-                (-xmax + 2 * pl.col("n_y") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_y_min"),
-                (-xmax + 2 * pl.col("n_z") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_z_min"),
+                (-xmax + 2.0 * pl.col("n_x") * xmax / fncoordgrid).cast(pl.Float32).alias("pos_x_min"),
+                (-xmax + 2.0 * pl.col("n_y") * xmax / fncoordgrid).cast(pl.Float32).alias("pos_y_min"),
+                (-xmax + 2.0 * pl.col("n_z") * xmax / fncoordgrid).cast(pl.Float32).alias("pos_z_min"),
             ]
         )
     )
 
     standardcols = get_standard_columns(3, includenico57=includenico57)
 
     dfmodel = dfmodel.with_columns(
```

### Comparing `artistools-2024.4.23/artistools/inputmodel/makeartismodel.py` & `artistools-2024.4.29/artistools/inputmodel/makeartismodel.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/map_1d_to_3d_grid.py` & `artistools-2024.4.29/artistools/inputmodel/map_1d_to_3d_grid.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/maptogrid.py` & `artistools-2024.4.29/artistools/inputmodel/maptogrid.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/modelfromhydro.py` & `artistools-2024.4.29/artistools/inputmodel/modelfromhydro.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/opacityinputfile.py` & `artistools-2024.4.29/artistools/inputmodel/opacityinputfile.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/plotdensity.py` & `artistools-2024.4.29/artistools/inputmodel/plotdensity.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/plotinitialcomposition.py` & `artistools-2024.4.29/artistools/inputmodel/plotinitialcomposition.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/recombinationenergy.py` & `artistools-2024.4.29/artistools/inputmodel/recombinationenergy.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/rprocess_from_trajectory.py` & `artistools-2024.4.29/artistools/inputmodel/rprocess_from_trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,15 @@
     print(f" took {time.perf_counter() - timestart:.1f} seconds")
     print(f" there are {nuclidesincluded} nuclides from {elementsincluded} elements included")
 
     return dfelabundances
 
 
 def open_tar_file_or_extracted(traj_root: Path, particleid: int, memberfilename: str):
-    """Trajectory files are generally stored as {particleid}.tar.xz, but this is slow
-    to access, so first check for extracted files, or decompressed .tar files,
-    which are much faster to access.
+    """Trajectory files are generally stored as {particleid}.tar.xz, but this is slow to access, so first check for extracted files, or decompressed .tar files, which are much faster to access.
 
     memberfilename: file path within the trajectory tarfile, eg. ./Run_rprocess/evol.dat
     """
     path_extracted_file = Path(traj_root, str(particleid), memberfilename)
     tarfilepaths = [
         Path(traj_root, filename)
         for filename in (
@@ -137,17 +135,19 @@
             dtype_backend="pyarrow",
         )
 
 
 def get_closest_network_timestep(
     traj_root: Path, particleid: int, timesec: float, cond: t.Literal["lessthan", "greaterthan", "nearest"] = "nearest"
 ) -> int:
-    """cond:
-    'lessthan': find highest timestep less than time_sec
-    'greaterthan': find lowest timestep greater than time_sec.
+    """Find the closest network timestep to a given time in seconds.
+
+    cond:
+      - 'lessthan': find highest timestep less than time_sec
+      - 'greaterthan': find lowest timestep greater than time_sec.
     """
     dfevol = get_dfevol(traj_root, particleid)
 
     if cond == "nearest":
         idx = np.abs(dfevol.timesec.to_numpy() - timesec).argmin()
         return int(dfevol["nstep"].to_numpy()[idx])
 
@@ -159,17 +159,15 @@
 
     raise AssertionError
 
 
 def get_trajectory_timestepfile_nuc_abund(
     traj_root: Path, particleid: int, memberfilename: str
 ) -> tuple[pd.DataFrame, float]:
-    """Get the nuclear abundances for a particular trajectory id number and time
-    memberfilename should be something like "./Run_rprocess/tday_nz-plane".
-    """
+    """Get the nuclear abundances for a particular trajectory id number and time memberfilename should be something like "./Run_rprocess/tday_nz-plane"."""
     with open_tar_file_or_extracted(traj_root, particleid, memberfilename) as trajfile:
         try:
             _, str_t_model_init_seconds, _, rho, _, _ = trajfile.readline().split()
         except ValueError as exc:
             print(f"Problem with {memberfilename}")
             msg = f"Problem with {memberfilename}"
             raise ValueError(msg) from exc
@@ -244,20 +242,18 @@
     return qdotintegral
 
 
 def get_trajectory_abund_q(
     particleid: int,
     traj_root: Path,
     t_model_s: float | None = None,
-    nts: int | None = None,
+    nts: int | None = None,  # GSI network timestep number
     getqdotintegral: bool = False,
 ) -> dict[tuple[int, int] | str, float]:
-    """Get the nuclear mass fractions (and Qdotintegral) for a particle particle number as a given time
-    nts: GSI network timestep number.
-    """
+    """Get the nuclear mass fractions (and Qdotintegral) for a particle particle number as a given time."""
     assert t_model_s is not None or nts is not None
     try:
         if nts is not None:
             memberfilename = f"./Run_rprocess/nz-plane{nts:05d}"
         elif t_model_s is not None:
             # find the closest timestep to the required time
             nts = get_closest_network_timestep(traj_root, particleid, t_model_s)
```

### Comparing `artistools-2024.4.23/artistools/inputmodel/rprocess_solar.py` & `artistools-2024.4.29/artistools/inputmodel/rprocess_solar.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/scalevelocity.py` & `artistools-2024.4.29/artistools/inputmodel/scalevelocity.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/shen2018.py` & `artistools-2024.4.29/artistools/inputmodel/shen2018.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/slice1dfromconein3dmodel.py` & `artistools-2024.4.29/artistools/inputmodel/slice1dfromconein3dmodel.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/inputmodel/test_inputmodel.py` & `artistools-2024.4.29/artistools/inputmodel/test_inputmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
 
     dfmodel[75000, "rho"] = 1
     dfmodel[75001, "rho"] = 2
     dfmodel[95200, "rho"] = 3
     dfmodel[75001, "rho"] = 0.5
 
     outpath = outputpath / "test_save_load_3d_model"
+    outpath.mkdir(exist_ok=True, parents=True)
     at.inputmodel.save_modeldata(outpath=outpath, dfmodel=dfmodel, modelmeta=modelmeta)
     dfmodel2, modelmeta2 = at.inputmodel.get_modeldata_polars(modelpath=outpath)
     assert dfmodel.equals(dfmodel2.collect())
     assert modelmeta == modelmeta2
 
     # next load will use the parquet file
     dfmodel3, modelmeta3 = at.inputmodel.get_modeldata_polars(modelpath=outpath)
```

### Comparing `artistools-2024.4.23/artistools/inputmodel/to_tardis.py` & `artistools-2024.4.29/artistools/inputmodel/to_tardis.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/lightcurve/__init__.py` & `artistools-2024.4.29/artistools/lightcurve/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/lightcurve/lightcurve.py` & `artistools-2024.4.29/artistools/lightcurve/lightcurve.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,16 +262,15 @@
     for filter_name in filters_list:
         if filter_name == "bol":
             continue
         zeropointenergyflux, wavefilter, transmission, wavefilter_min, wavefilter_max = get_filter_data(
             filterdir, filter_name
         )
 
-        for timestep, time in enumerate(timearray):
-            time = float(time)
+        for timestep, time in enumerate(float(time) for time in timearray):
             if (args.timemin is None or args.timemin <= time) and (args.timemax is None or args.timemax >= time):
                 wavelength_from_spectrum, flux = get_spectrum_in_filter_range(
                     modelpath=modelpath,
                     timestep=timestep,
                     time=time,
                     wavefilter_min=wavefilter_min,
                     wavefilter_max=wavefilter_max,
@@ -309,16 +308,15 @@
     angle: int = -1,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
 ) -> tuple[list[float], list[float]]:
     magnitudes = []
     times = []
 
-    for timestep, time in enumerate(timearray):
-        time = float(time)
+    for timestep, time in enumerate(float(time) for time in timearray):
         if (args.timemin is None or args.timemin <= time) and (args.timemax is None or args.timemax >= time):
             if angle == -1:
                 spectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=timestep, timestepmax=timestep)[-1]
 
             elif args.plotvspecpol:
                 spectrum = at.spectra.get_vspecpol_spectrum(modelpath, time, angle, args)
             else:
```

### Comparing `artistools-2024.4.23/artistools/lightcurve/plotlightcurve.py` & `artistools-2024.4.29/artistools/lightcurve/plotlightcurve.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     #     axistherm.plot(depdata['tmid_days'], f, **dict(
     #         plotkwargs, **{
     #             'label': plotkwargs['label'] + r' $\dot{E}_{dep}/\dot{E}_{rad}$',
     #             'linestyle': 'solid',
     #             'color': color_total,
     #         }))
 
-    color_gamma = axis._get_lines.get_next_color()
-    color_gamma = axis._get_lines.get_next_color()
+    color_gamma = axis._get_lines.get_next_color()  # noqa: SLF001
+    color_gamma = axis._get_lines.get_next_color()  # noqa: SLF001
 
     # axis.plot(depdata['tmid_days'], depdata['eps_gamma_Lsun'] * 3.826e33, **dict(
     #     plotkwargs, **{
     #         'label': plotkwargs['label'] + r' $\dot{E}_{rad,\gamma}$',
     #         'linestyle': 'dashed',
     #         'color': color_gamma,
     #     }))
@@ -86,15 +86,15 @@
             **plotkwargs,
             "label": plotkwargs["label"] + r" $\dot{E}_{dep,\gamma}$",
             "linestyle": "dashed",
             "color": color_gamma,
         },
     )
 
-    color_beta = axis._get_lines.get_next_color()
+    color_beta = axis._get_lines.get_next_color()  # noqa: SLF001
 
     if "eps_elec_Lsun" in depdata:
         axis.plot(
             depdata["tmid_days"],
             depdata["eps_elec_Lsun"] * 3.826e33,
             **{
                 **plotkwargs,
@@ -600,25 +600,29 @@
             )
 
     axis.set_xlabel(r"Time [days]")
 
     if args.magnitude:
         axis.set_ylabel("Absolute Bolometric Magnitude")
     else:
-        str_units = "$/ \\mathrm{L}_\\odot$" if args.Lsun else " [erg/s]"
+        str_units = r" [{}$\mathrm{{L}}_\odot$]" if args.Lsun else " [{}erg/s]"
         if args.plotdeposition:
-            yvarname = r"$L$ or $\dot{E}$"
+            yvarname = r"$L$ or $\dot{{E}}$"
         elif escape_type == "TYPE_GAMMA":
-            yvarname = r"$\mathrm{L}_\gamma$"
+            yvarname = r"$\mathrm{{L}}_\gamma$"
         elif escape_type == "TYPE_RPKT":
-            yvarname = r"$\mathrm{L}_{\mathrm{UVOIR}}$"
+            yvarname = r"$\mathrm{{L}}_{{\mathrm{{UVOIR}}}}$"
         else:
-            yvarname = r"$\mathrm{L}_{\mathrm{" + escape_type.replace("_", r"\_") + r"}}$"
+            yvarname = r"$\mathrm{{L}}_{{\mathrm{{" + escape_type.replace("_", r"\_") + r"}}}}$"
+
         axis.set_ylabel(yvarname + str_units)
 
+        if "{" in axis.get_ylabel() and not args.logscaley:
+            axis.yaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(axis.get_ylabel(), decimalplaces=1))
+
     if args.colorbarcostheta or args.colorbarphi:
         costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels(
             usedegrees=args.usedegrees
         )
         scaledmap = make_colorbar_viewingangles_colormap()
         make_colorbar_viewingangles(phi_viewing_angle_bins, scaledmap, args, ax=axis)
 
@@ -840,17 +844,15 @@
     if args.colorbarcostheta or args.colorbarphi:
         costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels(
             usedegrees=args.usedegrees
         )
         scaledmap = make_colorbar_viewingangles_colormap()
 
     first_band_name = None
-    for modelnumber, modelpath in enumerate(modelpaths):
-        modelpath = Path(modelpath)  # Make sure modelpath is defined as path. May not be necessary
-
+    for modelnumber, modelpath in enumerate(Path(m) for m in modelpaths):
         # check if doing viewing angle stuff, and if so define which data to use
         angles, angle_definition = at.lightcurve.parse_directionbin_args(modelpath, args)
 
         for index, angle in enumerate(angles):
             modelname = at.get_model_name(modelpath)
             print(f"Reading spectra: {modelname} (angle {angle})")
             band_lightcurve_data = at.lightcurve.generate_band_lightcurve_data(
```

### Comparing `artistools-2024.4.23/artistools/lightcurve/test_lightcurve.py` & `artistools-2024.4.29/artistools/lightcurve/test_lightcurve.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/lightcurve/viewingangleanalysis.py` & `artistools-2024.4.29/artistools/lightcurve/viewingangleanalysis.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/lightcurve/writebollightcurvedata.py` & `artistools-2024.4.29/artistools/lightcurve/writebollightcurvedata.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/linefluxes.py` & `artistools-2024.4.29/artistools/linefluxes.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/logfiles.py` & `artistools-2024.4.29/artistools/logfiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 import matplotlib.pyplot as plt
 
 import artistools as at
 
 
 def read_logfiles(modelpath):
-    modeldata, _ = at.inputmodel.get_modeldata(modelpath)
-
     mpiranklist = at.get_mpiranklist(modelpath)
     # nprocs = at.get_nprocs(modelpath)
 
     logfilepaths = []
 
     for folderpath in at.get_runfolders(modelpath):
         # for mpirank in range(nprocs):
```

### Comparing `artistools-2024.4.23/artistools/macroatom.py` & `artistools-2024.4.29/artistools/macroatom.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/make_vpkt_input.py` & `artistools-2024.4.29/artistools/make_vpkt_input.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/matplotlibrc` & `artistools-2024.4.29/artistools/matplotlibrc`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/misc.py` & `artistools-2024.4.29/artistools/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from itertools import chain
 from pathlib import Path
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import polars as pl
-import pyzstd
 import xz
+import zstandard as zstd
 from typeguard import typechecked
 
 import artistools as at
 
 roman_numerals = (
     "",
     "I",
@@ -43,14 +43,16 @@
     "XVIII",
     "XIX",
     "XX",
 )
 
 
 class CustomArgHelpFormatter(argparse.ArgumentDefaultsHelpFormatter):
+    """Custom argparse formatter to show default values in help text, sorted with dashes last."""
+
     def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         kwargs["max_help_position"] = 39
         super().__init__(*args, **kwargs)
 
     def add_arguments(self, actions: t.Iterable[argparse.Action]) -> None:
         getinvocation = super()._format_action_invocation
 
@@ -58,14 +60,16 @@
             return getinvocation(action).upper().replace("-", "z")  # push dash chars below alphabet
 
         actions = sorted(actions, key=my_sort)
         super().add_arguments(actions)
 
 
 class AppendPath(argparse.Action):
+    """Append a path to a list of paths."""
+
     def __call__(self, parser, args, values, option_string=None) -> None:  # type: ignore[no-untyped-def] # noqa: ARG002
         # if getattr(args, self.dest) is None:
         #     setattr(args, self.dest, [])
         if hasattr(values, "__iter__"):
             pathlist = getattr(args, self.dest)
             # not pathlist avoids repeated appending of the same items when called from Python
             # instead of from the command line
@@ -143,20 +147,19 @@
     composition_df = pd.DataFrame([(Z, atomic_composition[Z]) for Z in atomic_composition], columns=["Z", "nions"])
     composition_df["lowermost_ion_stage"] = [1] * composition_df.shape[0]
     composition_df["uppermost_ion_stage"] = composition_df["nions"]
     return composition_df
 
 
 def split_dataframe_dirbins(
-    res_df: pl.DataFrame | pd.DataFrame, index_of_repeated_value: int = 0, output_polarsdf: bool = False
+    res_df: pl.DataFrame | pd.DataFrame,
+    index_of_repeated_value: int = 0,  # is the column index to look for repeating eg. time of ts 0. In spec_res files it's 1 , but in lc_res file it's 0.
+    output_polarsdf: bool = False,
 ) -> dict[int, pd.DataFrame | pl.DataFrame]:
-    """Res files repeat output for each angle.
-    index_of_repeated_value is the column index to look for repeating eg. time of ts 0.
-    In spec_res files it's 1 , but in lc_res file it's 0.
-    """
+    """Res (angle-resolved) files include a table for each direction bin."""
     if isinstance(res_df, pd.DataFrame):
         res_df = pl.from_pandas(res_df)
 
     indexes_to_split = pl.arg_where(
         res_df[:, index_of_repeated_value] == res_df[0, index_of_repeated_value], eager=True
     )
 
@@ -248,17 +251,15 @@
         )
 
     return vpkt_config
 
 
 @lru_cache(maxsize=8)
 def get_grid_mapping(modelpath: Path | str) -> tuple[dict[int, list[int]], dict[int, int]]:
-    """Return dict with the associated propagation cells for each model grid cell and
-    a dict with the associated model grid cell of each propagration cell.
-    """
+    """Return dict with the associated propagation cells for each model grid cell and a dict with the associated model grid cell of each propagration cell."""
     modelpath = Path(modelpath)
     filename = firstexisting("grid.out", tryzipped=True, folder=modelpath) if modelpath.is_dir() else Path(modelpath)
 
     assoc_cells: dict[int, list[int]] = {}
     mgi_of_propcells: dict[int, int] = {}
     with zopen(filename) as fgrid:
         for line in fgrid:
@@ -292,15 +293,15 @@
     t_model_days: float | None = None,
     xmax: float | None = None,
 ) -> float:
     """Return the Cartesian cell width [cm] at the model snapshot time."""
     if ngridpoints is None or t_model_days is None or xmax is None:
         # Luke: ngridpoint only equals the number of model cells if the model is 3D
         assert modelpath is not None
-        dfmodel, modelmeta = at.get_modeldata(modelpath, getheadersonly=True)
+        _, modelmeta = at.get_modeldata(modelpath, getheadersonly=True)
         assert modelmeta["dimensions"] == 3
         ngridpoints = modelmeta["npts_model"]
         xmax = modelmeta["vmax_cmps"] * modelmeta["t_model_init_days"] * 86400.0
     assert ngridpoints is not None
     ncoordgridx: int = round(ngridpoints ** (1.0 / 3.0))
 
     assert xmax is not None
@@ -433,21 +434,24 @@
 @typechecked
 def get_time_range(
     modelpath: Path,
     timestep_range_str: str | None = None,
     timemin: float | None = None,
     timemax: float | None = None,
     timedays_range_str: None | str | float = None,
+    clamp_to_timesteps: bool = True,
 ) -> tuple[int, int, float | None, float | None]:
     """Handle a time range specified in either days or timesteps."""
     # assertions make sure time is specified either by timesteps or times in days, but not both!
     tstarts = get_timestep_times(modelpath, loc="start")
     tmids = get_timestep_times(modelpath, loc="mid")
     tends = get_timestep_times(modelpath, loc="end")
 
+    time_days_lower, time_days_upper = None, None
+
     if timemin and timemin > tends[-1]:
         print(f"{get_model_name(modelpath)}: WARNING timemin {timemin} is after the last timestep at {tends[-1]:.1f}")
         return -1, -1, timemin, timemax
     if timemax and timemax < tstarts[0]:
         print(
             f"{get_model_name(modelpath)}: WARNING timemax {timemax} is before the first timestep at {tstarts[0]:.1f}"
         )
@@ -462,14 +466,17 @@
     elif (timemin is not None and timemax is not None) or timedays_range_str is not None:
         # time days range is specified
         timestepmin = None
         timestepmax = None
         if timedays_range_str is not None:
             if isinstance(timedays_range_str, str) and "-" in timedays_range_str:
                 timemin, timemax = (float(timedays) for timedays in timedays_range_str.split("-"))
+                if not clamp_to_timesteps:
+                    time_days_lower = timemin
+                    time_days_upper = timemax
             else:
                 timeavg = float(timedays_range_str)
                 timestepmin = get_timestep_of_timedays(modelpath, timeavg)
                 timestepmax = timestepmin
                 timemin = tstarts[timestepmin]
                 timemax = tends[timestepmax]
                 # timedelta = 10
@@ -491,26 +498,30 @@
         assert timemax is not None
 
         for timestep, tmid in enumerate(tmids):
             if tmid <= float(timemax):
                 timestepmax = timestep
 
         if timestepmax < timestepmin:
-            msg = "Specified time range does not include any full timesteps."
-            raise ValueError(msg)
+            if clamp_to_timesteps:
+                msg = f"Specified time range does not include any full timesteps. {timestepmin=} {timestepmax=}"
+                raise ValueError(msg)
+            timestepmax = timestepmin
     else:
         msg = "Either time or timesteps must be specified."
         raise ValueError(msg)
 
     timesteplast = len(tmids) - 1
     if timestepmax is not None and timestepmax > timesteplast:
         print(f"Warning timestepmax {timestepmax} > timesteplast {timesteplast}")
         timestepmax = timesteplast
-    time_days_lower = float(tstarts[timestepmin])
-    time_days_upper = float(tends[timestepmax])
+    if time_days_lower is None:
+        time_days_lower = float(tstarts[timestepmin]) if clamp_to_timesteps else timemin
+    if time_days_upper is None:
+        time_days_upper = float(tends[timestepmax]) if clamp_to_timesteps else timemax
     assert timestepmin is not None
     assert timestepmax is not None
 
     return timestepmin, timestepmax, time_days_lower, time_days_upper
 
 
 def get_timestep_time(modelpath: Path | str, timestep: int) -> float:
@@ -729,21 +740,21 @@
 
     return f"{get_elsymbol(atomic_number)}{strcharge}"
 
 
 def set_args_from_dict(parser: argparse.ArgumentParser, kwargs: dict[str, t.Any]) -> None:
     """Set argparse defaults from a dictionary."""
     # set_defaults expects the dest of an argument. Here we allow the option strings to be used as keys
-    for arg in parser._actions:
+    for arg in parser._actions:  # noqa: SLF001
         for optstring in arg.option_strings:
             if optstring.lstrip("-") in kwargs and arg.dest not in kwargs:
                 kwargs[arg.dest] = kwargs.pop(optstring.lstrip("-"))
 
     parser.set_defaults(**kwargs)
-    if unknown := {k: v for k, v in kwargs.items() if k not in (arg.dest for arg in parser._actions)}:
+    if unknown := {k: v for k, v in kwargs.items() if k not in (arg.dest for arg in parser._actions)}:  # noqa: SLF001
         msg = f"Unknown argument names: {unknown}"
         raise ValueError(msg)
 
 
 def parse_range(rng: str, dictvars: dict[str, int]) -> t.Iterable[t.Any]:
     """Parse a string with an integer range and return a list of numbers, replacing special variables in dictvars."""
     strparts = rng.split("-")
@@ -805,15 +816,15 @@
         else:
             listout.append(elem)
     return listout
 
 
 def zopen(filename: Path | str, mode: str = "rt", encoding: str | None = None) -> t.Any:
     """Open filename, filename.zst, filename.gz or filename.xz."""
-    ext_fopen: dict[str, t.Callable] = {".zst": pyzstd.open, ".gz": gzip.open, ".xz": xz.open}
+    ext_fopen: dict[str, t.Callable] = {".zst": zstd.open, ".gz": gzip.open, ".xz": xz.open}
 
     for ext, fopen in ext_fopen.items():
         file_withext = str(filename) if str(filename).endswith(ext) else str(filename) + ext
         if Path(file_withext).exists():
             return fopen(file_withext, mode=mode, encoding=encoding)
 
     # open() can raise file not found if this file doesn't exist
@@ -1062,14 +1073,17 @@
 
 
 linetuple = namedtuple("linetuple", "lambda_angstroms atomic_number ion_stage upperlevelindex lowerlevelindex")
 
 
 def read_linestatfile(filepath: Path | str) -> tuple[int, list[float], list[int], list[int], list[int], list[int]]:
     """Load linestat.out containing transitions wavelength, element, ion, upper and lower levels."""
+    if Path(filepath).is_dir():
+        filepath = firstexisting("linestat.out", folder=filepath, tryzipped=True)
+
     print(f"Reading {filepath}")
 
     data = np.loadtxt(zopen(filepath))
     lambda_angstroms = data[0] * 1e8
     nlines = len(lambda_angstroms)
 
     atomic_numbers = data[1].astype(int)
@@ -1321,16 +1335,18 @@
     return list(range(nstart, nstart + ndo))
 
 
 @lru_cache(maxsize=16)
 def get_dfrankassignments(modelpath: Path | str) -> pd.DataFrame | None:
     filerankassignments = Path(modelpath, "modelgridrankassignments.out")
     if filerankassignments.is_file():
-        df = pd.read_csv(filerankassignments, sep=r"\s+")
-        return df.rename(columns={df.columns[0]: str(df.columns[0]).lstrip("#")})
+        dfrankassignments = pd.read_csv(filerankassignments, sep=r"\s+")
+        return dfrankassignments.rename(
+            columns={dfrankassignments.columns[0]: str(dfrankassignments.columns[0]).lstrip("#")}
+        )
     return None
 
 
 def get_mpirankofcell(modelgridindex: int, modelpath: Path | str) -> int:
     """Return the rank number of the MPI process responsible for handling a specified cell's updating and output."""
     modelpath = Path(modelpath)
     npts_model = get_npts_model(modelpath)
@@ -1451,21 +1467,21 @@
 
 
 def get_vspec_dir_labels(modelpath: str | Path, usedegrees: bool = False) -> dict[int, str]:
     vpkt_config = at.get_vpkt_config(modelpath)
     dirlabels = {}
     for dirindex in range(vpkt_config["nobsdirections"]):
         phi_angle = round(vpkt_config["phi"][dirindex])
-        for specindex in range(vpkt_config["nspectraperobs"]):
-            opacity_condition_label = get_opacity_condition_label(int(vpkt_config["z_excludelist"][specindex]))
-            ind_comb = vpkt_config["nspectraperobs"] * dirindex + specindex
+        for opacchoiceindex in range(vpkt_config["nspectraperobs"]):
+            opacity_condition_label = get_opacity_condition_label(int(vpkt_config["z_excludelist"][opacchoiceindex]))
+            ind_comb = vpkt_config["nspectraperobs"] * dirindex + opacchoiceindex
             cos_theta = vpkt_config["cos_theta"][dirindex]
             if usedegrees:
                 theta_degrees = round(math.degrees(math.acos(cos_theta)))
-                dirlabels[ind_comb] = rf"θ = {theta_degrees}°, ϕ = {phi_angle}° {specindex} {opacity_condition_label}"
+                dirlabels[ind_comb] = rf"θ = {theta_degrees}°, ϕ = {phi_angle}° {opacity_condition_label}"
             else:
                 dirlabels[ind_comb] = rf"cos θ = {cos_theta}, ϕ = {phi_angle}° {opacity_condition_label}"
 
     return dirlabels
 
 
 def get_dirbin_labels(
```

### Comparing `artistools-2024.4.23/artistools/nltepops/nltepops.py` & `artistools-2024.4.29/artistools/nltepops/nltepops.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/nltepops/plotnltepops.py` & `artistools-2024.4.29/artistools/nltepops/plotnltepops.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 
     if args.departuremode:
         ax.axhline(y=1.0, color="0.7", linestyle="dashed", linewidth=1.5)
         ax.set_ylabel("Departure coefficient")
 
         ycolumnname = "departure_coeff"
 
-        ax._get_lines.get_next_color()  # skip one color, since T_e is not plotted in departure mode
+        ax._get_lines.get_next_color()  # noqa: SLF001  # skip one color, since T_e is not plotted in departure mode
         if floers_levelnums is not None:
             ax.plot(
                 floers_levelnums,
                 floers_levelpop_values / dfpopthision["n_LTE_T_e_normed"],
                 linewidth=1.5,
                 label=f"{ionstr} Flörs NLTE",
                 linestyle="None",
```

### Comparing `artistools-2024.4.23/artistools/nonthermal/__init__.py` & `artistools-2024.4.29/artistools/nonthermal/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/nonthermal/_nonthermal_core.py` & `artistools-2024.4.29/artistools/nonthermal/_nonthermal_core.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/nonthermal/leptontransport.py` & `artistools-2024.4.29/artistools/nonthermal/leptontransport.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/nonthermal/plotnonthermal.py` & `artistools-2024.4.29/artistools/nonthermal/plotnonthermal.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/nonthermal/solvespencerfanocmd.py` & `artistools-2024.4.29/artistools/nonthermal/solvespencerfanocmd.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/packets/__init__.py` & `artistools-2024.4.29/artistools/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/packets/packets.py` & `artistools-2024.4.29/artistools/packets/packets.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,17 +468,15 @@
         if parquet_mtime > last_textfile_mtime and parquet_mtime > t_lastschemachange:
             conversion_needed = False
         else:
             print(f"  outdated file: {parquetfilepath}. Will overwrite")
 
     if conversion_needed:
         time_start_load = time.perf_counter()
-        print(
-            f"  generating {parquetfilepath.relative_to(modelpath.parent)}. Reading text files...", end="", flush=True
-        )
+        print(f"  generating {parquetfilepath.relative_to(modelpath)}...")
 
         text_file_paths = [
             at.firstexisting(filename, folder=modelpath, tryzipped=True, search_subfolders=True)
             for filename in text_filenames
         ]
 
         column_names = (
@@ -515,15 +513,17 @@
             ).sort(by=["type_id", "escape_type_id", "t_arrive_d"])
 
             syn_dir = at.get_syn_dir(modelpath)
 
             pldf_batch = add_packet_directions_lazypolars(pldf_batch, syn_dir)
             pldf_batch = bin_packet_directions_lazypolars(pldf_batch)
 
-        print(f"took {time.perf_counter() - time_start_load:.1f} seconds. Writing parquet file...", end="", flush=True)
+        print(
+            f"   took {time.perf_counter() - time_start_load:.1f} seconds. Writing parquet file...", end="", flush=True
+        )
         time_start_write = time.perf_counter()
         pldf_batch.sink_parquet(parquetfilepath, compression="zstd", statistics=True, compression_level=8)
         print(f"took {time.perf_counter() - time_start_write:.1f} seconds")
     else:
         print(f"  scanning {parquetfilepath.relative_to(modelpath)}")
 
     return parquetfilepath
@@ -939,24 +939,26 @@
     bins: list[float | int],
     sumcols: list[str] | None = None,
     getcounts: bool = False,
 ) -> pl.LazyFrame:
     """Bins is a list of lower edges, and the final upper edge."""
     # Polars method
 
-    df = df.lazy().with_columns(
-        (pl.col(bincol).cut(breaks=bins, labels=[str(x) for x in range(-1, len(bins))])).alias(f"{bincol}_bin")
+    dfcut = df.lazy().with_columns(
+        (pl.col(bincol).cut(breaks=bins, labels=[str(x) for x in range(-1, len(bins))]))
+        .alias(f"{bincol}_bin")
+        .cast(pl.Int32)
     )
 
     aggs = [pl.col(col).sum().alias(col + "_sum") for col in sumcols] if sumcols is not None else []
 
     if getcounts:
         aggs.append(pl.col(bincol).count().alias("count"))
 
-    wlbins = df.group_by(f"{bincol}_bin").agg(aggs).with_columns(pl.col(f"{bincol}_bin").cast(pl.Int32))
+    wlbins = dfcut.group_by(f"{bincol}_bin").agg(aggs)
 
     # now we will include the empty bins
     return (
         pl.DataFrame({f"{bincol}_bin": range(len(bins) - 1)}, schema={f"{bincol}_bin": pl.Int32})
         .lazy()
         .join(wlbins, how="left", on=f"{bincol}_bin")
         .fill_null(0)
```

### Comparing `artistools-2024.4.23/artistools/packets/packetsplots.py` & `artistools-2024.4.29/artistools/packets/packetsplots.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/packets/test_packets.py` & `artistools-2024.4.29/artistools/packets/test_packets.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/plotspherical.py` & `artistools-2024.4.29/artistools/plotspherical.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         cbar.outline.set_linewidth(0)  # type: ignore[operator]
         cbar.ax.tick_params(axis="both", direction="out")
         cbar.ax.xaxis.set_ticks_position("top")
         # cbar.ax.set_title(colorbartitle)
         cbar.ax.set_xlabel(colorbartitle)
         cbar.ax.xaxis.set_label_position("top")
         if r"{}" in colorbartitle:
-            cbar.ax.xaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(colorbartitle, useMathText=True))
+            cbar.ax.xaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(colorbartitle))
 
         # ax.set_xlabel("Azimuthal angle")
         # ax.set_ylabel("Polar angle")
         # ax.set_xlabel(r"$\phi$")
         # ax.set_ylabel(r"$\theta$")
         # ax.set_xticklabels([])
         # ax.set_yticklabels([])
```

### Comparing `artistools-2024.4.23/artistools/plottools.py` & `artistools-2024.4.29/artistools/plottools.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
     def set_locs(self, locs):
         if self.decimalplaces is not None:
             self.format = f"%1.{self.decimalplaces!s}f"
             if self._usetex:
                 self.format = f"${self.format}$"
             elif self._useMathText:
-                self.format = "$%s$" % ("\\mathdefault{%s}" % self.format)
+                self.format = rf"$\mathdefault{{{self.format}}}$"
+
         super().set_locs(locs)
 
         if self.decimalplaces is not None:
             # rounding the tick labels will make the locations incorrect unless we round these too
             newlocs = [
                 (float(f"%1.{self.decimalplaces!s}f" % (x / (10**self.orderOfMagnitude))) * 10**self.orderOfMagnitude)
                 for x in self.locs
@@ -58,15 +59,15 @@
     def _set_format(self, *args, **kwargs):
         if self.decimalplaces is None:
             return super()._set_format(*args, **kwargs)
 
         sigfigs = self.decimalplaces
         self.format = f"%1.{sigfigs}f"
         if self._usetex or self._useMathText:
-            self.format = r"$\mathdefault{%s}$" % self.format
+            self.format = rf"$\mathdefault{{{self.format}}}$"
 
         return None
 
     def set_axis(self, axis):
         super().set_axis(axis)
         self._set_formatted_label_text()
 
@@ -167,17 +168,15 @@
                 elif plot_axes == "xz" and y == round(ngrid / 2) - 1:
                     data[z, x] = plot_variable_3d_array[x, y, z]
 
     return data, extent
 
 
 def autoscale(ax=None, axis="y", margin=0.1):
-    """Autoscales the x or y axis of a given matplotlib ax object
-    to fit the margins set by manually limits of the other axis,
-    with margins in fraction of the width of the plot.
+    """Autoscales the x or y axis of a given matplotlib ax object to fit the margins set by manually limits of the other axis, with margins in fraction of the width of the plot.
 
     Defaults to current axes object if not specified.
     From https://stackoverflow.com/questions/29461608/matplotlib-fixing-x-axis-scale-and-autoscale-y-axis
     """
 
     def calculate_new_limit(fixed, dependent, limit):
         """Calculate the min/max of the dependent axis given a fixed axis with limits."""
```

### Comparing `artistools-2024.4.23/artistools/radfield.py` & `artistools-2024.4.29/artistools/radfield.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,15 +769,15 @@
     axis.set_ylabel(r"J$_\lambda$ [{}erg/s/cm$^2$/$\mathrm{{\AA}}$]")
     from matplotlib import ticker
 
     axis.xaxis.set_minor_locator(ticker.MultipleLocator(base=500))
     axis.set_xlim(left=xmin, right=xmax)
     axis.set_ylim(bottom=0.0, top=ymax)
 
-    axis.yaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(axis.get_ylabel(), useMathText=True))
+    axis.yaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(axis.get_ylabel()))
 
     axis.legend(loc="best", handlelength=2, frameon=False, numpoints=1, fontsize=9)
 
     print(f"Saving to {outputfile}")
     fig.savefig(str(outputfile), format="pdf")
     plt.close()
     return True
```

### Comparing `artistools-2024.4.23/artistools/spectra/__init__.py` & `artistools-2024.4.29/artistools/spectra/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/spectra/plotspectra.py` & `artistools-2024.4.29/artistools/spectra/plotspectra.py`

 * *Files 7% similar despite different names*

```diff
@@ -242,21 +242,27 @@
     if directionbins is None:
         directionbins = [-1]
 
     if plotpacketcount:
         from_packets = True
 
     for axindex, axis in enumerate(axes):
+        clamp_to_timesteps = not args.notimeclamp
         if args.multispecplot:
             (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
-                modelpath, timedays_range_str=args.timedayslist[axindex]
+                modelpath, timedays_range_str=args.timedayslist[axindex], clamp_to_timesteps=clamp_to_timesteps
             )
         else:
             (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
-                modelpath, args.timestep, args.timemin, args.timemax, args.timedays
+                modelpath,
+                args.timestep,
+                args.timemin,
+                args.timemax,
+                args.timedays,
+                clamp_to_timesteps=clamp_to_timesteps,
             )
 
         modelname = at.get_model_name(modelpath)
         if timestepmin == timestepmax == -1:
             return None
 
         assert args.timemin is not None
@@ -273,15 +279,15 @@
             if not args.hidemodeltimerange and not args.multispecplot and timedelta >= 0.1:
                 linelabel += rf" ($\pm$ {timedelta:.1f}d)"
         # Luke: disabled below because line label has already been formatted with e.g. timeavg values
         # formatting for a second time makes it impossible to use curly braces in line labels (needed for LaTeX math)
         # else:
         #     linelabel = linelabel.format(**locals())
         print(
-            f"====> '{linelabel}' timesteps {timestepmin} to {timestepmax} ({args.timemin:.3f} to {args.timemax:.3f}d)"
+            f"====> '{linelabel}' timesteps {timestepmin} to {timestepmax} ({args.timemin:.3f} to {args.timemax:.3f}d{'' if clamp_to_timesteps else ' not necessarily clamped to timestep start/end'})"
         )
         print(f" modelpath {modelpath}")
 
         viewinganglespectra = {}
 
         supxmin, supxmax = axis.get_xlim()
         if from_packets:
@@ -357,19 +363,15 @@
         for dirbin in directionbins:
             if len(directionbins) > 1 and dirbin != directionbins[0]:
                 # only one colour was specified, but we have multiple direction bins
                 # to zero out all but the first one
                 plotkwargs = plotkwargs.copy()
                 plotkwargs["color"] = None
 
-            dfspectrum = (
-                pl.from_pandas(viewinganglespectra[dirbin])
-                if isinstance(viewinganglespectra[dirbin], pd.DataFrame)
-                else viewinganglespectra[dirbin].lazy().collect()
-            )
+            dfspectrum = viewinganglespectra[dirbin].lazy().collect()
             dfspectrum = dfspectrum.filter(pl.col("lambda_angstroms").is_between(supxmin * 0.9, supxmax * 1.1))
 
             linelabel_withdirbin = linelabel
             if dirbin != -1:
                 print(f" direction {dirbin:4d}  {dirbin_definitions[dirbin]}")
                 if len(directionbins) > 1 or not linelabel_is_custom:
                     linelabel_withdirbin = linelabel + " " + dirbin_definitions[dirbin]
@@ -418,17 +420,17 @@
 
 def make_spectrum_plot(
     speclist: t.Collection[Path | str],
     axes: t.Sequence[plt.Axes],
     filterfunc: t.Callable[[np.ndarray], np.ndarray] | None,
     args,
     scale_to_peak: float | None = None,
-) -> pd.DataFrame:
+) -> pl.DataFrame:
     """Plot reference spectra and ARTIS spectra."""
-    dfalldata = pd.DataFrame()
+    dfalldata = pl.DataFrame()
     artisindex = 0
     refspecindex = 0
     seriesindex = 0
 
     # take any specified colours our of the cycle
     colors = [
         color for i, color in enumerate(plt.rcParams["axes.prop_cycle"].by_key()["color"]) if f"C{i}" not in args.color
@@ -445,15 +447,15 @@
         }
 
         if args.dashes[seriesindex]:
             plotkwargs["dashes"] = args.dashes[seriesindex]
         if args.linewidth[seriesindex]:
             plotkwargs["linewidth"] = args.linewidth[seriesindex]
 
-        seriesdata = pd.DataFrame()
+        seriesdata: pl.DataFrame | None
         if (
             Path(specpath).is_file()
             or Path(at.get_config()["path_artistools_dir"], "data", "refspectra", specpath).is_file()
             or Path(at.get_config()["path_artistools_dir"], "data", "refspectra", f"{specpath!s}.xz").is_file()
             or Path(at.get_config()["path_artistools_dir"], "data", "refspectra", f"{specpath!s}.zstd").is_file()
         ):
             # reference spectrum
@@ -485,15 +487,15 @@
                         scale_to_peak,
                         scaletoreftime=args.scaletoreftime,
                         **plotkwargs,
                     )
             refspecindex += 1
         elif not specpath.exists() and specpath.parts[0] == "codecomparison":
             # timeavg = (args.timemin + args.timemax) / 2.
-            (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
+            (_timestepmin, _timestepmax, args.timemin, args.timemax) = at.get_time_range(
                 specpath, args.timestep, args.timemin, args.timemax, args.timedays
             )
             timeavg = args.timedays
             at.codecomparison.plot_spectrum(specpath, timedays=timeavg, ax=axes[0], **plotkwargs)
             refspecindex += 1
         else:
             # ARTIS model spectrum
@@ -524,22 +526,21 @@
                 print(e)
                 continue
 
             if seriesdata is not None:
                 seriesname = at.get_model_name(specpath)
                 artisindex += 1
 
-        if args.write_data and not seriesdata.empty:
-            if dfalldata.empty:
-                dfalldata = pd.DataFrame(index=seriesdata["lambda_angstroms"].to_numpy())
-                dfalldata.index.name = "lambda_angstroms"
+        if args.write_data and seriesdata is not None:
+            if dfalldata.is_empty():
+                dfalldata = pl.DataFrame({"lambda_angstroms": seriesdata["lambda_angstroms"]})
             else:
                 # make sure we can share the same set of wavelengths for this series
-                assert np.allclose(dfalldata.index.values, seriesdata["lambda_angstroms"].to_numpy())
-            dfalldata[f"f_lambda.{seriesname}"] = seriesdata["f_lambda"].to_numpy()
+                assert np.allclose(dfalldata["lambda_angstroms"], seriesdata["lambda_angstroms"].to_numpy())
+            dfalldata = dfalldata.with_columns(seriesdata["f_lambda"].alias(f"f_lambda.{seriesname}"))
 
     plottedsomething = artisindex > 0 or refspecindex > 0
     assert plottedsomething
 
     for axis in axes:
         if args.showfilterfunctions:
             if not args.normalised:
@@ -592,40 +593,44 @@
 
 def make_emissionabsorption_plot(
     modelpath: Path,
     axis: plt.Axes,
     filterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
     args=None,
     scale_to_peak: float | None = None,
-) -> tuple[list[Artist], list[str], pd.DataFrame | None]:
+) -> tuple[list[Artist], list[str], pl.DataFrame | None]:
     """Plot the emission and absorption contribution spectra, grouped by ion/line/term for an ARTIS model."""
     modelname = at.get_model_name(modelpath)
 
     print(f"====> {modelname}")
-    arraynu = at.get_nu_grid(modelpath)
+    clamp_to_timesteps = not args.notimeclamp
 
     (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
-        modelpath, args.timestep, args.timemin, args.timemax, args.timedays
+        modelpath, args.timestep, args.timemin, args.timemax, args.timedays, clamp_to_timesteps=clamp_to_timesteps
     )
 
     if timestepmin == timestepmax == -1:
         print(f"Can't plot {modelname}...skipping")
         return [], [], None
 
+    if args.plotvspecpol and not args.frompackets:
+        args.frompackets = True
+        print("Enabling --frompackets, since --plotvspecpol was specified")
+
     assert args.timemin is not None
     assert args.timemax is not None
 
-    print(f"Plotting {modelname} timesteps {timestepmin} to {timestepmax} ({args.timemin:.3f} to {args.timemax:.3f}d)")
+    print(
+        f"Plotting {modelname} timesteps {timestepmin} to {timestepmax} ({args.timemin:.3f} to {args.timemax:.3f}d{'' if clamp_to_timesteps else ' not necessarily clamped to timestep start/end'})"
+    )
 
     xmin, xmax = axis.get_xlim()
 
+    dirbin = args.plotviewingangle[0] if args.plotviewingangle else args.plotvspecpol[0] if args.plotvspecpol else None
     if args.frompackets:
-        dirbin = (
-            args.plotviewingangle[0] if args.plotviewingangle else args.plotvspecpol[0] if args.plotvspecpol else None
-        )
         (
             contribution_list,
             array_flambda_emission_total,
             arraylambda_angstroms,
         ) = at.spectra.get_flux_contributions_from_packets(
             modelpath,
             args.timemin,
@@ -642,26 +647,28 @@
             delta_lambda=args.deltalambda,
             use_lastemissiontype=not args.use_thermalemissiontype,
             emissionvelocitycut=args.emissionvelocitycut,
             directionbin=dirbin,
             average_over_phi=args.average_over_phi_angle,
             average_over_theta=args.average_over_theta_angle,
             directionbins_are_vpkt_observers=args.plotvspecpol is not None,
+            vpkt_match_emission_exclusion_to_opac=args.vpkt_match_emission_exclusion_to_opac,
         )
     else:
-        arraylambda_angstroms = 2.99792458e18 / arraynu
+        assert not args.vpkt_match_emission_exclusion_to_opac
+        arraylambda_angstroms = 2.99792458e18 / at.get_nu_grid(modelpath)
         contribution_list, array_flambda_emission_total = at.spectra.get_flux_contributions(
             modelpath,
             filterfunc,
             timestepmin,
             timestepmax,
             getemission=args.showemission,
             getabsorption=args.showabsorption,
             use_lastemissiontype=not args.use_thermalemissiontype,
-            directionbin=args.plotviewingangle[0] if args.plotviewingangle else None,
+            directionbin=dirbin,
             average_over_phi=args.average_over_phi_angle,
             average_over_theta=args.average_over_theta_angle,
         )
 
     at.spectra.print_integrated_flux(array_flambda_emission_total, arraylambda_angstroms)
 
     # print("\n".join([f"{x[0]}, {x[1]}" for x in contribution_list]))
@@ -688,21 +695,24 @@
     if not args.hidenetspectrum:
         plotobjectlabels.append("Spectrum")
         (line,) = axis.plot(
             arraylambda_angstroms, array_flambda_emission_total * scalefactor, linewidth=1.5, color="black", zorder=100
         )
         plotobjects.append(line)
 
-    dfaxisdata = pd.DataFrame(index=arraylambda_angstroms)
-    dfaxisdata.index.name = "lambda_angstroms"
+    dfaxisdata = pl.DataFrame({"lambda_angstroms": arraylambda_angstroms})
     # dfaxisdata['nu_hz'] = arraynu
     for x in contributions_sorted_reduced:
-        dfaxisdata["emission_flambda." + x.linelabel] = x.array_flambda_emission
+        dfaxisdata = dfaxisdata.with_columns(
+            pl.Series(name="emission_flambda." + x.linelabel, values=x.array_flambda_emission)
+        )
         if args.showabsorption:
-            dfaxisdata["absorption_flambda." + x.linelabel] = x.array_flambda_absorption
+            dfaxisdata = dfaxisdata.with_columns(
+                pl.Series(name="absorption_flambda." + x.linelabel, values=x.array_flambda_absorption)
+            )
 
     if args.nostack:
         for x in contributions_sorted_reduced:
             if args.showemission:
                 (emissioncomponentplot,) = axis.plot(
                     arraylambda_angstroms, x.array_flambda_emission * scalefactor, linewidth=1, color=x.color
                 )
@@ -784,23 +794,27 @@
 
     axis.axhline(color="black", linewidth=1)
 
     if args.title:
         plotlabel = args.title
     else:
         plotlabel = f"{modelname}\n{args.timemin:.2f}d to {args.timemax:.2f}d"
-        if args.plotviewingangle:
-            dirbin_definitions = at.get_dirbin_labels(
-                dirbins=args.plotviewingangle,
-                modelpath=modelpath,
-                average_over_phi=args.average_over_phi_angle,
-                average_over_theta=args.average_over_theta_angle,
-                usedegrees=args.usedegrees,
+        if args.plotviewingangle or args.plotvspecpol:
+            dirbin_definitions = (
+                at.get_vspec_dir_labels(modelpath=modelpath, usedegrees=args.usedegrees)
+                if args.plotvspecpol
+                else at.get_dirbin_labels(
+                    dirbins=args.plotviewingangle,
+                    modelpath=modelpath,
+                    average_over_phi=args.average_over_phi_angle,
+                    average_over_theta=args.average_over_theta_angle,
+                    usedegrees=args.usedegrees,
+                )
             )
-            plotlabel += f", directionbin {dirbin_definitions[args.plotviewingangle[0]]}"
+            plotlabel += f", {dirbin_definitions[dirbin]}"
 
     if not args.notitle:
         if args.inset_title:
             axis.annotate(
                 plotlabel,
                 xy=(0.03, 0.96),
                 xycoords="axes fraction",
@@ -825,15 +839,15 @@
         binedges = at.radfield.get_binedges(radfielddata)
         axis.vlines(binedges, ymin=0.0, ymax=ymax, linewidth=0.5, color="red", label="", zorder=-1, alpha=0.4)
 
     return plotobjects, plotobjectlabels, dfaxisdata
 
 
 def make_contrib_plot(axes: t.Iterable[plt.Axes], modelpath: Path, densityplotyvars: list[str], args) -> None:
-    (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
+    (_timestepmin, _timestepmax, args.timemin, args.timemax) = at.get_time_range(
         modelpath, args.timestep, args.timemin, args.timemax, args.timedays
     )
 
     modeldata, _ = at.inputmodel.get_modeldata(modelpath)
 
     if args.classicartis:
         modeldata, _ = at.inputmodel.get_modeldata(modelpath)
@@ -917,15 +931,15 @@
         #
         # nbins = 30
         # xi, yi = np.mgrid[x.min():x.max():nbins*1j, y.min():y.max():nbins*1j]
         # zi = k(np.vstack([xi.flatten(), yi.flatten()]))
         # ax.pcolormesh(xi, yi, zi.reshape(xi.shape), shading='gouraud', cmap=plt.cm.BuGn_r)
 
 
-def make_plot(args) -> tuple[plt.Figure, list[plt.Axes], pd.DataFrame]:
+def make_plot(args) -> tuple[plt.Figure, list[plt.Axes], pl.DataFrame]:
     # font = {'size': 16}
     # mpl.rc('font', **font)
 
     densityplotyvars: list[str] = []
     # densityplotyvars = ['emission_velocity', 'Te', 'nne']
     # densityplotyvars = ['true_emission_velocity', 'emission_velocity', 'Te', 'nne']
 
@@ -950,15 +964,15 @@
 
     axes = [axes] if nrows == 1 else list(axes)
 
     filterfunc = at.get_filterfunc(args)
 
     scale_to_peak = 1.0 if args.normalised else None
 
-    dfalldata = pd.DataFrame()
+    dfalldata: pl.DataFrame | None = pl.DataFrame()
 
     if not args.hideyticklabels:
         if args.multispecplot:
             for ax in axes:
                 ax.set_ylabel(r"F$_\lambda$ at 1 Mpc [{}erg/s/cm$^2$/$\mathrm{{\AA}}$]")
 
         elif args.logscale:
@@ -1042,17 +1056,15 @@
     if args.ymax is not None:
         axes[-1].set_ylim(top=args.ymax)
 
     for index, ax in enumerate(axes):
         # ax.xaxis.set_major_formatter(plt.NullFormatter())
 
         if "{" in ax.get_ylabel() and not args.logscale:
-            ax.yaxis.set_major_formatter(
-                at.plottools.ExponentLabelFormatter(ax.get_ylabel(), useMathText=True, decimalplaces=1)
-            )
+            ax.yaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(ax.get_ylabel(), decimalplaces=1))
 
         if args.hidexticklabels:
             ax.tick_params(
                 axis="x",
                 which="both",
                 labelbottom=False,
             )
@@ -1061,15 +1073,15 @@
                 axis="y",
                 which="both",
                 labelleft=False,
             )
         ax.set_xlabel("")
 
         if args.multispecplot and args.showtime:
-            ymin, ymax = ax.get_ylim()
+            _ymin, ymax = ax.get_ylim()
             ax.text(5500, ymax * 0.9, f"{args.timedayslist[index]} days")  # multispecplot text
 
     if not args.hidexticklabels:
         axes[-1].set_xlabel(args.xlabel)
 
     if not args.outputfile:
         args.outputfile = defaultoutputfile
@@ -1090,14 +1102,15 @@
             xy=(0.03, 0.97),
             xycoords="axes fraction",
             horizontalalignment="left",
             verticalalignment="top",
             fontsize="x-large",
         )
 
+    assert dfalldata is not None
     return fig, axes, dfalldata
 
 
 def addargs(parser) -> None:
     parser.add_argument(
         "specpath",
         default=[],
@@ -1179,14 +1192,18 @@
     )
 
     parser.add_argument("-timemin", type=float, help="Lower time in days to integrate spectrum")
 
     parser.add_argument("-timemax", type=float, help="Upper time in days to integrate spectrum")
 
     parser.add_argument(
+        "--notimeclamp", action="store_true", help="When plotting from packets, don't clamp to timestep start/end"
+    )
+
+    parser.add_argument(
         "-xmin", "-lambdamin", dest="xmin", type=int, default=2500, help="Plot range: minimum wavelength in Angstroms"
     )
 
     parser.add_argument(
         "-xmax", "-lambdamax", dest="xmax", type=int, default=19000, help="Plot range: maximum wavelength in Angstroms"
     )
 
@@ -1282,14 +1299,16 @@
 
     parser.add_argument("--write_data", action="store_true", help="Save data used to generate the plot in a CSV file")
 
     parser.add_argument(
         "-outputfile", "-o", action="store", dest="outputfile", type=Path, help="path/filename for PDF file"
     )
 
+    parser.add_argument("-dpi", type=int, default=250, help="Dots Per Inch for output file")
+
     parser.add_argument(
         "--output_spectra", "--write_spectra", action="store_true", help="Write out all timestep spectra to text files"
     )
 
     # Combines all vspecpol files into one file which can then be read by artistools
     parser.add_argument(
         "--makevspecpol", action="store_true", help="Make file summing the virtual packet spectra from all ranks"
@@ -1360,14 +1379,20 @@
 
     parser.add_argument("--showtime", action="store_true", help="Write time on plot")
 
     parser.add_argument(
         "--classicartis", action="store_true", help="Flag to show using output from classic ARTIS branch"
     )
 
+    parser.add_argument(
+        "--vpkt_match_emission_exclusion_to_opac",
+        action="store_true",
+        help="Exclude packets with emission type no-bb/no-bf/no-(element) matching the vpkt opacity exclusion",
+    )
+
 
 def main(args: argparse.Namespace | None = None, argsraw: t.Sequence[str] | None = None, **kwargs) -> None:
     """Plot spectra from ARTIS and reference data."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
             description=__doc__,
@@ -1411,14 +1436,19 @@
                 args.color.append(refspeccolors[refspecnum])
                 refspecnum += 1
 
     args.color, args.label, args.linestyle, args.linealpha, args.dashes, args.linewidth = at.trim_or_pad(
         len(args.specpath), args.color, args.label, args.linestyle, args.linealpha, args.dashes, args.linewidth
     )
 
+    if args.vpkt_match_emission_exclusion_to_opac:
+        assert args.showemission
+        assert args.frompackets
+        assert args.plotvspecpol
+
     if args.emissionvelocitycut or args.groupby == "line":
         args.frompackets = True
 
     if args.makevspecpol:
         at.spectra.make_virtual_spectra_summed_file(args.specpath[0])
         return
 
@@ -1446,22 +1476,22 @@
             if args.plotviewingangle
             else ""
         )
         filenameout = str(args.outputfile).format(
             time_days_min=args.timemin, time_days_max=args.timemax, directionbins=strdirectionbins
         )
 
-        if args.write_data and not dfalldata.empty:
+        if args.write_data and len(dfalldata.columns) > 0:
             datafilenameout = Path(filenameout).with_suffix(".txt")
-            dfalldata.to_csv(datafilenameout)
+            dfalldata.write_csv(datafilenameout, separator=" ")
             print(f"Saved {datafilenameout}")
 
         # plt.minorticks_on()
 
-        fig.savefig(filenameout)
+        fig.savefig(filenameout, dpi=args.dpi)
         # plt.show()
         print(f"Saved {filenameout}")
         plt.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2024.4.23/artistools/spectra/sampleblackbodyfrompacket_tr.py` & `artistools-2024.4.29/artistools/spectra/sampleblackbodyfrompacket_tr.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
                     / PARSEC
                     * n_angle_bins
                     / nprocs
                 )
                 # packet_contribution_count_res[angle][timedays] += 1
 
 for angle in range(n_angle_bins):
-    df = pd.DataFrame.from_dict(specpol_res_data_bb[angle])
+    dfspec = pd.DataFrame.from_dict(specpol_res_data_bb[angle])
     if angle == 0:
-        df.to_csv(modelpath / "spec_res_bb.out", sep=" ", index=False)  # create file
+        dfspec.to_csv(modelpath / "spec_res_bb.out", sep=" ", index=False)  # create file
     else:
         # append to file
-        df.to_csv(modelpath / "spec_res_bb.out", mode="a", sep=" ", index=False)
+        dfspec.to_csv(modelpath / "spec_res_bb.out", mode="a", sep=" ", index=False)
 
 print("Blackbody spectra written to spec_res_bb.out")
```

### Comparing `artistools-2024.4.23/artistools/spectra/spectra.py` & `artistools-2024.4.29/artistools/spectra/spectra.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,15 @@
             mnubins = dfspec.height
 
         nu_centre_min = dfspec.item(0, 0)
         nu_centre_max = dfspec.item(dfspec.height - 1, 0)
 
         # This is not an exact solution for dlognu since we're assuming the bin centre spacing matches the bin edge spacing
         # but it's close enough for our purposes and avoids the difficulty of finding the exact solution (lots more algebra)
-        dlognu = math.log(
-            dfspec.item(1, 0) / dfspec.item(0, 0)  # second nu value divided by the first nu value
-        )
+        dlognu = math.log(dfspec.item(1, 0) / dfspec.item(0, 0))  # second nu value divided by the first nu value
 
         if nu_min_r is None:
             nu_min_r = nu_centre_min / (1 + 0.5 * dlognu)
 
         if nu_max_r is None:
             nu_max_r = nu_centre_max * (1 + 0.5 * dlognu)
 
@@ -313,15 +311,15 @@
                 )
 
             dfbinned_lazy = dfbinned_lazy.join(dfbinned_dirbin, on="lambda_binindex", how="left")
 
     if fluxfilterfunc:
         print("Applying filter to ARTIS spectrum")
         dfbinned_lazy = dfbinned_lazy.with_columns(
-            cs.starts_with("f_lambda_dirbin").map(lambda x: fluxfilterfunc(x.to_numpy()))
+            cs.starts_with("f_lambda_").map(lambda x: fluxfilterfunc(x.to_numpy()))
         )
 
     dfbinned = dfbinned_lazy.collect(streaming=True)
     assert isinstance(dfbinned, pl.DataFrame)
 
     dfdict = {}
     for dirbin in directionbins:
@@ -446,14 +444,15 @@
 ) -> dict[int, pl.DataFrame]:
     """Return a pandas DataFrame containing an ARTIS emergent spectrum."""
     if timestepmax is None or timestepmax < 0:
         timestepmax = timestepmin
 
     if directionbins is None:
         directionbins = [-1]
+
     # keys are direction bins (or -1 for spherical average)
     specdata: dict[int, pl.DataFrame] = {}
 
     if any(dirbin != -1 for dirbin in directionbins):
         assert stokesparam == "I"
         try:
             specdata |= get_spec_res(
@@ -466,51 +465,52 @@
             print(msg)
             directionbins = [-1]
 
     if -1 in directionbins:
         # spherically averaged spectra
         if stokesparam == "I":
             try:
-                specdata[-1] = read_spec(modelpath=modelpath).to_pandas(use_pyarrow_extension_array=True)
+                specdata[-1] = read_spec(modelpath=modelpath)
 
             except FileNotFoundError:
-                specdata[-1] = get_specpol_data(angle=-1, modelpath=modelpath)[stokesparam]
+                specdata[-1] = pl.from_pandas(get_specpol_data(angle=-1, modelpath=modelpath)[stokesparam])
 
         else:
-            specdata[-1] = get_specpol_data(angle=-1, modelpath=modelpath)[stokesparam]
+            specdata[-1] = pl.from_pandas(get_specpol_data(angle=-1, modelpath=modelpath)[stokesparam])
 
     specdataout: dict[int, pl.DataFrame] = {}
     for dirbin in directionbins:
         if dirbin not in specdata:
             print(f"WARNING: Direction bin {dirbin} not found in specdata. Dirbins: {list(specdata.keys())}")
             continue
-        arr_nu = specdata[dirbin]["nu"].to_numpy()
         arr_tdelta = at.get_timestep_times(modelpath, loc="delta")
 
         try:
-            arr_f_nu = stackspectra(
-                [
-                    (specdata[dirbin][specdata[dirbin].columns[timestep + 1]].to_numpy(), arr_tdelta[timestep])
+            arr_f_nu = specdata[dirbin].select(
+                pl.sum_horizontal(
+                    pl.col(specdata[dirbin].columns[timestep + 1]) * arr_tdelta[timestep]
                     for timestep in range(timestepmin, timestepmax + 1)
-                ]
+                )
+                / sum(arr_tdelta[timestepmin : timestepmax + 1])
             )
-        except IndexError:
-            print(" ERROR: data not available for timestep range")
-            return specdataout
-
-        if fluxfilterfunc:
-            if dirbin == directionbins[0]:
-                print("Applying filter to ARTIS spectrum")
-            arr_f_nu = fluxfilterfunc(arr_f_nu)
+        except IndexError as e:
+            msg = " ERROR: data not available for timestep range"
+            raise ValueError(msg) from e
 
+        arr_nu = specdata[dirbin]["nu"]
         arr_lambda = 2.99792458e18 / arr_nu
         dfspectrum = pl.DataFrame({"lambda_angstroms": arr_lambda, "f_lambda": arr_f_nu * arr_nu / arr_lambda}).sort(
             by="lambda_angstroms"
         )
 
+        if fluxfilterfunc:
+            if dirbin == directionbins[0]:
+                print("Applying filter to ARTIS spectrum")
+            dfspectrum = dfspectrum.with_columns(cs.starts_with("f_lambda").map(lambda x: fluxfilterfunc(x.to_numpy())))
+
         specdataout[dirbin] = dfspectrum
 
     return specdataout
 
 
 def make_virtual_spectra_summed_file(modelpath: Path) -> Path:
     nprocs = at.get_nprocs(modelpath)
@@ -657,51 +657,55 @@
     angle: int,
     args: argparse.Namespace,
     fluxfilterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
 ) -> pl.DataFrame:
     stokes_params = get_vspecpol_data(vspecangle=angle, modelpath=Path(modelpath))
     if "stokesparam" not in args:
         args.stokesparam = "I"
-    vspecdata = stokes_params[args.stokesparam]
-
-    nu = vspecdata.loc[:, "nu"].to_numpy()
+    vspecdata = pl.from_pandas(stokes_params[args.stokesparam])
 
-    arr_tmid = [float(i) for i in vspecdata.columns.to_numpy()[1:]]
+    arr_tmid = [float(i) for i in vspecdata.columns[1:]]
+    vspec_timesteps = range(len(arr_tmid))
     arr_tdelta = [l1 - l2 for l1, l2 in zip(arr_tmid[1:], arr_tmid[:-1])] + [arr_tmid[-1] - arr_tmid[-2]]
 
-    def match_closest_time(reftime: float) -> str:
-        return str(min(arr_tmid, key=lambda x: abs(x - reftime)))
+    def match_closest_time(reftime: float) -> int:
+        return min(vspec_timesteps, key=lambda ts: abs(arr_tmid[ts] - reftime))
 
-    # if 'timemin' and 'timemax' in args:
-    #     timelower = match_closest_time(args.timemin)  # how timemin, timemax are used changed at some point
-    #     timeupper = match_closest_time(args.timemax)  # to average over multiple timesteps needs to fix this
-    # else:
-    timelower = match_closest_time(timeavg)
-    timeupper = match_closest_time(timeavg)
-    timestepmin = vspecdata.columns.get_loc(timelower)
-    timestepmax = vspecdata.columns.get_loc(timeupper)
+    if "timemin" and "timemax" in args:
+        timestepmin = match_closest_time(args.timemin)  # how timemin, timemax are used changed at some point
+        timestepmax = match_closest_time(args.timemax)  # to average over multiple timesteps needs to fix this
+    else:
+        timestepmin = match_closest_time(timeavg)
+        timestepmax = match_closest_time(timeavg)
+
+    timelower = arr_tmid[timestepmin]
+    timeupper = arr_tmid[timestepmax]
     print(f" vpacket spectrum timesteps {timestepmin} ({timelower}d) to {timestepmax} ({timeupper}d)")
 
-    f_nu = stackspectra(
-        [
-            (vspecdata[vspecdata.columns[timestep + 1]].to_numpy(), arr_tdelta[timestep])
-            for timestep in range(timestepmin - 1, timestepmax)
-        ]
+    dfout = (
+        vspecdata.select(
+            f_nu=(
+                pl.sum_horizontal(
+                    pl.col(vspecdata.columns[timestep + 1]) * arr_tdelta[timestep]
+                    for timestep in range(timestepmin, timestepmax + 1)
+                )
+                / sum(arr_tdelta[timestepmin : timestepmax + 1])
+            ),
+            nu=vspecdata["nu"],
+        )
+        .with_columns(lambda_angstroms=2.99792458e18 / pl.col("nu"))
+        .sort(by="lambda_angstroms")
+        .with_columns(f_lambda=pl.col("f_nu") * pl.col("nu") / pl.col("lambda_angstroms"))
     )
 
     if fluxfilterfunc:
         print("Applying filter to ARTIS spectrum")
-        f_nu = fluxfilterfunc(f_nu)
+        dfout = dfout.with_columns(cs.starts_with("f_lambda").map(lambda x: fluxfilterfunc(x.to_numpy())))
 
-    return (
-        pl.DataFrame({"nu": nu, "f_nu": f_nu})
-        .sort(by="nu", descending=True)
-        .with_columns(lambda_angstroms=2.99792458e18 / pl.col("nu"))
-        .with_columns(f_lambda=pl.col("f_nu") * pl.col("nu") / pl.col("lambda_angstroms"))
-    )
+    return dfout
 
 
 @lru_cache(maxsize=4)
 def get_flux_contributions(
     modelpath: Path,
     filterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
     timestepmin: int = -1,
@@ -892,14 +896,15 @@
     use_time: t.Literal["arrival", "emission", "escape"] = "arrival",
     use_lastemissiontype: bool = True,
     emissionvelocitycut: float | None = None,
     directionbin: int | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
     directionbins_are_vpkt_observers: bool = False,
+    vpkt_match_emission_exclusion_to_opac: bool = False,
 ) -> tuple[list[fluxcontributiontuple], np.ndarray, np.ndarray]:
     assert groupby in {"ion", "line"}
 
     if directionbin is None:
         directionbin = -1
 
     emtypecolumn = "emissiontype" if use_lastemissiontype else "trueemissiontype"
@@ -982,17 +987,28 @@
                 bflistlazy.select(
                     [
                         pl.col(emtypecolumn),
                         expr_bflist_to_str.alias("emissiontype_str"),
                     ]
                 ),
             ],
-        ).with_columns(pl.col("emissiontype_str").cast(pl.Categorical))
+        )
 
         lzdfpackets = lzdfpackets.join(emtypestrings, on=emtypecolumn, how="left")
+        z_exclude = int(vpkt_config["z_excludelist"][opacchoiceindex])
+        if vpkt_match_emission_exclusion_to_opac:
+            if z_exclude == -1:
+                # no bound-bound
+                lzdfpackets = lzdfpackets.filter(pl.col("emissiontype_str").str.contains("bound-free"))
+            elif z_exclude == -2:
+                # no bound-free
+                lzdfpackets = lzdfpackets.filter(pl.col("emissiontype_str").str.contains("bound-free").is_not())
+            elif z_exclude > 0:
+                elsymb = at.get_elsymbol(z_exclude)
+                lzdfpackets = lzdfpackets.filter(pl.col("emissiontype_str").str.starts_with(f"{elsymb} ").is_not())
 
     if getabsorption:
         cols |= {"absorptiontype_str", "absorption_freq"}
 
         abstypestrings = pl.concat(
             [
                 linelistlazy.select(
```

### Comparing `artistools-2024.4.23/artistools/spectra/test_spectra.py` & `artistools-2024.4.29/artistools/spectra/test_spectra.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/spectra/test_vspectra.py` & `artistools-2024.4.29/artistools/spectra/test_vspectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 @mock.patch.object(matplotlib.axes.Axes, "plot", side_effect=matplotlib.axes.Axes.plot, autospec=True)
 def test_vspectraplot(mockplot):
     at.spectra.plot(
         argsraw=[],
         specpath=[at.get_config()["path_testdata"] / "vspecpolmodel", "sn2011fe_PTF11kly_20120822_norm.txt"],
         outputfile=at.get_config()["path_testoutput"] / "test_vspectra.pdf",
         plotvspecpol=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
-        timemin=10,
+        timemin=11,
         timemax=12,
     )
 
     arr_time_d = np.array(mockplot.call_args_list[0][0][1])
     assert all(np.array_equal(arr_time_d, np.array(mockplot.call_args_list[vspecdir][0][1])) for vspecdir in range(10))
 
     arr_allvspec = np.vstack([np.array(mockplot.call_args_list[vspecdir][0][2]) for vspecdir in range(10)])
@@ -33,15 +33,15 @@
             2.85477069e-12,
             3.34384407e-12,
             2.94892344e-12,
             2.29084411e-12,
             2.05916843e-12,
             2.00515984e-12,
         ],
-        atol=1e-20,
+        atol=1e-16,
     )
 
     assert np.allclose(
         arr_allvspec.mean(axis=1),
         [
             2.9864681492951925e-12,
             3.0063451037690416e-12,
@@ -50,15 +50,15 @@
             4.097482117229833e-12,
             4.663450168092402e-12,
             4.231106733071208e-12,
             3.350080172063692e-12,
             3.0234533505898177e-12,
             2.9721539798925583e-12,
         ],
-        atol=1e-20,
+        atol=1e-16,
     )
 
 
 @mock.patch.object(matplotlib.axes.Axes, "plot", side_effect=matplotlib.axes.Axes.plot, autospec=True)
 def test_vpkt_contrib_spectrum_plot(mockplot):
     at.spectra.plot(
         argsraw=[],
```

### Comparing `artistools-2024.4.23/artistools/spectra/writespectra.py` & `artistools-2024.4.29/artistools/spectra/writespectra.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/stats.py` & `artistools-2024.4.29/artistools/stats.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/test_artistools.py` & `artistools-2024.4.29/artistools/test_artistools.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/transitions.py` & `artistools-2024.4.29/artistools/transitions.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/artistools/viewing_angles_visualization.py` & `artistools-2024.4.29/artistools/viewing_angles_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,16 +91,15 @@
     isomax=None,
     opacity=2.5,
     surface_count=20,
     linewidth=2.5,
     linelength=1.0,
     show_plot=False,
 ):
-    """Tool to generate a 3D visualization of an ARTIS model.
-    Viewing angle bins will get overplottet with an animation.
+    """Tool to generate a 3D visualization of an ARTIS model. Viewing angle bins will get overplotted with an animation.
 
     Parameters
     ----------
     modelfile : str
         File where ARTIS  model is stored.
     outfile : str
         Name of the output file. If name contains 'html',
```

### Comparing `artistools-2024.4.23/artistools/writecomparisondata.py` & `artistools-2024.4.29/artistools/writecomparisondata.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,24 +158,25 @@
                 f.write("\n")
 
 
 def write_lbol_edep(
     modelpath: str | Path, model_id: str, selected_timesteps: t.Sequence[int], outputpath: Path
 ) -> None:
     # times = at.get_timestep_times(modelpath)
-    dflightcurve = at.lightcurve.readfile(Path(modelpath, "light_curve.out"))[-1].to_pandas()
-    dfdep = at.get_deposition(modelpath)
-
-    df = dflightcurve.merge(dfdep, left_index=True, right_index=True, suffixes=("", "_dep"))
+    dflightcurve = (
+        at.lightcurve.readfile(Path(modelpath, "light_curve.out"))[-1]
+        .to_pandas()
+        .merge(at.get_deposition(modelpath), left_index=True, right_index=True, suffixes=("", "_dep"))
+    )
 
     with outputpath.open("w") as f:
         f.write(f"#NTIMES: {len(selected_timesteps)}\n")
         f.write("#time[d] Lbol[erg/s] Edep[erg/s] \n")
 
-        for timestep, row in df.iterrows():
+        for timestep, row in dflightcurve.iterrows():
             if timestep not in selected_timesteps:
                 continue
             f.write(f"{row.time:.2f} {row.lum * 3.826e33:.2e} {row.total_dep_Lsun * 3.826e33:.2e}\n")
 
     f.close()
```

### Comparing `artistools-2024.4.23/artistools.egg-info/SOURCES.txt` & `artistools-2024.4.29/artistools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -262,23 +262,23 @@
 artistools/estimators/__main__.py
 artistools/estimators/estimators.py
 artistools/estimators/estimators_classic.py
 artistools/estimators/exportmassfractions.py
 artistools/estimators/plot3destimators_classic.py
 artistools/estimators/plotestimators.py
 artistools/estimators/test_estimators.py
-artistools/inputmodel/1dslicefrom3d.py
 artistools/inputmodel/__init__.py
 artistools/inputmodel/botyanski2017.py
 artistools/inputmodel/describeinputmodel.py
 artistools/inputmodel/downscale3dgrid.py
 artistools/inputmodel/energyinputfiles.py
 artistools/inputmodel/from_alcar.py
 artistools/inputmodel/fullymixed.py
 artistools/inputmodel/inputmodel_misc.py
+artistools/inputmodel/make1dslicefrom3d.py
 artistools/inputmodel/makeartismodel.py
 artistools/inputmodel/map_1d_to_3d_grid.py
 artistools/inputmodel/maptogrid.py
 artistools/inputmodel/modelfromhydro.py
 artistools/inputmodel/opacityinputfile.py
 artistools/inputmodel/plotdensity.py
 artistools/inputmodel/plotinitialcomposition.py
```

### Comparing `artistools-2024.4.23/artistoolscompletions.sh` & `artistools-2024.4.29/artistoolscompletions.sh`

 * *Files identical despite different names*

### Comparing `artistools-2024.4.23/pyproject.toml` & `artistools-2024.4.29/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 plotartisspectrum = 'artistools.spectra.plotspectra:main'
 plotartistransitions = 'artistools.transitions:main'
 plotartisinitialcomposition = 'artistools.inputmodel.plotinitialcomposition:main'
 plotartisviewingangles = 'artistools.viewing_angles_visualization:main'
 
 [tool.black]
 line-length = 120
-target-versions = ["py310", "py311", "py312"]
+target-version = ["py310", "py311", "py312", "py313"]
 
 [tool.mypy]
 local_partial_types = true
 check_untyped_defs = false
 disallow_any_explicit = false
 disallow_any_generics = false
 disallow_any_unimported = false
@@ -193,60 +193,51 @@
     "B005",  # strip-with-multi-characters
     "B007",  # variable not used in loop body (but sometimes it is with DataFrame.eval)
     "B905", # zip without explicit strict parameter
     "C901",  # complex-structure
     "COM812",  # missing-trailing-comma
     "CPY001", # missing-copyright-notice
     "D100",  # undocumented-public-module
-    "D101",  # undocumented-public-class
     "D102",  # undocumented-public-method
     "D103",  # undocumented-public-function
     "D104",  # undocumented-public-package
     "D107",  # undocumented-public-init
     "D203",  # one-blank-line-before-class
-    "D205",  # blank-line-after-summary
     "D213",  # multi-line-summary-second-line
     "D417",  # undocumented-param
     "E501", # Line too long
     "ERA001",  # commented-out-code
     "FBT",
     "FIX002",  # line contains TODO
     "ISC001", # single-line-implicit-string-concatenation
     "N802",  # Function name should be lowercase
     "N803",  # Argument name should be lowercase
     "N806",  # non-lowercase-variable-in-function
-    "N999",  # invalid-module-name
     "PLC0415", # import-outside-toplevel
     "PLR0914", # too-many-locals
     "PLR0917", # too-many-positional
     "PLR1702", # too-many-nested-blocks
-    "PD901",  # df is a bad variable name
     "PERF203", # try-except-in-loop
-    #"PGH001",  # No builtin `eval()` allowed
     "PLR0911",  # too-many-return-statements
     "PLR0912",  # too-many-branches
     "PLR0913",  # too-many-arguments
     "PLR0915",  # too-many-statements
     "PLR2004",  # magic-value-comparison
     "PLW2901",  # redefined-loop-name
     "PYI024", # Use `typing.NamedTuple` instead of `collections.namedtuple`
     "S101",  # Use of assert detected
-    "S301",  # suspicious-pickle-usage
-    #"S307",  # suspicious-eval-usage
     "S311",  # suspicious-non-cryptographic-random-usage
     "S603",  # subprocess-without-shell-equals-true
     "S607",  # start-process-with-partial-path
-    "SLF001",  # private-member-access
     "T201",  # print found
     "TD002",  # missing-todo-author
     "TD003",  # missing-todo-link
 ]
 fixable = ["ALL"]
 unfixable = [
-    "COM812",  # missing-trailing-comma
     "ERA001",  # commented-out-code (will just delete it!)
     "F401",  # unused-import
     "F841",  # unused-variable
     "SIM222", # expr-or-true
     "SIM223", # expr-and-false
 ]
```

### Comparing `artistools-2024.4.23/requirements.txt` & `artistools-2024.4.29/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 argcomplete>=3.3.0
 astropy>=6.0.1
-coverage>=7.4.4
+coverage>=7.5.0
 extinction>=0.4.6
 imageio>=2.34.1
 matplotlib>=3.8.4
-mypy>=1.9.0
+mypy>=1.10.0
 numexpr>=2.10.0
 numpy>=1.26.4
 pandas[compression,parquet,pyarrow]>=2.2.2
-polars>=0.20.22
+polars>=0.20.23
 pre-commit>=3.7.0
 pyarrow>=16.0.0
 pynonthermal>=2024.2.17
 pypdf2>=3.0.1
-pytest>=8.1.1
+pytest>=8.2.0
 pytest-cov>=5.0.0
-pytest-xdist[psutil]>=3.5.0
+pytest-xdist[psutil]>=3.6.1
 python-xz>=0.5
-pyvista>=0.43.5
+pyvista>=0.43.6
 PyYAML>=6.0.1
-pyzstd>=0.15.10
-ruff>=0.4.1
+ruff>=0.4.2
 scipy>=1.13.0
 setuptools_scm[toml]>=8.0.4
 tabulate>=0.9
 typeguard>=4.2.1
 types-PyYAML>=6.0.12.20240311
 types-tabulate>=0.9.0.20240106
 #vtk>=9.2.3
 wheel>=0.43.0
+zstandard>=0.22.0
```

