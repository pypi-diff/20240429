# Comparing `tmp/tom_fink-0.5.2.tar.gz` & `tmp/tom_fink-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_fink-0.5.2.tar", max compression
+gzip compressed data, was "tom_fink-0.6.0.tar", max compression
```

## Comparing `tom_fink-0.5.2.tar` & `tom_fink-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35149 2024-03-25 19:09:10.345004 tom_fink-0.5.2/LICENSE
--rw-r--r--   0        0        0     1803 2024-03-25 19:09:10.345004 tom_fink-0.5.2/README.md
--rw-r--r--   0        0        0     2164 2024-03-25 19:09:24.233179 tom_fink-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      805 2024-03-25 19:09:24.233179 tom_fink-0.5.2/tom_fink/__init__.py
--rw-r--r--   0        0        0    13513 2024-03-25 19:09:10.349004 tom_fink-0.5.2/tom_fink/fink.py
--rw-r--r--   0        0        0        0 2024-03-25 19:09:10.349004 tom_fink-0.5.2/tom_fink/tests/__init__.py
--rw-r--r--   0        0        0     1041 2024-03-25 19:09:10.349004 tom_fink-0.5.2/tom_fink/tests/boot_django.py
--rwxr-xr-x   0        0        0      149 2024-03-25 19:09:10.349004 tom_fink-0.5.2/tom_fink/tests/django_shell.py
--rwxr-xr-x   0        0        0      429 2024-03-25 19:09:10.349004 tom_fink-0.5.2/tom_fink/tests/run_canary_tests.py
--rwxr-xr-x   0        0        0      429 2024-03-25 19:09:10.349004 tom_fink-0.5.2/tom_fink/tests/run_tests.py
--rw-r--r--   0        0        0      541 2024-03-25 19:09:10.349004 tom_fink-0.5.2/tom_fink/tests/tests.py
--rw-r--r--   0        0        0      344 2024-03-25 19:09:10.349004 tom_fink-0.5.2/tom_fink/tests/tests_canary.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 tom_fink-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-29 11:33:21.897519 tom_fink-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7247 2024-04-29 11:33:21.897519 tom_fink-0.6.0/README.md
+-rw-r--r--   0        0        0     2213 2024-04-29 11:33:34.349630 tom_fink-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      805 2024-04-29 11:33:34.349630 tom_fink-0.6.0/tom_fink/__init__.py
+-rw-r--r--   0        0        0     5108 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/alertstream.py
+-rw-r--r--   0        0        0    13513 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/fink.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/tests/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/tests/boot_django.py
+-rwxr-xr-x   0        0        0      149 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/tests/django_shell.py
+-rwxr-xr-x   0        0        0      429 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/tests/run_canary_tests.py
+-rwxr-xr-x   0        0        0      429 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/tests/run_tests.py
+-rw-r--r--   0        0        0      541 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/tests/tests.py
+-rw-r--r--   0        0        0      344 2024-04-29 11:33:21.897519 tom_fink-0.6.0/tom_fink/tests/tests_canary.py
+-rw-r--r--   0        0        0     8715 1970-01-01 00:00:00.000000 tom_fink-0.6.0/PKG-INFO
```

### Comparing `tom_fink-0.5.2/LICENSE` & `tom_fink-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_fink-0.5.2/pyproject.toml` & `tom_fink-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tom-fink"
-version = "0.5.2"  # version supplied by poetry-dynamic-versioning
+version = "0.6.0"  # version supplied by poetry-dynamic-versioning
 description = "The Fink Alert Broker Module for the TOM Toolkit. Fink is a broker currently connected to ZTF. More information on Fink at https://fink-portal.org"
 authors = ["Julien Peloton <peloton@lal.in2p3.fr>"]
 maintainers = [
     "William Lindstrom <llindstrom@lco.global>",
     "Joey Chatelain <jchatelain@lco.global>",
     "Rachel Street <rstreet@lco.global>"
 ]
@@ -36,14 +36,16 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 tomtoolkit = "^2.17.2"
 elasticsearch-dsl = "^8.12.0"
 Markdown = "^3.5.2"
+fink-client = "^7.2"
+tom-alertstreams = "^0.6.2"
 
 [tool.poetry.group.test.dependencies]
 factory_boy = ">=3.1,<3.3"
 
 [tool.poetry.group.coverage.dependencies]
 coverage = "~6" # coveralls needs ~6 even though 7.3.2 is latest
 coveralls = "~3"
```

### Comparing `tom_fink-0.5.2/tom_fink/__init__.py` & `tom_fink-0.6.0/tom_fink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 # this is a placeholder for poetry-dynamic-versioning (see pyproject.toml)
-__version__ = "0.5.2"
+__version__ = "0.6.0"
```

### Comparing `tom_fink-0.5.2/tom_fink/fink.py` & `tom_fink-0.6.0/tom_fink/fink.py`

 * *Files identical despite different names*

### Comparing `tom_fink-0.5.2/tom_fink/tests/boot_django.py` & `tom_fink-0.6.0/tom_fink/tests/boot_django.py`

 * *Files identical despite different names*

### Comparing `tom_fink-0.5.2/tom_fink/tests/tests.py` & `tom_fink-0.6.0/tom_fink/tests/tests.py`

 * *Files identical despite different names*

