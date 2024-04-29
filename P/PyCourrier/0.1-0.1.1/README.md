# Comparing `tmp/pycourrier-0.1.tar.gz` & `tmp/pycourrier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycourrier-0.1.tar", last modified: Mon Apr 29 17:11:53 2024, max compression
+gzip compressed data, was "pycourrier-0.1.1.tar", last modified: Mon Apr 29 17:18:37 2024, max compression
```

## Comparing `pycourrier-0.1.tar` & `pycourrier-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:11:53.863600 pycourrier-0.1/
--rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 pycourrier-0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-29 17:11:53.803332 pycourrier-0.1/MailSender/
--rw-rw-rw-   0        0        0     4086 2024-04-29 16:54:54.000000 pycourrier-0.1/MailSender/MailSender.py
--rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 pycourrier-0.1/MailSender/__init__.py
--rw-rw-rw-   0        0        0      392 2024-04-29 17:11:53.853288 pycourrier-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2439 2024-04-29 17:09:37.000000 pycourrier-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 17:11:53.848938 pycourrier-0.1/pycourrier.egg-info/
--rw-rw-rw-   0        0        0      392 2024-04-29 17:11:53.000000 pycourrier-0.1/pycourrier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-29 17:11:53.000000 pycourrier-0.1/pycourrier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:11:53.000000 pycourrier-0.1/pycourrier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-29 17:11:53.000000 pycourrier-0.1/pycourrier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 17:11:53.864597 pycourrier-0.1/setup.cfg
--rw-rw-rw-   0        0        0      531 2024-04-29 17:11:30.000000 pycourrier-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:18:36.980414 pycourrier-0.1.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 pycourrier-0.1.1/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-29 17:18:36.889303 pycourrier-0.1.1/MailSender/
+-rw-rw-rw-   0        0        0     4086 2024-04-29 16:54:54.000000 pycourrier-0.1.1/MailSender/MailSender.py
+-rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 pycourrier-0.1.1/MailSender/__init__.py
+-rw-rw-rw-   0        0        0     2878 2024-04-29 17:18:36.970338 pycourrier-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2439 2024-04-29 17:09:37.000000 pycourrier-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 17:18:36.965287 pycourrier-0.1.1/pycourrier.egg-info/
+-rw-rw-rw-   0        0        0     2878 2024-04-29 17:18:36.000000 pycourrier-0.1.1/pycourrier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-29 17:18:36.000000 pycourrier-0.1.1/pycourrier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:18:36.000000 pycourrier-0.1.1/pycourrier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 17:18:36.000000 pycourrier-0.1.1/pycourrier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:18:36.981389 pycourrier-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      685 2024-04-29 17:18:04.000000 pycourrier-0.1.1/setup.py
```

### Comparing `pycourrier-0.1/LICENSE` & `pycourrier-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycourrier-0.1/MailSender/MailSender.py` & `pycourrier-0.1.1/MailSender/MailSender.py`

 * *Files identical despite different names*

### Comparing `pycourrier-0.1/README.md` & `pycourrier-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycourrier-0.1/setup.py` & `pycourrier-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r") as f:
+    description = f.read()
+
 setup(
     name='pycourrier',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     description='A simple email sender utility',
     author='Abdelmajid Habouch',
     author_email='Habush1610@gmail.com',
     url='https://github.com/mjiid/pycourier',
     license='MIT',
     install_requires=[
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+    long_description=description,
+    long_description_content_type="text/markdown",
 )
```

