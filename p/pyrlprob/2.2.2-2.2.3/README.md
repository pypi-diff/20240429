# Comparing `tmp/pyrlprob-2.2.2.tar.gz` & `tmp/pyrlprob-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrlprob-2.2.2.tar", last modified: Wed Feb 28 00:07:43 2024, max compression
+gzip compressed data, was "pyrlprob-2.2.3.tar", last modified: Mon Apr 29 21:01:59 2024, max compression
```

## Comparing `pyrlprob-2.2.2.tar` & `pyrlprob-2.2.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/LICENSE.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/MANIFEST.in
--rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2800 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/PKG-INFO
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1787 2024-02-16 17:50:32.000000 pyrlprob-2.2.2/README.md
--rw-------   0 lorenzof (332258323) domainusers (245600513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyproject.toml
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.887734 pyrlprob-2.2.2/pyrlprob/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/__main__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    15478 2024-02-16 19:14:22.000000 pyrlprob-2.2.2/pyrlprob/base_funs.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/commands.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.887734 pyrlprob-2.2.2/pyrlprob/include/
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/pyrlprob/include/pyrlprob/
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/include/pyrlprob/binding.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/include/pyrlprob/mdp.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/include/pyrlprob/mdp_vec.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/include/pyrlprob/py_mdp.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     7733 2024-02-16 19:04:09.000000 pyrlprob-2.2.2/pyrlprob/mdp.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/pyrlprob/models/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      151 2024-02-19 17:55:58.000000 pyrlprob-2.2.2/pyrlprob/models/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    40403 2024-02-27 23:51:50.000000 pyrlprob-2.2.2/pyrlprob/models/models.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    13568 2024-02-19 17:56:10.000000 pyrlprob-2.2.2/pyrlprob/problem.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/pyrlprob/tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/__init__.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/binding.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d.py
--rwx------   0 lorenzof (332258323) domainusers (245600513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
--rw-------   0 lorenzof (332258323) domainusers (245600513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d_dyn.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/rk4.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1358 2024-02-16 18:24:51.000000 pyrlprob-2.2.2/pyrlprob/tests/landing1d_cpp.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1961 2024-02-27 23:55:41.000000 pyrlprob-2.2.2/pyrlprob/tests/landing1d_gtrxl_py.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1637 2024-02-16 19:31:26.000000 pyrlprob-2.2.2/pyrlprob/tests/landing1d_load.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1811 2024-02-27 23:01:24.000000 pyrlprob-2.2.2/pyrlprob/tests/landing1d_lstm_py.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1341 2024-02-16 19:10:05.000000 pyrlprob-2.2.2/pyrlprob/tests/landing1d_py.yaml
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/pyrlprob/tests/py_tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4931 2024-02-16 18:20:05.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/landing1d.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/landing1d_dyn.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     6379 2024-02-16 18:26:17.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/landing1d_gym.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     5904 2024-02-16 19:32:59.000000 pyrlprob-2.2.2/pyrlprob/tests/test_landing1d.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2813 2024-02-16 17:36:47.000000 pyrlprob-2.2.2/pyrlprob/tests/test_multiple_gym.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/pyrlprob/tune/
--rw-------   0 lorenzof (332258323) domainusers (245600513)       87 2024-02-16 18:28:30.000000 pyrlprob-2.2.2/pyrlprob/tune/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3393 2024-02-16 18:35:28.000000 pyrlprob-2.2.2/pyrlprob/tune/tune.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/pyrlprob/utils/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.2.2/pyrlprob/utils/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3446 2024-02-16 17:36:47.000000 pyrlprob-2.2.2/pyrlprob/utils/auxiliary.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4722 2024-02-16 19:07:37.000000 pyrlprob-2.2.2/pyrlprob/utils/callbacks.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2835 2024-02-16 19:07:46.000000 pyrlprob-2.2.2/pyrlprob/utils/plots.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-02-28 00:07:43.887734 pyrlprob-2.2.2/pyrlprob.egg-info/
--rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2800 2024-02-28 00:07:43.000000 pyrlprob-2.2.2/pyrlprob.egg-info/PKG-INFO
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2633 2024-02-28 00:07:43.000000 pyrlprob-2.2.2/pyrlprob.egg-info/SOURCES.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)        1 2024-02-28 00:07:43.000000 pyrlprob-2.2.2/pyrlprob.egg-info/dependency_links.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)      219 2024-02-28 00:07:43.000000 pyrlprob-2.2.2/pyrlprob.egg-info/requires.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)        9 2024-02-28 00:07:43.000000 pyrlprob-2.2.2/pyrlprob.egg-info/top_level.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)       38 2024-02-28 00:07:43.891734 pyrlprob-2.2.2/setup.cfg
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1278 2024-02-27 23:55:52.000000 pyrlprob-2.2.2/setup.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/LICENSE.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/MANIFEST.in
+-rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2800 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/PKG-INFO
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1787 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/README.md
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyproject.toml
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/__main__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    16762 2024-04-29 20:54:47.000000 pyrlprob-2.2.3/pyrlprob/base_funs.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/commands.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/include/
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/binding.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/mdp.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/mdp_vec.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/py_mdp.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     7733 2024-02-16 19:04:09.000000 pyrlprob-2.2.3/pyrlprob/mdp.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/models/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      151 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/models/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    29760 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/models/models.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    14323 2024-04-29 20:57:36.000000 pyrlprob-2.2.3/pyrlprob/problem.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/__init__.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/binding.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.py
+-rwx------   0 lorenzof (332258323) domainusers (245600513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/rk4.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1358 2024-02-16 18:24:51.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_cpp.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1961 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_gtrxl_py.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1637 2024-02-16 19:31:26.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_load.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1811 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_lstm_py.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1341 2024-02-16 19:10:05.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_py.yaml
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/tests/py_tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4931 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d_dyn.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     6379 2024-02-16 18:26:17.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d_gym.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     5902 2024-04-29 20:57:24.000000 pyrlprob-2.2.3/pyrlprob/tests/test_landing1d.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2813 2024-02-16 17:36:47.000000 pyrlprob-2.2.3/pyrlprob/tests/test_multiple_gym.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/tune/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)       87 2024-02-16 18:28:30.000000 pyrlprob-2.2.3/pyrlprob/tune/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3393 2024-02-16 18:35:28.000000 pyrlprob-2.2.3/pyrlprob/tune/tune.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/utils/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/utils/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3446 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/utils/auxiliary.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4722 2024-02-16 19:07:37.000000 pyrlprob-2.2.3/pyrlprob/utils/callbacks.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2835 2024-02-16 19:07:46.000000 pyrlprob-2.2.3/pyrlprob/utils/plots.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob.egg-info/
+-rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2800 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/PKG-INFO
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2633 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/SOURCES.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)        1 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/dependency_links.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      219 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/requires.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)        9 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/top_level.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)       38 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/setup.cfg
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1278 2024-04-29 20:58:42.000000 pyrlprob-2.2.3/setup.py
```

### Comparing `pyrlprob-2.2.2/LICENSE.txt` & `pyrlprob-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/PKG-INFO` & `pyrlprob-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.2.2
+Version: 2.2.3
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrlprob-2.2.2/README.md` & `pyrlprob-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/__main__.py` & `pyrlprob-2.2.3/pyrlprob/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/base_funs.py` & `pyrlprob-2.2.3/pyrlprob/base_funs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from pyrlprob.utils.auxiliary import *
 import pyrlprob.utils.callbacks as callbacks
 
 
 def training(trainer: Union[str, Callable, Type], 
              config: Dict[str, Any], 
              stop: Dict[str, Any], 
+             num_cp_to_keep: str="all",
+             evaluation_active: bool=False,
              logdir: Optional[str]=None,
              create_out_file: bool=True, 
              load: Optional[Dict[str, Any]]=None, 
              debug: bool=False,
              open_ray: bool=True,
              return_time: bool=False) -> \
                  Union[Tuple[Dict[str, Any], str, str, int, float], \
@@ -27,14 +29,16 @@
     """
     Train the current model with ray.tune, using the specified trainer and configs.
 
     Args:
         trainer (str or callable): trainer (i.e., RL algorithm) to train the model with
         config (dict): config file (dictionary)
         stop (dict): stopping conditions (dictionary)
+        num_cp_to_keep (str): number of checkpoints to keep. If "all", all checkpoints are kept, if "best", only the best checkpoint is kept
+        evaluation_active (bool): whether evaluation is active
         logdir (str): name of the directory where training results are saved
         create_out_file (bool): whether to create an outfile with run time and best result
         load (dict): dictionary containing the directory and checkpoint where the 
             pre-trained model to load is located
         debug (bool): whether to print worker's logs.
         open_ray (bool): whether to open/close ray
         return_time (bool): whether to return run time per iter
@@ -43,62 +47,81 @@
         best_result (str): best result of the experiment
         trainer_dir (str): trainer's output directory
         best_exp_dir (str): directory containing the best experiment's output
         last_checkpoint (int): last checkpoint saved
         (optional) run_time (float): total run time
     """
 
-    #Create output folder
+    # Create output folder
     if load is not None:
         outdir = load["logdir"]
         restore = load["checkpoint_dir"]
     else:
         if logdir is None:
             outdir = "./results/"
         else:
             outdir = logdir
         os.makedirs(outdir, exist_ok=True)
         restore = None
 
-    #Initialize ray
+    # Initialize ray
     if open_ray:
         if debug:
             logging_level = "INFO"
         else:
             logging_level = "ERROR"
         ray.init(logging_level=logging_level, 
             log_to_driver=debug, 
             ignore_reinit_error=True)
     
-    #Train the model
+    # Checkpoint saving
+    if num_cp_to_keep == "all":
+        keep_checkpoints_num = None
+        checkpoint_score_attr = None
+    elif num_cp_to_keep == "best":
+        keep_checkpoints_num = 1
+        if evaluation_active:
+            checkpoint_score_attr = "evaluation/episode_reward_mean"
+        else:
+            checkpoint_score_attr = "episode_reward_mean"
+    else:
+        keep_checkpoints_num = None
+        checkpoint_score_attr = None
+
+    # Train the model
     start_time = time.time()
     analysis = tune.run(trainer,
                         config=config,
                         local_dir=outdir,
                         restore=restore,
                         stop=stop,
                         metric="episode_reward_mean",
                         mode="max",
                         checkpoint_freq=1,
                         checkpoint_at_end=True,
-                        keep_checkpoints_num=None)
+                        keep_checkpoints_num=keep_checkpoints_num,
+                        checkpoint_score_attr=checkpoint_score_attr)
     end_time = time.time()
     run_time = end_time - start_time
 
-    #Last iteration stats
+    # Last iteration stats
     best_result = analysis.best_result
     last_result = analysis.get_best_trial("training_iteration", "max").last_result
     best_exp_dir = analysis.best_logdir
     trainer_dir = best_exp_dir[:best_exp_dir.rfind("/")+1]
     best_exp_dir = best_exp_dir + "/"
 
-    #Last checkpoint
-    last_checkpoint = last_result["training_iteration"]
-
-    #Run time per iter
+    # Last checkpoint
+    best_checkpoint_path = analysis.best_checkpoint
+    if num_cp_to_keep == "best":
+        last_checkpoint = int(best_checkpoint_path[best_checkpoint_path.rfind("-")+1:])
+    else:
+        last_checkpoint = last_result["training_iteration"]
+    
+    # Run time per iter
     run_time_per_iter = last_result["time_this_iter_s"]
 
     # Save elapsed time and results
     if create_out_file:
         f_out_res = open(best_exp_dir + "result.txt", "w")
         f_out_res.write("%22s %22s %22s %22s %22s\n" \
             % ("# elapsed time [s]", "training_iteration", \
@@ -106,20 +129,20 @@
         f_out_res.write("%22.7f %22d %22.7f %22.7f %22.7f\n" \
             % (run_time, best_result["training_iteration"], \
                 best_result["episode_reward_mean"], \
                 best_result["episode_reward_max"], \
                 best_result["episode_reward_min"]))
         f_out_res.close()
 
-    #Terminate ray
+    # Terminate ray
     if open_ray:
         ray.shutdown()
 
-    #Return trainer and best experiment directory + last checkpoint saved
-    #and the run time per iter
+    # Return trainer and best experiment directory + last checkpoint saved
+    # and the run time per iter
     if return_time:
         return best_result, trainer_dir, best_exp_dir, last_checkpoint, run_time_per_iter
     else:
         return best_result, trainer_dir, best_exp_dir, last_checkpoint
 
 
 def evaluation(trainer: Union[str, Callable, Type], 
@@ -148,37 +171,43 @@
         last_cps (list): list with last checkpoint number of each experiment in exp_dirs
         config (dict): config file (dictionary)
         env_name (str): environment class name
         env_config (dict): dictionary containing the environment configs
         evaluation_num_episodes (int): number of evaluation episodes
         evaluation_config (dict): dictionary containing the evaluation configs
         custom_eval_function (callable or str): Custom evaluation function (or function name)
-        best_metric (str): metric to be used to determine the best checkpoint in exp_dirs
+        best_metric (str): metric to be used to determine the best checkpoint in exp_dirs.
+            It it is a number, that checkpoint will be used.
         min_or_max (str): if best_metric must be minimized or maximized
         metrics_and_data (dict): dictionary containing the metrics and data to save
             in the new file progress.csv
         is_evaluation_env (bool): are metrics computed through an evaluation environment?
         do_postprocess (bool): whether to do postprocessing
         debug (bool):  whether to print data fro debugging
     """
     
     # Path of metrics
     metric_path = ""
     if is_evaluation_env:
         metric_path = "evaluation/"
 
     if trainer_dir is not None:
-        # Determine the best checkpoint
-        best_metric_trend = metric_training_trend(metric_path + best_metric,
-                                            exp_dirs,
-                                            last_cps)
-        if min_or_max == "max":
-            best_cp = np.argmax(best_metric_trend)+1
+        # Check if best_metric is a number
+        best_metric = str(best_metric)
+        if best_metric.isdigit():
+            best_cp = int(best_metric)
         else:
-            best_cp = np.argmin(best_metric_trend)+1
+            # Get the best metric trend
+            best_metric_trend = metric_training_trend(metric_path + best_metric,
+                                                exp_dirs,
+                                                last_cps)
+            if min_or_max == "max":
+                best_cp = np.argmax(best_metric_trend)+1
+            else:
+                best_cp = np.argmin(best_metric_trend)+1
         best_exp = next(exp for exp, cp in enumerate(last_cps) if cp >= best_cp)
         best_exp_dir = exp_dirs[best_exp]
 
         # Define load properties
         load = {}
         load["logdir"] = trainer_dir
         _, load["checkpoint_dir"] = \
```

### Comparing `pyrlprob-2.2.2/pyrlprob/commands.py` & `pyrlprob-2.2.3/pyrlprob/commands.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/include/pyrlprob/binding.cpp` & `pyrlprob-2.2.3/pyrlprob/include/pyrlprob/binding.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/include/pyrlprob/mdp.h` & `pyrlprob-2.2.3/pyrlprob/include/pyrlprob/mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/include/pyrlprob/mdp_vec.h` & `pyrlprob-2.2.3/pyrlprob/include/pyrlprob/mdp_vec.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/include/pyrlprob/py_mdp.h` & `pyrlprob-2.2.3/pyrlprob/include/pyrlprob/py_mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/mdp.py` & `pyrlprob-2.2.3/pyrlprob/mdp.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/models/models.py` & `pyrlprob-2.2.3/pyrlprob/models/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -401,255 +401,14 @@
 
 
     @override(ModelV2)
     def value_function(self):
         return tf.reshape(self._value_out, [-1])
 
 
-# class MLPplusGTrXL(RecurrentNetwork):
-#     """GTrXL-based model for meta-RL. The policy model is made up of an encoder and a GTrXL net.
-#      The encoder is a simple feedforward network that preprocesses the observation before sending
-#      it to the GTrXL. The GTrXL then outputs the logits.
-#      The value function estimate is computed by a separate feedforward network that takes the
-#      same observation as input.
-    
-#      Args:
-#         custom_model_kwargs:
-#             num_transformer_units (int): The number of transformer units.
-#             attention_dim (int): The dimension of the transformer units.
-#             num_heads (int): The number of heads in the attention.
-#             head_dim (int): The dimension of each head.
-#             memory_inference (int): The number of previous outputs to use as memory input to each layer.
-#             position_wise_mlp_dim (int): The dimension of the position-wise MLP.
-#             init_gru_gate_bias (float): The initial bias of the GRU gate.
-#             encoder_hiddens (list): The sizes of the hidden layers of the encoder.
-#             encoder_activation (str): The activation function of the encoder.
-#             vf_hiddens (list): The sizes of the hidden layers of the value function.
-#             vf_activation (str): The activation function of the value function.
-#         model_config:
-#             max_seq_len (int): The maximum length of the input observation sequence.
-#             vf_share_layers (bool): Whether to share the layers of the value function with the policy.
-#             free_log_std (bool): Whether to generate free-floating bias variables for the second half of the model outputs.
-#     """
-
-#     def __init__(
-#         self,
-#         obs_space,
-#         action_space,
-#         num_outputs,
-#         model_config,
-#         name,
-#         **custom_model_kwargs
-#     ):
-#         super(MLPplusGTrXL, self).__init__(
-#             obs_space, action_space, num_outputs, model_config, name
-#         )
-
-#         if logger.isEnabledFor(logging.INFO):
-#             print("custom_model_kwargs: {}".format(custom_model_kwargs))
-
-#         self.num_transformer_units = custom_model_kwargs.get("num_transformer_units")
-#         self.attention_dim = custom_model_kwargs.get("attention_dim")
-#         self.num_heads = custom_model_kwargs.get("num_heads")
-#         self.head_dim = custom_model_kwargs.get("head_dim")
-#         self.memory_inference = custom_model_kwargs.get("memory_inference")
-#         self.position_wise_mlp_dim = custom_model_kwargs.get("position_wise_mlp_dim")
-#         self.init_gru_gate_bias = custom_model_kwargs.get("init_gru_gate_bias")
-#         self.max_seq_len = model_config.get("max_seq_len")
-        
-#         self.encoder_hiddens = list(custom_model_kwargs.get("encoder_hiddens", []))
-#         self.encoder_activation = custom_model_kwargs.get("encoder_activation")
-#         encoder_activation = get_activation_fn(self.encoder_activation)
-
-#         vf_share_layers = model_config.get("vf_share_layers")
-#         free_log_std = model_config.get("free_log_std")
-#         if not vf_share_layers:
-#             self.vf_hiddens = list(custom_model_kwargs.get("vf_hiddens", []))
-#             self.vf_activation = custom_model_kwargs.get("vf_activation")
-#             vf_activation = get_activation_fn(self.vf_activation)
-
-#         self.obs_dim = obs_space.shape[0]
-#         self.num_outputs = num_outputs
-
-#         # Generate free-floating bias variables for the second half of
-#         # the outputs.
-#         if free_log_std:
-#             assert num_outputs % 2 == 0, (
-#                 "num_outputs must be divisible by two",
-#                 num_outputs,
-#             )
-#             num_outputs = num_outputs // 2
-#             self.log_std_var = tf.Variable(
-#                 [0.0] * num_outputs, dtype=tf.float32, name="log_std"
-#             )
-
-#         # Observation input: sequence of last max_seq_len observations
-#         input_layer = tf.keras.layers.Input(
-#             shape=(self.max_seq_len, self.obs_dim), name="inputs"
-#         )
-
-#         # Memory inputs: sequence of last memory_inference outputs,
-#         # each with dimension (max_seq_len, attention_dim), of each transformer unit
-#         memory_ins = [
-#             tf.keras.layers.Input(
-#                 shape=(self.memory_inference*self.max_seq_len, self.attention_dim),
-#                 dtype=tf.float32,
-#                 name="memory_in_{}".format(i),
-#             )
-#             for i in range(self.num_transformer_units)
-#         ]
-
-#         # Preprocess observation with the encoder_hiddens and send the output to the LSTM cell
-#         last_layer = input_layer
-#         if len(self.encoder_hiddens) > 0:
-#             i = 1
-#             for size in self.encoder_hiddens:
-#                 last_layer = tf.keras.layers.Dense(
-#                     size,
-#                     name="fc_encoder_{}".format(i),
-#                     activation=encoder_activation,
-#                     kernel_initializer=normc_initializer(1.0),
-#                 )(last_layer)
-#                 i += 1
-
-#         # Map encoder dim to input/output transformer (attention) dim.
-#         E_out = tf.keras.layers.Dense(self.attention_dim)(last_layer)
-
-#         # Output, collected and concat'd to build the internal
-#         # memory units used for additional contextual information.
-#         memory_outs = []
-
-#         # 2) Create N Transformer blocks
-#         for i in range(self.num_transformer_units):
-#             # RelativeMultiHeadAttention part.
-#             MHA_out = SkipConnection(
-#                 RelativeMultiHeadAttention(
-#                     out_dim=self.attention_dim,
-#                     num_heads=self.num_heads,
-#                     head_dim=self.head_dim,
-#                     input_layernorm=True,
-#                     output_activation=tf.nn.relu,
-#                 ),
-#                 fan_in_layer=GRUGate(self.init_gru_gate_bias),
-#                 name="mha_{}".format(i + 1),
-#             )(E_out, memory=memory_ins[i])
-
-#             # Position-wise MLP part.
-#             E_out = SkipConnection(
-#                 tf.keras.Sequential(
-#                     (
-#                         tf.keras.layers.LayerNormalization(axis=-1),
-#                         PositionwiseFeedforward(
-#                             out_dim=self.attention_dim,
-#                             hidden_dim=self.position_wise_mlp_dim,
-#                             output_activation=tf.nn.relu,
-#                         ),
-#                     )
-#                 ),
-#                 fan_in_layer=GRUGate(self.init_gru_gate_bias),
-#                 name="pos_wise_mlp_{}".format(i + 1),
-#             )(MHA_out)
-#             # Output of position-wise MLP == E(l-1), which is concat'd
-#             # to the current Mem block (M(l-1)) to yield E~(l-1), which is then
-#             # used by the next transformer block.
-#             memory_outs.append(E_out)
-
-#         # Postprocess TrXL output with another hidden layer and compute values.
-#         logits = tf.keras.layers.Dense(
-#             num_outputs, activation=tf.keras.activations.linear, name="logits"
-#         )(E_out)
-
-#         # Concat the log std vars to the end of the state-dependent means.
-#         if free_log_std:
-
-#             def tiled_log_std(x):
-#                 return tf.tile(tf.expand_dims(tf.expand_dims(self.log_std_var, 0),1), [tf.shape(x)[0], tf.shape(x)[1], 1])
-
-#             log_std_out = tf.keras.layers.Lambda(tiled_log_std)(input_layer)
-#             logits = tf.keras.layers.Concatenate(axis=2)([logits, log_std_out])
-        
-#         # Compute value estimate with the vf_hiddens
-#         if not vf_share_layers:
-#             last_vf_layer = input_layer
-#             i = 1
-#             for size in self.vf_hiddens:
-#                 last_vf_layer = tf.keras.layers.Dense(
-#                     size,
-#                     name="fc_value_{}".format(i),
-#                     activation=vf_activation,
-#                     kernel_initializer=normc_initializer(1.0),
-#                 )(last_vf_layer)
-#                 i += 1
-#         else:
-#             last_vf_layer = E_out
-#         value_out = tf.keras.layers.Dense(
-#             1,
-#             name="value_out",
-#             activation=None,
-#             kernel_initializer=normc_initializer(0.01),
-#         )(last_vf_layer)
-
-#         outs = [logits, value_out]
-
-#         self.gtrxl_model = tf.keras.models.Model(inputs=[input_layer] + memory_ins, \
-#                                                  outputs=outs + memory_outs)
-
-#         # Print out model summary in INFO logging mode.
-#         # if logger.isEnabledFor(logging.INFO):
-#         self.gtrxl_model.summary()
-
-#     @override(RecurrentNetwork)
-#     def forward_rnn(
-#         self, inputs: TensorType, state: List[TensorType], seq_lens: TensorType
-#     ) -> tuple[TensorType, List[TensorType]]:
-        
-#         # Last max_seq_len observations
-#         observations = state[0]
-#         observations = tf.concat((observations, inputs), axis=1)[:, -self.max_seq_len:, :]
-
-#         # Memory inputs
-#         memory_ins = state[1:]
-        
-#         # Pass the observations and the previous memory to the model
-#         all_outs = self.gtrxl_model([observations] + memory_ins)
-
-#         # Logits and value estimate
-#         logits = all_outs[0]
-#         T = tf.shape(inputs)[1]  # Length of input segment (time).
-#         logits = logits[:, -T:, :]  # Only take the last T logits.
-#         self._value_out = all_outs[1]
-
-#         # Memory outputs
-#         memory_outs = all_outs[2:]
-
-#         # New memory inputs
-#         memory_ins_new = []
-#         for i in range(self.num_transformer_units):
-#             memory_ins_new.append(tf.concat((memory_ins[i], memory_outs[i]), axis=1)[:, -self.memory_inference*self.max_seq_len:, :])
-
-#         # New state
-#         new_state = [observations] + memory_ins_new
-
-#         return logits, new_state
-
-#     @override(RecurrentNetwork)
-#     def get_initial_state(self) -> List[np.ndarray]:
-#         # Initialize last max_seq_len observations to zeros
-#         state = [np.zeros((self.max_seq_len, self.obs_dim), np.float32)]
-
-#         # Initialize memory inputs to zeros
-#         for _ in range(self.num_transformer_units):
-#             state.append(np.zeros((self.memory_inference*self.max_seq_len, self.attention_dim), np.float32))
-#         return state
-
-#     @override(ModelV2)
-#     def value_function(self) -> TensorType:
-#         return tf.reshape(self._value_out, [-1])
-
-
 class MLPplusGTrXL(RecurrentNetwork):
     """GTrXL-based model for meta-RL. The policy model is made up of an encoder and a GTrXL net.
      The encoder is a simple feedforward network that preprocesses the observation before sending
      it to the GTrXL, plus, possibly, the previous n actions and rewards. The GTrXL then outputs the logits.
      The value function estimate is either computed by a separate feedforward network that takes the
      same observation as input, or is an additional output of the GTrXL.
```

### Comparing `pyrlprob-2.2.2/pyrlprob/problem.py` & `pyrlprob-2.2.3/pyrlprob/problem.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,14 +140,15 @@
             self.load["last_cps"] = settings["load"]["prev_last_cps"]
             _, self.load["checkpoint_dir"] = \
                 get_cp_dir_and_model(self.load["exp_dirs"][-1], self.load["last_cps"][-1])
     
 
     def solve(self,
               logdir: Optional[str]=None,
+              num_cp_to_keep: str="all",
               evaluate: bool=True, 
               best_metric: str="episode_reward_mean",
               min_or_max: str="max",
               postprocess: bool=True,
               debug: bool=False,
               open_ray: bool=True,
               return_time: bool=False) ->  \
@@ -156,16 +157,18 @@
         """
         Solve a RL problem.
         It include pre-processing and training, 
         and may include evaluation and post-processing.
 
         Args:
             logdir (str): name of the directory where training results are saved
+            num_cp_to_keep (str): number of checkpoints to keep. If "all", all checkpoints are kept, if "best", only the best checkpoint is kept
             evaluate (bool): whether to do evaluation
-            best_metric (str): metric to be used to determine the best checkpoint in exp_dir during evaluation
+            best_metric (str): metric to be used to determine the best checkpoint in exp_dir during evaluation.
+                It it is a number, that checkpoint will be used.
             min_or_max (str): if best_metric must be minimized or maximized
             postprocess (bool): whether to do postprocessing
             debug (bool): whether to print worker's logs.
             open_ray (bool): whether to open/close ray
             return_time (bool): whether to return run time per iter
         
         Return:
@@ -178,35 +181,41 @@
         """
         
         #Training
         if return_time:
             best_result, trainer_dir, best_exp_dir, last_checkpoint, run_time = training(trainer=self.trainer, 
                                                                             config=self.config, 
                                                                             stop=self.stop,
+                                                                            num_cp_to_keep=num_cp_to_keep,
+                                                                            evaluation_active=self.evaluation,
                                                                             logdir=logdir,
                                                                             load=self.load,
                                                                             debug=debug,
                                                                             open_ray=open_ray,
                                                                             return_time=return_time)
         else:
             best_result, trainer_dir, best_exp_dir, last_checkpoint = training(trainer=self.trainer, 
                                                                   config=self.config, 
                                                                   stop=self.stop,
+                                                                  num_cp_to_keep=num_cp_to_keep,
+                                                                  evaluation_active=self.evaluation,
                                                                   logdir=logdir,
                                                                   load=self.load,
                                                                   debug=debug,
                                                                   open_ray=open_ray,
                                                                   return_time=return_time)
         
         #Save config file
         with open(best_exp_dir + "config.yaml", 'w') as outfile:
             yaml.dump(self.input_config, outfile)
         
         #Evaluation and Postprocessing
         if evaluate:
+            if num_cp_to_keep == "best":
+                best_metric = last_checkpoint
             exp_dirs, last_cps, best_cp_dir = self.evaluate(trainer_dir=trainer_dir,
                                                             exp_dir=best_exp_dir,
                                                             last_checkpoint=last_checkpoint,
                                                             best_metric=best_metric,
                                                             min_or_max=min_or_max,
                                                             do_postprocess=postprocess,
                                                             debug=debug)
```

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d.cpp` & `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d.h` & `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d.py` & `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so` & `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/landing1d_dyn.h` & `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/cpp_tests/rk4.h` & `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/rk4.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/landing1d_cpp.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/landing1d_cpp.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/landing1d_gtrxl_py.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/landing1d_gtrxl_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/landing1d_load.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/landing1d_load.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/landing1d_lstm_py.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/landing1d_lstm_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/landing1d_py.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/landing1d_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/landing1d.py` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/landing1d_dyn.py` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d_dyn.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/landing1d_gym.py` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml` & `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/test_landing1d.py` & `pyrlprob-2.2.3/pyrlprob/tests/test_landing1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         py_or_cpp: python or cpp version of the environment?
         res_dir: path where results are saved. Current directory if not specified.
     """
 
     #Config file
     __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
     if py_or_cpp == "py":
-        if model == "fcnet":
+        if model == "mlp":
             config = os.path.join(__location__, "landing1d_py.yaml")
         elif model == "lstm":
             config = os.path.join(__location__, "landing1d_lstm_py.yaml")
         elif model == "gtrxl":
             config = os.path.join(__location__, "landing1d_gtrxl_py.yaml")
         else:
             assert False, "Model not implemented."
```

### Comparing `pyrlprob-2.2.2/pyrlprob/tests/test_multiple_gym.py` & `pyrlprob-2.2.3/pyrlprob/tests/test_multiple_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/tune/tune.py` & `pyrlprob-2.2.3/pyrlprob/tune/tune.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/utils/__init__.py` & `pyrlprob-2.2.3/pyrlprob/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/utils/auxiliary.py` & `pyrlprob-2.2.3/pyrlprob/utils/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/utils/callbacks.py` & `pyrlprob-2.2.3/pyrlprob/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob/utils/plots.py` & `pyrlprob-2.2.3/pyrlprob/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/pyrlprob.egg-info/PKG-INFO` & `pyrlprob-2.2.3/pyrlprob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.2.2
+Version: 2.2.3
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrlprob-2.2.2/pyrlprob.egg-info/SOURCES.txt` & `pyrlprob-2.2.3/pyrlprob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.2/setup.py` & `pyrlprob-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pyrlprob',
-    version='2.2.2',
+    version='2.2.3',
     author='Lorenzo Federici',
     author_email = 'federicilorenzo94@gmail.com',
     description = 'Train Gym-derived environments in Python/C++ through Ray RLlib',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/LorenzoFederici/pyrlprob',
     classifiers = [
```

