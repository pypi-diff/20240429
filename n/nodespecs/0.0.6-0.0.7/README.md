# Comparing `tmp/nodespecs-0.0.6.tar.gz` & `tmp/nodespecs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodespecs-0.0.6.tar", last modified: Tue Apr 23 13:38:25 2024, max compression
+gzip compressed data, was "nodespecs-0.0.7.tar", last modified: Mon Apr 29 18:55:28 2024, max compression
```

## Comparing `nodespecs-0.0.6.tar` & `nodespecs-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 13:38:25.835840 nodespecs-0.0.6/
--rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     6207 2024-04-23 13:38:25.832850 nodespecs-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4326 2024-04-23 13:35:19.000000 nodespecs-0.0.6/README.md
--rw-rw-rw-   0        0        0      899 2024-04-23 13:30:54.000000 nodespecs-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 13:38:25.835840 nodespecs-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 13:38:25.786956 nodespecs-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 13:38:25.830858 nodespecs-0.0.6/src/nodespecs.egg-info/
--rw-rw-rw-   0        0        0     6207 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 13:38:25.824559 nodespecs-0.0.6/src/specs/
--rw-rw-rw-   0        0        0      125 2024-04-23 13:35:20.000000 nodespecs-0.0.6/src/specs/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-18 19:09:52.000000 nodespecs-0.0.6/src/specs/__main__.py
--rw-rw-rw-   0        0        0     1479 2024-04-23 13:35:21.000000 nodespecs-0.0.6/src/specs/benchmark.py
--rw-rw-rw-   0        0        0      172 2024-04-18 19:56:34.000000 nodespecs-0.0.6/src/specs/cmd.py
--rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.6/src/specs/cpuinfo.py
--rw-rw-rw-   0        0        0     7189 2024-04-19 22:18:04.000000 nodespecs-0.0.6/src/specs/hardware.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:55:28.903619 nodespecs-0.0.7/
+-rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     7013 2024-04-29 18:55:28.901621 nodespecs-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5132 2024-04-29 18:54:55.000000 nodespecs-0.0.7/README.md
+-rw-rw-rw-   0        0        0      899 2024-04-29 18:18:43.000000 nodespecs-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 18:55:28.903619 nodespecs-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 18:55:28.860757 nodespecs-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 18:55:28.899628 nodespecs-0.0.7/src/nodespecs.egg-info/
+-rw-rw-rw-   0        0        0     7013 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 18:55:28.896638 nodespecs-0.0.7/src/specs/
+-rw-rw-rw-   0        0        0      158 2024-04-29 18:13:46.000000 nodespecs-0.0.7/src/specs/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-18 19:09:52.000000 nodespecs-0.0.7/src/specs/__main__.py
+-rw-rw-rw-   0        0        0     1479 2024-04-23 13:35:21.000000 nodespecs-0.0.7/src/specs/benchmark.py
+-rw-rw-rw-   0        0        0      488 2024-04-23 20:58:02.000000 nodespecs-0.0.7/src/specs/cmd.py
+-rw-rw-rw-   0        0        0     2783 2024-04-29 18:53:57.000000 nodespecs-0.0.7/src/specs/comm.py
+-rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.7/src/specs/cpuinfo.py
+-rw-rw-rw-   0        0        0     7189 2024-04-25 04:50:36.000000 nodespecs-0.0.7/src/specs/hardware.py
```

### Comparing `nodespecs-0.0.6/LICENSE` & `nodespecs-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.6/PKG-INFO` & `nodespecs-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.6
+Version: 0.0.7
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -32,30 +32,48 @@
 
 
 ### install and use with pip
 
 ```shell
 pip install nodespecs
 python -m specs
+python -c "import specs; specs.bench_cpu()"
+python -c "import specs; specs.info_gpu()"
+```
+
+```shell
+## server
+python -c "import specs; specs.server()"
+
+## client upload wt progress bar
+python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
+
+## client upload wo progress bar
+python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
 ```
 
 ```
+sudo apt update
 sudo apt install python3-pip
 python3 -m pip install nodespecs && python3 -m specs
 ```
 
+
+
 ```python
 import specs
 
 specs.info_gpu()
 specs.bench_cpu()
 ```
 
 
 
+
+
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
 
@@ -76,19 +94,21 @@
 
 | Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
 | ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
 | TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
 | TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
 | Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
 | TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux      | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
 | WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
 | TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
 | JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux      | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
 | TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows    | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
 | google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux      | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux      | 49.396       |                                                              |       |
 | JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows    | 62.969       |                                                              |       |
 | Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux      | 98.732       | EPYC-7551                                                    | 14.67 |
 
 
 
 ### GPU collection
```

### Comparing `nodespecs-0.0.6/README.md` & `nodespecs-0.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,30 +4,48 @@
 
 
 ### install and use with pip
 
 ```shell
 pip install nodespecs
 python -m specs
+python -c "import specs; specs.bench_cpu()"
+python -c "import specs; specs.info_gpu()"
+```
+
+```shell
+## server
+python -c "import specs; specs.server()"
+
+## client upload wt progress bar
+python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
+
+## client upload wo progress bar
+python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
 ```
 
 ```
+sudo apt update
 sudo apt install python3-pip
 python3 -m pip install nodespecs && python3 -m specs
 ```
 
+
+
 ```python
 import specs
 
 specs.info_gpu()
 specs.bench_cpu()
 ```
 
 
 
+
+
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
 
@@ -48,19 +66,21 @@
 
 | Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
 | ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
 | TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
 | TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
 | Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
 | TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux      | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
 | WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
 | TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
 | JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux      | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
 | TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows    | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
 | google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux      | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux      | 49.396       |                                                              |       |
 | JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows    | 62.969       |                                                              |       |
 | Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux      | 98.732       | EPYC-7551                                                    | 14.67 |
 
 
 
 ### GPU collection
```

### Comparing `nodespecs-0.0.6/pyproject.toml` & `nodespecs-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodespecs"
-version = "0.0.6"
+version = "0.0.7"
 description = "The specs summarize utilities for computer instance"
 readme = "README.md"
 authors = [{ name = "jinsanity", email = "jinsanityff@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodespecs-0.0.6/src/nodespecs.egg-info/PKG-INFO` & `nodespecs-0.0.7/src/nodespecs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.6
+Version: 0.0.7
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -32,30 +32,48 @@
 
 
 ### install and use with pip
 
 ```shell
 pip install nodespecs
 python -m specs
+python -c "import specs; specs.bench_cpu()"
+python -c "import specs; specs.info_gpu()"
+```
+
+```shell
+## server
+python -c "import specs; specs.server()"
+
+## client upload wt progress bar
+python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
+
+## client upload wo progress bar
+python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
 ```
 
 ```
+sudo apt update
 sudo apt install python3-pip
 python3 -m pip install nodespecs && python3 -m specs
 ```
 
+
+
 ```python
 import specs
 
 specs.info_gpu()
 specs.bench_cpu()
 ```
 
 
 
+
+
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
 
@@ -76,19 +94,21 @@
 
 | Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
 | ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
 | TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
 | TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
 | Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
 | TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux      | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
 | WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
 | TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
 | JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux      | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
 | TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows    | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
 | google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux      | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux      | 49.396       |                                                              |       |
 | JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows    | 62.969       |                                                              |       |
 | Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux      | 98.732       | EPYC-7551                                                    | 14.67 |
 
 
 
 ### GPU collection
```

### Comparing `nodespecs-0.0.6/src/specs/benchmark.py` & `nodespecs-0.0.7/src/specs/benchmark.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.6/src/specs/cpuinfo.py` & `nodespecs-0.0.7/src/specs/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.6/src/specs/hardware.py` & `nodespecs-0.0.7/src/specs/hardware.py`

 * *Files identical despite different names*

