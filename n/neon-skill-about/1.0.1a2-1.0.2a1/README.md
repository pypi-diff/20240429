# Comparing `tmp/neon-skill-about-1.0.1a2.tar.gz` & `tmp/neon-skill-about-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-about-1.0.1a2.tar", last modified: Fri Mar  1 23:37:55 2024, max compression
+gzip compressed data, was "neon-skill-about-1.0.2a1.tar", last modified: Mon Apr 29 18:29:04 2024, max compression
```

## Comparing `neon-skill-about-1.0.1a2.tar` & `neon-skill-about-1.0.2a1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:55.005682 neon-skill-about-1.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-01 23:37:55.001682 neon-skill-about-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:54.997682 neon-skill-about-1.0.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:54.997682 neon-skill-about-1.0.1a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:55.001682 neon-skill-about-1.0.1a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/en-us/dialog/license_long.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/en-us/dialog/license_short.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/en-us/dialog/skills_list.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:55.001682 neon-skill-about-1.0.1a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/en-us/vocab/license.voc
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/en-us/vocab/long.voc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/en-us/vocab/skills.voc
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/en-us/vocab/tell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:54.997682 neon-skill-about-1.0.1a2/locale/uk-ua/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:55.001682 neon-skill-about-1.0.1a2/locale/uk-ua/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/uk-ua/dialog/license_long.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/uk-ua/dialog/license_short.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/uk-ua/dialog/skills_list.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:55.001682 neon-skill-about-1.0.1a2/locale/uk-ua/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/uk-ua/vocab/license.voc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/uk-ua/vocab/long.voc
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/uk-ua/vocab/skills.voc
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/locale/uk-ua/vocab/tell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:55.001682 neon-skill-about-1.0.1a2/neon_skill_about.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-01 23:37:54.000000 neon-skill-about-1.0.1a2/neon_skill_about.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-01 23:37:54.000000 neon-skill-about-1.0.1a2/neon_skill_about.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 23:37:54.000000 neon-skill-about-1.0.1a2/neon_skill_about.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-01 23:37:54.000000 neon-skill-about-1.0.1a2/neon_skill_about.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-01 23:37:54.000000 neon-skill-about-1.0.1a2/neon_skill_about.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-01 23:37:54.000000 neon-skill-about-1.0.1a2/neon_skill_about.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 23:37:55.005682 neon-skill-about-1.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:37:55.001682 neon-skill-about-1.0.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-01 23:37:47.000000 neon-skill-about-1.0.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.232305 neon-skill-about-1.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-29 18:29:04.232305 neon-skill-about-1.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.228305 neon-skill-about-1.0.2a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.224305 neon-skill-about-1.0.2a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.228305 neon-skill-about-1.0.2a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/en-us/dialog/license_long.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/en-us/dialog/license_short.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/en-us/dialog/skills_list.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.228305 neon-skill-about-1.0.2a1/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/en-us/vocab/license.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/en-us/vocab/long.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/en-us/vocab/skills.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/en-us/vocab/tell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.228305 neon-skill-about-1.0.2a1/locale/uk-ua/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.228305 neon-skill-about-1.0.2a1/locale/uk-ua/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/uk-ua/dialog/license_long.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/uk-ua/dialog/license_short.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/uk-ua/dialog/skills_list.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.228305 neon-skill-about-1.0.2a1/locale/uk-ua/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/uk-ua/vocab/license.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/uk-ua/vocab/long.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/uk-ua/vocab/skills.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/locale/uk-ua/vocab/tell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.232305 neon-skill-about-1.0.2a1/neon_skill_about.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-29 18:29:04.000000 neon-skill-about-1.0.2a1/neon_skill_about.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-29 18:29:04.000000 neon-skill-about-1.0.2a1/neon_skill_about.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:29:04.000000 neon-skill-about-1.0.2a1/neon_skill_about.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 18:29:04.000000 neon-skill-about-1.0.2a1/neon_skill_about.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 18:29:04.000000 neon-skill-about-1.0.2a1/neon_skill_about.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 18:29:04.000000 neon-skill-about-1.0.2a1/neon_skill_about.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:29:04.232305 neon-skill-about-1.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:29:04.232305 neon-skill-about-1.0.2a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-29 18:29:00.000000 neon-skill-about-1.0.2a1/version.py
```

### Comparing `neon-skill-about-1.0.1a2/LICENSE.md` & `neon-skill-about-1.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-about-1.0.1a2/PKG-INFO` & `neon-skill-about-1.0.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-about
-Version: 1.0.1a2
+Version: 1.0.2a1
 Summary: Neon About Skill
 Home-page: https://github.com/NeonGeckoCom/skill-about
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `neon-skill-about-1.0.1a2/README.md` & `neon-skill-about-1.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-about-1.0.1a2/__init__.py` & `neon-skill-about-1.0.2a1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import json
 
 from typing import List
 from random import shuffle
 from os.path import isdir
-from ovos_utils.skills.locations import get_skill_directories, get_plugin_skills
+from ovos_plugin_manager.skills import get_skill_directories, get_plugin_skills
 from ovos_utils import classproperty
 from ovos_utils.process_utils import RuntimeRequirements
 from neon_utils.skills.neon_skill import NeonSkill
 from neon_utils.log_utils import LOG
 from adapt.intent import IntentBuilder
 from os import listdir, path
```

### Comparing `neon-skill-about-1.0.1a2/locale/uk-ua/dialog/license_long.dialog` & `neon-skill-about-1.0.2a1/locale/uk-ua/dialog/license_long.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-about-1.0.1a2/neon_skill_about.egg-info/PKG-INFO` & `neon-skill-about-1.0.2a1/neon_skill_about.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-about
-Version: 1.0.1a2
+Version: 1.0.2a1
 Summary: Neon About Skill
 Home-page: https://github.com/NeonGeckoCom/skill-about
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `neon-skill-about-1.0.1a2/neon_skill_about.egg-info/SOURCES.txt` & `neon-skill-about-1.0.2a1/neon_skill_about.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-about-1.0.1a2/setup.py` & `neon-skill-about-1.0.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-about-1.0.1a2/skill.json` & `neon-skill-about-1.0.2a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-about-1.0.1a2/test/test_skill.py` & `neon-skill-about-1.0.2a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-about-1.0.1a2/version.py` & `neon-skill-about-1.0.2a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a2"
+__version__ = "1.0.2a1"
```

