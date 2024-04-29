# Comparing `tmp/fileformats_medimage_mrtrix3-0.1.tar.gz` & `tmp/fileformats_medimage_mrtrix3-3.0.3a0.tar.gz`

## Comparing `fileformats_medimage_mrtrix3-0.1.tar` & `fileformats_medimage_mrtrix3-3.0.3a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/.codespell-ignorewords
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/.flake8
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/conftest.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/pytest.ini
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/_version.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/dwi.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/image.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/in_out.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/track.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/LICENSE
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/README.rst
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/pyproject.toml
--rw-r--r--   0        0        0    18623 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-0.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/.codespell-ignorewords
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/.flake8
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/conftest.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/pytest.ini
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/_version.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/dwi.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/image.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/in_out.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/track.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/.gitignore
+-rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/LICENSE
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/README.rst
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/PKG-INFO
```

### Comparing `fileformats_medimage_mrtrix3-0.1/conftest.py` & `fileformats_medimage_mrtrix3-3.0.3a0/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/dwi.py` & `fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/dwi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from fileformats.core import hook
 from fileformats.core.mixin import WithAdjacentFiles
 from fileformats.medimage import DwiEncoding, Nifti1, NiftiGz, NiftiX, NiftiGzX
 from .image import ImageFormat, ImageHeader, ImageFormatGz
 
+
 class BFile(DwiEncoding):
     """MRtrix-style diffusion encoding, all in one file"""
 
     ext = ".b"
 
 
 # NIfTI file format gzipped with BIDS side car
```

### Comparing `fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/image.py` & `fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,23 +83,25 @@
     ext = ".mif"
 
     @hook.check
     def check_data_file(self):
         if self.data_fspath != self.fspath:
             raise FormatMismatchError(
                 f"Data file ('{self.data_fspath}') is not set to the same file as header "
-                f"('{self.fspath}')")
+                f"('{self.fspath}')"
+            )
 
     @property
     def data_file(self):
         return self
 
 
 class ImageFormatGz(Gzip[ImageFormat]):
 
+    iana_mime = None
     ext = ".mif.gz"
 
 
 class ImageHeader(BaseMrtrixImage):
 
     ext = ".mih"
```

### Comparing `fileformats_medimage_mrtrix3-0.1/fileformats/medimage_mrtrix3/in_out.py` & `fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/in_out.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,21 @@
     Nifti2,
     Mgh,
     MghGz,
     Analyze,
 )
 from .image import ImageFormat, ImageHeader, ImageFormatGz
 from .dwi import (
-    NiftiB, NiftiGzB, NiftiGzXB, NiftiXB, ImageFormatB, ImageFormatGzB, ImageHeaderB
+    NiftiB,
+    NiftiGzB,
+    NiftiGzXB,
+    NiftiXB,
+    ImageFormatB,
+    ImageFormatGzB,
+    ImageHeaderB,
 )
 
 
 ImageIn = ty.Union[
     ImageFormat,
     ImageFormatGz,
     ImageHeader,
```

### Comparing `fileformats_medimage_mrtrix3-0.1/LICENSE` & `fileformats_medimage_mrtrix3-3.0.3a0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,8 @@
 To the extent possible, if any provision of this Public License is deemed unenforceable, it shall be automatically reformed to the minimum extent necessary to make it enforceable. If the provision cannot be reformed, it shall be severed from this Public License without affecting the enforceability of the remaining terms and conditions.
 No term or condition of this Public License will be waived and no failure to comply consented to unless expressly agreed to by the Licensor.
 Nothing in this Public License constitutes or may be interpreted as a limitation upon, or waiver of, any privileges and immunities that apply to the Licensor or You, including from the legal processes of any jurisdiction or authority.
 Creative Commons is not a party to its public licenses. Notwithstanding, Creative Commons may elect to apply one of its public licenses to material it publishes and in those instances will be considered the “Licensor.” The text of the Creative Commons public licenses is dedicated to the public domain under the CC0 Public Domain Dedication. Except for the limited purpose of indicating that material is shared under a Creative Commons public license or as otherwise permitted by the Creative Commons policies published at creativecommons.org/policies, Creative Commons does not authorize the use of the trademark “Creative Commons” or any other trademark or logo of Creative Commons without its prior written consent including, without limitation, in connection with any unauthorized modifications to any of its public licenses or any other arrangements, understandings, or agreements concerning use of licensed material. For the avoidance of doubt, this paragraph does not form part of the public licenses.
 
 Creative Commons may be contacted at creativecommons.org.
 
-Additional languages available: العربية, čeština, Deutsch, Ελληνικά, Español, euskara, suomeksi, français, hrvatski, Bahasa Indonesia, italiano, 日本語, 한국어, Lietuvių, latviski, te reo Māori, Nederlands, norsk, polski, português, română, русский, Slovenščina, svenska, Türkçe, українська, 中文, 華語. Please read the FAQ for more information about official translations.
+Additional languages available: العربية, čeština, Deutsch, Ελληνικά, Español, euskara, suomeksi, français, hrvatski, Bahasa Indonesia, italiano, 日本語, 한국어, Lietuvių, latviski, te reo Māori, Nederlands, norsk, polski, português, română, русский, Slovenščina, svenska, Türkçe, українська, 中文, 華語. Please read the FAQ for more information about official translations.
```

### Comparing `fileformats_medimage_mrtrix3-0.1/README.rst` & `fileformats_medimage_mrtrix3-3.0.3a0/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3-0.1/pyproject.toml` & `fileformats_medimage_mrtrix3-3.0.3a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 ]
 
 [project.urls]
 repository = "https://github.com/MRtrix3/mrtrix3"
 
 [tool.hatch.version]
 source = "vcs"
-raw-options = { root = "../../" }
+raw-options = { root = ".." }
 
 [tool.hatch.build.hooks.vcs]
 version-file = "fileformats/medimage_mrtrix3/_version.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["fileformats"]
```

### Comparing `fileformats_medimage_mrtrix3-0.1/PKG-INFO` & `fileformats_medimage_mrtrix3-3.0.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fileformats-medimage-mrtrix3
-Version: 0.1
+Version: 3.0.3a0
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/MRtrix3/mrtrix3
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

