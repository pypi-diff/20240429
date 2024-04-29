# Comparing `tmp/gene-loci-comparison-0.0.3.tar.gz` & `tmp/gene_loci_comparison-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene-loci-comparison-0.0.3.tar", last modified: Wed Aug 10 17:28:18 2022, max compression
+gzip compressed data, was "gene_loci_comparison-0.0.4.tar", last modified: Mon Apr 29 10:45:00 2024, max compression
```

## Comparing `gene-loci-comparison-0.0.3.tar` & `gene_loci_comparison-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-10 17:28:18.314008 gene-loci-comparison-0.0.3/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1069 2021-11-24 20:14:40.000000 gene-loci-comparison-0.0.3/LICENCE.md
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3112 2022-08-10 17:28:18.314008 gene-loci-comparison-0.0.3/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2565 2021-11-24 21:57:32.000000 gene-loci-comparison-0.0.3/README.md
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-10 17:28:18.313008 gene-loci-comparison-0.0.3/gene_loci_comparison/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1611 2021-11-24 20:23:36.000000 gene-loci-comparison-0.0.3/gene_loci_comparison/CustomBiopythonTranslator.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5123 2021-11-24 22:02:39.000000 gene-loci-comparison-0.0.3/gene_loci_comparison/Loci.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     8656 2021-11-24 22:13:01.000000 gene-loci-comparison-0.0.3/gene_loci_comparison/Locus.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)       71 2022-08-10 17:26:21.000000 gene-loci-comparison-0.0.3/gene_loci_comparison/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2000 2022-08-10 17:24:50.000000 gene-loci-comparison-0.0.3/gene_loci_comparison/utils.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-10 17:28:18.314008 gene-loci-comparison-0.0.3/gene_loci_comparison.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3112 2022-08-10 17:28:18.000000 gene-loci-comparison-0.0.3/gene_loci_comparison.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)      420 2022-08-10 17:28:18.000000 gene-loci-comparison-0.0.3/gene_loci_comparison.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2022-08-10 17:28:18.000000 gene-loci-comparison-0.0.3/gene_loci_comparison.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       43 2022-08-10 17:28:18.000000 gene-loci-comparison-0.0.3/gene_loci_comparison.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       21 2022-08-10 17:28:18.000000 gene-loci-comparison-0.0.3/gene_loci_comparison.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2022-08-10 17:28:18.314008 gene-loci-comparison-0.0.3/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1002 2022-08-10 17:26:21.000000 gene-loci-comparison-0.0.3/setup.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-29 10:45:00.112147 gene_loci_comparison-0.0.4/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1069 2021-11-24 20:14:40.000000 gene_loci_comparison-0.0.4/LICENCE.md
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3195 2024-04-29 10:45:00.112147 gene_loci_comparison-0.0.4/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2565 2021-11-24 21:57:32.000000 gene_loci_comparison-0.0.4/README.md
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-29 10:45:00.111147 gene_loci_comparison-0.0.4/gene_loci_comparison/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1222 2024-04-29 10:27:16.000000 gene_loci_comparison-0.0.4/gene_loci_comparison/CustomBiopythonTranslator.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5123 2024-04-29 09:49:34.000000 gene_loci_comparison-0.0.4/gene_loci_comparison/Loci.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     8699 2024-04-29 10:41:46.000000 gene_loci_comparison-0.0.4/gene_loci_comparison/Locus.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       71 2022-08-10 17:26:21.000000 gene_loci_comparison-0.0.4/gene_loci_comparison/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2031 2024-04-29 10:39:58.000000 gene_loci_comparison-0.0.4/gene_loci_comparison/utils.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-29 10:45:00.111147 gene_loci_comparison-0.0.4/gene_loci_comparison.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3195 2024-04-29 10:45:00.000000 gene_loci_comparison-0.0.4/gene_loci_comparison.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      459 2024-04-29 10:45:00.000000 gene_loci_comparison-0.0.4/gene_loci_comparison.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2024-04-29 10:45:00.000000 gene_loci_comparison-0.0.4/gene_loci_comparison.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       43 2024-04-29 10:45:00.000000 gene_loci_comparison-0.0.4/gene_loci_comparison.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       21 2024-04-29 10:45:00.000000 gene_loci_comparison-0.0.4/gene_loci_comparison.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2024-04-29 10:45:00.112147 gene_loci_comparison-0.0.4/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1002 2024-04-29 08:30:39.000000 gene_loci_comparison-0.0.4/setup.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-29 10:45:00.111147 gene_loci_comparison-0.0.4/tests/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4041 2024-04-29 09:06:57.000000 gene_loci_comparison-0.0.4/tests/test_loci.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6810 2024-04-29 10:31:26.000000 gene_loci_comparison-0.0.4/tests/test_locus.py
```

### Comparing `gene-loci-comparison-0.0.3/LICENCE.md` & `gene_loci_comparison-0.0.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `gene-loci-comparison-0.0.3/PKG-INFO` & `gene_loci_comparison-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: gene-loci-comparison
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create fancy (bokeh) gene locus plots from GenBank files
 Home-page: https://github.com/MrTomRod/gene_loci_comparison
 Author: Thomas Roder
 Author-email: roder.thomas@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
+Requires-Dist: pandas
+Requires-Dist: biopython
+Requires-Dist: dna-features-viewer
+Requires-Dist: bokeh
 
 # Gene Loci Comparison
 
 Create fancy (bokeh) gene locus plots from GenBank files!
 
 This repository extends the functionality of the excellent [DnaFeaturesViewer](https://edinburgh-genome-foundry.github.io/DnaFeaturesViewer/)
 
@@ -113,9 +116,7 @@
     auto_reverse=True,
     window_bp=200
 )
 
 ```
 
 ![](tests/output/loci/test_multiple_auto_reverse_gc.svg)
-
-
```

### Comparing `gene-loci-comparison-0.0.3/README.md` & `gene_loci_comparison-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gene-loci-comparison-0.0.3/gene_loci_comparison/Loci.py` & `gene_loci_comparison-0.0.4/gene_loci_comparison/Loci.py`

 * *Files identical despite different names*

### Comparing `gene-loci-comparison-0.0.3/gene_loci_comparison/Locus.py` & `gene_loci_comparison-0.0.4/gene_loci_comparison/Locus.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,21 @@
         self.scaffold_id = self.scaffold.id
 
         unique_features: {(int, int, str)} = set()
 
         def add_unique(f: SeqFeature) -> bool:
             if 'locus_tag' not in f.qualifiers:
                 return False
-            feature = (f.location.nofuzzy_start, f.location.nofuzzy_end, f.qualifiers['locus_tag'][0])
-            if feature in unique_features:
-                return False
-            else:
-                unique_features.add(feature)
-                return True
+            return_bool = False
+            for loc in f.location.parts:
+                feature = (loc.start, loc.end, f.qualifiers['locus_tag'][0])
+                if feature not in unique_features:
+                    unique_features.add(feature)
+                    return_bool = True
+            return return_bool
 
         self.graphic_record: GraphicRecord = CustomBiopythonTranslator(
             label_fields=description_order,
             features_filters=[add_unique, lambda f: f.type != 'source'],
             features_properties=lambda f: dict(qualifiers=f.qualifiers)
         ).translate_record(self.scaffold)
 
@@ -104,16 +105,16 @@
         if auto_reverse and self.is_backward:
             ax.set_xlim(self.gene_location + self.span, self.gene_location - self.span)
         else:
             ax.set_xlim(self.gene_location - self.span, self.gene_location + self.span)
 
         # add title
         if add_title and self.title is not None:
-            # ax.set_title(graphic_record.title)
-            plt.text(s=self.title, transform=ax.transAxes, **title_kwargs)
+            # ax.set_title(self.title)
+            ax.text(s=self.title, transform=ax.transAxes, **title_kwargs)
 
         return ax, _
 
     def plot_to_string(self, tight_layout=True, *args, **kwargs):
         ax, _ = self.plot(*args, **kwargs)
         if tight_layout: ax.figure.tight_layout()
         f = BytesIO()
```

### Comparing `gene-loci-comparison-0.0.3/gene_loci_comparison/utils.py` & `gene_loci_comparison-0.0.4/gene_loci_comparison/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 
 def get_locus_tag(feature: GraphicFeature) -> str:
     return feature.data['qualifiers']['locus_tag'][0]
 
 
 def get_scaffold_and_geneposition(gbk_file, locus) -> (SeqRecord, int):
+    """If a feature has multiple parts, take the location of the first part."""
     assert os.path.isfile(gbk_file)
     with open(gbk_file, "r") as input_handle:
         for scf in SeqIO.parse(input_handle, "genbank"):
             for f in scf.features:
                 if f.type in ["gene", "CDS"] and "locus_tag" in f.qualifiers and f.qualifiers['locus_tag'][0] == locus:
-                    location = f.location if f.location_operator != 'join' else f.location.parts[0]
+                    location = f.location.parts[0]
                     f_start, f_end = location.start, location.end
                     gene_location = f_start + (f_end - f_start) // 2
                     return (scf, gene_location)
     raise KeyError(F'Gene {locus} was not found in file {gbk_file}')
 
 
 JAVASCRIPT_TAP_CALLBACK = """\
```

### Comparing `gene-loci-comparison-0.0.3/gene_loci_comparison.egg-info/PKG-INFO` & `gene_loci_comparison-0.0.4/gene_loci_comparison.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: gene-loci-comparison
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create fancy (bokeh) gene locus plots from GenBank files
 Home-page: https://github.com/MrTomRod/gene_loci_comparison
 Author: Thomas Roder
 Author-email: roder.thomas@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
+Requires-Dist: pandas
+Requires-Dist: biopython
+Requires-Dist: dna-features-viewer
+Requires-Dist: bokeh
 
 # Gene Loci Comparison
 
 Create fancy (bokeh) gene locus plots from GenBank files!
 
 This repository extends the functionality of the excellent [DnaFeaturesViewer](https://edinburgh-genome-foundry.github.io/DnaFeaturesViewer/)
 
@@ -113,9 +116,7 @@
     auto_reverse=True,
     window_bp=200
 )
 
 ```
 
 ![](tests/output/loci/test_multiple_auto_reverse_gc.svg)
-
-
```

### Comparing `gene-loci-comparison-0.0.3/setup.py` & `gene_loci_comparison-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / 'README.md').read_text()
 
 # This call to setup() does all the work
 setup(
     name='gene-loci-comparison',
-    version='0.0.3',
+    version='0.0.4',
     description='Create fancy (bokeh) gene locus plots from GenBank files',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/MrTomRod/gene_loci_comparison',
     author='Thomas Roder',
     author_email='roder.thomas@gmail.com',
     license='MIT',
```

