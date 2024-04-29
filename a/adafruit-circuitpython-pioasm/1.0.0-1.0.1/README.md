# Comparing `tmp/adafruit-circuitpython-pioasm-1.0.0.tar.gz` & `tmp/adafruit_circuitpython_pioasm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pioasm-1.0.0.tar", last modified: Mon Jan 29 21:03:14 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_pioasm-1.0.1.tar", last modified: Mon Apr 29 19:14:04 2024, max compression
```

## Comparing `adafruit-circuitpython-pioasm-1.0.0.tar` & `adafruit_circuitpython_pioasm-1.0.1.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.736659 adafruit-circuitpython-pioasm-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.728659 adafruit-circuitpython-pioasm-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.728659 adafruit-circuitpython-pioasm-1.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.728659 adafruit-circuitpython-pioasm-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.732659 adafruit-circuitpython-pioasm-1.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-01-29 21:03:14.736659 adafruit-circuitpython-pioasm-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.736659 adafruit-circuitpython-pioasm-1.0.0/adafruit_circuitpython_pioasm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-01-29 21:03:14.000000 adafruit-circuitpython-pioasm-1.0.0/adafruit_circuitpython_pioasm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-01-29 21:03:14.000000 adafruit-circuitpython-pioasm-1.0.0/adafruit_circuitpython_pioasm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 21:03:14.000000 adafruit-circuitpython-pioasm-1.0.0/adafruit_circuitpython_pioasm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-29 21:03:14.000000 adafruit-circuitpython-pioasm-1.0.0/adafruit_circuitpython_pioasm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-29 21:03:14.000000 adafruit-circuitpython-pioasm-1.0.0/adafruit_circuitpython_pioasm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/adafruit_pioasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.732659 adafruit-circuitpython-pioasm-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.732659 adafruit-circuitpython-pioasm-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.736659 adafruit-circuitpython-pioasm-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_7seg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_7seg_fader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_background_morse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_blink.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_hello.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_i2sout.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_led_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_neopixel_bg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_pdm.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_print_c_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_pulsegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_rotaryencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_rxuart.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_txuart.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-29 21:03:01.000000 adafruit-circuitpython-pioasm-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 21:03:14.736659 adafruit-circuitpython-pioasm-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:03:14.736659 adafruit-circuitpython-pioasm-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/tests/pytest_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/tests/test_mov.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/tests/test_nop.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/tests/test_pseudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/tests/test_radix.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-29 21:03:08.000000 adafruit-circuitpython-pioasm-1.0.0/tests/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.828555 adafruit_circuitpython_pioasm-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.816555 adafruit_circuitpython_pioasm-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.820555 adafruit_circuitpython_pioasm-1.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.820555 adafruit_circuitpython_pioasm-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.820555 adafruit_circuitpython_pioasm-1.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-29 19:14:04.828555 adafruit_circuitpython_pioasm-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.828555 adafruit_circuitpython_pioasm-1.0.1/adafruit_circuitpython_pioasm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-29 19:14:04.000000 adafruit_circuitpython_pioasm-1.0.1/adafruit_circuitpython_pioasm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-29 19:14:04.000000 adafruit_circuitpython_pioasm-1.0.1/adafruit_circuitpython_pioasm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:14:04.000000 adafruit_circuitpython_pioasm-1.0.1/adafruit_circuitpython_pioasm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 19:14:04.000000 adafruit_circuitpython_pioasm-1.0.1/adafruit_circuitpython_pioasm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 19:14:04.000000 adafruit_circuitpython_pioasm-1.0.1/adafruit_circuitpython_pioasm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/adafruit_pioasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.824555 adafruit_circuitpython_pioasm-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.824555 adafruit_circuitpython_pioasm-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.828555 adafruit_circuitpython_pioasm-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_7seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_7seg_fader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_background_morse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_blink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_i2sout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_led_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_neopixel_bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_pdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_print_c_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_pulsegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_rotaryencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_rxuart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_txuart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-29 19:13:56.000000 adafruit_circuitpython_pioasm-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:14:04.828555 adafruit_circuitpython_pioasm-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:04.828555 adafruit_circuitpython_pioasm-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/tests/pytest_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/tests/test_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/tests/test_mov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/tests/test_nop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/tests/test_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/tests/test_pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/tests/test_radix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 19:14:02.000000 adafruit_circuitpython_pioasm-1.0.1/tests/test_wrap.py
```

### Comparing `adafruit-circuitpython-pioasm-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_pioasm-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/.gitignore` & `adafruit_circuitpython_pioasm-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/.pre-commit-config.yaml` & `adafruit_circuitpython_pioasm-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/.pylintrc` & `adafruit_circuitpython_pioasm-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_pioasm-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/LICENSE` & `adafruit_circuitpython_pioasm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/LICENSES/BSD-3-Clause.txt` & `adafruit_circuitpython_pioasm-1.0.1/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_pioasm-1.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/LICENSES/MIT.txt` & `adafruit_circuitpython_pioasm-1.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_pioasm-1.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/PKG-INFO` & `adafruit_circuitpython_pioasm-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pioasm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple assembler to convert pioasm to bytes
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PIOASM
 Keywords: adafruit,blinka,circuitpython,micropython,pioasm,rp2040
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pioasm-1.0.0/README.rst` & `adafruit_circuitpython_pioasm-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/adafruit_circuitpython_pioasm.egg-info/PKG-INFO` & `adafruit_circuitpython_pioasm-1.0.1/adafruit_circuitpython_pioasm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pioasm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple assembler to convert pioasm to bytes
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PIOASM
 Keywords: adafruit,blinka,circuitpython,micropython,pioasm,rp2040
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pioasm-1.0.0/adafruit_circuitpython_pioasm.egg-info/SOURCES.txt` & `adafruit_circuitpython_pioasm-1.0.1/adafruit_circuitpython_pioasm.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -48,12 +48,14 @@
 examples/pioasm_pulsegroup.py
 examples/pioasm_rotaryencoder.py
 examples/pioasm_rxuart.py
 examples/pioasm_simpletest.py
 examples/pioasm_txuart.py
 examples/pioasm_wrap.py
 tests/pytest_helpers.py
+tests/test_in.py
 tests/test_mov.py
 tests/test_nop.py
+tests/test_out.py
 tests/test_pseudo.py
 tests/test_radix.py
 tests/test_wrap.py
```

### Comparing `adafruit-circuitpython-pioasm-1.0.0/adafruit_pioasm.py` & `adafruit_circuitpython_pioasm-1.0.1/adafruit_pioasm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import array
 import re
 
 splitter = re.compile(r",\s*|\s+(?:,\s*)?").split
 mov_splitter = re.compile("!|~|::").split
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PIOASM.git"
 
 CONDITIONS = ["", "!x", "x--", "!y", "y--", "x!=y", "pin", "!osre"]
 IN_SOURCES = ["pins", "x", "y", "null", None, None, "isr", "osr"]
 OUT_DESTINATIONS = ["pins", "x", "y", "null", "pindirs", "pc", "isr", "exec"]
 WAIT_SOURCES = ["gpio", "pin", "irq", None]
 MOV_DESTINATIONS = ["pins", "x", "y", None, "exec", "pc", "isr", "osr"]
@@ -143,23 +143,33 @@
                     raise RuntimeError("Wait num out of range")
                 assembled[-1] |= num
                 if instruction[-1] == "rel":
                     assembled[-1] |= 0x10  # Set the high bit of the irq value
             elif instruction[0] == "in":
                 #                instr delay src count
                 assembled.append(0b010_00000_000_00000)
-                assembled[-1] |= IN_SOURCES.index(instruction[1]) << 5
+                source = instruction[1]
+                try:
+                    assembled[-1] |= IN_SOURCES.index(source) << 5
+                except ValueError as exc:
+                    raise ValueError(f"Invalid in source '{source}'") from exc
                 count = int(instruction[-1], 0)
                 if not 1 <= count <= 32:
                     raise RuntimeError("Count out of range")
                 assembled[-1] |= count & 0x1F  # 32 is 00000 so we mask the top
             elif instruction[0] == "out":
                 #                instr delay dst count
                 assembled.append(0b011_00000_000_00000)
-                assembled[-1] |= OUT_DESTINATIONS.index(instruction[1]) << 5
+                destination = instruction[1]
+                try:
+                    assembled[-1] |= OUT_DESTINATIONS.index(destination) << 5
+                except ValueError as exc:
+                    raise ValueError(
+                        f"Invalid out destination '{destination}'"
+                    ) from exc
                 count = int(instruction[-1], 0)
                 if not 1 <= count <= 32:
                     raise RuntimeError("Count out of range")
                 assembled[-1] |= count & 0x1F  # 32 is 00000 so we mask the top
             elif instruction[0] == "push" or instruction[0] == "pull":
                 #                instr delay d i b zero
                 assembled.append(0b100_00000_0_0_0_00000)
```

### Comparing `adafruit-circuitpython-pioasm-1.0.0/docs/_static/favicon.ico` & `adafruit_circuitpython_pioasm-1.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/docs/conf.py` & `adafruit_circuitpython_pioasm-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/docs/index.rst` & `adafruit_circuitpython_pioasm-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_7seg.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_7seg.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_7seg_fader.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_7seg_fader.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_background_morse.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_background_morse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_blink.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_blink.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_hello.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_hello.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_i2sout.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_i2sout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_led_brightness.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_led_brightness.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_neopixel.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_neopixel_bg.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_neopixel_bg.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_pdm.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_pdm.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_print_c_program.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_print_c_program.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_pulsegroup.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_pulsegroup.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_rotaryencoder.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_rotaryencoder.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_rxuart.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_rxuart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_simpletest.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/examples/pioasm_txuart.py` & `adafruit_circuitpython_pioasm-1.0.1/examples/pioasm_txuart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/pyproject.toml` & `adafruit_circuitpython_pioasm-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pioasm"
 description = "Simple assembler to convert pioasm to bytes"
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_PIOASM"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-pioasm-1.0.0/tests/pytest_helpers.py` & `adafruit_circuitpython_pioasm-1.0.1/tests/pytest_helpers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/tests/test_mov.py` & `adafruit_circuitpython_pioasm-1.0.1/tests/test_mov.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-1.0.0/tests/test_nop.py` & `adafruit_circuitpython_pioasm-1.0.1/tests/test_nop.py`

 * *Files identical despite different names*

