# Comparing `tmp/libsoni-1.0.1.tar.gz` & `tmp/libsoni-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsoni-1.0.1.tar", last modified: Tue Mar 12 13:55:58 2024, max compression
+gzip compressed data, was "libsoni-1.0.2.tar", last modified: Mon Apr 29 14:17:33 2024, max compression
```

## Comparing `libsoni-1.0.1.tar` & `libsoni-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 13:55:58.717965 libsoni-1.0.1/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1505 2024-03-11 15:06:28.000000 libsoni-1.0.1/LICENCE
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6017 2024-03-12 13:55:58.713965 libsoni-1.0.1/PKG-INFO
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     5271 2024-03-12 13:55:20.000000 libsoni-1.0.1/README.md
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 13:55:58.713965 libsoni-1.0.1/libsoni/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 09:12:36.000000 libsoni-1.0.1/libsoni/__init__.py
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 13:55:58.713965 libsoni-1.0.1/libsoni/core/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 09:12:50.000000 libsoni-1.0.1/libsoni/core/__init__.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7501 2024-03-11 12:43:50.000000 libsoni-1.0.1/libsoni/core/chroma.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     5073 2024-03-12 10:06:30.000000 libsoni-1.0.1/libsoni/core/f0.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    15970 2024-03-12 13:55:20.000000 libsoni-1.0.1/libsoni/core/methods.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    14264 2024-03-12 13:55:20.000000 libsoni-1.0.1/libsoni/core/pianoroll.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6839 2024-03-11 12:43:50.000000 libsoni-1.0.1/libsoni/core/spectrogram.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    13948 2024-03-11 12:43:50.000000 libsoni-1.0.1/libsoni/core/tse.py
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 13:55:58.713965 libsoni-1.0.1/libsoni/util/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 09:13:05.000000 libsoni-1.0.1/libsoni/util/__init__.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    12285 2024-03-11 12:43:50.000000 libsoni-1.0.1/libsoni/util/utils.py
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 13:55:58.713965 libsoni-1.0.1/libsoni.egg-info/
--rw-r--r--   0 yiitozer  (1001) yiitozer  (1001)     6017 2024-03-12 13:55:58.000000 libsoni-1.0.1/libsoni.egg-info/PKG-INFO
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)      475 2024-03-12 13:55:58.000000 libsoni-1.0.1/libsoni.egg-info/SOURCES.txt
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        1 2024-03-12 13:55:58.000000 libsoni-1.0.1/libsoni.egg-info/dependency_links.txt
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)      247 2024-03-12 13:55:58.000000 libsoni-1.0.1/libsoni.egg-info/requires.txt
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        8 2024-03-12 13:55:58.000000 libsoni-1.0.1/libsoni.egg-info/top_level.txt
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)       38 2024-03-12 13:55:58.717965 libsoni-1.0.1/setup.cfg
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1532 2024-03-12 13:55:37.000000 libsoni-1.0.1/setup.py
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-03-12 13:55:58.713965 libsoni-1.0.1/tests/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1234 2024-03-12 10:19:31.000000 libsoni-1.0.1/tests/test_f0.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     2218 2024-03-12 13:55:20.000000 libsoni-1.0.1/tests/test_methods.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     2084 2024-03-12 13:55:20.000000 libsoni-1.0.1/tests/test_pianoroll.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-29 14:17:33.933996 libsoni-1.0.2/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1505 2024-04-29 14:13:45.000000 libsoni-1.0.2/LICENSE
+-rw-r--r--   0 yiitozer  (1001) yiitozer  (1001)     6613 2024-04-29 14:17:33.933996 libsoni-1.0.2/PKG-INFO
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     5420 2024-04-29 14:13:45.000000 libsoni-1.0.2/README.md
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-29 14:17:33.929996 libsoni-1.0.2/libsoni/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-24 08:35:14.000000 libsoni-1.0.2/libsoni/__init__.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-29 14:17:33.929996 libsoni-1.0.2/libsoni/core/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-24 08:35:14.000000 libsoni-1.0.2/libsoni/core/__init__.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7971 2024-04-29 14:13:45.000000 libsoni-1.0.2/libsoni/core/chroma.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     5519 2024-04-29 14:13:45.000000 libsoni-1.0.2/libsoni/core/f0.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    16588 2024-04-29 14:13:45.000000 libsoni-1.0.2/libsoni/core/methods.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    14806 2024-04-29 14:13:45.000000 libsoni-1.0.2/libsoni/core/pianoroll.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7185 2024-04-29 14:13:45.000000 libsoni-1.0.2/libsoni/core/spectrogram.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    14349 2024-04-29 14:13:45.000000 libsoni-1.0.2/libsoni/core/tse.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-29 14:17:33.929996 libsoni-1.0.2/libsoni/util/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-24 08:35:14.000000 libsoni-1.0.2/libsoni/util/__init__.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    13234 2024-04-29 14:13:45.000000 libsoni-1.0.2/libsoni/util/utils.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-29 14:17:33.929996 libsoni-1.0.2/libsoni.egg-info/
+-rw-r--r--   0 yiitozer  (1001) yiitozer  (1001)     6613 2024-04-29 14:17:33.000000 libsoni-1.0.2/libsoni.egg-info/PKG-INFO
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)      501 2024-04-29 14:17:33.000000 libsoni-1.0.2/libsoni.egg-info/SOURCES.txt
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        1 2024-04-29 14:17:33.000000 libsoni-1.0.2/libsoni.egg-info/dependency_links.txt
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)      247 2024-04-29 14:17:33.000000 libsoni-1.0.2/libsoni.egg-info/requires.txt
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        8 2024-04-29 14:17:33.000000 libsoni-1.0.2/libsoni.egg-info/top_level.txt
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)       38 2024-04-29 14:17:33.933996 libsoni-1.0.2/setup.cfg
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1532 2024-04-29 14:13:56.000000 libsoni-1.0.2/setup.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2024-04-29 14:17:33.933996 libsoni-1.0.2/tests/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     2862 2024-04-29 14:13:45.000000 libsoni-1.0.2/tests/test_f0.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     3473 2024-04-29 14:13:45.000000 libsoni-1.0.2/tests/test_methods.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     3836 2024-04-29 14:13:45.000000 libsoni-1.0.2/tests/test_pianoroll.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1300 2024-04-29 14:13:45.000000 libsoni-1.0.2/tests/test_spectrogram.py
```

### Comparing `libsoni-1.0.1/LICENCE` & `libsoni-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libsoni-1.0.1/PKG-INFO` & `libsoni-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,29 @@
-Metadata-Version: 2.1
-Name: libsoni
-Version: 1.0.1
-Summary: A Python Toolbox for Sonifying Music Annotations and Feature Representations
-Home-page: https://github.com/groupmm/libsoni
-Download-URL: https://github.com/groupmm/libsoni
-Author: Yigitcan Özer, Leo Brütting, Simon Schwär, Meinard Müller
-Author-email: yigitcan.oezer@audiolabs-erlangen.de
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7, <4.0
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENCE
-
 [![Python package using Conda](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml/badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml)
 [![Python package using pip](https://github.com/groupmm/libsoni/actions/workflows/test_pip.yml/badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/test_pip.yml)
 
 
 <table border="0">
   <tr>
-    <td><img src=https://github.com/groupmm/libsoni/blob/unit_tests/docs/build/html/_static/libsoni_logo.png alt="libsoni logo" width="1000"></td>
+    <td><img src=https://github.com/groupmm/libsoni/blob/main/docs/build/html/_static/libsoni_logo.png alt="libsoni logo" width="1000"></td>
     <td><h2>libsoni: A Python Toolbox for Sonifying Music Annotations and Feature Representations</h2>
 <br> <br>
 </td>
   </tr>
 </table>
 
-``libsoni`` an open-source Python toolbox tailored for the sonification of music annotations and feature representations. 
+``libsoni`` is an open-source Python toolbox tailored for the sonification of music annotations and feature representations. 
 By employing explicit and easy-to-understand sound synthesis techniques, the toolbox offers functionalities
 for generating and triggering sound events, enabling the sonification of spectral, harmonic, tonal, melodic,
 and rhythmic aspects. Unlike existing software libraries focused on creative applications of sound generation, 
 the toolbox is designed to meet the specific needs of MIR researchers and educators. It aims to simplify the process
 of music exploration, promoting a more intuitive and efficient approach to data analysis by enabling users to interact 
-with their data in acoustically meaningful ways.
+with their data in acoustically meaningful ways. 
+
+See the [API documentation](https://groupmm.github.io/libsoni/build/html/index.html) for a detailed view of the provided functions in ``libsoni``.
 
 ## Installation Guide
 We outline two primary methods for setting up ``libsoni`` using pip and setting up a dedicated environment.
 
 ### Method I: Installing with pip
 Utilize Python's package manager, pip, for a straightforward installation of ``libsoni``:
 
@@ -87,21 +69,21 @@
 ## Contributing
 
 We are happy for suggestions and contributions.  We would be grateful for either
 directly contacting us via email (meinard.mueller@audiolabs-erlangen.de) or for creating 
 an issue in our GitHub repository. Please do not submit a pull request without prior consultation
 with us.
 
-## Licence
-The code for this toolbox is published under an [MIT licence](LICENCE).
+## License
+The code for this toolbox is published under an [MIT license](LICENSE).
 This does not apply to the data files:
 * Schubert songs are taken from the [Schubert Winterreise Dataset](https://zenodo.org/record/4122060). 
 * Recording of the cantata *Ach Gott und Herr* by Bach is taken fom [Bach10 Dataset](https://labsites.rochester.edu/air/datasets/Bach10%20Dataset_v1.0.pdf).
 * Recording of *Locus Iste* by Anton Bruckner is taken from the [Dagstuhl Choir Set](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiJ1JnT9uuEAxXclP0HHUOXC4EQFnoECBMQAQ&url=https%3A%2F%2Fwww.audiolabs-erlangen.de%2Fresources%2FMIR%2F2020-DagstuhlChoirSet&usg=AOvVaw1sPox9R_Sh1eh5hqV2kgNs&opi=89978449).
-* Custom piano audio sample is taken from the [Single Note Database (SNDB)](https://github.com/audiolabs/SNDB)
+* Custom piano audio samples are taken from the [Single Note Database (SNDB)](https://github.com/audiolabs/SNDB).
 * Other audio files are taken from the [FMP notebooks](https://www.audiolabs-erlangen.de/resources/MIR/FMP/C0/C0.html).
 
 ## Acknowledgements
 
 The libsoni package originated from collaboration with various individuals over the past
 years. We extend our gratitude to former and current students, collaborators, 
 and colleagues, including Jonathan Driedger, Angel Villar-Corrales, and Tim Zunner,
```

#### html2text {}

```diff
@@ -1,36 +1,28 @@
-Metadata-Version: 2.1 Name: libsoni Version: 1.0.1 Summary: A Python Toolbox
-for Sonifying Music Annotations and Feature Representations Home-page: https://
-github.com/groupmm/libsoni Download-URL: https://github.com/groupmm/libsoni
-Author: Yigitcan Ãzer, Leo BrÃ¼tting, Simon SchwÃ¤r, Meinard MÃ¼ller Author-
-email: yigitcan.oezer@audiolabs-erlangen.de License: MIT Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Developers Classifier: Topic :: Multimedia ::
-Sound/Audio :: Analysis Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7, <4.0 Description-Content-Type: text/markdown Provides-
-Extra: tests Provides-Extra: docs License-File: LICENCE [![Python package using
-Conda](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml/
-badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/
-test_conda.yml) [![Python package using pip](https://github.com/groupmm/
-libsoni/actions/workflows/test_pip.yml/badge.svg)](https://github.com/groupmm/
-libsoni/actions/workflows/test_pip.yml)
+[![Python package using Conda](https://github.com/groupmm/libsoni/actions/
+workflows/test_conda.yml/badge.svg)](https://github.com/groupmm/libsoni/
+actions/workflows/test_conda.yml) [![Python package using pip](https://
+github.com/groupmm/libsoni/actions/workflows/test_pip.yml/badge.svg)](https://
+github.com/groupmm/libsoni/actions/workflows/test_pip.yml)
                ********** lliibbssoonnii:: AA PPyytthhoonn TToooollbbooxx ffoorr SSoonniiffyyiinngg MMuussiicc AAnnnnoottaattiioonnss
 [libsoni logo] aanndd FFeeaattuurree RReepprreesseennttaattiioonnss **********
 
 
-``libsoni`` an open-source Python toolbox tailored for the sonification of
+``libsoni`` is an open-source Python toolbox tailored for the sonification of
 music annotations and feature representations. By employing explicit and easy-
 to-understand sound synthesis techniques, the toolbox offers functionalities
 for generating and triggering sound events, enabling the sonification of
 spectral, harmonic, tonal, melodic, and rhythmic aspects. Unlike existing
 software libraries focused on creative applications of sound generation, the
 toolbox is designed to meet the specific needs of MIR researchers and
 educators. It aims to simplify the process of music exploration, promoting a
 more intuitive and efficient approach to data analysis by enabling users to
-interact with their data in acoustically meaningful ways. ## Installation Guide
+interact with their data in acoustically meaningful ways. See the [API
+documentation](https://groupmm.github.io/libsoni/build/html/index.html) for a
+detailed view of the provided functions in ``libsoni``. ## Installation Guide
 We outline two primary methods for setting up ``libsoni`` using pip and setting
 up a dedicated environment. ### Method I: Installing with pip Utilize Python's
 package manager, pip, for a straightforward installation of ``libsoni``: ```
 pip install libsoni ``` Note: We advise performing this installation within a
 Python environment (such as conda or a virtual environment) to prevent any
 conflicts with other packages. Ensure your environment runs Python 3.7 or
 higher. ### Method II: Setting Up a Conda Environment Alternatively, you can
@@ -48,26 +40,26 @@
 install Jupyter to run the notebooks: ``` pip install jupyter ``` 4. **Launch
 Jupyter Notebook:** Start the Jupyter notebook server by executing: ``` jupyter
 notebook ``` This will open a browser window from where you can navigate to and
 open the example notebooks. ## Contributing We are happy for suggestions and
 contributions. We would be grateful for either directly contacting us via email
 (meinard.mueller@audiolabs-erlangen.de) or for creating an issue in our GitHub
 repository. Please do not submit a pull request without prior consultation with
-us. ## Licence The code for this toolbox is published under an [MIT licence]
-(LICENCE). This does not apply to the data files: * Schubert songs are taken
+us. ## License The code for this toolbox is published under an [MIT license]
+(LICENSE). This does not apply to the data files: * Schubert songs are taken
 from the [Schubert Winterreise Dataset](https://zenodo.org/record/4122060). *
 Recording of the cantata *Ach Gott und Herr* by Bach is taken fom [Bach10
 Dataset](https://labsites.rochester.edu/air/datasets/
 Bach10%20Dataset_v1.0.pdf). * Recording of *Locus Iste* by Anton Bruckner is
 taken from the [Dagstuhl Choir Set](https://www.google.com/
 url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiJ1JnT9uuEAxXclP0HHUOXC4EQFnoECBMQAQ&url=https%3A%2F%2Fwww.audiolabs-
 erlangen.de%2Fresources%2FMIR%2F2020-
 DagstuhlChoirSet&usg=AOvVaw1sPox9R_Sh1eh5hqV2kgNs&opi=89978449). * Custom piano
-audio sample is taken from the [Single Note Database (SNDB)](https://
-github.com/audiolabs/SNDB) * Other audio files are taken from the [FMP
+audio samples are taken from the [Single Note Database (SNDB)](https://
+github.com/audiolabs/SNDB). * Other audio files are taken from the [FMP
 notebooks](https://www.audiolabs-erlangen.de/resources/MIR/FMP/C0/C0.html). ##
 Acknowledgements The libsoni package originated from collaboration with various
 individuals over the past years. We extend our gratitude to former and current
 students, collaborators, and colleagues, including Jonathan Driedger, Angel
 Villar-Corrales, and Tim Zunner, for their support and influence in creating
 this Python package. This work was funded by the Deutsche
 Forschungsgemeinschaft (DFG, German Research Foundation) under Grant No.
```

### Comparing `libsoni-1.0.1/README.md` & `libsoni-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,60 @@
+Metadata-Version: 2.1
+Name: libsoni
+Version: 1.0.2
+Summary: A Python Toolbox for Sonifying Music Annotations and Feature Representations
+Home-page: https://github.com/groupmm/libsoni
+Download-URL: https://github.com/groupmm/libsoni
+Author: Yigitcan Özer, Leo Brütting, Simon Schwär, Meinard Müller
+Author-email: yigitcan.oezer@audiolabs-erlangen.de
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7, <4.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython<8.0.0,>=7.8.0
+Requires-Dist: librosa<1.0.0,>=0.8.0
+Requires-Dist: matplotlib<4.0.0,>=3.1.0
+Requires-Dist: numpy<2.0.0,>=1.17.0
+Requires-Dist: pandas<2.0.0,>=1.0.0
+Requires-Dist: pysoundfile<1.0.0,>=0.9.0
+Requires-Dist: scipy<2.0.0,>=1.7.0
+Requires-Dist: libfmp<2.0.0,>=1.2.0
+Provides-Extra: tests
+Requires-Dist: pytest==6.2.*; extra == "tests"
+Provides-Extra: docs
+Requires-Dist: sphinx==6.2.*; extra == "docs"
+Requires-Dist: sphinx_rtd_theme==1.2.*; extra == "docs"
+
 [![Python package using Conda](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml/badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml)
 [![Python package using pip](https://github.com/groupmm/libsoni/actions/workflows/test_pip.yml/badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/test_pip.yml)
 
 
 <table border="0">
   <tr>
-    <td><img src=https://github.com/groupmm/libsoni/blob/unit_tests/docs/build/html/_static/libsoni_logo.png alt="libsoni logo" width="1000"></td>
+    <td><img src=https://github.com/groupmm/libsoni/blob/main/docs/build/html/_static/libsoni_logo.png alt="libsoni logo" width="1000"></td>
     <td><h2>libsoni: A Python Toolbox for Sonifying Music Annotations and Feature Representations</h2>
 <br> <br>
 </td>
   </tr>
 </table>
 
-``libsoni`` an open-source Python toolbox tailored for the sonification of music annotations and feature representations. 
+``libsoni`` is an open-source Python toolbox tailored for the sonification of music annotations and feature representations. 
 By employing explicit and easy-to-understand sound synthesis techniques, the toolbox offers functionalities
 for generating and triggering sound events, enabling the sonification of spectral, harmonic, tonal, melodic,
 and rhythmic aspects. Unlike existing software libraries focused on creative applications of sound generation, 
 the toolbox is designed to meet the specific needs of MIR researchers and educators. It aims to simplify the process
 of music exploration, promoting a more intuitive and efficient approach to data analysis by enabling users to interact 
-with their data in acoustically meaningful ways.
+with their data in acoustically meaningful ways. 
+
+See the [API documentation](https://groupmm.github.io/libsoni/build/html/index.html) for a detailed view of the provided functions in ``libsoni``.
 
 ## Installation Guide
 We outline two primary methods for setting up ``libsoni`` using pip and setting up a dedicated environment.
 
 ### Method I: Installing with pip
 Utilize Python's package manager, pip, for a straightforward installation of ``libsoni``:
 
@@ -67,21 +100,21 @@
 ## Contributing
 
 We are happy for suggestions and contributions.  We would be grateful for either
 directly contacting us via email (meinard.mueller@audiolabs-erlangen.de) or for creating 
 an issue in our GitHub repository. Please do not submit a pull request without prior consultation
 with us.
 
-## Licence
-The code for this toolbox is published under an [MIT licence](LICENCE).
+## License
+The code for this toolbox is published under an [MIT license](LICENSE).
 This does not apply to the data files:
 * Schubert songs are taken from the [Schubert Winterreise Dataset](https://zenodo.org/record/4122060). 
 * Recording of the cantata *Ach Gott und Herr* by Bach is taken fom [Bach10 Dataset](https://labsites.rochester.edu/air/datasets/Bach10%20Dataset_v1.0.pdf).
 * Recording of *Locus Iste* by Anton Bruckner is taken from the [Dagstuhl Choir Set](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiJ1JnT9uuEAxXclP0HHUOXC4EQFnoECBMQAQ&url=https%3A%2F%2Fwww.audiolabs-erlangen.de%2Fresources%2FMIR%2F2020-DagstuhlChoirSet&usg=AOvVaw1sPox9R_Sh1eh5hqV2kgNs&opi=89978449).
-* Custom piano audio sample is taken from the [Single Note Database (SNDB)](https://github.com/audiolabs/SNDB)
+* Custom piano audio samples are taken from the [Single Note Database (SNDB)](https://github.com/audiolabs/SNDB).
 * Other audio files are taken from the [FMP notebooks](https://www.audiolabs-erlangen.de/resources/MIR/FMP/C0/C0.html).
 
 ## Acknowledgements
 
 The libsoni package originated from collaboration with various individuals over the past
 years. We extend our gratitude to former and current students, collaborators, 
 and colleagues, including Jonathan Driedger, Angel Villar-Corrales, and Tim Zunner,
```

#### html2text {}

```diff
@@ -1,26 +1,44 @@
-[![Python package using Conda](https://github.com/groupmm/libsoni/actions/
-workflows/test_conda.yml/badge.svg)](https://github.com/groupmm/libsoni/
-actions/workflows/test_conda.yml) [![Python package using pip](https://
-github.com/groupmm/libsoni/actions/workflows/test_pip.yml/badge.svg)](https://
-github.com/groupmm/libsoni/actions/workflows/test_pip.yml)
+Metadata-Version: 2.1 Name: libsoni Version: 1.0.2 Summary: A Python Toolbox
+for Sonifying Music Annotations and Feature Representations Home-page: https://
+github.com/groupmm/libsoni Download-URL: https://github.com/groupmm/libsoni
+Author: Yigitcan Ãzer, Leo BrÃ¼tting, Simon SchwÃ¤r, Meinard MÃ¼ller Author-
+email: yigitcan.oezer@audiolabs-erlangen.de License: MIT Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers Classifier: Topic :: Multimedia ::
+Sound/Audio :: Analysis Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7, <4.0 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: ipython<8.0.0,>=7.8.0 Requires-Dist:
+librosa<1.0.0,>=0.8.0 Requires-Dist: matplotlib<4.0.0,>=3.1.0 Requires-Dist:
+numpy<2.0.0,>=1.17.0 Requires-Dist: pandas<2.0.0,>=1.0.0 Requires-Dist:
+pysoundfile<1.0.0,>=0.9.0 Requires-Dist: scipy<2.0.0,>=1.7.0 Requires-Dist:
+libfmp<2.0.0,>=1.2.0 Provides-Extra: tests Requires-Dist: pytest==6.2.*; extra
+== "tests" Provides-Extra: docs Requires-Dist: sphinx==6.2.*; extra == "docs"
+Requires-Dist: sphinx_rtd_theme==1.2.*; extra == "docs" [![Python package using
+Conda](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml/
+badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/
+test_conda.yml) [![Python package using pip](https://github.com/groupmm/
+libsoni/actions/workflows/test_pip.yml/badge.svg)](https://github.com/groupmm/
+libsoni/actions/workflows/test_pip.yml)
                ********** lliibbssoonnii:: AA PPyytthhoonn TToooollbbooxx ffoorr SSoonniiffyyiinngg MMuussiicc AAnnnnoottaattiioonnss
 [libsoni logo] aanndd FFeeaattuurree RReepprreesseennttaattiioonnss **********
 
 
-``libsoni`` an open-source Python toolbox tailored for the sonification of
+``libsoni`` is an open-source Python toolbox tailored for the sonification of
 music annotations and feature representations. By employing explicit and easy-
 to-understand sound synthesis techniques, the toolbox offers functionalities
 for generating and triggering sound events, enabling the sonification of
 spectral, harmonic, tonal, melodic, and rhythmic aspects. Unlike existing
 software libraries focused on creative applications of sound generation, the
 toolbox is designed to meet the specific needs of MIR researchers and
 educators. It aims to simplify the process of music exploration, promoting a
 more intuitive and efficient approach to data analysis by enabling users to
-interact with their data in acoustically meaningful ways. ## Installation Guide
+interact with their data in acoustically meaningful ways. See the [API
+documentation](https://groupmm.github.io/libsoni/build/html/index.html) for a
+detailed view of the provided functions in ``libsoni``. ## Installation Guide
 We outline two primary methods for setting up ``libsoni`` using pip and setting
 up a dedicated environment. ### Method I: Installing with pip Utilize Python's
 package manager, pip, for a straightforward installation of ``libsoni``: ```
 pip install libsoni ``` Note: We advise performing this installation within a
 Python environment (such as conda or a virtual environment) to prevent any
 conflicts with other packages. Ensure your environment runs Python 3.7 or
 higher. ### Method II: Setting Up a Conda Environment Alternatively, you can
@@ -38,26 +56,26 @@
 install Jupyter to run the notebooks: ``` pip install jupyter ``` 4. **Launch
 Jupyter Notebook:** Start the Jupyter notebook server by executing: ``` jupyter
 notebook ``` This will open a browser window from where you can navigate to and
 open the example notebooks. ## Contributing We are happy for suggestions and
 contributions. We would be grateful for either directly contacting us via email
 (meinard.mueller@audiolabs-erlangen.de) or for creating an issue in our GitHub
 repository. Please do not submit a pull request without prior consultation with
-us. ## Licence The code for this toolbox is published under an [MIT licence]
-(LICENCE). This does not apply to the data files: * Schubert songs are taken
+us. ## License The code for this toolbox is published under an [MIT license]
+(LICENSE). This does not apply to the data files: * Schubert songs are taken
 from the [Schubert Winterreise Dataset](https://zenodo.org/record/4122060). *
 Recording of the cantata *Ach Gott und Herr* by Bach is taken fom [Bach10
 Dataset](https://labsites.rochester.edu/air/datasets/
 Bach10%20Dataset_v1.0.pdf). * Recording of *Locus Iste* by Anton Bruckner is
 taken from the [Dagstuhl Choir Set](https://www.google.com/
 url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiJ1JnT9uuEAxXclP0HHUOXC4EQFnoECBMQAQ&url=https%3A%2F%2Fwww.audiolabs-
 erlangen.de%2Fresources%2FMIR%2F2020-
 DagstuhlChoirSet&usg=AOvVaw1sPox9R_Sh1eh5hqV2kgNs&opi=89978449). * Custom piano
-audio sample is taken from the [Single Note Database (SNDB)](https://
-github.com/audiolabs/SNDB) * Other audio files are taken from the [FMP
+audio samples are taken from the [Single Note Database (SNDB)](https://
+github.com/audiolabs/SNDB). * Other audio files are taken from the [FMP
 notebooks](https://www.audiolabs-erlangen.de/resources/MIR/FMP/C0/C0.html). ##
 Acknowledgements The libsoni package originated from collaboration with various
 individuals over the past years. We extend our gratitude to former and current
 students, collaborators, and colleagues, including Jonathan Driedger, Angel
 Villar-Corrales, and Tim Zunner, for their support and influence in creating
 this Python package. This work was funded by the Deutsche
 Forschungsgemeinschaft (DFG, German Research Foundation) under Grant No.
```

### Comparing `libsoni-1.0.1/libsoni/core/chroma.py` & `libsoni-1.0.2/libsoni/core/chroma.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     The sound can be changed either by the filter option or by the specified pitch-range.
     Both options can also be used in combination. Using the filter option shapes the spectrum
     like a bell curve centered around the center frequency, while the octave cutoff determines
     at which octave the amplitude of the corresponding sinusoid is 0.5.
 
     Parameters
     ----------
-    chroma_vector: np.ndarray
+    chroma_vector: np.ndarray (np.float32 / np.float64) [shape=(N, 12)]
         Chroma vector to sonify.
 
     pitch_range: Tuple[int, int], default = [20,108]
         Determines the pitches to encounter for shepard tones.
 
     filter: bool, default: False
         Enables filtering of shepard tones.
@@ -52,15 +52,15 @@
         Determines if output signal is normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    chroma_sonification: np.ndarray
+    chroma_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified chroma vector.
     """
 
     assert len(chroma_vector) == 12, f'The chroma vector must have length 12.'
 
     # Determine length of sonification
     num_samples = sonification_duration
@@ -104,15 +104,15 @@
     The sound can be changed either by the filter option or by the specified pitch-range.
     Both options can also be used in combination.
     Using the filter option shapes the spectrum like a bell curve centered around the center frequency,
     while the octave cutoff determines at which octave the amplitude of the corresponding sinusoid is 0.5.
 
     Parameters
     ----------
-    chromagram: np.ndarray
+    chromagram: np.ndarray (np.float32 / np.float64) [shape=(N, 12)]
         Chromagram to sonify.
 
     H: int, default = 0
         Hop size of STFT used to calculate chromagram.
 
     pitch_range: Tuple[int, int], default = [20,108]
         Determines the pitch range to encounter for shepard tones.
@@ -140,26 +140,25 @@
         Determines if output signal is normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    chroma_sonification: np.ndarray
+    chroma_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified chromagram.
     """
-
-    assert chromagram.shape[0] == 12, f'The chromagram must have shape 12xN.'
+    if chromagram.shape[0] != 12:
+        raise IndexError(f'The chromagram must have shape 12xN.')
 
     # Compute frame rate
     frame_rate = fs / H
 
     # Determine length of sonification
-    num_samples = sonification_duration if sonification_duration is not None else int(
-        chromagram.shape[1] * fs / frame_rate)
+    num_samples = int(chromagram.shape[1] * fs / frame_rate)
 
     # Initialize sonification
     chroma_sonification = np.zeros(num_samples)
 
     for pitch_class in range(12):
         if np.sum(np.abs(chromagram[pitch_class, :])) > 0:
             weighting_vector = np.repeat(chromagram[pitch_class, :], H)
@@ -175,8 +174,16 @@
                                                  fading_duration=fading_duration,
                                                  fs=fs)
             chroma_sonification += (shepard_tone * weighting_vector_smoothed)
 
     chroma_sonification = fade_signal(chroma_sonification, fading_duration=fading_duration, fs=fs)
     chroma_sonification = normalize_signal(chroma_sonification) if normalize else chroma_sonification
 
+    if sonification_duration is not None:
+        if len(chroma_sonification) > sonification_duration:
+            chroma_sonification = chroma_sonification[:sonification_duration]
+        else:
+            tmp = np.zeros(sonification_duration)
+            tmp[:len(chroma_sonification)] = np.copy(chroma_sonification)
+            chroma_sonification = tmp
+
     return chroma_sonification
```

### Comparing `libsoni-1.0.1/libsoni/core/f0.py` & `libsoni-1.0.2/libsoni/core/f0.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 
     The 2D array must contain time positions and the associated instantaneous frequencies.
     The sonification is based on the phase information by summation of the instantaneous frequencies.
     The parameters partials, partials_amplitudes and partials_phase_offsets can be used to shape the sound.
 
     Parameters
     ----------
-    time_f0: np.ndarray
+    time_f0: np.ndarray  (np.float32 / np.float64) [shape=(N, 2)]
         2D array of time positions and f0s.
 
-    gains: np.ndarray, default = None
+    gains: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing gain values for f0 values.
 
-    partials: np.ndarray, default = [1]
+    partials: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = [1]
         Array containing the desired partials of the fundamental frequencies for sonification.
         An array [1] leads to sonification with only the fundamental frequency,
         while an array [1,2] leads to sonification with the fundamental frequency and twice the fundamental frequency.
 
-    partials_amplitudes: np.ndarray, default = None
+    partials_amplitudes: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing the amplitudes for partials.
         An array [1,0.5] causes the first partial to have amplitude 1,
         while the second partial has amplitude 0.5.
         If None, the amplitudes for all partials are set to 1.
 
-    partials_phase_offsets: np.ndarray, default = None
+    partials_phase_offsets: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing the phase offsets for partials.
         When not defined, the phase offsets for all partials are set to 0.
 
     sonification_duration: int, default = None
         Determines duration of sonification, in samples.
 
     fading_duration: float, default = 0.05
@@ -52,17 +52,23 @@
         Determines if output signal is normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    f0_sonification: np.ndarray
+    f0_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified f0-trajectory.
     """
+    if time_f0.ndim != 2:
+        raise IndexError('time_f0 must be a numpy array of size [N, 2]')
+    if time_f0.shape[1] != 2:
+        raise IndexError('time_f0 must be a numpy array of size [N, 2]')
+
+
     if gains is not None:
         assert len(gains) == time_f0.shape[0], 'Array for confidence must have same length as time_f0.'
     else:
         gains = np.ones(time_f0.shape[0])
     time_positions = time_f0[:, 0]
     f0s = time_f0[:, 1]
     num_samples = int(time_positions[-1] * fs)
```

### Comparing `libsoni-1.0.1/libsoni/core/methods.py` & `libsoni-1.0.2/libsoni/core/methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Tuning frequency, in Hertz.
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    click : np.ndarray
+    click : np.ndarray (np.float32) [shape=(M, )]
         Generated click signal.
     """
 
     assert 0 <= pitch <= 127, f'Pitch is out of range [0,127].'
 
     click_frequency = pitch_to_frequency(pitch=pitch, tuning_frequency=tuning_frequency)
     angular_frequency = 2 * np.pi * click_frequency / fs
@@ -70,15 +70,15 @@
         Determines duration of fade-in and fade-out, in seconds.
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    sinusoid: np.ndarray
+    sinusoid: np.ndarray (np.float32) [shape=(M, )]
         Generated sinusoid.
     """
     sinusoid = amplitude * np.sin((2 * np.pi * frequency * (np.arange(int(duration * fs)) / fs)) + phase)
     sinusoid = fade_signal(signal=sinusoid, fs=fs, fading_duration=fading_duration)
 
     return sinusoid
 
@@ -130,15 +130,15 @@
         Determines duration of fade-in and fade-out, in seconds.
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    shepard_tone: np.ndarray
+    shepard_tone: np.ndarray (np.float32) [shape=(M, )]
         Generated shepard tone.
     """
 
     assert 0 <= pitch_class <= 11, f'Pitch class is out of range [0,11].'
     assert all(0 <= p <= 127 for p in pitch_range), f'Pitch range has to be defined within [0,127].'
 
     pitches = pitch_class + np.arange(11) * 12
@@ -180,26 +180,26 @@
     The sound can be customized using parameters partials, partials_amplitudes and partials_phase_offsets.
 
     Parameters
     ----------
     pitch: int, default = 69
         Pitch of the generated tone.
 
-    partials: np.ndarray, default = [1]
+    partials: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = [1]
         Array containing the desired partials of the fundamental frequencies for sonification.
         An array [1] leads to sonification with only the fundamental frequency,
         while an array [1,2] leads to sonification with the fundamental frequency and twice the fundamental frequency.
 
-    partials_amplitudes: np.ndarray, default = None
+    partials_amplitudes: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing the amplitudes for partials.
         An array [1,0.5] causes the first partial to have amplitude 1,
         while the second partial has amplitude 0.5.
         When not defined, the amplitudes for all partials are set to 1.
 
-    partials_phase_offsets: np.ndarray, default = None
+    partials_phase_offsets: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing the phase offsets for partials.
         When not defined, the phase offsets for all partials are set to 0.
 
     gain: float, default = 1.0
         Gain of generated tone.
 
     duration: float, default: 1.0
@@ -212,35 +212,34 @@
         Determines duration of fade-in and fade-out, given in seconds.
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    generated_tone: np.ndarray
+    generated_tone: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Generated tone signal.
     """
-
     assert 0 <= pitch <= 127, f'Pitch is out of range [0,127].'
 
     partials_amplitudes = np.ones(len(partials)) if partials_amplitudes is None else partials_amplitudes
     partials_phase_offsets = np.zeros(len(partials)) if partials_phase_offsets is None else partials_phase_offsets
 
     assert len(partials) == len(partials_amplitudes) == len(partials_phase_offsets), \
         f'Arrays partials, partials_amplitudes and partials_phase_offsets must be of equal length.'
 
     generated_tone = np.zeros(int(duration * fs))
     pitch_frequency = pitch_to_frequency(pitch=pitch, tuning_frequency=tuning_frequency)
 
     for partial, partial_amplitude, partials_phase_offset in zip(partials, partials_amplitudes, partials_phase_offsets):
         generated_tone += partial_amplitude * np.sin(2 * np.pi * pitch_frequency * partial * (np.arange(int(duration * fs)) / fs) + partials_phase_offset)
 
-    generated_tone = fade_signal(signal=generated_tone, fs=fs, fading_duration=fading_duration)
+    generated_tone = fade_signal(signal=generated_tone, fs=fs, fading_duration=fading_duration) * gain
 
-    return generated_tone * gain
+    return generated_tone
 
 
 def generate_tone_fm_synthesis(pitch: int = 69,
                                modulation_rate_relative: float = 0.0,
                                modulation_amplitude: float = 0.0,
                                gain: float = 1.0,
                                duration: float = 1.0,
@@ -275,15 +274,15 @@
         Determines duration of fade-in and fade-out, given in seconds.
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    generated_tone: np.ndarray
+    generated_tone: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Generated tone signal.
     """
 
     assert 0 <= pitch <= 127, f'Pitch is out of range [0,127].'
 
     pitch_frequency = pitch_to_frequency(pitch=pitch, tuning_frequency=tuning_frequency)
     generated_tone = np.sin(2 * np.pi * pitch_frequency * (np.arange(int(duration * fs))) / fs +
@@ -306,15 +305,15 @@
     The sound depends on the given wavetable.
 
     Parameters
     ----------
     pitch: int, default = 69
         Pitch of the synthesized tone.
 
-    wavetable: np.ndarray, default = None
+    wavetable: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Wavetable to be resampled.
 
     gain: float, default = 1.0
         Gain for generated signal
 
     duration: float, default: 1.0
         Determines duration of tone, given in seconds.
@@ -326,15 +325,15 @@
         Determines duration of fade-in and fade-out, in seconds.
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    generated_tone: np.ndarray
+    generated_tone: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Generated signal
     """
 
     assert 0 <= pitch <= 127, f'Pitch is out of range [0,127].'
 
     generated_tone = []
     pitch_frequency = pitch_to_frequency(pitch=pitch, tuning_frequency=tuning_frequency)
@@ -361,49 +360,49 @@
                                       fs: int = 22050) -> np.ndarray:
     """Generates signal out of instantaneous frequency.
 
     The sound can be customized using parameters partials, partials_amplitudes and partials_phase_offsets.
 
     Parameters
     ----------
-    frequency_vector: np.ndarray
+    frequency_vector: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Array containing sample-wise instantaneous frequencies.
 
-    gain_vector: np.ndarray, default = None
+    gain_vector: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing sample-wise gains.
 
-    partials: np.ndarray, default = [1]
+    partials: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = [1]
         An array containing the desired partials of the fundamental frequencies for sonification.
             An array [1] leads to sonification with only the fundamental frequency core,
             while an array [1,2] causes sonification with the fundamental frequency and twice the fundamental frequency.
 
-    partials_amplitudes: np.ndarray, default = [1]
+    partials_amplitudes: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = [1]
         Array containing the amplitudes for partials.
             An array [1,0.5] causes the sinusoid with frequency core to have amplitude 1,
             while the sinusoid with frequency 2*core has amplitude 0.5.
 
-    partials_phase_offsets: np.ndarray, default = [0]
+    partials_phase_offsets: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = [0]
         Array containing the phase offsets for partials.
 
     fading_duration: float, default: 0.01
         Determines duration of fade-in and fade-out, given in seconds.
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    generated_tone: np.ndarray
+    generated_tone: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Generated signal
     """
     partials_amplitudes = np.ones(len(partials)) if partials_amplitudes is None else partials_amplitudes
     partials_phase_offsets = np.zeros(len(partials)) if partials_phase_offsets is None else partials_phase_offsets
 
-    assert len(partials) == len(partials_amplitudes) == len(partials_phase_offsets), \
-        'Partials, Partials_amplitudes and Partials_phase_offsets must be of equal length.'
+    if not (len(partials) == len(partials_amplitudes) == len(partials_phase_offsets)):
+        raise ValueError('Partials, Partials_amplitudes and Partials_phase_offsets must be of equal length.')
 
     generated_tone = np.zeros_like(frequency_vector)
 
     if gain_vector is None:
         gain_vector = np.ones_like(frequency_vector)
 
     else:
```

### Comparing `libsoni-1.0.1/libsoni/core/pianoroll.py` & `libsoni-1.0.2/libsoni/core/pianoroll.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,28 @@
     and the corresponding pitch.
     The sonification is based on additive synthesis, where parameters partials, partials_amplitudes and
     partials_phase_offsets can be used to shape the sound.
 
     Parameters
     ----------
     pianoroll_df: pd.DataFrame
-        Dataframe containing pitch-event information.
+        Dataframe containing pitch-event information with columns ['start', 'duration', 'pitch', 'velocity', 'label'].
 
-    partials: np.ndarray, default = [1]
+    partials: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = [1]
         Array containing the desired partials of the fundamental frequencies for sonification.
         An array [1] leads to sonification with only the fundamental frequency,
         while an array [1,2] leads to sonification with the fundamental frequency and twice the fundamental frequency.
 
-    partials_amplitudes: np.ndarray, default = None
+    partials_amplitudes: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing the amplitudes for partials.
         An array [1,0.5] causes the first partial to have amplitude 1,
         while the second partial has amplitude 0.5.
         When not defined, the amplitudes for all partials are set to 1.
 
-    partials_phase_offsets: np.ndarray, default = None
+    partials_phase_offsets: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing the phase offsets for partials.
         When not defined, the phase offsets for all partials are set to 0.
 
     tuning_frequency: float, default = 440.0
         Tuning frequency, in Hertz.
 
     sonification_duration: float, default = None
@@ -58,15 +58,15 @@
         Determines if output signal is normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    pianoroll_sonification: np.ndarray
+    pianoroll_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified piano-roll.
     """
 
     pianoroll_df, pianoroll_sonification = __init_pianoroll_sonification(pianoroll_df, fs, sonification_duration)
 
     if 'velocity' in list(pianoroll_df.columns) and pianoroll_df['velocity'].max() > 1:
         pianoroll_df['velocity'] /= pianoroll_df['velocity'].max()
@@ -103,15 +103,15 @@
     The DataFrame representation is assumed to contain row-wise pitch events described by start, duration or end
     and the corresponding pitch.
     For sonification, coloured clicks are used.
 
     Parameters
     ----------
     pianoroll_df: pd.DataFrame
-        Dataframe containing pitch-event information.
+        Dataframe containing pitch-event information with columns ['start', 'duration', 'pitch', 'velocity', 'label'].
 
     tuning_frequency: float, default = 440.0
         Tuning Frequency, in Hertz
 
     sonification_duration: float, default = None
         Determines duration of sonification, in seconds.
 
@@ -122,15 +122,15 @@
         Determines if output signal is normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    pianoroll_sonification: np.ndarray
+    pianoroll_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified waveform in form of a 1D Numpy array.
     """
 
     pianoroll_df, pianoroll_sonification = __init_pianoroll_sonification(pianoroll_df, fs, sonification_duration)
 
     if 'velocity' in list(pianoroll_df.columns) and pianoroll_df['velocity'].max() > 1:
         pianoroll_df['velocity'] /= pianoroll_df['velocity'].max()
@@ -151,37 +151,37 @@
 
     return pianoroll_sonification
 
 
 def sonify_pianoroll_sample(pianoroll_df: pd.DataFrame,
                             sample: np.ndarray = None,
                             reference_pitch: int = 69,
-                            sonification_duration: float = None,
+                            sonification_duration: int = None,
                             signal_fading_duration: float = 0.05,
                             note_fading_duration: float = 0.01,
                             normalize: bool = True,
                             fs: int = 22050) -> np.ndarray:
     """Sonifies a piano-roll based on custom audio samples.
 
     The DataFrame representation is assumed to contain row-wise pitch events described by start, duration or end
     and the corresponding pitch. For sonification, warped versions of the given sample are used.
 
     Parameters
     ----------
     pianoroll_df: pd.DataFrame
-        Dataframe containing pitch-event information.
+        Dataframe containing pitch-event information with columns ['start', 'duration', 'pitch', 'velocity', 'label'].
 
-    sample: np.ndarray
+    sample: np.ndarray (np.float32 / np.float64) [shape=(K, )]
         Sample to use for sonification.
 
     reference_pitch: int, default = 69
         Original pitch of the sample.
 
-    sonification_duration: float, default = None
-        Determines duration of sonification, in seconds.
+    sonification_duration: int, default = None
+        Determines duration of sonification, in samples.
 
     signal_fading_duration: float, default = 0.05
         Determines duration of fade-in and fade-out at beginning and end of the final sonification, in seconds.
 
     note_fading_duration: float, default = 0.01
         Determines duration of fade-in and fade-out at beginning and end of each note event, in seconds.
 
@@ -189,15 +189,15 @@
         Determines if output signal is normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    pianoroll_sonification: np.ndarray
+    pianoroll_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified piano-roll.
     """
 
     pianoroll_df, pianoroll_sonification = __init_pianoroll_sonification(pianoroll_df, fs, sonification_duration)
 
     if 'velocity' in list(pianoroll_df.columns) and pianoroll_df['velocity'].max() > 1:
         pianoroll_df['velocity'] /= pianoroll_df['velocity'].max()
@@ -222,41 +222,41 @@
     return pianoroll_sonification
 
 
 def sonify_pianoroll_fm_synthesis(pianoroll_df: pd.DataFrame,
                                   mod_rate_relative: float = 0.0,
                                   mod_amp: float = 0.0,
                                   tuning_frequency: float = 440.0,
-                                  sonification_duration: float = None,
+                                  sonification_duration: int = None,
                                   signal_fading_duration: float = 0.05,
                                   note_fading_duration: float = 0.01,
                                   normalize: bool = True,
                                   fs: int = 22050) -> np.ndarray:
     """Sonifies a piano-roll with frequency modulation (FM) synthesis.
 
     The DataFrame representation is assumed to contain row-wise pitch events described by start, duration or end
     and the corresponding pitch. The sonification is based on FM synthesis, where parameters mod_rate_relative and
     mod_amp can be used to shape the sound.
 
     Parameters
     ----------
     pianoroll_df: pd.DataFrame
-        Dataframe containing pitch-event information.
+        Dataframe containing pitch-event information with columns ['start', 'duration', 'pitch', 'velocity', 'label'].
 
     mod_rate_relative: float, default = 0.0
         Determines the modulation frequency as multiple or fraction of the frequency for the given pitch.
 
     mod_amp: float, default = 0.0
         Determines the amount of modulation in the generated signal.
 
     tuning_frequency: float, default = 440.0
         Tuning frequency in Hertz.
 
-    sonification_duration: float, default = None
-        Determines duration of sonification, in seconds.
+    sonification_duration: int, default = None
+        Determines duration of sonification, in samples.
 
     signal_fading_duration: float, default = 0.05
         Determines duration of fade-in and fade-out at beginning and end of the final sonification, in seconds.
 
     note_fading_duration: float, default = 0.01
         Determines duration of fade-in and fade-out at beginning and end of each note event, in seconds.
 
@@ -264,15 +264,15 @@
         Determines if output signal is normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    pianoroll_sonification: np.ndarray
+    pianoroll_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified piano-roll.
     """
     pianoroll_df, pianoroll_sonification = __init_pianoroll_sonification(pianoroll_df, fs, sonification_duration)
 
     if 'velocity' in list(pianoroll_df.columns) and pianoroll_df['velocity'].max() > 1:
         pianoroll_df['velocity'] /= pianoroll_df['velocity'].max()
 
@@ -294,27 +294,27 @@
     pianoroll_sonification = normalize_signal(pianoroll_sonification) if normalize else pianoroll_sonification
 
     return pianoroll_sonification
 
 
 def __init_pianoroll_sonification(pianoroll_df: pd.DataFrame,
                                   fs: int,
-                                  sonification_duration: float = None):
+                                  sonification_duration: int = None):
 
     pianoroll_df = format_df(pianoroll_df)
     num_samples = int(pianoroll_df['end'].max() * fs)
 
     if sonification_duration is None:
-        sonification_duration = pianoroll_df['end'].max()
-    sonification_duration_samples = int(sonification_duration * fs)
+        sonification_duration = int(pianoroll_df['end'].max()) * fs
+
+    sonification_duration_secs = sonification_duration / fs
 
     # if sonification_duration is less than num_samples, crop the arrays
-    if sonification_duration_samples < num_samples:
-        pianoroll_df = pianoroll_df[pianoroll_df['start'] < sonification_duration]
-        pianoroll_df.loc[pianoroll_df['end'] > sonification_duration, 'end'] = sonification_duration
+    if sonification_duration < num_samples:
+        pianoroll_df = pianoroll_df[pianoroll_df['start'] < sonification_duration_secs]
+        pianoroll_df.loc[pianoroll_df['end'] > sonification_duration_secs, 'end'] = sonification_duration_secs
 
     pianoroll_df['duration'] = pianoroll_df['end'] - pianoroll_df['start']
 
-    num_samples = sonification_duration_samples
-    pianoroll_sonification = np.zeros(num_samples)
+    pianoroll_sonification = np.zeros(sonification_duration)
 
     return pianoroll_df, pianoroll_sonification
```

### Comparing `libsoni-1.0.1/libsoni/core/spectrogram.py` & `libsoni-1.0.2/libsoni/core/spectrogram.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,21 @@
                        sonification_duration: int = None,
                        normalize: bool = True,
                        fs: int = 22050) -> np.ndarray:
     """Sonifies a spectrogram using sinusoids.
 
     Parameters
     ----------
-    spectrogram: np.ndarray
+    spectrogram: np.ndarray (np.float32 / np.float64) [shape=(N, K)]
         Spectrogram to be sonified.
 
-    frequency_coefficients: np.ndarray, default = None
+    frequency_coefficients: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing frequency coefficients, in Hertz.
 
-    time_coefficients: np.ndarray, default = None
+    time_coefficients: np.ndarray (np.float32 / np.float64) [shape=(K, )], default = None
         Array containing time coefficients, in seconds.
 
     sonification_duration: int, default = None
         Determines duration of sonification, in samples.
 
     fading_duration: float, default = 0.05
         Determines duration of fade-in and fade-out at beginning and end of the sonification, in seconds.
@@ -35,24 +35,18 @@
         Determines if output signal is normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    spectrogram_sonification: np.ndarray
+    spectrogram_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified spectrogram.
     """
-
-    # Check if lengths of coefficient vectors match shape of spectrogram
-    assert spectrogram.shape[0] == len(frequency_coefficients),\
-        f'The length of frequency_coefficients must match spectrogram.shape[0]'
-
-    assert spectrogram.shape[1] == len(time_coefficients), \
-        f'The length of time_coefficients must match spectrogram.shape[1]'
+    __check_spect_shape(spectrogram, len(frequency_coefficients), len(time_coefficients))
 
     # Calculate Hop size from time_coefficients if not explicitly given
     H = int((time_coefficients[1] - time_coefficients[0]) * fs)
 
     # Determine length of sonification
     num_samples = sonification_duration if sonification_duration is not None else int(np.ceil(time_coefficients[-1] * fs) + H)
 
@@ -68,15 +62,14 @@
                                      phase=0,
                                      duration=num_samples / fs,
                                      fs=fs)
 
         spectrogram_sonification += (sinusoid * weighting_vector)
 
     spectrogram_sonification = fade_signal(spectrogram_sonification, fs=fs, fading_duration=fading_duration)
-
     spectrogram_sonification = normalize_signal(spectrogram_sonification) if normalize else spectrogram_sonification
 
     return spectrogram_sonification
 
 
 def sonify_spectrogram_multi(spectrogram: np.ndarray,
                              frequency_coefficients: np.ndarray = None,
@@ -85,21 +78,21 @@
                              fading_duration: float = 0.05,
                              fs: int = 22050,
                              num_processes: int = None) -> np.ndarray:
     """Sonifies a spectrogram using sinusoids, using multiprocessing for efficiency.
 
     Parameters
     ----------
-    spectrogram: np.ndarray
+    sample: np.ndarray (np.float32 / np.float64) [shape=(N, K)]
         Spectrogram to be sonified.
 
-    frequency_coefficients: np.ndarray, default = None
+    frequency_coefficients: np.ndarray (np.float32 / np.float64) [shape=(N, )], default = None
         Array containing frequency coefficients, in Hertz.
 
-    time_coefficients: np.ndarray, default = None
+    time_coefficients: np.ndarray (np.float32 / np.float64) [shape=(K, )], default = None
         Array containing time coefficients, in seconds.
 
     sonification_duration: int, default = None
         Determines duration of sonification, in samples.
 
     fading_duration: float, default = 0.05
         Determines duration of fade-in and fade-out at beginning and end of the sonification, in seconds.
@@ -107,22 +100,18 @@
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     num_processes: int, default = None
         Number of processes
     Returns
     -------
-    spectrogram_sonification: np.ndarray
+    spectrogram_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified spectrogram.
     """
-
-    assert spectrogram.shape[0] == len(frequency_coefficients), \
-        f'The length of frequency_coefficients must match spectrogram.shape[0]'
-    assert spectrogram.shape[1] == len(time_coefficients), \
-        f'The length of time_coefficients must match spectrogram.shape[1]'
+    __check_spect_shape(spectrogram, len(frequency_coefficients), len(time_coefficients))
 
     if num_processes is None:
         num_processes = os.cpu_count() or 1
 
     H = int(np.ceil((time_coefficients[1] - time_coefficients[0]) * fs))
     num_samples = sonification_duration if sonification_duration is not None else int(np.ceil(time_coefficients[-1] * fs) + H)
 
@@ -150,17 +139,17 @@
         spectrogram_sonification += result
 
     spectrogram_sonification = fade_signal(spectrogram_sonification, fs=fs, fading_duration=fading_duration)
     spectrogram_sonification /= np.max(spectrogram_sonification)
 
     return spectrogram_sonification
 
+
 def __sonify_chunk(args):
     start, end, spectrogram_chunk, frequency_coefficients_chunk, time_coefficients, num_samples, H, fs = args
-
     spectrogram_sonification_chunk = np.zeros(num_samples)
 
     for i in range(spectrogram_chunk.shape[0]):
         weighting_vector = np.repeat(spectrogram_chunk[i, :], H)
 
         weighting_vector = smooth_weights(weights=weighting_vector, fading_samples=int(H / 8))
 
@@ -169,7 +158,18 @@
                                      duration=(len(weighting_vector)/fs),
                                      fading_duration=0.05,
                                      fs=fs)
 
         spectrogram_sonification_chunk += (sinusoid * weighting_vector)
     return spectrogram_sonification_chunk
 
+
+def __check_spect_shape(spect: np.ndarray,
+                        num_freq_bins: int,
+                        num_time_frames: int):
+    # Check if lengths of coefficient vectors match shape of spectrogram
+    if not spect.shape[0] == num_freq_bins:
+        raise ValueError('The length of frequency_coefficients must match spectrogram.shape[0]')
+
+    if not spect.shape[1] == num_time_frames:
+        raise ValueError('The length of time_coefficients must match spectrogram.shape[1]')
+
```

### Comparing `libsoni-1.0.1/libsoni/core/tse.py` & `libsoni-1.0.2/libsoni/core/tse.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                       normalize: bool = True,
                       fs: int = 22050) -> np.ndarray:
 
     """Sonifies array of time positions with clicks.
 
     Parameters
     ----------
-    time_positions: np.ndarray
+    time_positions: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Array with time positions for clicks.
 
     click_pitch: int, default = 69
         Pitch for click signal.
 
     click_fading_duration: float, default = 0.25
         Fading duration for click signal, in seconds
@@ -46,15 +46,15 @@
         Determines if output signal is max-normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    tse_sonification: np.ndarray
+    tse_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified time positions.
     """
 
     assert 0 <= click_pitch <= 127, f'Pitch is out of range [0,127].'
     assert 0 <= offset_relative <= 1, f'Relative offset is out of range [0,1].'
 
     num_samples = int((time_positions[-1] + click_fading_duration) * fs)
@@ -90,18 +90,18 @@
                       fading_duration: float = 0.05,
                       normalize: bool = True,
                       fs: int = 22050) -> np.ndarray:
     """Sonifies time positions with warped versions of a custom sample (e.g., metronome sounds).
 
     Parameters
     ----------
-    time_positions: np.ndarray
+    time_positions: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Array with time positions for clicks.
 
-    sample: np.ndarray
+    sample: np.ndarray (np.float32 / np.float64) [shape=(K, )]
         Sample to be used.
 
     offset_relative: float, default = 0.0
         Relative offset coefficient for the beginning of a click.
         0 indicates that the beginning of the click event is at the time position. 1 indicates the ending of the click
         event corresponds to the time position.
 
@@ -115,15 +115,15 @@
         Determines if output signal is max-normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    tse_sonification: np.ndarray
+    tse_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified time positions.
     """
     sample_len = len(sample)
     num_samples = int((time_positions[-1]) * fs) + sample_len
 
     assert sample_len < time_positions[-1] * fs, f'The custom sample cannot be longer than the annotations.'
 
@@ -190,15 +190,15 @@
         Determines if output signal is max-normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    tse_sonification: np.ndarray
+    tse_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified time positions.
     """
 
     if sonification_duration is None:
         max_duration = 0
         for times_pitch in times_pitches:
             sonification_duration = times_pitch[0][-1]
@@ -252,15 +252,15 @@
         Determines if output signal is max-normalized to [-1,1].
 
     fs: int, default = 22050
         Sampling rate, in samples per seconds.
 
     Returns
     -------
-    tse_sonification: np.ndarray
+    tse_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified waveform in form of a 1D Numpy array.
     """
 
     if sonification_duration is None:
         max_duration = 0
         max_sample_duration_samples = 0
 
@@ -297,23 +297,23 @@
                                   fs: int,
                                   fading_duration: float,
                                   normalize: bool) -> np.ndarray:
     """Sonify with sound events (e.g., beats, downbeats, etc.)
 
     Parameters
     ----------
-    sound_event: np.ndarray
+    sound_event: np.ndarray (np.float32 / np.float64) [shape=(K, )]
         A click signal or sample loaded from the disk
 
     offset_relative: float, default = 0.0
         Relative offset for the beginning of a sound event.
         0 indicates that the beginning of the sound event is at the time position,
         1 indicates the ending of the sound event corresponds to the time position.:
 
-    time_positions: np.ndarray
+    time_positions: np.ndarray  (np.float32 / np.float64) [shape=(N, )]
         Array with time positions of the annotations.
 
     num_samples: int
         Number of samples of the output signals
 
     fs: int
         Sampling rate
@@ -322,15 +322,15 @@
         Determines duration of fade-in and fade-out at beginning and end of the sonification, in seconds.
 
     normalize: bool, default = True
         Determines if output signal is max-normalized to [-1,1].
 
     Returns
     -------
-    tse_sonification: np.ndarray
+    tse_sonification: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Sonified signal with multiple sound events, given the time positions
     """
 
     tse_sonification = np.zeros(num_samples)
     num_click_samples = len(sound_event)
     offset_samples = int(offset_relative * num_click_samples)
```

### Comparing `libsoni-1.0.1/libsoni/util/utils.py` & `libsoni-1.0.2/libsoni/util/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 def fade_signal(signal: np.ndarray,
                 fading_duration: float = 0,
                 fs: int = 22050) -> np.ndarray:
     """Fade in / out audio signal
 
     Parameters
     ----------
-    signal: np.ndarray
+    signal: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Signal to be faded
 
     fs: int, default = 22050
         sampling rate
 
     fading_duration: float, default = 0
         duration of fade-in and fade-out, in seconds
 
     Returns
     -------
-    normalized_signal: np.ndarray
+    normalized_signal: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Normalized signal
     """
     num_samples = int(fading_duration * fs)
 
     # if the signal is shorter than twice of the length of the fading duration, multiply signal with sinus half-wave
     if len(signal) < 2 * num_samples:
         signal *= np.sin(np.pi * np.arange(len(signal)) / len(signal))
@@ -47,20 +47,20 @@
 
 
 def normalize_signal(signal: np.ndarray) -> np.ndarray:
     """Max-normalize audio signal
 
     Parameters
     ----------
-    signal: np.ndarray
+    signal: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Signal to be normalized
 
     Returns
     -------
-    normalized_signal: np.ndarray
+    normalized_signal: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Normalized signal
     """
     normalized_signal = signal / np.max(np.abs(signal))
     return normalized_signal
 
 
 def warp_sample(sample: np.ndarray,
@@ -73,15 +73,15 @@
     """This function warps a sample. Given the reference pitch of the sample provided as np.ndarray, the warped version
     of the sample gets pitch-shifted using librosa.effects.pitch_shift(). For the temporal alignment, if the desired
     duration is shorter than the original sample, the sample gets cropped, else if the desired duration is longer of
     the provided sample, the returned signal gets zero-padded at the end.
 
     Parameters
     ----------
-    sample: np.ndarray
+    sample: np.ndarray (np.float32 / np.float64) [shape=(K, )]
         Sample to be warped.
 
     reference_pitch: int
         Reference pitch for the given sample.
 
     target_pitch: int
         Target pitch for the warped sample.
@@ -96,15 +96,15 @@
         Sampling rate, in samples per seconds.
 
     fading_duration: float, default = 0.01
         Duration of fade in and fade out (to avoid clicks)
 
     Returns
     -------
-    warped_sample: np.ndarray
+    warped_sample: np.ndarray (np.float32 / np.float64) [shape=(M, )]
         Warped sample.
     """
     # Compute pitch difference
     pitch_steps = target_pitch - reference_pitch
 
     # Apply pitch-shifting to original sample
     pitch_shifted_sample = librosa.effects.pitch_shift(y=sample,
@@ -172,15 +172,15 @@
     plt.show()
 
     return fig, ax
 
 
 def format_df(df: pd.DataFrame) -> pd.DataFrame:
     df = df.copy().rename(columns=str.lower)
-
+    check_df_schema(df)
     if 'duration' not in df.columns:
         try:
             df['duration'] = df['end'] - df['start']
         except ValueError:
             print('Input DataFrame must have start and duration/end columns.')
     else:
         try:
@@ -197,18 +197,18 @@
                                   gain_lin_original_audio: float = 1.0,
                                   panning: float = 1.0,
                                   duration: int = None):
     """This function takes a sonification and an original_audio and mixes it to stereo
 
     Parameters
     ----------
-    sonification: np.ndarray
+    sonification: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Sonification
 
-    original_audio: np.ndarray
+    original_audio: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Original audio
 
     gain_lin_sonification: float, default = 1.0
         linear gain for sonification
 
     gain_lin_original_audio: float, default = 1.0
         linear gain for original audio
@@ -220,15 +220,15 @@
             panning = 0.0 means sonification on left and original audio on right channel
 
     duration: int, default = None
         Duration of the output waveform, given in samples.
 
     Returns
     -------
-    mixed_audio : np.ndarray
+    stereo_audio : np.ndarray (np.float32 / np.float64) [shape=(N, 2)]
         Mix of the signals
     """
     assert 0.0 <= panning <= 1.0, f'Panning must a value between 0.0 and 1.0.'
     if duration is None:
         num_samples = len(original_audio)
 
     else:
@@ -267,23 +267,23 @@
 @jit(nopython=True)
 def smooth_weights(weights: np.ndarray,
                    fading_samples: int = 0) -> np.ndarray:
     """Weight smoothing
 
     Parameters
     ----------
-    weights: np.ndarray
+    weights: (np.float32 / np.float64) [shape=(N, )]
         Input weights
 
     fading_samples: int
         Number of samples for fade-in/out.
 
     Returns
     -------
-    weights_smoothed: np.ndarray
+    weights_smoothed: np.ndarray (np.float32 / np.float64) [shape=(N, )]
         Smoothed weights
     """
 
     weights_smoothed = weights.copy()
 
     for i in range(1, len(weights) - 1):
         if weights[i] != weights[i - 1]:
@@ -304,15 +304,15 @@
 def visualize_pianoroll(pianoroll_df: pd.DataFrame,
                         xlabel: str = 'Time (seconds)',
                         ylabel: str = 'Pitch',
                         title: str = None,
                         colors: str = 'FMP_1',
                         velocity_alpha: bool = False,
                         figsize : Tuple[float, float] = (12, 4),
-                        ax: matplotlib.axes = None,
+                        ax: matplotlib.axes.Axes = None,
                         dpi: int = 72) -> Tuple[matplotlib.figure.Figure, matplotlib.axes.Axes]:
     """Visualization function for piano-roll representations, given in a pd.DataFrame format
 
     Parameters
     ----------
     pianoroll_df: pd.DataFrame
         Dataframe containing pitch-event information.
@@ -329,14 +329,15 @@
     colors: str, default = 'FMP_1'
         Colormap, for the default colormap see https://github.com/meinardmueller/libfmp.
 
     velocity_alpha: bool = False
         Set True to weight the visualized rectangular regions for each pitch based on their velocity value.
 
     figsize: Tuple[float, float], default: [12, 4])
+        Figure size
 
     ax: matplotlib.axes.Axes
          Axes object
 
     dpi: int
         Resolution of the figure.
 
@@ -380,7 +381,17 @@
     ax.legend([patches.Patch(linewidth=1, edgecolor='k', facecolor=colors[key]) for key in labels_set],
               labels_set, loc='upper right', framealpha=1)
 
     if fig is not None:
         plt.tight_layout()
 
     return fig, ax
+
+
+def check_df_schema(df: pd.DataFrame):
+    try:
+        columns_bool = (df.columns == ['start', 'duration', 'pitch', 'velocity', 'label']).all() and \
+                       len(df.columns) == 5
+        if not columns_bool:
+            raise ValueError("Columns of the dataframe must be ['start', 'duration', 'pitch', 'velocity', 'label'].")
+    except:
+        raise ValueError("Columns of the dataframe must be ['start', 'duration', 'pitch', 'velocity', 'label'].")
```

### Comparing `libsoni-1.0.1/libsoni.egg-info/PKG-INFO` & `libsoni-1.0.2/libsoni.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 Metadata-Version: 2.1
 Name: libsoni
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python Toolbox for Sonifying Music Annotations and Feature Representations
 Home-page: https://github.com/groupmm/libsoni
 Download-URL: https://github.com/groupmm/libsoni
 Author: Yigitcan Özer, Leo Brütting, Simon Schwär, Meinard Müller
 Author-email: yigitcan.oezer@audiolabs-erlangen.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7, <4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython<8.0.0,>=7.8.0
+Requires-Dist: librosa<1.0.0,>=0.8.0
+Requires-Dist: matplotlib<4.0.0,>=3.1.0
+Requires-Dist: numpy<2.0.0,>=1.17.0
+Requires-Dist: pandas<2.0.0,>=1.0.0
+Requires-Dist: pysoundfile<1.0.0,>=0.9.0
+Requires-Dist: scipy<2.0.0,>=1.7.0
+Requires-Dist: libfmp<2.0.0,>=1.2.0
 Provides-Extra: tests
+Requires-Dist: pytest==6.2.*; extra == "tests"
 Provides-Extra: docs
-License-File: LICENCE
+Requires-Dist: sphinx==6.2.*; extra == "docs"
+Requires-Dist: sphinx_rtd_theme==1.2.*; extra == "docs"
 
 [![Python package using Conda](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml/badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml)
 [![Python package using pip](https://github.com/groupmm/libsoni/actions/workflows/test_pip.yml/badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/test_pip.yml)
 
 
 <table border="0">
   <tr>
-    <td><img src=https://github.com/groupmm/libsoni/blob/unit_tests/docs/build/html/_static/libsoni_logo.png alt="libsoni logo" width="1000"></td>
+    <td><img src=https://github.com/groupmm/libsoni/blob/main/docs/build/html/_static/libsoni_logo.png alt="libsoni logo" width="1000"></td>
     <td><h2>libsoni: A Python Toolbox for Sonifying Music Annotations and Feature Representations</h2>
 <br> <br>
 </td>
   </tr>
 </table>
 
-``libsoni`` an open-source Python toolbox tailored for the sonification of music annotations and feature representations. 
+``libsoni`` is an open-source Python toolbox tailored for the sonification of music annotations and feature representations. 
 By employing explicit and easy-to-understand sound synthesis techniques, the toolbox offers functionalities
 for generating and triggering sound events, enabling the sonification of spectral, harmonic, tonal, melodic,
 and rhythmic aspects. Unlike existing software libraries focused on creative applications of sound generation, 
 the toolbox is designed to meet the specific needs of MIR researchers and educators. It aims to simplify the process
 of music exploration, promoting a more intuitive and efficient approach to data analysis by enabling users to interact 
-with their data in acoustically meaningful ways.
+with their data in acoustically meaningful ways. 
+
+See the [API documentation](https://groupmm.github.io/libsoni/build/html/index.html) for a detailed view of the provided functions in ``libsoni``.
 
 ## Installation Guide
 We outline two primary methods for setting up ``libsoni`` using pip and setting up a dedicated environment.
 
 ### Method I: Installing with pip
 Utilize Python's package manager, pip, for a straightforward installation of ``libsoni``:
 
@@ -87,21 +100,21 @@
 ## Contributing
 
 We are happy for suggestions and contributions.  We would be grateful for either
 directly contacting us via email (meinard.mueller@audiolabs-erlangen.de) or for creating 
 an issue in our GitHub repository. Please do not submit a pull request without prior consultation
 with us.
 
-## Licence
-The code for this toolbox is published under an [MIT licence](LICENCE).
+## License
+The code for this toolbox is published under an [MIT license](LICENSE).
 This does not apply to the data files:
 * Schubert songs are taken from the [Schubert Winterreise Dataset](https://zenodo.org/record/4122060). 
 * Recording of the cantata *Ach Gott und Herr* by Bach is taken fom [Bach10 Dataset](https://labsites.rochester.edu/air/datasets/Bach10%20Dataset_v1.0.pdf).
 * Recording of *Locus Iste* by Anton Bruckner is taken from the [Dagstuhl Choir Set](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiJ1JnT9uuEAxXclP0HHUOXC4EQFnoECBMQAQ&url=https%3A%2F%2Fwww.audiolabs-erlangen.de%2Fresources%2FMIR%2F2020-DagstuhlChoirSet&usg=AOvVaw1sPox9R_Sh1eh5hqV2kgNs&opi=89978449).
-* Custom piano audio sample is taken from the [Single Note Database (SNDB)](https://github.com/audiolabs/SNDB)
+* Custom piano audio samples are taken from the [Single Note Database (SNDB)](https://github.com/audiolabs/SNDB).
 * Other audio files are taken from the [FMP notebooks](https://www.audiolabs-erlangen.de/resources/MIR/FMP/C0/C0.html).
 
 ## Acknowledgements
 
 The libsoni package originated from collaboration with various individuals over the past
 years. We extend our gratitude to former and current students, collaborators, 
 and colleagues, including Jonathan Driedger, Angel Villar-Corrales, and Tim Zunner,
```

#### html2text {}

```diff
@@ -1,36 +1,44 @@
-Metadata-Version: 2.1 Name: libsoni Version: 1.0.1 Summary: A Python Toolbox
+Metadata-Version: 2.1 Name: libsoni Version: 1.0.2 Summary: A Python Toolbox
 for Sonifying Music Annotations and Feature Representations Home-page: https://
 github.com/groupmm/libsoni Download-URL: https://github.com/groupmm/libsoni
 Author: Yigitcan Ãzer, Leo BrÃ¼tting, Simon SchwÃ¤r, Meinard MÃ¼ller Author-
 email: yigitcan.oezer@audiolabs-erlangen.de License: MIT Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers Classifier: Topic :: Multimedia ::
 Sound/Audio :: Analysis Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7, <4.0 Description-Content-Type: text/markdown Provides-
-Extra: tests Provides-Extra: docs License-File: LICENCE [![Python package using
+Requires-Python: >=3.7, <4.0 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: ipython<8.0.0,>=7.8.0 Requires-Dist:
+librosa<1.0.0,>=0.8.0 Requires-Dist: matplotlib<4.0.0,>=3.1.0 Requires-Dist:
+numpy<2.0.0,>=1.17.0 Requires-Dist: pandas<2.0.0,>=1.0.0 Requires-Dist:
+pysoundfile<1.0.0,>=0.9.0 Requires-Dist: scipy<2.0.0,>=1.7.0 Requires-Dist:
+libfmp<2.0.0,>=1.2.0 Provides-Extra: tests Requires-Dist: pytest==6.2.*; extra
+== "tests" Provides-Extra: docs Requires-Dist: sphinx==6.2.*; extra == "docs"
+Requires-Dist: sphinx_rtd_theme==1.2.*; extra == "docs" [![Python package using
 Conda](https://github.com/groupmm/libsoni/actions/workflows/test_conda.yml/
 badge.svg)](https://github.com/groupmm/libsoni/actions/workflows/
 test_conda.yml) [![Python package using pip](https://github.com/groupmm/
 libsoni/actions/workflows/test_pip.yml/badge.svg)](https://github.com/groupmm/
 libsoni/actions/workflows/test_pip.yml)
                ********** lliibbssoonnii:: AA PPyytthhoonn TToooollbbooxx ffoorr SSoonniiffyyiinngg MMuussiicc AAnnnnoottaattiioonnss
 [libsoni logo] aanndd FFeeaattuurree RReepprreesseennttaattiioonnss **********
 
 
-``libsoni`` an open-source Python toolbox tailored for the sonification of
+``libsoni`` is an open-source Python toolbox tailored for the sonification of
 music annotations and feature representations. By employing explicit and easy-
 to-understand sound synthesis techniques, the toolbox offers functionalities
 for generating and triggering sound events, enabling the sonification of
 spectral, harmonic, tonal, melodic, and rhythmic aspects. Unlike existing
 software libraries focused on creative applications of sound generation, the
 toolbox is designed to meet the specific needs of MIR researchers and
 educators. It aims to simplify the process of music exploration, promoting a
 more intuitive and efficient approach to data analysis by enabling users to
-interact with their data in acoustically meaningful ways. ## Installation Guide
+interact with their data in acoustically meaningful ways. See the [API
+documentation](https://groupmm.github.io/libsoni/build/html/index.html) for a
+detailed view of the provided functions in ``libsoni``. ## Installation Guide
 We outline two primary methods for setting up ``libsoni`` using pip and setting
 up a dedicated environment. ### Method I: Installing with pip Utilize Python's
 package manager, pip, for a straightforward installation of ``libsoni``: ```
 pip install libsoni ``` Note: We advise performing this installation within a
 Python environment (such as conda or a virtual environment) to prevent any
 conflicts with other packages. Ensure your environment runs Python 3.7 or
 higher. ### Method II: Setting Up a Conda Environment Alternatively, you can
@@ -48,26 +56,26 @@
 install Jupyter to run the notebooks: ``` pip install jupyter ``` 4. **Launch
 Jupyter Notebook:** Start the Jupyter notebook server by executing: ``` jupyter
 notebook ``` This will open a browser window from where you can navigate to and
 open the example notebooks. ## Contributing We are happy for suggestions and
 contributions. We would be grateful for either directly contacting us via email
 (meinard.mueller@audiolabs-erlangen.de) or for creating an issue in our GitHub
 repository. Please do not submit a pull request without prior consultation with
-us. ## Licence The code for this toolbox is published under an [MIT licence]
-(LICENCE). This does not apply to the data files: * Schubert songs are taken
+us. ## License The code for this toolbox is published under an [MIT license]
+(LICENSE). This does not apply to the data files: * Schubert songs are taken
 from the [Schubert Winterreise Dataset](https://zenodo.org/record/4122060). *
 Recording of the cantata *Ach Gott und Herr* by Bach is taken fom [Bach10
 Dataset](https://labsites.rochester.edu/air/datasets/
 Bach10%20Dataset_v1.0.pdf). * Recording of *Locus Iste* by Anton Bruckner is
 taken from the [Dagstuhl Choir Set](https://www.google.com/
 url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiJ1JnT9uuEAxXclP0HHUOXC4EQFnoECBMQAQ&url=https%3A%2F%2Fwww.audiolabs-
 erlangen.de%2Fresources%2FMIR%2F2020-
 DagstuhlChoirSet&usg=AOvVaw1sPox9R_Sh1eh5hqV2kgNs&opi=89978449). * Custom piano
-audio sample is taken from the [Single Note Database (SNDB)](https://
-github.com/audiolabs/SNDB) * Other audio files are taken from the [FMP
+audio samples are taken from the [Single Note Database (SNDB)](https://
+github.com/audiolabs/SNDB). * Other audio files are taken from the [FMP
 notebooks](https://www.audiolabs-erlangen.de/resources/MIR/FMP/C0/C0.html). ##
 Acknowledgements The libsoni package originated from collaboration with various
 individuals over the past years. We extend our gratitude to former and current
 students, collaborators, and colleagues, including Jonathan Driedger, Angel
 Villar-Corrales, and Tim Zunner, for their support and influence in creating
 this Python package. This work was funded by the Deutsche
 Forschungsgemeinschaft (DFG, German Research Foundation) under Grant No.
```

### Comparing `libsoni-1.0.1/setup.py` & `libsoni-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r') as fdesc:
     long_description = fdesc.read()
 
 setup(
     name='libsoni',
-    version='1.0.1',
+    version='1.0.2',
     description='A Python Toolbox for Sonifying Music Annotations and Feature Representations',
     author='Yigitcan Özer, Leo Brütting, Simon Schwär, Meinard Müller',
     author_email='yigitcan.oezer@audiolabs-erlangen.de',
     url='https://github.com/groupmm/libsoni',
     download_url='https://github.com/groupmm/libsoni',
     packages=find_packages(exclude=['tests*']),
     long_description=long_description,
```

