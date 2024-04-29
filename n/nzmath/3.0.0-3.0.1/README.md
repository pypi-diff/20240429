# Comparing `tmp/nzmath-3.0.0.tar.gz` & `tmp/nzmath-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzmath-3.0.0.tar", last modified: Thu Jul 27 06:39:23 2023, max compression
+gzip compressed data, was "nzmath-3.0.1.tar", last modified: Mon Apr 29 06:34:43 2024, max compression
```

## Comparing `nzmath-3.0.0.tar` & `nzmath-3.0.1.tar`

### file list

```diff
@@ -1,131 +1,162 @@
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.786937 nzmath-3.0.0/
--rw-r--r--   0 satoru   (197609) なし       (197121)     1555 2023-05-25 06:40:05.000000 nzmath-3.0.0/LICENSE
--rw-r--r--   0 satoru   (197609) なし       (197121)     2705 2023-07-27 06:39:23.785937 nzmath-3.0.0/PKG-INFO
--rw-r--r--   0 satoru   (197609) なし       (197121)     2027 2023-07-27 06:20:52.000000 nzmath-3.0.0/README.txt
--rwxr-xr-x   0 satoru   (197609) なし       (197121)      800 2023-07-27 06:38:58.000000 nzmath-3.0.0/pyproject.toml
--rw-r--r--   0 satoru   (197609) なし       (197121)       38 2023-07-27 06:39:23.787938 nzmath-3.0.0/setup.cfg
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.520946 nzmath-3.0.0/src/
--rw-r--r--   0 satoru   (197609) なし       (197121)      790 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/__init__.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    27475 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/algfield.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     6061 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/algorithm.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2346 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/all.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    10111 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/arith1.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4717 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/arygcd.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2456 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/bigrandom.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     6324 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/bigrange.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    18853 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/combinatorial.py
--rw-r--r--   0 satoru   (197609) なし       (197121)      962 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/compatibility.py
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.522946 nzmath-3.0.0/src/config/
--rw-r--r--   0 satoru   (197609) なし       (197121)     3216 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/config/nzmathconf.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     8005 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/config.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     5188 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/cubic_root.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    15623 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/ecpp.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    53548 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/elliptic.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     9601 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/equation.py
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.546945 nzmath-3.0.0/src/factor/
--rw-r--r--   0 satoru   (197609) なし       (197121)      166 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/__init__.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     9206 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/ecm.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     3752 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/find.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     8654 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/methods.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     6817 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/misc.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    27139 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/mpqs.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     9156 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/util.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    33296 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/finitefield.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2389 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/gcd.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    13682 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/group.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     8182 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/imaginary.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    10806 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/intresidue.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     6622 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/lattice.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    64136 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/matrix.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    37722 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/module.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1242 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/multiplicative.py
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.556945 nzmath-3.0.0/src/nzmath.egg-info/
--rw-r--r--   0 satoru   (197609) なし       (197121)     2705 2023-07-27 06:39:23.000000 nzmath-3.0.0/src/nzmath.egg-info/PKG-INFO
--rw-r--r--   0 satoru   (197609) なし       (197121)     2412 2023-07-27 06:39:23.000000 nzmath-3.0.0/src/nzmath.egg-info/SOURCES.txt
--rw-r--r--   0 satoru   (197609) なし       (197121)        1 2023-07-27 06:39:23.000000 nzmath-3.0.0/src/nzmath.egg-info/dependency_links.txt
--rw-r--r--   0 satoru   (197609) なし       (197121)      326 2023-07-27 06:39:23.000000 nzmath-3.0.0/src/nzmath.egg-info/top_level.txt
--rw-r--r--   0 satoru   (197609) なし       (197121)    21369 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/permute.py
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.559945 nzmath-3.0.0/src/plugin/
--rw-r--r--   0 satoru   (197609) なし       (197121)      256 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugin/__init__.py
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.566945 nzmath-3.0.0/src/plugin/math/
--rw-r--r--   0 satoru   (197609) なし       (197121)      998 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugin/math/__init__.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1005 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugin/math/_mpmath.py
--rw-r--r--   0 satoru   (197609) なし       (197121)      614 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugin/math/default.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1162 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugins.py
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.608943 nzmath-3.0.0/src/poly/
--rw-r--r--   0 satoru   (197609) なし       (197121)      223 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/__init__.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    14884 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/array.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     9210 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/factor.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    12870 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/formalsum.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4771 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/groebner.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    16993 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/hensel.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    24835 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/multiutil.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    13718 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/multivar.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2769 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/ratfunc.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    22954 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/ring.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    13939 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/termorder.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    58733 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/uniutil.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    26211 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/univar.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    34893 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/prime.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    14333 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/prime_decomp.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    33044 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/quad.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    31782 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/rational.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     8399 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/real.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    26077 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/ring.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    16533 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/round2.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1096 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/sequence.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     7604 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/squarefree.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4027 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/vector.py
-drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.783939 nzmath-3.0.0/tests/
--rw-r--r--   0 satoru   (197609) なし       (197121)     4451 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testAlgfield.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1928 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testAlgorithm.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1479 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testAll.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     5386 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testArith1.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1130 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testArygcd.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2809 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testBigrandom.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2339 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testBigrange.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    11714 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testCombinatorial.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1502 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testCompatibility.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1266 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testCubic_root.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     3393 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testEcpp.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    11731 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testElliptic.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     5321 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testEquation.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2864 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorEcm.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     3799 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorMethods.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4539 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorMisc.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     3284 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorMpqs.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2770 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorUtil.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    12587 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFiniteField.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     5698 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFormalsum.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2023 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testGcd.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4429 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testGroebner.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4247 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testGroup.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2655 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testImaginary.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     6764 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testIntresidue.py
--rw-r--r--   0 satoru   (197609) なし       (197121)      555 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testLattice.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    16528 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMatrix.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2598 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMatrixFiniteField.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    15370 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testModule.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1298 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMultiplicative.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     8007 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMultiutil.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     5293 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMultivar.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4626 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPermute.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1473 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPlugins.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     5569 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPolyArray.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     3540 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPolyFactor.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     7325 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPolyHensel.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4970 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPolyRing.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     7563 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPrime.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     6453 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPrime_decomp.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     6075 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testQuad.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1312 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testRatfunc.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    14984 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testRational.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     2686 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testReal.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4472 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testRing.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     4103 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testRound2.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1286 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testSequence.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     5140 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testSquarefree.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     7687 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testTermOrder.py
--rw-r--r--   0 satoru   (197609) なし       (197121)    14563 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testUniutil.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     6981 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testUnivar.py
--rw-r--r--   0 satoru   (197609) なし       (197121)     1918 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testVector.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:43.610344 nzmath-3.0.1/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2781 2024-04-18 07:15:41.000000 nzmath-3.0.1/ACKNOWLEDGEMENTS.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)    10566 2024-04-18 07:15:41.000000 nzmath-3.0.1/CHANGES.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1593 2024-04-18 07:15:41.000000 nzmath-3.0.1/HISTORY.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1555 2024-04-18 06:50:57.000000 nzmath-3.0.1/LICENSE.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)      199 2024-04-18 07:19:35.000000 nzmath-3.0.1/MANIFEST.in
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3551 2024-04-29 06:34:43.608344 nzmath-3.0.1/PKG-INFO
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2869 2024-04-18 07:28:28.000000 nzmath-3.0.1/README.txt
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.253392 nzmath-3.0.1/data/
+-rw-r--r--   0 satoru   (197609) なし       (197121)   556049 2024-04-18 07:20:02.000000 nzmath-3.0.1/data/discriminant.csv
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.351387 nzmath-3.0.1/enttakagi/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4733 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3264 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/sec01.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6214 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/sec02.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4410 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/sec03.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5117 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/sec04.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7950 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/sec04a.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9605 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/sec04b.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8411 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/sec04c.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7143 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/sec04d.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3361 2024-04-18 07:16:04.000000 nzmath-3.0.1/enttakagi/utils.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.170395 nzmath-3.0.1/manual/
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.369387 nzmath-3.0.1/manual/en/
+-rw-r--r--   0 satoru   (197609) なし       (197121)   720276 2024-04-18 07:15:55.000000 nzmath-3.0.1/manual/en/nzmath_doc.pdf
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.383386 nzmath-3.0.1/manual/ja/
+-rw-r--r--   0 satoru   (197609) なし       (197121)   911799 2024-04-18 07:15:55.000000 nzmath-3.0.1/manual/ja/nzmath_doc.pdf
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2662 2024-04-18 07:20:08.000000 nzmath-3.0.1/nzmathconf.py.example
+-rw-r--r--   0 satoru   (197609) なし       (197121)      800 2024-04-18 07:20:51.000000 nzmath-3.0.1/pyproject.toml
+-rw-r--r--   0 satoru   (197609) なし       (197121)       38 2024-04-29 06:34:43.610344 nzmath-3.0.1/setup.cfg
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.841372 nzmath-3.0.1/src/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      790 2024-04-18 06:53:38.000000 nzmath-3.0.1/src/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    27475 2024-04-18 06:52:56.000000 nzmath-3.0.1/src/algfield.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6061 2024-04-18 06:52:56.000000 nzmath-3.0.1/src/algorithm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2346 2024-04-18 06:52:56.000000 nzmath-3.0.1/src/all.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    10111 2024-04-18 06:52:56.000000 nzmath-3.0.1/src/arith1.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4717 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/arygcd.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2556 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/bigrandom.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6085 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/bigrange.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    18845 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/combinatorial.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)      962 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/compatibility.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.844371 nzmath-3.0.1/src/config/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2687 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/config/nzmathconf.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7190 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/config.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5188 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/cubic_root.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9206 2024-03-26 09:23:00.000000 nzmath-3.0.1/src/ecm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    15212 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/ecpp.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    53548 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/elliptic.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9601 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/equation.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.904370 nzmath-3.0.1/src/factor/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      166 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/factor/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9206 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/factor/ecm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4010 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/factor/find.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9426 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/factor/methods.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7989 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/factor/misc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    27284 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/factor/mpqs.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9156 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/factor/util.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4010 2024-03-26 09:23:00.000000 nzmath-3.0.1/src/find.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    33296 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/finitefield.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6397 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/gcd.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    13682 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/group.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8182 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/imaginary.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    10806 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/intresidue.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6622 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/lattice.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    64136 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/matrix.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9426 2024-03-26 09:23:00.000000 nzmath-3.0.1/src/methods.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7989 2024-03-26 09:23:00.000000 nzmath-3.0.1/src/misc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    37722 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/module.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    27284 2024-03-26 09:23:00.000000 nzmath-3.0.1/src/mpqs.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1251 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/multiplicative.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:43.606344 nzmath-3.0.1/src/nzmath.egg-info/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3551 2024-04-29 06:34:42.000000 nzmath-3.0.1/src/nzmath.egg-info/PKG-INFO
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2869 2024-04-29 06:34:42.000000 nzmath-3.0.1/src/nzmath.egg-info/SOURCES.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)        1 2024-04-29 06:34:42.000000 nzmath-3.0.1/src/nzmath.egg-info/dependency_links.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)      369 2024-04-29 06:34:42.000000 nzmath-3.0.1/src/nzmath.egg-info/top_level.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2687 2024-03-26 09:23:00.000000 nzmath-3.0.1/src/nzmathconf.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    21369 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/permute.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.922367 nzmath-3.0.1/src/plugin/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      256 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/plugin/__init__.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:42.946369 nzmath-3.0.1/src/plugin/math/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      998 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/plugin/math/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1005 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/plugin/math/_mpmath.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)      614 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/plugin/math/default.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1162 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/plugins.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:43.084362 nzmath-3.0.1/src/poly/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      223 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    14884 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/array.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9210 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/factor.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    12870 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/formalsum.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4771 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/groebner.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    16993 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/hensel.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    24835 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/multiutil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    13718 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/multivar.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2769 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/ratfunc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    22954 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/ring.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    13939 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/termorder.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    58733 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/uniutil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    26211 2024-04-18 06:54:20.000000 nzmath-3.0.1/src/poly/univar.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    34242 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/prime.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    14333 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/prime_decomp.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    33044 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/quad.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    31782 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/rational.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8399 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/real.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    26077 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/ring.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    16533 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/round2.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1253 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/sequence.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7604 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/squarefree.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9156 2024-03-26 09:23:00.000000 nzmath-3.0.1/src/util.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4027 2024-04-18 06:52:57.000000 nzmath-3.0.1/src/vector.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2024-04-29 06:34:43.603345 nzmath-3.0.1/tests/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4451 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testAlgfield.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1928 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testAlgorithm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1479 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testAll.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5386 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testArith1.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1130 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testArygcd.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2809 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testBigrandom.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2339 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testBigrange.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    11714 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testCombinatorial.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1502 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testCompatibility.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1266 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testCubic_root.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3393 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testEcpp.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    11731 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testElliptic.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5321 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testEquation.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2864 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testFactorEcm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3799 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testFactorMethods.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4539 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testFactorMisc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3284 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testFactorMpqs.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2770 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testFactorUtil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    12587 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testFiniteField.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5698 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testFormalsum.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2023 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testGcd.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4429 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testGroebner.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4247 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testGroup.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2655 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testImaginary.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6764 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testIntresidue.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)      555 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testLattice.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    16510 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testMatrix.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2598 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testMatrixFiniteField.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    15370 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testModule.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1298 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testMultiplicative.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8007 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testMultiutil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5293 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testMultivar.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4626 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testPermute.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1473 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testPlugins.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5569 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testPolyArray.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3540 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testPolyFactor.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7325 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testPolyHensel.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4970 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testPolyRing.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7563 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testPrime.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6453 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testPrime_decomp.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6075 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testQuad.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1312 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testRatfunc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    14984 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testRational.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2686 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testReal.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4472 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testRing.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4103 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testRound2.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1286 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testSequence.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5140 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testSquarefree.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7687 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testTermOrder.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    14563 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testUniutil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6981 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testUnivar.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1918 2024-04-18 06:52:18.000000 nzmath-3.0.1/tests/testVector.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9431 2024-04-18 07:24:51.000000 nzmath-3.0.1/tutorial.txt
```

### Comparing `nzmath-3.0.0/LICENSE` & `nzmath-3.0.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2003-2022 development group
+Copyright (c) 2003-2024 development group
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
     * Redistributions of source code must retain the above copyright
```

### Comparing `nzmath-3.0.0/PKG-INFO` & `nzmath-3.0.1/README.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,69 @@
-Metadata-Version: 2.1
-Name: nzmath
-Version: 3.0.0
-Summary: number theory oriented calculation system
-Author-email: NZMATH development group <nzmath-user@sf.net>
-Project-URL: Homepage, https://nzmath.sourceforge.io/
-Project-URL: Documentation, https://nzmath.sourceforge.io/
-Project-URL: Source, https://sourceforge.net/p/nzmath/code/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-NZMATH 3.0.0 (Python 3 calculator on number theory)
+NZMATH 3.0.1 (Python 3 calculator on number theory)
 ===================================================
 
 Introduction
 ------------
 
-NZMATH is a Python based number theory oriented calculation system.
-Its development started at Nakamula laboratory, Tokyo Metropolitan
-University.  Today it is developed at SourceForge.net .
-
-This version 3.0.0 is based on Python 3, while former versions are all
-based on Python 2.  Most features are equal to those of version 1.2.0.
-The API can still be changed with versions.
+NZMATH is a Python calculator on number theory.  It started development
+at Nakamula laboratory, Tokyo Metropolitan University.  Today it is
+developed at SourceForge.net .  Download the file NZMATH-3.0.1.tar.gz
+for installation from the SourceForge
+https://sourceforge.net/projects/nzmath/files/nzmath/ .
+Test programs for NZMATH is available as NZMATH-test-3.0.1.tar.gz at
+https://sourceforge.net/projects/nzmath/files/nzmath-test/ .
+
+This version 3.0.1 contains several program corrections/additions by
+the "notebook" of the book 'Elementary Number Theory' (TAKAGI, Teiji)
+in Python-NZMATH language.  On the other hand, the "notebook" itself
+is available as an archive NZMATH-enttakagi-0.0.1.tar.gz at
+https://sourceforge.net/projects/nzmath/files/nzmath-enttakagi/ .
+The "notebook" is designed for beginning students on algorithmic number
+theory to self-study Number Theory, Programming and English together.
 
 Installation
 ------------
 
 To install NZMATH on your computer, you must have Python 3.8 or later.
 If you don't have a copy of Python, please install it first.
 Python is available from https://www.python.org/ .
 
-The next step is to expand the NZMATH-3.0.0.tar.gz.  The way to do it
+The next step is to expand the NZMATH-3.0.1.tar.gz.  The way to do it
 depends on your operating system.  On the systems with recent GNU tar,
 you can do it with a single command::
 
- % tar xf NZMATH-3.0.0.tar.gz
+ % tar xf NZMATH-3.0.1.tar.gz
 
-where, % is the command line prompt.  Or with standard tar, you can do
+Here % is the command line prompt.  Or with standard tar, you can do
 it as::
 
- % gzip -cd NZMATH-3.0.0.tar.gz | tar xf -
+ % gzip -cd NZMATH-3.0.1.tar.gz | tar xf -
 
-Then, you have a child directory named NZMATH-3.0.0.
+Then, you have a child directory named NZMATH-3.0.1 .
 
 The third step is the last step, to install NZMATH to the standard
 python path.  Usually, this means to write files to somewhere under
-/usr/lib or /usr/local/lib, and thus you have to have appropriate
+/usr/lib or /usr/local/lib , and thus you have to have appropriate
 write permission.  Typically, do as the following::
 
- % cd NZMATH-3.0.0
+ % cd NZMATH-3.0.1
  % su
  # python setup.py install
 
+Depending on system, you may get SetuptoolsDeprecationWarning.
+Please do not worry for the moment.  Installed NZMATH works well.
+
 Usage
 -----
 
 NZMATH is provided as a Python library package named 'nzmath', so
 please use it as a usual package.  For more information please refer
 Tutorial_.
 
-.. _Tutorial: tutorial.html
+.. _Tutorial: https://nzmath.sourceforge.io/tutorial.html
 
 Feedback
 --------
 
 Your feedbacks are always welcomed.  Please consider to join the
 mailing list nzmath-user@lists.sourceforge.net .  You can join the list
 by visiting the web page
@@ -77,11 +71,12 @@
 
 Copyright
 ---------
 
 NZMATH is distributed under the BSD license.  Please read LICENSE.txt_
 in the distribution tar ball for detail.
 
-.. _LICENSE.txt: LICENSE.txt
+.. _LICENSE.txt: https://nzmath.sourceforge.io/LICENSE.txt
 
 
-AddressObject
+Copyright (C) 2003-2024, NZMATH development group. All Right Reserved.
+(Chief developer: TANAKA, Satoru / Supervisor: NAKAMULA, Ken)
```

### Comparing `nzmath-3.0.0/pyproject.toml` & `nzmath-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nzmath"
-version = "3.0.0"
+version = "3.0.1"
 authors = [
   { name="NZMATH development group", email="nzmath-user@sf.net" },
 ]
 description = "number theory oriented calculation system"
 readme = {file = "README.txt", content-type = "text/x-rst"}
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `nzmath-3.0.0/src/__init__.py` & `nzmath-3.0.1/src/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 NZMATH is a Python based number theory oriented calculation system.
 It is developed at Tokyo Metropolitan University.
 
 NZMATH is distributed under the BSD license.  See LICENSE.txt for
 detail.
 
-Copyright (c) 2003-2022, NZMATH development group, all right reserved.
+Copyright (c) 2003-2024, NZMATH development group, all right reserved.
 """
 
 __all__ = [
     "algfield",
     "arith1",
     "arygcd",
     "bigrandom",
```

### Comparing `nzmath-3.0.0/src/algfield.py` & `nzmath-3.0.1/src/algfield.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/algorithm.py` & `nzmath-3.0.1/src/algorithm.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/all.py` & `nzmath-3.0.1/src/all.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/arith1.py` & `nzmath-3.0.1/src/arith1.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/arygcd.py` & `nzmath-3.0.1/src/arygcd.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/bigrandom.py` & `nzmath-3.0.1/src/bigrandom.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 #bigrandom.py
 
 import sys
 import random as _random
 import nzmath.arith1 as arith1
 
 
-def randrange(start, stop=None, step=1):
-    """
-    Choose a random item from range([start,] stop[, step]).
-    (Return long integer.)
-
-    see random.randrange
-    """
-    if stop is None:
-        if abs(start) < sys.maxsize:
-            return _random.randrange(start)
-    elif abs(stop - start) < sys.maxsize:
-        return _random.randrange(start, stop, step)
-
-    negative_step = False
-    if stop is None:
-        start, stop = 0, start
-    if step < 0:
-        start, stop, step = -start, -stop, -step
-        negative_step = True
-
-    _validate_for_randrange(start, stop, step)
-
-    if (stop - start) % step != 0:
-        v = (stop - start)//step + 1
-    else:
-        v = (stop - start)//step
-
-    bitlength = arith1.log(v, base=2)
-    if v != 2**bitlength:
-        bitlength += 1
-    randomized = v + 1 # to pass the first test
-    while randomized >= v:
-        randomized = 0
-        for i in range(bitlength):
-            if random() < 0.5:
-                randomized += 1 << i
-    result = randomized * step + start
-    if negative_step:
-        return -result
-    return result
+# def randrange(start, stop=None, step=1):
+#     """
+#     Choose a random item from range([start,] stop[, step]).
+#     (Return long integer.)
+
+#     see random.randrange
+#     """
+#     if stop is None:
+#         if abs(start) < sys.maxsize:
+#             return _random.randrange(start)
+#     elif abs(stop - start) < sys.maxsize:
+#         return _random.randrange(start, stop, step)
+
+#     negative_step = False
+#     if stop is None:
+#         start, stop = 0, start
+#     if step < 0:
+#         start, stop, step = -start, -stop, -step
+#         negative_step = True
+
+#     _validate_for_randrange(start, stop, step)
+
+#     if (stop - start) % step != 0:
+#         v = (stop - start)//step + 1
+#     else:
+#         v = (stop - start)//step
+
+#     bitlength = arith1.log(v, base=2)
+#     if v != 2**bitlength:
+#         bitlength += 1
+#     randomized = v + 1 # to pass the first test
+#     while randomized >= v:
+#         randomized = 0
+#         for i in range(bitlength):
+#             if random() < 0.5:
+#                 randomized += 1 << i
+#     result = randomized * step + start
+#     if negative_step:
+#         return -result
+#     return result
+randrange = _random.randrange
 
 def _validate_for_randrange(start, stop, step):
     """
     Check validity of arguments for randrange.
     """
     if step == 0:
         raise ValueError("zero step for randrange()")
```

### Comparing `nzmath-3.0.0/src/bigrange.py` & `nzmath-3.0.1/src/bigrange.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 """
 bigrange
 
 Generators for range like sequences.
 """
-
+import builtins
+import itertools
 
 def count(n=0):
     """
     Count up infinitely from 'n' (default to 0),
 
     see itertools.count
     """
     while True:
         yield n
         n += 1
 
 
-def range(start, stop=None, step=None):
-    """
-    Generate range like finite integer sequence but can generate more
-    than sys.maxint elements.
-    """
-    if step is None:
-        step = 1
-    elif not isinstance(step, int):
-        raise ValueError("non-integer step for range()")
-    if not isinstance(start, int):
-        raise ValueError("non-integer arg 1 for range()")
-    if stop is None:
-        start, stop = 0, start
-    elif not isinstance(stop, int):
-        raise ValueError("non-integer stop for range()")
-
-    if step > 0:
-        n = start
-        while n < stop:
-            yield n
-            n += step
-    elif step < 0:
-        n = start
-        while n > stop:
-            yield n
-            n += step
-    else:
-        raise ValueError("zero step for range()")
+# def range(start, stop=None, step=None):
+#     """
+#     Generate range like finite integer sequence but can generate more
+#     than sys.maxint elements.
+#     NOTE: 
+#     """
+#     if step is None:
+#         step = 1
+#     elif not isinstance(step, int):
+#         raise ValueError("non-integer step for range()")
+#     if not isinstance(start, int):
+#         raise ValueError("non-integer arg 1 for range()")
+#     if stop is None:
+#         start, stop = 0, start
+#     elif not isinstance(stop, int):
+#         raise ValueError("non-integer stop for range()")
+
+#     if step > 0:
+#         n = start
+#         while n < stop:
+#             yield n
+#             n += step
+#     elif step < 0:
+#         n = start
+#         while n > stop:
+#             yield n
+#             n += step
+#     else:
+#         raise ValueError("zero step for range()")
 
+range = builtins.range
 
 def arithmetic_progression(init, difference):
     """
     Generate an arithmetic progression start form 'init' and
     'difference' step.
     """
     return _iterate(lambda x: x + difference, init)
@@ -83,27 +86,15 @@
 
     The range triples may be doubles (start, stop) or single (stop,),
     but they have to be always tuples.
 
     Be cautious that using this module usually means you are trying to
     do brute force looping.
     """
-    starts, stops, steps = _split_triples(triples)
-    if _empty(starts, stops, steps):
-        raise StopIteration("empty range")
-    i, values = len(triples) - 1, list(starts)
-    yield tuple(values)
-    while i >= 0:
-        values[i] += steps[i]
-        if _range_exhausted(i, values, steps, stops):
-            values[i] = starts[i]
-            i -= 1
-            continue
-        yield tuple(values)
-        i = len(triples) - 1
+    return itertools.product(*itertools.starmap(builtins.range, triples))
 
 def _split_triples(triples):
     """
     Convert a list of triples into three lists each consists of 1st,
     2nd and 3rd element of each triples.
 
     The range triples may be doubles (start, stop) or single (stop,),
```

### Comparing `nzmath-3.0.0/src/combinatorial.py` & `nzmath-3.0.1/src/combinatorial.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     if n < m:
         return 0
     if m*2 > n:
         m = n - m
     retval = n
     for i in range(1, m):
         retval *= (n - i)
-        retval /= (i + 1)
-    return Integer(retval)
+        retval //= (i + 1)
+    return retval
 
 def factorial(n):
     """
     Return n! for non negative integer n.
     """
     if not isinstance(n, int):
         raise TypeError("integer is expected, %s detected." % n.__class__)
```

### Comparing `nzmath-3.0.0/src/compatibility.py` & `nzmath-3.0.1/src/compatibility.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/config/nzmathconf.py` & `nzmath-3.0.1/src/config/nzmathconf.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,33 +57,14 @@
 #HAVE_NET = False
 #CHECK_NET = False
 # Or you can let NZMATH check connectivity every time, set as the following:
 #HAVE_NET = None
 #CHECK_NET = True
 
 #
-# psyco
-# -----
-#
-# psyco is a package providing JIT compiler for Python.
-# http://psyco.sourceforge.net/
-# The package is usable only on x86 CPUs.
-# This package is used in factor/mpqs module.
-#
-# If you have psyco installed, and would like to use it fully, set:
-#HAVE_PSYCO = True
-#CHECK_PSYCO = False
-# If you would like to disable it no matter whether it is available:
-#HAVE_PSYCO = False
-#CHECK_PSYCO = False
-# The default values mean "I don't know, check it and use it if possible":
-HAVE_PSYCO = None
-CHECK_PSYCO = True
-
-#
 # Assumptions
 # ===========
 #
 # Some conjectures are useful for assuring the validity of a fast
 # algorithm.
 #
 # All assumptions are default to False, but you can set them True if
```

### Comparing `nzmath-3.0.0/src/config.py` & `nzmath-3.0.1/src/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 import warnings
 
 WINDOWS_PLATFORMS = ('win32', 'win64', 'cli', )
 
 def nzmath_info():
-    print("NZMATH [Version 3.0.0]")
+    print("NZMATH [Version 3.0.1]")
 
 # ----------------
 # Default Settings
 # ----------------
 #
 # Dependencies
 # ============
@@ -71,33 +71,14 @@
 #HAVE_NET = False
 #CHECK_NET = False
 # Or you can let NZMATH check connectivity every time, set as the following:
 #HAVE_NET = None
 #CHECK_NET = True
 
 #
-# psyco
-# -----
-#
-# psyco is a package providing JIT compiler for Python.
-# http://psyco.sourceforge.net/
-# The package is usable only on x86 CPUs.
-# This package is used in factor/mpqs module.
-#
-# If you have psyco installed, and would like to use it fully, set:
-#HAVE_PSYCO = True
-#CHECK_PSYCO = False
-# If you would like to disable it no matter whether it is available:
-#HAVE_PSYCO = False
-#CHECK_PSYCO = False
-# The default values mean "I don't know, check it and use it if possible":
-HAVE_PSYCO = None
-CHECK_PSYCO = True
-
-#
 # plug-ins
 # ========
 #
 # math
 # ----
 # Python standard float/comple types and math/cmath modules only
 # provide fixed precision (double precision), but sometimes
@@ -261,31 +242,15 @@
     except Exception:
         # I don't know the reason, but something wrong
         return False
 
 if CHECK_NET:
     HAVE_NET = check_net()
 
-#
-# psyco availability
-# ------------------
-#
-def check_psyco():
-    """
-    Check if psyco is importable or not.
-    """
-    try:
-        import psyco
-        return True
-    except ImportError:
-        return False
 
-if CHECK_PSYCO:
-    HAVE_PSYCO = check_psyco()
-        
 #
 # math plug-in
 #
 def check_plugin_math():
     """
     Return 'mpmath' if HAVE_MPMATH, None otherwise.
     """
@@ -326,9 +291,9 @@
     DATADIR = default_datadir()
     if DATADIR is None:
         warnings.warn('no datadir found')
 
 
 # Declare exported variables.
 
-__all__ = ['HAVE_MPMATH', 'HAVE_SQLITE3', 'HAVE_NET', 'HAVE_PSYCO',
+__all__ = ['HAVE_MPMATH', 'HAVE_SQLITE3', 'HAVE_NET', 
            'PLUGIN_MATH', 'GRH', 'DATADIR']
```

### Comparing `nzmath-3.0.0/src/cubic_root.py` & `nzmath-3.0.1/src/cubic_root.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/ecpp.py` & `nzmath-3.0.1/src/ecpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,26 +130,14 @@
     T = [(int(nearest_integer(c.real)) if hasattr(c, 'real') else c) for c in T]
     return h, T
 
 def hilbert(D):
     """
     wrapper to split mpmath part and others.
     """
-    if HAVE_NET:
-        try:
-            import urllib.request, urllib.error, urllib.parse
-            url = 'http://hilbert-class-polynomial.appspot.com/%d/' % D
-            result = urllib.request.urlopen(url).read()
-            if result == 'null':
-                pass
-            else:
-                hcp = eval(result)
-                return len(hcp) - 1, hcp
-        except Exception:
-            pass
 
     if HAVE_MPMATH:
         return hilbert_mpmath(D)
 
     raise prime.ImplementLimit("impliment limit")
```

### Comparing `nzmath-3.0.0/src/elliptic.py` & `nzmath-3.0.1/src/elliptic.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/equation.py` & `nzmath-3.0.1/src/equation.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/factor/ecm.py` & `nzmath-3.0.1/src/ecm.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/factor/find.py` & `nzmath-3.0.1/src/factor/find.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 _log = logging.getLogger('nzmath.factor.find')
 
 # Pollard's rho method
 def rhomethod(n, **options):
     """
     Find a non-trivial factor of n using Pollard's rho algorithm.
     The implementation refers the explanation in C.Pomerance's book.
+    Due to the nature of the method, a factorization may return
+    the trivial factor only.
     """
     # verbosity
     verbose = options.get('verbose', False)
     if not verbose:
         _silence()
 
     if n <= 3:
@@ -44,15 +46,17 @@
     return g
 
 # p-1 method
 def pmom(n, **options):
     """
     This function tries to find a non-trivial factor of n using
     Algorithm 8.8.2 (p-1 first stage) of Cohen's book.
-    In case of N = pow(2,i), this program will not terminate.
+    In the case that n is a power of 2, this program will always return 1.
+    Due to the nature of the method, another factorization may return
+    the trivial factor only.
     """
     # verbosity
     verbose = options.get('verbose', False)
     if not verbose:
         _silence()
 
     # initialize
@@ -93,14 +97,15 @@
                 if not verbose:
                     _verbose()
                 if g == n:
                     return 1
                 return g
             q1 *= q
 
+###nzmath###bug# no reply for n == primonial(67) + 1
 def trialDivision(n, **options):
     """
     Return a factor of given integer by trial division.
 
     options can be either:
     1) 'start' and 'stop' as range parameters.
     2) 'iterator' as an iterator of primes.
```

### Comparing `nzmath-3.0.0/src/factor/methods.py` & `nzmath-3.0.1/src/factor/methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -199,14 +199,15 @@
     def find(self, target, **options):
         """
         Find a factor from the target number.
         """
         return ecmfind(target, **options)
 
 
+###nzmath###bug# no reply for n == primonial(67) + 1
 def trialDivision(n, **options):
     """
     Factor the given integer by trial division.
 
     options for the trial sequence can be either:
     1) 'start' and 'stop' as range parameters.
     2) 'iterator' as an iterator of primes.
@@ -217,41 +218,52 @@
     method = TrialDivision()
     options['return_type'] = 'list'
     return method.factor(n, **options)
 
 def pmom(n, **options):
     """
     Factor the given integer by Pollard's p-1 method.
+    The method may fail unless n has an appropriate factor for the method.
+    The method always fails if n%4 == 0.  (See pmom of factor.find module.)
     """
     method = PMinusOneMethod()
     options['return_type'] = 'list'
     options['need_sort'] = True
     return method.factor(n, **options)
 
 def rhomethod(n, **options):
     """
-    Factor the given integer by rho method.
+    Factor the given integer n by Pollard's rho method.
+    The method is a probabilistic method, possibly fails in factorizations.
+    (See rhomethod of factor.find module.)
     """
     method = RhoMethod()
     options['return_type'] = 'list'
     options['need_sort'] = True
     return method.factor(n, **options)
 
 def mpqs(n, **options):
     """
     Factor the given integer by multi-polynomial quadratic sieve method.
+    The number n should be composite and prime to 2*3*5*7*11*13.
+    The method may fail unless n has an appropriate factor for the method.
+    Unfortunately, this always seems to fail for non-squarefree n.
+    (See mpqsfind of factor.mpqs module.)
     """
     method = MPQSMethod()
     options['return_type'] = 'list'
     options['need_sort'] = True
     return method.factor(n, **options)
 
 def ecm(n, **options):
     """
     Factor the given integer by elliptic curve method.
+    The method may fail unless n has an appropriate factor for the method.
+    Unfortunately, this always does not seem to return for non-squarefree n.
+    (See ecm of factor.ecm module.)
     """
     method = EllipticCurveMethod()
     options['return_type'] = 'list'
     options['need_sort'] = True
     return method.factor(n, **options)
 
 def factor(n, method='default', **options):
```

### Comparing `nzmath-3.0.0/src/factor/misc.py` & `nzmath-3.0.1/src/factor/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 misc functions using factorization.
 """
 
 import nzmath.gcd as gcd
 import nzmath.arith1 as arith1
+prod = arith1.product
 import nzmath.prime as prime
 import nzmath.factor.methods as methods
 
-
 def primePowerTest(n):
     """
     This program using Algo. 1.7.5 in Cohen's book judges whether
     n is of the form p**k with prime p or not.
     If it is True, then (p,k) will be returned,
     otherwise (n,0).
     """
@@ -34,15 +34,19 @@
 
     k, q = arith1.vp(n, p)
     if q == 1:
         return (p, k)
     else:
         return (n, 0)
 
-
+###nzmath###bug# N=FactoredInteger(12,{2:3,3:1}) is no error
+# should modify __init__ to check the consistency of integer and factors
+#     self.integer == prod(p**e for p, e in self.factors.items())
+# also should check self.integer > 0
+# further check another class FactoredInteger in nzmath.prime
 class FactoredInteger(object):
     """
     Integers with factorization information.
     """
     def __init__(self, integer, factors=None):
         """
         FactoredInteger(integer [, factors])
@@ -223,10 +227,48 @@
         if asfactored:
             return result
         else:
             return result.integer
 
 
 # for backward compatibility
-allDivisors = lambda n: FactoredInteger(n).divisors()
-primeDivisors = lambda n: FactoredInteger(n).prime_divisors()
-squarePart = lambda n: FactoredInteger(n).square_part()
+def allDivisors(n):
+    """
+    Return all divisors of n as a list.
+    """
+    return FactoredInteger(n).divisors()
+
+# for backward compatibility
+def primeDivisors(n):
+    """
+    Return all prime divisors of n as a list.
+    """
+    return FactoredInteger(n).prime_divisors()
+
+# for backward compatibility
+def squarePart(n, asfactored=False):
+    """
+    Return the largest integer whose square divides the number.
+
+    If an optional argument asfactored is true, then the result is
+    also a FactoredInteger object. (default is False)
+    """
+    return FactoredInteger(n).square_part(asfactored)
+
+def countDivisors(a):
+    """
+    Input
+        a: positive integer
+    Output
+        the number of positive divisors of a by factorization
+    """
+    return prod(e + 1 for p, e in FactoredInteger(a))
+
+def sumDivisors(a):
+    """
+    Input
+        a: positive integer
+    Output
+        the sum of positive divisors of a by factorization
+    """
+    return prod((p**(e + 1) - 1)//(p - 1) for p, e in FactoredInteger(a))
+
```

### Comparing `nzmath-3.0.0/src/factor/mpqs.py` & `nzmath-3.0.1/src/factor/mpqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -806,14 +806,16 @@
 
 def mpqsfind(n, s=0, f=0, m=0, verbose=False):
     """
     This is the main function of MPQS.
     The main argument is the composite_number to be factored.
     Parameters are s=sieve_range, f=factorbase_size, m=multiplier
     and verbose.
+    The number n should be composite and prime to 2*3*5*7*11*13.
+    Unfortunately, this always seems to fail for non-squarefree n.
     """
     # verbosity
     if verbose:
         _log.setLevel(logging.DEBUG)
         _log.debug("verbose")
     else:
         _log.setLevel(logging.NOTSET)
@@ -836,7 +838,8 @@
             Y = Y % M.number
         X = arith1.floorsqrt(X) % M.number
         if X != Y:
             divisor = gcd.gcd(X - Y, N)
             if 1 < divisor < N:
                 _log.info("Total time = %f sec", time.time() - starttime)
                 return divisor
+    return 1
```

### Comparing `nzmath-3.0.0/src/factor/util.py` & `nzmath-3.0.1/src/factor/util.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/finitefield.py` & `nzmath-3.0.1/src/finitefield.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/group.py` & `nzmath-3.0.1/src/group.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/imaginary.py` & `nzmath-3.0.1/src/imaginary.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/intresidue.py` & `nzmath-3.0.1/src/intresidue.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/lattice.py` & `nzmath-3.0.1/src/lattice.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/matrix.py` & `nzmath-3.0.1/src/matrix.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/module.py` & `nzmath-3.0.1/src/module.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/multiplicative.py` & `nzmath-3.0.1/src/multiplicative.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,13 +47,13 @@
     """
     if n == 1:
         return 1
     if prime.primeq(n):
         return 1 + n**m
     s = 1
     for p, e in factor_misc.FactoredInteger(n):
-        t = 1
-        for i in range(1, e + 1):
-            t += (p**i)**m
+        pm = p**m; t = pm + 1
+        for i in range(e - 1):
+            t = t*pm+1
         s *= t
     return s
```

### Comparing `nzmath-3.0.0/src/permute.py` & `nzmath-3.0.1/src/permute.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/plugin/math/__init__.py` & `nzmath-3.0.1/src/plugin/math/__init__.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/plugin/math/_mpmath.py` & `nzmath-3.0.1/src/plugin/math/_mpmath.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/plugin/math/default.py` & `nzmath-3.0.1/src/plugin/math/default.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/plugins.py` & `nzmath-3.0.1/src/plugins.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/array.py` & `nzmath-3.0.1/src/poly/array.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/factor.py` & `nzmath-3.0.1/src/poly/factor.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/formalsum.py` & `nzmath-3.0.1/src/poly/formalsum.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/groebner.py` & `nzmath-3.0.1/src/poly/groebner.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/hensel.py` & `nzmath-3.0.1/src/poly/hensel.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/multiutil.py` & `nzmath-3.0.1/src/poly/multiutil.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/multivar.py` & `nzmath-3.0.1/src/poly/multivar.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/ratfunc.py` & `nzmath-3.0.1/src/poly/ratfunc.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/ring.py` & `nzmath-3.0.1/src/poly/ring.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/termorder.py` & `nzmath-3.0.1/src/poly/termorder.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/uniutil.py` & `nzmath-3.0.1/src/poly/uniutil.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/poly/univar.py` & `nzmath-3.0.1/src/poly/univar.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/prime.py` & `nzmath-3.0.1/src/prime.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,37 +424,14 @@
     elif n < 10 ** 12:
         # 1369 == 37**2
         # 1662803 is the only prime base in smallSpsp which has not checked
         return n < 1369 or n == 1662803 or smallSpsp(n)
     else:
         return full_euler(n, pdivisors)
 
-def properDivisors(n):
-    """
-    Return proper divisors of n (divisors of n excluding 1 and n).
-
-    It is only useful for a product of small primes.
-    One can use FactoredInteger.proper_divisors() as well.
-
-    DEPRECATION: this function will be removed in version 1.3.
-    """
-    warnings.warn(DeprecationWarning("properDivisor is deprecated"))
-
-    if n in (1, 2, 3, 5, 7, 11, 13, 17, 19, 23):
-        return []
-    else:
-        l = [1]
-        for p, e in _factor(n):
-            for j in range(1, e + 1):
-                l += [k*pow(p, j) for k in l if k % p != 0]
-        l.remove(1)
-        l.remove(n)
-        l.sort()
-        return l
-
 def _factor(n, bound=0):
     """
     Trial division factorization for a natural number.
     Optional second argument is a search bound of primes.
     If the bound is given and less than the sqaure root of n,
     result is not proved to be a prime factorization.
     """
```

### Comparing `nzmath-3.0.0/src/prime_decomp.py` & `nzmath-3.0.1/src/prime_decomp.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/quad.py` & `nzmath-3.0.1/src/quad.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/rational.py` & `nzmath-3.0.1/src/rational.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/real.py` & `nzmath-3.0.1/src/real.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/ring.py` & `nzmath-3.0.1/src/ring.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/round2.py` & `nzmath-3.0.1/src/round2.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/sequence.py` & `nzmath-3.0.1/src/sequence.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import lru_cache
+
 def generator_fibonacci(n=None):
     """
     Generate Fibonacci number up to n-th term if n is assigned
     else infinity.
     """
     a = 0
     b = 1
@@ -24,31 +26,35 @@
             yield a
             count += 1
             if n <= count:
                 break
             b += a
 
 
-FIBONACCI = {0:0, 1:1}
+#FIBONACCI = {0:0, 1:1}
+@lru_cache(maxsize=None)
 def fibonacci(n):
     """
     param non-negative integer n
     return the n-th term of the Fibonacci
     effect FIBONACCI[n] = fibonacci(n)
     """
     if n < 0:
         raise ValueError("fibonacci(n)  0 <= n  ?")
+    if n < 2:
+        return n
+    return fibonacci(n-1) + fibonacci(n-2)
+
+    # if n in FIBONACCI:
+    #     return FIBONACCI[n]
+
+    # m = n >> 1
+    # if n & 1 == 0:
+    #     f1 = fibonacci(m - 1)
+    #     f2 = fibonacci(m)
+    #     FIBONACCI[n] = (f1 + f1 + f2) * f2
+    # else:
+    #     f1 = fibonacci(m)
+    #     f2 = fibonacci(m + 1)
+    #     FIBONACCI[n] = f1 ** 2 + f2 ** 2
 
-    if n in FIBONACCI:
-        return FIBONACCI[n]
-
-    m = n >> 1
-    if n & 1 == 0:
-        f1 = fibonacci(m - 1)
-        f2 = fibonacci(m)
-        FIBONACCI[n] = (f1 + f1 + f2) * f2
-    else:
-        f1 = fibonacci(m)
-        f2 = fibonacci(m + 1)
-        FIBONACCI[n] = f1 ** 2 + f2 ** 2
-
-    return FIBONACCI[n]
+    # return FIBONACCI[n]
```

### Comparing `nzmath-3.0.0/src/squarefree.py` & `nzmath-3.0.1/src/squarefree.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/src/vector.py` & `nzmath-3.0.1/src/vector.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testAlgfield.py` & `nzmath-3.0.1/tests/testAlgfield.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testAlgorithm.py` & `nzmath-3.0.1/tests/testAlgorithm.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testAll.py` & `nzmath-3.0.1/tests/testAll.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testArith1.py` & `nzmath-3.0.1/tests/testArith1.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testArygcd.py` & `nzmath-3.0.1/tests/testArygcd.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testBigrandom.py` & `nzmath-3.0.1/tests/testBigrandom.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testBigrange.py` & `nzmath-3.0.1/tests/testBigrange.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testCombinatorial.py` & `nzmath-3.0.1/tests/testCombinatorial.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testCompatibility.py` & `nzmath-3.0.1/tests/testCompatibility.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testCubic_root.py` & `nzmath-3.0.1/tests/testCubic_root.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testEcpp.py` & `nzmath-3.0.1/tests/testEcpp.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testElliptic.py` & `nzmath-3.0.1/tests/testElliptic.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testEquation.py` & `nzmath-3.0.1/tests/testEquation.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testFactorEcm.py` & `nzmath-3.0.1/tests/testFactorEcm.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testFactorMethods.py` & `nzmath-3.0.1/tests/testFactorMethods.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testFactorMisc.py` & `nzmath-3.0.1/tests/testFactorMisc.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testFactorMpqs.py` & `nzmath-3.0.1/tests/testFactorMpqs.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testFactorUtil.py` & `nzmath-3.0.1/tests/testFactorUtil.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testFiniteField.py` & `nzmath-3.0.1/tests/testFiniteField.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testFormalsum.py` & `nzmath-3.0.1/tests/testFormalsum.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testGcd.py` & `nzmath-3.0.1/tests/testGcd.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testGroebner.py` & `nzmath-3.0.1/tests/testGroebner.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testGroup.py` & `nzmath-3.0.1/tests/testGroup.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testImaginary.py` & `nzmath-3.0.1/tests/testImaginary.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testIntresidue.py` & `nzmath-3.0.1/tests/testIntresidue.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testLattice.py` & `nzmath-3.0.1/tests/testLattice.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testMatrix.py` & `nzmath-3.0.1/tests/testMatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 Ra = rational.Rational
 Poly = uniutil.polynomial
 Int = rational.theIntegerRing
 
 # sub test
 try:
-    from test.testMatrixFiniteField import *
+    from testMatrixFiniteField import *
 except:
     try:
-        from nzmath.test.testMatrixFiniteField import *
+        from testMatrixFiniteField import *
     except:
-        from .testMatrixFiniteField import *
+        from testMatrixFiniteField import *
 
 ## for RingMatrix
 a1 = createMatrix(1, 2, [3, 2])
 a2 = Matrix(1, 2, [5, -6])
 a3 = createMatrix(3, 2, [7, 8]+[3, -2]+[0, 10])
 a4 = Matrix(3, 2, [21, -12]+[1, -1]+[0, 0])
 a5 = createMatrix(1, 2, [Poly({0:3, 1:5}, Int), Poly({1:2}, Int)])
```

### Comparing `nzmath-3.0.0/tests/testMatrixFiniteField.py` & `nzmath-3.0.1/tests/testMatrixFiniteField.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testModule.py` & `nzmath-3.0.1/tests/testModule.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testMultiplicative.py` & `nzmath-3.0.1/tests/testMultiplicative.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testMultiutil.py` & `nzmath-3.0.1/tests/testMultiutil.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testMultivar.py` & `nzmath-3.0.1/tests/testMultivar.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testPermute.py` & `nzmath-3.0.1/tests/testPermute.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testPlugins.py` & `nzmath-3.0.1/tests/testPlugins.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testPolyArray.py` & `nzmath-3.0.1/tests/testPolyArray.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testPolyFactor.py` & `nzmath-3.0.1/tests/testPolyFactor.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testPolyHensel.py` & `nzmath-3.0.1/tests/testPolyHensel.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testPolyRing.py` & `nzmath-3.0.1/tests/testPolyRing.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testPrime.py` & `nzmath-3.0.1/tests/testPrime.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testPrime_decomp.py` & `nzmath-3.0.1/tests/testPrime_decomp.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testQuad.py` & `nzmath-3.0.1/tests/testQuad.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testRatfunc.py` & `nzmath-3.0.1/tests/testRatfunc.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testRational.py` & `nzmath-3.0.1/tests/testRational.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testReal.py` & `nzmath-3.0.1/tests/testReal.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testRing.py` & `nzmath-3.0.1/tests/testRing.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testRound2.py` & `nzmath-3.0.1/tests/testRound2.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testSequence.py` & `nzmath-3.0.1/tests/testSequence.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testSquarefree.py` & `nzmath-3.0.1/tests/testSquarefree.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testTermOrder.py` & `nzmath-3.0.1/tests/testTermOrder.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testUniutil.py` & `nzmath-3.0.1/tests/testUniutil.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testUnivar.py` & `nzmath-3.0.1/tests/testUnivar.py`

 * *Files identical despite different names*

### Comparing `nzmath-3.0.0/tests/testVector.py` & `nzmath-3.0.1/tests/testVector.py`

 * *Files identical despite different names*

