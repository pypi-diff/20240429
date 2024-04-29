# Comparing `tmp/AlleleFinder-0.1.6.tar.gz` & `tmp/allelefinder-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adamkoziol/PycharmProjects/AlleleFinder/dist/tmp8yujkd8g/AlleleFinder-0.1.6.tar", last modified: Fri Jan 19 14:43:59 2024, max compression
+gzip compressed data, was "allelefinder-0.1.7.tar", last modified: Mon Apr 29 18:45:40 2024, max compression
```

## Comparing `AlleleFinder-0.1.6.tar` & `allelefinder-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/
--rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)     1113 2023-02-24 20:49:53.000000 AlleleFinder-0.1.6/setup.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1077 2024-01-19 14:37:34.000000 AlleleFinder-0.1.6/LICENSE
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/PKG-INFO
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/AlleleFinder.egg-info/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      742 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/AlleleFinder.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       19 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/AlleleFinder.egg-info/top_level.txt
--rw-r--r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/AlleleFinder.egg-info/PKG-INFO
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/AlleleFinder.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     9315 2024-01-19 14:42:23.000000 AlleleFinder-0.1.6/README.md
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/allele_tools/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    24429 2023-03-24 14:27:36.000000 AlleleFinder-0.1.6/allele_tools/allele_profiler.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35819 2024-01-19 14:32:21.000000 AlleleFinder-0.1.6/allele_tools/stec.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-06-22 16:34:50.000000 AlleleFinder-0.1.6/allele_tools/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6600 2023-07-05 14:06:55.000000 AlleleFinder-0.1.6/allele_tools/profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    98496 2024-01-19 14:33:34.000000 AlleleFinder-0.1.6/allele_tools/methods.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       51 2024-01-19 14:42:23.000000 AlleleFinder-0.1.6/allele_tools/version.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    28340 2023-03-24 18:52:09.000000 AlleleFinder-0.1.6/allele_tools/allele_updater.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35343 2023-03-24 19:36:21.000000 AlleleFinder-0.1.6/allele_tools/allele_translate_reduce.py
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/tests/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4680 2023-12-18 15:48:41.000000 AlleleFinder-0.1.6/tests/test_5_stec_allele_find.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6584 2023-12-18 15:35:52.000000 AlleleFinder-0.1.6/tests/test_1_allele_translate_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4628 2023-03-13 20:02:00.000000 AlleleFinder-0.1.6/tests/test_3_stec_profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2107 2023-12-18 15:48:41.000000 AlleleFinder-0.1.6/tests/test_6_stec_aa_allele_find.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2022-03-21 20:37:30.000000 AlleleFinder-0.1.6/tests/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2829 2023-02-28 19:59:56.000000 AlleleFinder-0.1.6/tests/test_0_profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3249 2023-06-19 15:57:17.000000 AlleleFinder-0.1.6/tests/test_7_stec_allele_split.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4265 2023-06-19 15:58:02.000000 AlleleFinder-0.1.6/tests/test_8_stec_allele_concatenate.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     7795 2023-12-18 15:35:52.000000 AlleleFinder-0.1.6/tests/test_2_allele_updater.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3042 2023-03-13 19:11:01.000000 AlleleFinder-0.1.6/tests/test_4_stec_allele_translate_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2024-01-19 14:43:59.000000 AlleleFinder-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:45:40.648313 allelefinder-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:45:40.648313 allelefinder-0.1.7/AlleleFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-29 18:45:40.000000 allelefinder-0.1.7/AlleleFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-29 18:45:40.000000 allelefinder-0.1.7/AlleleFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:45:40.000000 allelefinder-0.1.7/AlleleFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 18:45:40.000000 allelefinder-0.1.7/AlleleFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 18:45:40.000000 allelefinder-0.1.7/AlleleFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 18:45:32.000000 allelefinder-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-29 18:45:40.648313 allelefinder-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-29 18:45:32.000000 allelefinder-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:45:40.644313 allelefinder-0.1.7/allele_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:45:32.000000 allelefinder-0.1.7/allele_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-04-29 18:45:32.000000 allelefinder-0.1.7/allele_tools/allele_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-04-29 18:45:32.000000 allelefinder-0.1.7/allele_tools/allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-04-29 18:45:32.000000 allelefinder-0.1.7/allele_tools/allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-04-29 18:45:32.000000 allelefinder-0.1.7/allele_tools/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-29 18:45:32.000000 allelefinder-0.1.7/allele_tools/profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-04-29 18:45:32.000000 allelefinder-0.1.7/allele_tools/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 18:45:32.000000 allelefinder-0.1.7/allele_tools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:45:40.648313 allelefinder-0.1.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2048 2024-04-29 18:45:32.000000 allelefinder-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:45:40.648313 allelefinder-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_0_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_1_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_2_allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_3_stec_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_4_stec_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_5_stec_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_6_stec_aa_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_7_stec_allele_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_8_stec_allele_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-29 18:45:32.000000 allelefinder-0.1.7/tests/test_9_stec_allele_translate_find.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `AlleleFinder-0.1.6/LICENSE` & `allelefinder-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.6/AlleleFinder.egg-info/SOURCES.txt` & `allelefinder-0.1.7/AlleleFinder.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 AlleleFinder.egg-info/PKG-INFO
 AlleleFinder.egg-info/SOURCES.txt
 AlleleFinder.egg-info/dependency_links.txt
+AlleleFinder.egg-info/requires.txt
 AlleleFinder.egg-info/top_level.txt
 allele_tools/__init__.py
 allele_tools/allele_profiler.py
 allele_tools/allele_translate_reduce.py
 allele_tools/allele_updater.py
 allele_tools/methods.py
 allele_tools/profile_reduce.py
@@ -18,8 +19,9 @@
 tests/test_1_allele_translate_reduce.py
 tests/test_2_allele_updater.py
 tests/test_3_stec_profile_reduce.py
 tests/test_4_stec_allele_translate_reduce.py
 tests/test_5_stec_allele_find.py
 tests/test_6_stec_aa_allele_find.py
 tests/test_7_stec_allele_split.py
-tests/test_8_stec_allele_concatenate.py
+tests/test_8_stec_allele_concatenate.py
+tests/test_9_stec_allele_translate_find.py
```

### Comparing `AlleleFinder-0.1.6/allele_tools/allele_profiler.py` & `allelefinder-0.1.7/allele_tools/allele_profiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,49 +11,63 @@
 import json
 import os
 
 # Third party imports
 from Bio.Seq import Seq
 from Bio import SeqIO
 
+from olctools.accessoryFunctions.accessoryFunctions import MetadataObject
+
 
 # Local imports
 from allele_tools.methods import \
      extract_novel_alleles
 from olctools.accessoryFunctions.accessoryFunctions import combinetargets
 from genemethods.geneseekr.geneseekr import GeneSeekr
 
 
 __author__ = 'adamkoziol'
 
 
 def allele_prep(allele_path, gene_names, combined_targets, amino_acid):
     """
     Create a 'combinedtargets.fasta' file
-    :param allele_path: Name and absolute path to folder containing allele database files
+    :param allele_path: Name and absolute path to folder containing allele
+    database files
     :param gene_names: List of all gene names in the analysis
-    :param combined_targets: String of absolute path to the combinedtargets.fasta file
-    :param amino_acid: Boolean of whether the query sequences are amino acid or nucleotide
+    :param combined_targets: String of absolute path to the
+    combinedtargets.fasta file
+    :param amino_acid: Boolean of whether the query sequences are amino acid
+    or nucleotide
     :return: records: Dictionary of allele_header:allele_sequence
     :return: gene_names: List of all gene names extracted from allele headers
-    :return: data: String of header including all gene names. To be used in creating final report
+    :return: data: String of header including all gene names. To be used in
+    creating final report
     """
     logging.info('Reading allele files')
     custom_targets = os.path.join(allele_path, 'custom.tfa')
     combined_targets_db = glob(os.path.join(allele_path, 'combinedtargets*'))
     records = {}
-    # Clear out any previously created combinedtargets files (and associated BLAST databases)
+    # Clear out any previously created combinedtargets files (and associated
+    # BLAST databases)
     clear_alleles(combined_targets_db=combined_targets_db,
                   custom_targets=custom_targets)
     alleles = glob(os.path.join(allele_path, '*.*fa*'))
-    # If the dictionary hasn't already been populated by a previous iteration, remove the path and
+    # If the dictionary hasn't already been populated by a previous iteration,
+    # remove the path and
     # the extension from each of the allele files to determine gene names
     if not gene_names:
         for allele in alleles:
-            gene_names.append(os.path.splitext(os.path.basename(allele))[0].replace('_alleles', ''))
+            gene_names.append(
+                os.path.splitext(
+                    os.path.basename(
+                        allele
+                    )
+                )[0].replace('_alleles', '')
+            )
     # Populate the header string for the final report
     genes = '\t'.join(sorted(gene_names))
     data = f'ST\t{genes}\n'
     # Create the combinedtargets file
     if not os.path.isfile(combined_targets):
         if amino_acid:
             combinetargets(
@@ -76,16 +90,18 @@
         for record in SeqIO.parse(allele_file, 'fasta'):
             records[record.id] = str(record.seq)
     return records, gene_names, data
 
 
 def clear_alleles(combined_targets_db, custom_targets):
     """
-    Remove any combinedtargets.fasta or custom.tfa files present in the allele path
-    :param combined_targets_db: List of combinedtargets files, including BLAST database files
+    Remove any combinedtargets.fasta or custom.tfa files present in the
+    allele path
+    :param combined_targets_db: List of combinedtargets files, including BLAST
+    database files
     :param custom_targets: Name and absolute path to custom.tfa target file
     :return:
     """
     # Iterate through all the combinedtargets files
     for combined_target in combined_targets_db:
         # Remove each file
         os.remove(combined_target)
@@ -103,382 +119,528 @@
     """
     # Initialise the dictionary
     profile_data = {}
     # Only load the profile file if it exists
     if os.path.isfile(profile_file):
         logging.info('Extracting profiles from profile file')
         # Open an Excel-formatted sequence profile file as a dictionary
-        profile = DictReader(open(profile_file, encoding='utf-8'), dialect='excel-tab')
+        profile = DictReader(
+            open(
+                profile_file,
+                encoding='utf-8'
+            ), dialect='excel-tab'
+        )
         # Iterate through the rows
         for row in profile:
-            # Populate the profile dictionary with profile number: {gene: allele}.
-            allele_comprehension = {gene: allele for gene, allele in row.items() if gene != 'ST'}
+            # Populate the profile dictionary with profile number:
+            # {gene: allele}.
+            allele_comprehension = {
+                gene[0].lower() +
+                gene[1:-1] +
+                gene[-1].upper():
+                    allele for gene, allele in row.items() if gene != 'ST'
+            }
             # Extract the sequence type number from the first field name
             seq_type = row[profile.fieldnames[0]]
             # Update the profile data dictionary
             profile_data[seq_type] = allele_comprehension
     return profile_data
 
 
-def parseable_blast_outputs(runmetadata, fieldnames, extended_fieldnames, records, cutoff=90):
-    """
-    Add a header to the BLAST report, so that it is easier to figure out what is in each column
-    :param runmetadata: Metadata object containing a list of all metadata objects
+def parseable_blast_outputs(
+        runmetadata: MetadataObject,
+        fieldnames: str,
+        extended_fieldnames: str,
+        records: dict,
+        cutoff: int = 90):
+    """
+    Add a header to the BLAST report, so that it is easier to figure out what
+    is in each column
+    :param runmetadata: Metadata object containing a list of all
+    metadata objects
     :param fieldnames: String of all the field names in the BLAST report
-    :param extended_fieldnames: String of the BLAST field names plus the calculated percent identity
+    :param extended_fieldnames: String of the BLAST field names plus the
+    calculated percent identity
     :param records: Dictionary of allele name: allele sequence
-    :param cutoff: Integer of the minimum percent identity between query and subject sequence. Default is 90
+    :param cutoff: Integer of the minimum percent identity between query and
+    subject sequence. Default is 90
     """
     logging.info('Adding headers to BLAST outputs')
     for sample in runmetadata.samples:
         data = []
         # Load the first line of the report
-        with open(sample.alleles.blast_report, 'r', encoding='utf-8') as report:
+        with open(
+            sample.alleles.blast_report,
+            'r',
+                encoding='utf-8') as report:
             header_line = report.readline().strip()
         # Split the header on tabs
         header_list = header_line.split('\t')
-        # Check to see if the header has already been added. Skip this step if it has been added.
+        # Check to see if the header has already been added. Skip this step
+        # if it has been added.
         if header_list[0] != fieldnames[0]:
-            with open(sample.alleles.blast_report, 'r', encoding='utf-8') as report:
+            with open(
+                sample.alleles.blast_report,
+                'r',
+                    encoding='utf-8') as report:
                 header = list(report.readline().split('\t'))
             if len(header) == len(fieldnames):
                 current_fieldnames = fieldnames
             else:
                 current_fieldnames = extended_fieldnames
-            blastdict = DictReader(open(sample.alleles.blast_report, encoding='utf-8'),
-                                   fieldnames=current_fieldnames,
-                                   dialect='excel-tab'
-                                   )
+            blastdict = DictReader(
+                open(
+                    sample.alleles.blast_report, encoding='utf-8'
+                ),
+                fieldnames=current_fieldnames,
+                dialect='excel-tab'
+            )
             # Go through each BLAST result
             for row in blastdict:
-                # Calculate the percent identity and extract the bit score from the row
-                # Percent identity is the (length of the alignment - num mismatches) /
-                # total query length
+                # Calculate the percent identity and extract the bit score
+                # from the row Percent identity is the (length of the
+                # alignment - num mismatches) / total query length
                 percent_identity = float(
-                    '{:0.2f}'.format((float(row['identical']) - float(row['gaps'])) /
-                                     len(records[row['subject_id']]) * 100)
+                    '{:0.2f}'.format(
+                        (float(
+                            row['identical']) - float(row['gaps'])
+                         ) / len(records[row['subject_id']]) * 100
+                    )
                 )
                 # Filter the results based on the cutoff value
                 if percent_identity < cutoff:
                     continue
-                # Create a percent match entry based on the calculated percent identity match
+                # Create a percent match entry based on the calculated
+                # percent identity match
                 row['percent_match'] = str(percent_identity)
                 # Add the updated row to the list
                 data.append(row)
 
-            # Overwrite the original BLAST outputs to include headers, and the percent match
-            with open(sample.alleles.blast_report, 'w', encoding='utf-8') as updated_report:
+            # Overwrite the original BLAST outputs to include headers,
+            # and the percent match
+            with open(
+                sample.alleles.blast_report,
+                'w',
+                    encoding='utf-8') as updated_report:
                 # Add the header
                 headers = '\t'.join(extended_fieldnames)
                 updated_report.write(f'{headers}\n')
                 # Add the results
                 for row in data:
                     for header in extended_fieldnames:
-                        # Write the value from the row with the header as the key
-                        try:
-                            updated_report.write('{value}\t'.format(value=row[header]))
-                        except KeyError:
-                            # noinspection PyTypeChecker
-                            updated_report.write('{value}\t'.format(value=''.join(row[None])))
+                        # Write the value from the row with the header as
+                        # the key
+                        updated_report.write(
+                            '{value}\t'.format(value=row[header])
+                        )
                     # Add a newline for each result
                     updated_report.write('\n')
 
 
-def parse_results(runmetadata, fieldnames, extended_fieldnames, amino_acid, genome_query=False):
+def parse_results(
+        runmetadata: MetadataObject,
+        fieldnames: str,
+        extended_fieldnames: str,
+        amino_acid: bool,
+        genome_query: bool = False):
     """
     Parse the BLAST results, and populate GenObjects
     :param runmetadata: Metadata object containing list of all metadata objects
     :param fieldnames: String of all the field names in the BLAST report
-    :param extended_fieldnames: String of the BLAST field names plus the calculated percent identity
+    :param extended_fieldnames: String of the BLAST field names plus the
+    calculated percent identity
     :param amino_acid: Variable on whether targets are protein
-    :param genome_query: Boolean of whether the query is a genome, and the subject is the allele
+    :param genome_query: Boolean of whether the query is a genome, and the
+    subject is the allele
     :return: Updated runmetadata
     """
     logging.info('Parsing BLAST outputs')
     for sample in runmetadata.samples:
         # Initialise GenObjects as required
         sample.alleles.blastlist = []
         sample.alleles.targetsequence = {}
         # Open the sequence profile file as a dictionary
-        blastdict = DictReader(open(sample.alleles.blast_report, encoding='utf-8'),
-                               fieldnames=extended_fieldnames,
-                               dialect='excel-tab')
+        blastdict = DictReader(
+            open(
+                sample.alleles.blast_report, encoding='utf-8'
+            ),
+            fieldnames=extended_fieldnames,
+            dialect='excel-tab'
+        )
         resultdict = {}
         # Go through each BLAST result
         for row in blastdict:
             # Ignore the headers
             if row['query_id'].startswith(fieldnames[0]):
                 pass
             else:
-                target_id = row['query_id'] if not genome_query else row['subject_id']
+                target_id = row['query_id'] if not genome_query else \
+                    row['subject_id']
                 target_start = row['subject_start']
                 target_end = row['subject_end']
                 target_seq = row['query_sequence']
                 # Remove unwanted pipes added to the name
-                target = target_id.lstrip('gb|').rstrip('|') if '|' in target_id else \
-                    target_id
+                target = target_id.lstrip('gb|').rstrip('|') if '|' \
+                    in target_id else target_id
                 # If the percent identity is equal to the cutoff
                 if float(row['percent_match']) == 100:
                     # Append the hit dictionary to the list
                     sample.alleles.blastlist.append(row)
-                    # Update the dictionary with the target and percent identity
+                    # Update the dictionary with the target and
+                    # percent identity
                     resultdict.update({target: row['percent_match']})
-                    # Determine if the orientation of the sequence is reversed compared to
+                    # Determine if the orientation of the sequence is
+                    # reversed compared to
                     # the reference sequence
                     if int(target_end) < int(target_start) and not amino_acid:
                         # Create a sequence object using BioPython
                         seq = Seq(target_seq)
                         # Calculate the reverse complement of the sequence
                         querysequence = str(seq.reverse_complement())
-                    # If the sequence is not reversed, use the sequence as it is in the output
+                    # If the sequence is not reversed, use the sequence as it
+                    # is in the output
                     else:
                         querysequence = target_seq
                     # Add the sequence in the correct orientation to the sample
                     try:
-                        sample.alleles.targetsequence[target].append(querysequence)
+                        sample.alleles.targetsequence[target].append(
+                            querysequence
+                        )
                     except (AttributeError, KeyError):
                         sample.alleles.targetsequence[target] = []
-                        sample.alleles.targetsequence[target].append(querysequence)
+                        sample.alleles.targetsequence[target].append(
+                            querysequence
+                        )
             # Add the percent identity to the object
             sample.alleles.blastresults = resultdict
         # Populate missing results with 'NA' values
         if len(resultdict) == 0:
             sample.alleles.blastresults = 'NA'
     return runmetadata
 
 
-def profile_alleles(runmetadata, profile_dict, profile_set, records, amino_acid=False,
-                    novel_alleles=False, genome_query=False, allele_path=None, report_path=None,
-                    cutoff=75):
+def profile_alleles(
+        runmetadata: MetadataObject,
+        profile_dict: dict,
+        profile_set: list,
+        records: list,
+        amino_acid: bool = False,
+        novel_alleles: bool = False,
+        genome_query: bool = False,
+        allele_path: str = None,
+        report_path: str = None,
+        cutoff: int = 75):
     """
     Create the gene:allele profile from the BLAST outputs from each sample
-    :param runmetadata: Metadata object containing a list of all metadata objects
-    :param profile_dict: Dictionary to store gene:allele profile for each sample
+    :param runmetadata: Metadata object containing a list of all
+    metadata objects
+    :param profile_dict: Dictionary to store gene:allele profile for
+    each sample
     :param profile_set: List of all unique profiles
     :param records: List of all gene names
-    :param novel_alleles: Boolean of whether novel alleles should be extracted from BLAST hit if
-    there is no 100% match
-    :param genome_query: Boolean of whether the query is a genome, and the subject is the allele
+    :param novel_alleles: Boolean of whether novel alleles should be extracted
+    from BLAST hit if there is no 100% match
+    :param genome_query: Boolean of whether the query is a genome, and the
+    subject is the allele
     :param amino_acid: Variable on whether targets are protein
-    :param allele_path: Name and absolute path to folder containing allele database files
-    :param report_path: Name and absolute path to folder in which reports are to be created
-    :param cutoff: Integer of the minimum percent identity between query and subject sequence. Default is 75
+    :param allele_path: Name and absolute path to folder containing allele
+    database files
+    :param report_path: Name and absolute path to folder in which reports are
+    to be created
+    :param cutoff: Integer of the minimum percent identity between query and
+    subject sequence. Default is 75
     :return: Updated profile_dict and profile_set
     """
     logging.info('Determining allele profiles')
     # Iterate through all the samples
     for sample in runmetadata.samples:
-        # Initialise a dictionary to store the profile information for each samples
+        # Initialise a dictionary to store the profile information for
+        # each sample
         profile_dict[sample.name] = {}
-        # Initialise a dictionary to store the gene:allele combinations for each sample
+        # Initialise a dictionary to store the gene:allele combinations for
+        # each sample
         allele_comprehension = {}
-        # Each gene in the analysis is stored in the list of genes created in allele_finder
+        # Each gene in the analysis is stored in the list of genes created
+        # in allele_finder
         for gene in records:
-            # Create a variable to track whether the current gene is present in the current sample
+            gene = gene[0].lower() + gene[1:-1] + gene[-1].upper()
+            # Create a variable to track whether the current gene is present
+            # in the current sample
             present = False
             # Iterate through all the BLAST outputs for the sample
             for allele in sample.alleles.blastresults:
-                # If the gene name is present as a substring of the allele e.g. adk in adk_1,
-                # then the gene is present in the BLAST outputs
-                if gene in allele:
-                    # Strip off the allele number from the allele e.g. adk_1 yields 1
+                # If the gene name is present as a substring of the allele
+                # e.g. adk in adk_1, then the gene is present in the
+                # BLAST outputs
+                if gene.lower() in allele.lower():
+                    # Strip off the allele number from the allele e.g.
+                    # adk_1 yields 1
                     allele_id = allele.split('_')[-1]
-                    # Update the dictionary with the new gene: allele number for the sample
+                    # Update the dictionary with the new gene: allele number
+                    # for the sample
                     allele_comprehension.update({gene: allele_id})
                     # Update the gene presence variable
                     present = True
-            # If, after iterating through all the BLAST outputs, the gene is not present in the
-            # sample, update the gene: allele to reflect this absence
+            # If, after iterating through all the BLAST outputs, the gene is
+            # not present in the sample, update the gene: allele to reflect
+            # this absence
             if not present:
                 if novel_alleles:
-                    sample, novel_allele, query_sequence = extract_novel_alleles(
-                        sample=sample,
-                        gene=gene,
-                        genome_query=genome_query,
-                        amino_acid=amino_acid,
-                        allele_path=allele_path,
-                        report_path=report_path,
-                        cutoff=cutoff,
-                    )
+                    sample, novel_allele, query_sequence = \
+                        extract_novel_alleles(
+                            sample=sample,
+                            gene=gene,
+                            genome_query=genome_query,
+                            amino_acid=amino_acid,
+                            allele_path=allele_path,
+                            report_path=report_path,
+                            cutoff=cutoff,
+                        )
+                    novel_allele = novel_allele.split('|')[0]
                     try:
-                        sample.alleles.targetsequence[novel_allele].append(query_sequence)
+                        sample.alleles.targetsequence[novel_allele].append(
+                            query_sequence
+                        )
                     except KeyError:
-                        sample.alleles.targetsequence[novel_allele] = [query_sequence]
+                        sample.alleles.targetsequence[novel_allele] = \
+                            [query_sequence]
                     if novel_allele:
-                        allele_comprehension.update({gene: novel_allele.split('_')[-1]})
+                        allele_comprehension.update(
+                            {
+                                gene: novel_allele.split('_')[-1]
+                                }
+                        )
                     else:
                         allele_comprehension.update({gene: '0'})
                 else:
                     # Set missing alleles to 'ND'
                     allele_comprehension.update({gene: '0'})
-        # In order to hash the dictionary, use JSON, with sorted keys to freeze it
-        frozen_allele_comprehension = json.dumps(allele_comprehension, sort_keys=True)
-        # Update the dictionary of profiles with the hash of the frozen dictionary: list of
-        # samples with that hash
+        # In order to hash the dictionary, use JSON, with sorted keys
+        # to freeze it
+        frozen_allele_comprehension = json.dumps(
+            allele_comprehension,
+            sort_keys=True
+        )
+        # Update the dictionary of profiles with the hash of the frozen
+        # dictionary: list of samples with that hash
         if hash(frozen_allele_comprehension) not in profile_dict:
             profile_dict[hash(frozen_allele_comprehension)] = [sample.name]
         else:
             profile_dict[hash(frozen_allele_comprehension)].append(sample.name)
         # Add the 'regular' dictionary to the list of all profiles as required
         if allele_comprehension not in profile_set:
             profile_set.append(allele_comprehension)
     return profile_dict, profile_set
 
 
-def match_profile(profile_data, profile_dict, profile_matches):
+def match_profile(
+        profile_data: dict,
+        profile_dict: dict,
+        profile_matches: dict):
     """
     Match current profiles to any previously created profiles
     :param profile_data: Dictionary of seq_type: {gene name:allele ID}
     :param profile_dict: Dictionary of gene:allele profile for each sample
     :param profile_matches: Dictionary of seq_type: matching profile
     :return: profile_matches: Updated dictionary of seq_type: matching profiles
     """
-    # If the profile_data dictionary was not populated in the read_profiles methods,
-    # there is nothing to match
+    # If the profile_data dictionary was not populated in the read_profiles
+    # methods, there is nothing to match
     if profile_data:
         logging.info('Matching new profiles against profile file')
         # Extract the sequence type and allele dictionary from the profile file
         for seq_type, allele_comprehension in profile_data.items():
             # Freeze the allele comprehension as above
-            frozen_allele_comprehension = json.dumps(allele_comprehension, sort_keys=True)
+            frozen_allele_comprehension = json.dumps(
+                allele_comprehension,
+                sort_keys=True
+            )
             try:
                 # Extract the samples that match this profile
                 matches = profile_dict[hash(frozen_allele_comprehension)]
                 # Update the dictionary with the matching samples
                 profile_matches[seq_type] = matches
-            # The profile will not necessarily match any of the profiles found in the analysis
+            # The profile will not necessarily match any of the profiles
+            # found in the analysis
             except KeyError:
                 pass
     return profile_matches
 
 
-def create_profile(profile_data, profile_set, new_profiles, profile_dict, profile_matches):
+def create_profile(
+        profile_data: dict,
+        profile_set: list,
+        new_profiles: list,
+        profile_dict: dict,
+        profile_matches: dict):
     """
     Create new profiles for novel profiles as required
     :param profile_data: Dictionary of seq_type: {gene name:allele ID}
     :param profile_set: List of all unique profiles
     :param new_profiles: List of novel profiles
     :param profile_dict: Dictionary of gene:allele profile for each sample
     :param profile_matches: Dictionary of seq_type: matching profile
     :return: profile_matches: Updated dictionary of seq_type: matching profiles
-    :return: profile_data: Updated dictionary of seq_type: {gene name: allele ID}
+    :return: profile_data: Updated dictionary of seq_type: {gene name:
+    allele ID}
     :return: new_profiles: Updated list of novel profiles
     """
     # Initialise the sequence type to be 1
     seq_type = 1
-    # If the profile_data dictionary exists, set the sequence type to be the last of the entries
-    # in the dictionary plus one, as that corresponds to the next sequence type
+    # If the profile_data dictionary exists, set the sequence type to be the
+    # last of the entries in the dictionary plus one, as that corresponds to
+    # the next sequence type
     if profile_data:
         # seq_type = len(profile_data) + 1
         seq_type = sorted(int(st) for st in profile_data.keys())[-1] + 1
     # Initialise a list to store the matched samples
     matched = []
     # Iterate through all the profiles in the analysis
     for allele_comprehension in profile_set:
-        # Ensure that the allele comprehension (profile) is not already in the profile file
-        if allele_comprehension not in [profiled_alleles for st, profiled_alleles in profile_data.items()]:
+        # Ensure that the allele comprehension (profile) is not already in
+        # the profile file
+        if allele_comprehension not in [
+                profiled_alleles for _,
+                profiled_alleles in profile_data.items()]:
             # Add the new profile to the list of new profiles
             alleles = '\t'.join(
                 allele_num.split('_')[-1] for gene, allele_num in sorted(
                     allele_comprehension.items()
                 )
             )
             new_profiles.append(
                 f'{seq_type}\t{alleles.rstrip()}'
             )
-            # Freeze the comprehension in order to be used as the key in the profile dictionary
-            frozen_allele_comprehension = json.dumps(allele_comprehension, sort_keys=True)
+            # Freeze the comprehension in order to be used as the key in the
+            # profile dictionary
+            frozen_allele_comprehension = json.dumps(
+                allele_comprehension,
+                sort_keys=True
+            )
             matches = profile_dict[hash(frozen_allele_comprehension)]
-            # Check to see if this sequence type hasn't already been found in the current analysis
+            # Check to see if this sequence type hasn't already been found in
+            # the current analysis
             if matches not in matched:
-                # Update the dictionary with the new sequence type: list of samples
+                # Update the dictionary with the new sequence type: list
+                # of samples
                 profile_matches[seq_type] = matches
                 profile_data[seq_type] = allele_comprehension
                 # Add the matches to the list of matches
                 matched.append(matches)
             # Increment the sequence type number of the next entry
             seq_type += 1
     return profile_matches, profile_data, new_profiles
 
 
-def sequence_typer(profile_report, data, runmetadata, profile_matches, profile_data,
-                   update=False, amino_acid=False):
+def sequence_typer(
+            profile_report: str,
+            data: str,
+            runmetadata: MetadataObject,
+            profile_matches: dict,
+            profile_data: dict,
+            update: bool = False,
+            amino_acid: bool = False):
     """
     Perform the final sequence typing, and create the report
     :param profile_report: String of absolute path to report file
-    :param data: String of header including all gene names. To be used in creating final report
-    :param runmetadata: Metadata object containing a list of all metadata objects
+    :param data: String of header including all gene names. To be used in
+    creating final report
+    :param runmetadata: Metadata object containing a list of all
+    metadata objects
     :param profile_matches: Dictionary of seq_type: matching profile
     :param profile_data: Dictionary of seq_type: {gene name:allele ID}
-    :param update: Boolean of whether the report is to be created or updated. Default is False (created)
-    :param amino_acid: Boolean of whether the query sequences are amino acid. Default is False
+    :param update: Boolean of whether the report is to be created or updated.
+    Default is False (created)
+    :param amino_acid: Boolean of whether the query sequences are amino acid.
+    Default is False
     """
     # Open the report
     mode = 'w' if not update else 'a+'
     if not update:
-        # Initialise the header with an extra 'Sample' column plus the comma-separate list
+        # Initialise the header with an extra 'Sample' column plus the
+        # comma-separated list
         # of gene names
         data = 'Sample\t' + data
     else:
         if not os.path.isfile(profile_report):
-            # Initialise the header with an extra 'Sample' column plus the comma-separate list
-            # of gene names
+            # Initialise the header with an extra 'Sample' column plus the
+            # comma-separated list of gene names
             data = 'Sample\t' + data
         else:
             data = str()
     with open(profile_report, mode, encoding='utf-8') as report:
         for sample in runmetadata.samples:
-            # Iterate through all the matches to sequence profiles in the analysis
+            # Iterate through all the matches to sequence profiles in
+            # the analysis
             for seq_type, sample_names in profile_matches.items():
-                # Check if the sample name is in the list of samples names with the current
-                # sequence type
+                # Check if the sample name is in the list of samples names
+                # with the current sequence type
                 if sample.name in sample_names:
-                    # Add the sample name, sequence type, and all the allele numbers to the
+                    # Add the sample name, sequence type, and all the allele
+                    # numbers to the
                     # report string
-                    complement = '\t'.join(allele_num.split('_')[-1] for gene, allele_num in sorted(
-                        profile_data[seq_type].items())
+                    complement = '\t'.join(
+                        allele_num.split('_')[-1] for _, allele_num in sorted(
+                            profile_data[seq_type].items())
                     )
-                    data += f'{sample.name}\t{seq_type}\t{complement.rstrip()}\n'
-                    # Update the appropriate GenObject based on the current molecule
-                    # (DNA or amino acid)
+                    data += \
+                        f'{sample.name}\t{seq_type}\t{complement.rstrip()}\n'
+                    # Update the appropriate GenObject based on the current
+                    # molecule (DNA or amino acid)
                     if not amino_acid:
                         sample.alleles.nt_st = seq_type
                         sample.alleles.nt_profile = profile_data[seq_type]
                     else:
                         sample.alleles.aa_st = seq_type
                         sample.alleles.aa_profile = profile_data[seq_type]
         # Write the report
         report.write(data)
     return runmetadata
 
 
-def append_profiles(new_profiles, profile_file, data, novel_profiles=False, profile_path=None, gene_names=None):
+def append_profiles(
+        new_profiles: list,
+        profile_file: str,
+        data: str,
+        novel_profiles: bool = False,
+        profile_path: str = None,
+        gene_names: str = None):
     """
     Add new profiles to the profile file
     :param new_profiles: List of all novel profiles in this analysis
     :param profile_file: Name and absolute path to a profile file
-    :param data: String of header including all gene names. To be used in creating final report
-    :param novel_profiles: Boolean of whether the novel_profiles.txt file is to be populated. Default is False
-    :param profile_path: String of absolute path of folder in which profiles are located
+    :param data: String of header including all gene names. To be used in
+    creating final report
+    :param novel_profiles: Boolean of whether the novel_profiles.txt file is
+    to be populated. Default is False
+    :param profile_path: String of absolute path of folder in which profiles
+    are located
     :param gene_names: List of all genes in the analysis
     """
     # Only try to add new profiles if there are new profiles in the analysis
     if new_profiles:
         # Initialise the string to store the new profile
         new_data = str()
-        # If the profile file does not exist, add the string of 'ST', comma-separated gene names
-        # to the headers
+        # If the profile file does not exist, add the string of 'ST',
+        # comma-separated gene names to the headers
         if not os.path.isfile(profile_file):
             new_data = data
-        # Iterate through all the new profiles, and add them to the new profile string
+        # Iterate through all the new profiles, and add them to the new
+        # profile string
         for profile in new_profiles:
             new_data += f'{profile}\n'
-        # Open the report with a+ to either create, or append the profile string to it
+        # Open the report with a+ to either create, or append the profile
+        # string to it
         with open(profile_file, 'a+', encoding='utf-8') as profile:
             profile.write(new_data)
         if novel_profiles:
-            novel_profile_file = os.path.join(profile_path, 'novel_profiles.txt')
+            novel_profile_file = os.path.join(
+                profile_path,
+                'novel_profiles.txt'
+            )
             if not os.path.isfile(novel_profile_file):
                 with open(novel_profile_file, 'w', encoding='utf-8') as novel:
-                    novel.write('ST\t{names}\n'.format(names='\t'.join(gene_names)))
+                    novel.write(
+                        'ST\t{names}\n'.format(names='\t'.join(gene_names))
+                    )
             with open(novel_profile_file, 'a+', encoding='utf-8') as novel:
                 novel.write(new_data)
```

### Comparing `AlleleFinder-0.1.6/allele_tools/stec.py` & `allelefinder-0.1.7/allele_tools/stec.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 )
 from allele_tools.allele_translate_reduce import Translate
 from allele_tools.profile_reduce import ProfileReduce
 from allele_tools.version import __version__
 from allele_tools.methods import (
     analyse_aa_alleles,
     blast_alleles,
+    blastx_alleles,
     common_allele_find_errors,
     concatenate_alleles,
     create_aa_allele_comprehension,
     create_frozen_allele_comprehension,
     create_gene_names,
     create_nt_allele_comprehension,
     create_stec_report,
@@ -47,14 +48,15 @@
     parse_colocated_results,
     pathfinder,
     profile_allele_check,
     query_prep,
     report_aa_alleles,
     setup_arguments,
     split_alleles,
+    translated_update_nucleotide,
     write_concatenated_sequences
 )
 
 __author__ = 'adamkoziol'
 
 
 class STEC:
@@ -80,23 +82,25 @@
                     combined_targets=self.combined_targets,
                     amino_acid=self.amino_acid
                 )
             gene_names = sorted(gene_names)
             logging.info('Loading profile')
             nt_profile_data = read_profile(profile_file=self.nt_profile_file)
             aa_profile_data = read_profile(profile_file=self.aa_profile_file)
-            # Extract the sequence type and allele dictionary from the profile file
+            # Extract the sequence type and allele dictionary from the
+            # profile file
             blast_alleles(
                 runmetadata=sample,
                 amino_acid=self.amino_acid,
                 combined_targets=self.combined_targets,
                 cpus=self.cpus,
                 outfmt=self.outfmt
             )
-            # Add the header to the BLAST outputs, and filter results based on cutoff
+            # Add the header to the BLAST outputs, and filter results based
+            # on cutoff
             parseable_blast_outputs(
                 runmetadata=sample,
                 fieldnames=self.fieldnames,
                 extended_fieldnames=self.extended_fieldnames,
                 records=records,
                 cutoff=90
             )
@@ -112,27 +116,30 @@
                 report_path=self.report_path
             )
             # Create nucleotide allele comprehensions from the BLAST outputs
             nt_allele_comprehension = create_nt_allele_comprehension(
                 runmetadata=sample,
                 gene_names=gene_names
             )
-            # Create an amino acid allele comprehensions from the translated BLAST outputs
+            # Create an amino acid allele comprehensions from the translated
+            # BLAST outputs
             aa_allele_comprehension = create_aa_allele_comprehension(
                 runmetadata=sample,
                 gene_names=gene_names,
             )
             # Freeze the nucleotide allele comprehension
-            nt_frozen_allele_comprehension = create_frozen_allele_comprehension(
-                allele_comprehension=nt_allele_comprehension
-            )
+            nt_frozen_allele_comprehension = \
+                create_frozen_allele_comprehension(
+                    allele_comprehension=nt_allele_comprehension
+                )
             # Freeze the amino acid allele comprehension
-            aa_frozen_allele_comprehension = create_frozen_allele_comprehension(
-                allele_comprehension=aa_allele_comprehension
-            )
+            aa_frozen_allele_comprehension = \
+                create_frozen_allele_comprehension(
+                    allele_comprehension=aa_allele_comprehension
+                )
             # Find nucleotide profile matches
             nt_profile_matches, nt_frozen_profiles = match_profile(
                 profile_data=nt_profile_data,
                 frozen_allele_comprehension=nt_frozen_allele_comprehension,
                 report_path=self.report_path,
                 profile_file=self.nt_profile_file,
                 genes=gene_names,
@@ -158,52 +165,325 @@
                 aa_alleles=aa_allele_comprehension,
                 report_file=self.report_file,
                 gene_names=gene_names,
                 aa_profile_path=self.aa_profile_path,
                 notes=notes
             )
 
-    def __init__(self, allele_path, aa_allele_path, profile_file, aa_profile_file, query_path, report_path,
-                 amino_acid=False):
+    def __init__(
+        self,
+        allele_path: str,
+        aa_allele_path: str,
+        profile_file: str,
+        aa_profile_file: str,
+        query_path: str,
+        report_path: str,
+            amino_acid: bool = False):
+        """
+        Constructs all the necessary attributes for the STEC object.
 
+        Args:
+            allele_path (str): Path to the nucleotide allele file.
+            aa_allele_path (str): Path to the amino acid allele file.
+            profile_file (str): Path to the nucleotide profile file.
+            aa_profile_file (str): Path to the amino acid profile file.
+            query_path (str): Path to the query file.
+            report_path (str): Path to the report directory.
+            amino_acid (bool, optional): Flag to indicate if the process is
+            for amino acids. Defaults to False.
+        """
+        # Set paths for allele and profile files
         self.nt_allele_path = pathfinder(path=allele_path)
         self.aa_allele_path = pathfinder(path=aa_allele_path)
         self.nt_profile_file = pathfinder(path=profile_file)
         self.aa_profile_file = pathfinder(path=aa_profile_file)
+
+        # Set paths for profile directories
         self.profile_path = os.path.dirname(self.nt_profile_file)
         self.aa_profile_path = os.path.dirname(self.aa_profile_file)
+
+        # Set paths for query and report files
         self.query_path = pathfinder(path=query_path)
         self.report_path = pathfinder(path=report_path)
         self.aa_report_path = self.report_path
+
+        # Create report directory if it doesn't exist
         make_path(inpath=self.report_path)
+
+        # Remove any existing fasta files in the report directory
         novel_alleles = glob(os.path.join(self.report_path, '*.fasta'))
         for novel_allele in novel_alleles:
             os.remove(novel_allele)
 
+        # Set amino acid flag and combined targets path
         self.amino_acid = amino_acid
         if not self.amino_acid:
-            self.combined_targets = os.path.join(self.nt_allele_path, 'combinedtargets.fasta')
+            self.combined_targets = os.path.join(
+                self.nt_allele_path, 'combinedtargets.fasta')
         else:
-            self.combined_targets = os.path.join(self.aa_allele_path, 'combinedtargets.fasta')
+            self.combined_targets = os.path.join(
+                self.aa_allele_path, 'combinedtargets.fasta')
+
+        # Initialize gene names and metadata
+        self.gene_names = []
+        self.runmetadata = MetadataObject()
+        self.runmetadata.samples = []
+
+        # Set number of CPUs for multiprocessing
+        self.cpus = multiprocessing.cpu_count() - 1
+
+        # Set paths for profile report files
+        self.profile_report = os.path.join(
+            self.report_path, 'nt_profiles.tsv')
+        self.aa_profile_report = os.path.join(
+            self.aa_report_path, 'aa_profiles.tsv')
+
+        # Remove existing profile report file if it exists
+        try:
+            os.remove(self.profile_report)
+        except FileNotFoundError:
+            pass
+
+        # Set path for report file and remove any existing tsv files in the
+        # report directory
+        self.report_file = os.path.join(self.report_path, 'stec_report.tsv')
+        reports = glob(os.path.join(self.report_path, '*.tsv'))
+        for report in reports:
+            os.remove(report)
+
+        # Set field names for BLAST output
+        self.fieldnames = [
+            'query_id',
+            'subject_id',
+            'identical',
+            'mismatches',
+            'gaps',
+            'evalue',
+            'bit_score',
+            'query_length',
+            'subject_length',
+            'alignment_length',
+            'query_start',
+            'query_end',
+            'subject_start',
+            'subject_end',
+            'query_sequence',
+            'subject_sequence'
+        ]
+        self.extended_fieldnames = self.fieldnames.copy()
+        self.extended_fieldnames.insert(14, 'percent_match')
+
+        # Set format string for BLAST output
+        self.outfmt = (
+            '6 qseqid sseqid nident mismatch gaps evalue bitscore qlen slen '
+            'length qstart qend sstart send qseq sseq'
+        )
+
+        # Initialize string for header formatting and dictionaries for alleles
+        self.data = str()
+        self.aa_allele_dict = {}
+        self.aa_nt_allele_link_dict = {}
+
+
+class STECTranslate:
+    """
+    Find alleles in genomes against an amino acid database
+    """
+
+    def main(self):
+        """
+        Run the necessary methods in the correct order
+        """
+        self.runmetadata = query_prep(
+            query_path=self.query_path,
+            runmetadata=self.runmetadata,
+            clear_report=True
+        )
+        for sample in self.runmetadata.samples:
+            logging.debug('Processing sample %s', sample.name)
+            notes = {}
+            records, gene_names, self.data = \
+                allele_prep(
+                    allele_path=self.aa_allele_path,
+                    gene_names=self.gene_names,
+                    combined_targets=self.combined_targets,
+                    amino_acid=True
+                )
+            gene_names = sorted(gene_names)
+            logging.info('Loading profile')
+            nt_profile_data = read_profile(profile_file=self.nt_profile_file)
+            aa_profile_data = read_profile(profile_file=self.aa_profile_file)
+            if not os.path.isfile(sample.alleles.blast_report):
+                # BLAST the query against the allele database
+                blastx_alleles(
+                    runmetadata=sample,
+                    combined_targets=self.combined_targets,
+                    cpus=self.cpus,
+                    outfmt=self.outfmt
+                )
+                # Add headers to the BLAST outputs, and filter based on
+                # cutoff value
+                parseable_blast_outputs(
+                    runmetadata=sample,
+                    fieldnames=self.fieldnames,
+                    extended_fieldnames=self.extended_fieldnames,
+                    records=records,
+                    cutoff=95
+                )
+                # Parse the amino acid BLAST results
+                sample, filtered, notes = parse_aa_blast(
+                    runmetadata=sample,
+                    extended_fieldnames=self.extended_fieldnames,
+                    fieldnames=self.fieldnames,
+                    gene_names=gene_names,
+                    notes=notes,
+                    aa_allele_path=self.aa_allele_path,
+                    report_path=self.report_path,
+                    cutoff=95
+                )
+                # Update the nucleotide database as required
+                sample, notes = translated_update_nucleotide(
+                    runmetadata=sample,
+                    nt_allele_path=self.nt_allele_path,
+                    report_path=self.report_path,
+                    notes=notes,
+                    gene_names=self.gene_names,
+                    filtered=filtered
+                )
+                # Create nucleotide allele comprehensions from the
+                # BLAST outputs
+                nt_allele_comprehension = create_nt_allele_comprehension(
+                    runmetadata=sample,
+                    gene_names=gene_names,
+                    translated=True
+                )
+                # Create an amino acid allele comprehensions from the
+                # translated BLAST outputs
+                aa_allele_comprehension = create_aa_allele_comprehension(
+                    runmetadata=sample,
+                    gene_names=gene_names,
+                )
+                # Freeze the nucleotide allele comprehension
+                nt_frozen_allele_comprehension = \
+                    create_frozen_allele_comprehension(
+                        allele_comprehension=nt_allele_comprehension
+                    )
+                # Freeze the amino acid allele comprehension
+                aa_frozen_allele_comprehension = \
+                    create_frozen_allele_comprehension(
+                        allele_comprehension=aa_allele_comprehension
+                    )
+                # Find nucleotide profile matches
+                nt_profile_matches, nt_frozen_profiles = match_profile(
+                    profile_data=nt_profile_data,
+                    frozen_allele_comprehension=nt_frozen_allele_comprehension,
+                    report_path=self.report_path,
+                    profile_file=self.nt_profile_file,
+                    genes=gene_names,
+                    allele_comprehension=nt_allele_comprehension,
+                    molecule='nt'
+                )
+                # Find amino acid profile matches
+                aa_profile_matches, aa_frozen_profiles = match_profile(
+                    profile_data=aa_profile_data,
+                    frozen_allele_comprehension=aa_frozen_allele_comprehension,
+                    report_path=self.report_path,
+                    profile_file=self.aa_profile_file,
+                    genes=gene_names,
+                    allele_comprehension=aa_allele_comprehension,
+                    molecule='aa'
+                )
+                # Create the STEC-specific report
+                create_stec_report(
+                    runmetadata=sample,
+                    nt_profile_matches=nt_profile_matches,
+                    nt_alleles=nt_allele_comprehension,
+                    aa_profile_matches=aa_profile_matches,
+                    aa_alleles=aa_allele_comprehension,
+                    report_file=self.report_file,
+                    gene_names=gene_names,
+                    aa_profile_path=self.aa_profile_path,
+                    notes=notes
+                )
+
+    def __init__(
+            self,
+            allele_path: str,
+            aa_allele_path: str,
+            profile_file: str,
+            aa_profile_file: str,
+            query_path: str,
+            report_path: str):
+        """
+        Constructs all the necessary attributes for the STECTranslate object.
+
+        Parameters:
+        allele_path (str): Path to the allele file
+        aa_allele_path (str): Path to the amino acid allele file
+        profile_file (str): Path to the profile file
+        aa_profile_file (str): Path to the amino acid profile file
+        query_path (str): Path to the query file
+        report_path (str): Path to the report file
+        """
+
+        # Set paths for allele and profile files
+        self.nt_allele_path = pathfinder(path=allele_path)
+        self.aa_allele_path = pathfinder(path=aa_allele_path)
+        self.nt_profile_file = pathfinder(path=profile_file)
+        self.aa_profile_file = pathfinder(path=aa_profile_file)
+
+        # Set paths for profile directories
+        self.profile_path = os.path.dirname(self.nt_profile_file)
+        self.aa_profile_path = os.path.dirname(self.aa_profile_file)
+
+        # Set paths for query and report files
+        self.query_path = pathfinder(path=query_path)
+        self.report_path = pathfinder(path=report_path)
+        self.aa_report_path = self.report_path
+
+        # Create report directory if it doesn't exist
+        make_path(inpath=self.report_path)
+
+        # Remove any existing fasta files in the report directory
+        novel_alleles = glob(os.path.join(self.report_path, '*.fasta'))
+        for novel_allele in novel_alleles:
+            os.remove(novel_allele)
+
+        # Set combined targets path
+        self.combined_targets = os.path.join(
+            self.aa_allele_path, 'combinedtargets.fasta')
+
+        # Initialize gene names and metadata
         self.gene_names = []
         self.runmetadata = MetadataObject()
         self.runmetadata.samples = []
+
+        # Set number of CPUs for multiprocessing
         self.cpus = multiprocessing.cpu_count() - 1
-        self.profile_report = os.path.join(self.report_path, 'nt_profiles.tsv')
-        self.aa_profile_report = os.path.join(self.aa_report_path, 'aa_profiles.tsv')
+
+        # Set paths for profile report files
+        self.profile_report = os.path.join(
+            self.report_path, 'nt_profiles.tsv')
+        self.aa_profile_report = os.path.join(
+            self.aa_report_path, 'aa_profiles.tsv')
+
+        # Remove existing profile report file if it exists
         try:
             os.remove(self.profile_report)
         except FileNotFoundError:
             pass
 
+        # Set path for report file and remove any existing tsv files in the
+        # report directory
         self.report_file = os.path.join(self.report_path, 'stec_report.tsv')
         reports = glob(os.path.join(self.report_path, '*.tsv'))
         for report in reports:
             os.remove(report)
-        # Fields used for custom outfmt 6 BLAST output:
+
+        # Set field names for BLAST output
         self.fieldnames = [
             'query_id',
             'subject_id',
             'identical',
             'mismatches',
             'gaps',
             'evalue',
@@ -216,17 +496,22 @@
             'subject_start',
             'subject_end',
             'query_sequence',
             'subject_sequence'
         ]
         self.extended_fieldnames = self.fieldnames.copy()
         self.extended_fieldnames.insert(14, 'percent_match')
-        self.outfmt = '6 qseqid sseqid nident mismatch gaps evalue bitscore qlen slen length ' \
-                      'qstart qend sstart send qseq sseq'
-        # A string of the header to use for formatting the profile file, and the report headers
+
+        # Set format string for BLAST output
+        self.outfmt = (
+            '6 qseqid sseqid nident mismatch gaps evalue bitscore qlen slen '
+            'length qstart qend sstart send qseq sseq'
+        )
+
+        # Initialize string for header formatting and dictionaries for alleles
         self.data = str()
         self.aa_allele_dict = {}
         self.aa_nt_allele_link_dict = {}
 
 
 class AASTEC:
 
@@ -239,15 +524,15 @@
             query_path=self.query_path,
             runmetadata=self.runmetadata,
             clear_report=True
         )
 
         for sample in self.runmetadata.samples:
             logging.debug('Processing sample %s', sample.name)
-            notes = []
+            notes = {}
             records, gene_names, self.data = \
                 allele_prep(
                     allele_path=self.aa_allele_path,
                     gene_names=self.gene_names,
                     combined_targets=self.combined_targets,
                     amino_acid=self.amino_acid
                 )
@@ -258,15 +543,16 @@
                 blast_alleles(
                     runmetadata=sample,
                     amino_acid=self.amino_acid,
                     combined_targets=self.combined_targets,
                     cpus=self.cpus,
                     outfmt=self.outfmt
                 )
-                # Add headers to the BLAST outputs, and filter based on cutoff value
+                # Add headers to the BLAST outputs, and filter based on
+                # cutoff value
                 parseable_blast_outputs(
                     runmetadata=sample,
                     fieldnames=self.fieldnames,
                     extended_fieldnames=self.extended_fieldnames,
                     records=records,
                     cutoff=self.cutoff
                 )
@@ -289,37 +575,70 @@
             # Create an amino acid query report
             report_aa_alleles(
                 runmetadata=sample,
                 report_file=self.report_file,
                 notes=notes
             )
 
-    def __init__(self, aa_allele_path, query_path, report_path, cutoff, amino_acid=True):
+    def __init__(
+            self,
+            aa_allele_path: str,
+            query_path: str,
+            report_path: str,
+            cutoff: float,
+            amino_acid: bool = True):
+        """
+        Constructs all the necessary attributes for the AASTEC object.
 
+        Parameters:
+        aa_allele_path (str): Path to the amino acid allele file
+        query_path (str): Path to the query file
+        report_path (str): Path to the report file
+        cutoff (float): Cutoff value for the process
+        amino_acid (bool): Flag to indicate if the process involves amino acids
+        """
+
+        # Set paths for allele, query, and report files
         self.aa_allele_path = pathfinder(path=aa_allele_path)
         self.query_path = pathfinder(path=query_path)
         self.report_path = pathfinder(path=report_path)
         self.aa_report_path = self.report_path
+
+        # Create report directory if it doesn't exist
         make_path(inpath=self.report_path)
+
+        # Remove any existing fasta files in the report directory
         novel_alleles = glob(os.path.join(self.report_path, '*.fasta'))
         for novel_allele in novel_alleles:
             os.remove(novel_allele)
+
+        # Set cutoff and amino acid flag
         self.cutoff = cutoff
         self.amino_acid = amino_acid
-        self.combined_targets = os.path.join(self.aa_allele_path, 'combinedtargets.fasta')
+
+        # Set combined targets path
+        self.combined_targets = os.path.join(
+            self.aa_allele_path, 'combinedtargets.fasta')
+
+        # Initialize gene names and metadata
         self.gene_names = []
         self.runmetadata = MetadataObject()
         self.runmetadata.samples = []
+
+        # Set number of CPUs for multiprocessing
         self.cpus = multiprocessing.cpu_count() - 1
+
+        # Set path for report file and remove it if it exists
         self.report_file = os.path.join(self.report_path, 'allele_report.tsv')
         try:
             os.remove(self.report_file)
         except FileNotFoundError:
             pass
-        # Fields used for custom outfmt 6 BLAST output:
+
+        # Set field names for BLAST output
         self.fieldnames = [
             'query_id',
             'subject_id',
             'identical',
             'mismatches',
             'gaps',
             'evalue',
@@ -332,24 +651,30 @@
             'subject_start',
             'subject_end',
             'query_sequence',
             'subject_sequence'
         ]
         self.extended_fieldnames = self.fieldnames.copy()
         self.extended_fieldnames.insert(14, 'percent_match')
-        self.outfmt = '6 qseqid sseqid nident mismatch gaps evalue bitscore qlen slen length ' \
-                      'qstart qend sstart send qseq sseq'
-        # A string of the header to use for formatting the profile file, and the report headers
+
+        # Set format string for BLAST output
+        self.outfmt = (
+            '6 qseqid sseqid nident mismatch gaps evalue bitscore qlen slen '
+            'length qstart qend sstart send qseq sseq'
+        )
+
+        # Initialize string for header formatting
         self.data = str()
 
 
 class AlleleConcatenate:
 
     """
-    Concatenate stx subunits. Read in profile files. Load alleles. Concatenate alleles with appropriate linker
+    Concatenate stx subunits. Read in profile files. Load alleles. Concatenate
+    alleles with appropriate linker
     """
 
     def main(self):
         """
         Run the necessary methods for AlleleConcatenate
         """
         self.gene, self.nt_alleles = load_alleles(
@@ -389,41 +714,67 @@
             concatenate_path=self.concatenate_path,
             file_name=self.gene_allele[self.gene],
             molecule='aa'
         )
 
     def __init__(
             self,
-            nt_allele_path,
-            aa_allele_path,
-            nt_profile_file,
-            aa_profile_file,
-            concatenate_path):
+            nt_allele_path: str,
+            aa_allele_path: str,
+            nt_profile_file: str,
+            aa_profile_file: str,
+            concatenate_path: str):
+        """
+        Constructs all the necessary attributes for the AlleleConcatenate
+        object.
+
+        Parameters:
+        nt_allele_path (str): Path to the nucleotide allele file
+        aa_allele_path (str): Path to the amino acid allele file
+        nt_profile_file (str): Path to the nucleotide profile file
+        aa_profile_file (str): Path to the amino acid profile file
+        concatenate_path (str): Path to the concatenate file
+        """
+
+        # Set paths for allele and profile files
         self.nt_allele_path = pathfinder(path=nt_allele_path)
         self.aa_allele_path = pathfinder(path=aa_allele_path)
         self.nt_profile_file = pathfinder(path=nt_profile_file)
         self.aa_profile_file = pathfinder(path=aa_profile_file)
+
+        # Set paths for profile directories
         self.nt_profile_path = os.path.dirname(self.nt_profile_file)
         self.aa_profile_path = os.path.dirname(self.aa_profile_file)
+
+        # Set path for concatenate file
         self.concatenate_path = pathfinder(path=concatenate_path)
+
+        # Set linker length dictionary
         self.linker_length_dict = {
             'stx1': 9,
             'stx2': 12,
         }
-        # Set the appropriate order for the genes in the report (stx1 genes are not in numerical order)
+
+        # Set the appropriate order for the genes in the report
         self.allele_order = {
-            'stx1': ['ECs2974', 'ECs2973'],
-            'stx2': ['ECs1205', 'ECs1206']
+            'stx1': ['stx1A', 'stx1B'],
+            'stx2': ['stx2A', 'stx2B']
         }
+
+        # Set gene allele dictionary
         self.gene_allele = {
-            'stx1': 'ECs2974_ECs2973',
-            'stx2': 'ECs1205_ECs1206'
+            'stx1': 'stx1A_stx1B',
+            'stx2': 'stx2A_stx2B'
         }
+
+        # Read profile data
         self.nt_profile_data = read_profile(profile_file=self.nt_profile_file)
         self.aa_profile_data = read_profile(profile_file=self.aa_profile_file)
+
+        # Initialize gene, alleles, and concatenated sequences
         self.gene = str()
         self.nt_alleles = {}
         self.aa_alleles = {}
         self.concatenated_nt_seq = []
         self.concatenated_aa_seq = []
 
 
@@ -437,36 +788,36 @@
     genes_file = os.path.basename(args.gene_names)
     logging.info(genes_path)
     logging.info(genes_file)
     if not os.path.isfile(args.gene_names):
         # Ensure that the path exists
         if not os.path.isdir(genes_path):
             logging.error(
-                'Could not locate the supplied path, %s, for the gene file. Please ensure that it'
-                ' exists, and that it either contains the gene file, or files with '
-                '.fasta extensions',
+                'Could not locate the supplied path, %s, for the gene file. '
+                'Please ensure that it exists, and that it either contains '
+                'the gene file, or files with .fasta extensions',
                 genes_path
             )
             raise SystemExit
         logging.warning(
-            'Could not locate the supplied gene file: %s. Will now attempt to create it in '
-            'directory %s',
+            'Could not locate the supplied gene file: %s. Will now attempt to '
+            'create it in directory %s',
             args.gene_names, genes_path
-            )
+        )
         # Attempt to create the file
         create_gene_names(
             path=genes_path,
             name=genes_file
         )
     else:
         # Ensure that the file isn't empty
         if os.stat(args.gene_names).st_size == 0:
             logging.warning(
-                'The supplied gene file, %s, is empty. Will now attempt to populate it in '
-                'directory %s',
+                'The supplied gene file, %s, is empty. Will now attempt to '
+                'populate it in directory %s',
                 args.gene_names, genes_path
             )
             # Attempt to repopulate the file
             create_gene_names(
                 path=genes_path,
                 name=genes_file
             )
@@ -487,25 +838,22 @@
 def translate_reduce(args):
     """
     Translate nucleotide alleles to amino acid, and remove duplicates
     :param args: type ArgumentParser arguments
     """
     log_str = f'Translating and reducing alleles in: {args.allele_path}'
     if args.profile_file:
-        log_str += f'. Parsing {args.profile_file} nucleotide profile to create corresponding,'\
-                    ' reduced amino acid profile'
+        log_str += \
+            f'. Parsing {args.profile_file} nucleotide profile to create ' \
+            f'corresponding, reduced amino acid profile'
     logging.info(log_str)
     length_dict = {
-        'ECs2973': 82,
         'stx1B': 82,
-        'ECs2974': 313,
         'stx1A': 313,
-        'ECs1205': 313,
         'stx2A': 313,
-        'ECs1206': 84,
         'stx2B': 84
     }
     allele_translate_reduce = Translate(
         path=args.allele_path,
         profile=args.profile_file,
         report_path=args.report_path,
         translated_path=args.translated_path,
@@ -516,56 +864,111 @@
 
 
 def allele_find(args):
     """
     Perform allele discovery analyses
     :param args: type ArgumentParser arguments
     """
-    log_str = f'Performing STEC allele discovery on sequences in {args.query_path} using ' \
-        f'nucleotide alleles in {args.nt_alleles}, nucleotide profile in {args.nt_profile}, amino' \
-        f' acid alleles in {args.aa_alleles}, and amino acid profile in {args.aa_profile}'
+    log_str = \
+        f'Performing STEC allele discovery on sequences in {args.query_path}' \
+        f' using nucleotide alleles in {args.nt_alleles}, nucleotide profile' \
+        f' in {args.nt_profile}, amino acid alleles in {args.aa_alleles}, ' \
+        f'and amino acid profile in {args.aa_profile}'
     logging.info(log_str)
     errors = []
 
     # Nucleotide allele checks
     if not os.path.isdir(args.nt_alleles):
-        errors.append(f'Could not find supplied nucleotide allele folder: {args.nt_alleles}')
+        errors.append(
+            f'Could not find supplied nucleotide allele folder: '
+            f'{args.nt_alleles}'
+        )
     else:
         if not glob(os.path.join(args.nt_alleles, '*.fasta')):
             errors.append(
-                f'Could not locate sequence files in supplied nucleotide allele folder: {args.nt_alleles}'
+                f'Could not locate sequence files in supplied nucleotide '
+                f'allele folder: {args.nt_alleles}'
             )
     # Find errors for amino acid and query checks
     errors = common_allele_find_errors(
         args=args,
         errors=errors,
         amino_acid=False
     )
     if not os.path.isfile(args.nt_profile):
-        errors.append(f'Could not locate supplied nucleotide profile file: {args.nt_profile}')
+        errors.append(
+            f'Could not locate supplied nucleotide profile file: '
+            f'{args.nt_profile}'
+        )
     if errors:
         error_print(errors=errors)
     stec = STEC(
         allele_path=args.nt_alleles,
         aa_allele_path=args.aa_alleles,
         profile_file=args.nt_profile,
         aa_profile_file=args.aa_profile,
         query_path=args.query_path,
         report_path=args.report_path
     )
     stec.main()
 
 
+def allele_translate_find(args):
+    """
+    Perform allele discovery analyses. Queries nucleotide sequences against
+    amino acid alleles
+    :param args: type ArgumentParser arguments
+    """
+    log_str = \
+        f'Performing STEC allele discovery on sequences in {args.query_path}' \
+        f' using amino acid alleles in {args.aa_alleles}, and amino acid ' \
+        f'profile in {args.aa_profile}'
+    logging.info(log_str)
+    errors = []
+
+    # Nucleotide allele checks
+    if not os.path.isdir(args.nt_alleles):
+        os.makedirs(args.nt_alleles)
+    else:
+        if not glob(os.path.join(args.nt_alleles, '*.fasta')):
+            # Create the necessary allele files
+            for gene in ['stx1.fasta', 'stx2.fasta']:
+                open(os.path.join(args.nt_alleles, gene), 'a').close()
+    # Find errors for amino acid and query checks
+    errors = common_allele_find_errors(
+        args=args,
+        errors=errors,
+        amino_acid=False
+    )
+    if not os.path.isfile(args.nt_profile):
+        # Create the folder if required
+        os.makedirs(os.path.dirname(args.nt_profile), exist_ok=True)
+        # Create the empty profile file
+        open(args.nt_profile, 'a').close()
+    if errors:
+        error_print(errors=errors)
+    stec = STECTranslate(
+        allele_path=args.nt_alleles,
+        aa_allele_path=args.aa_alleles,
+        profile_file=args.nt_profile,
+        aa_profile_file=args.aa_profile,
+        query_path=args.query_path,
+        report_path=args.report_path
+    )
+    stec.main()
+
+
 def aa_allele_find(args):
     """
     Perform allele discovery analyses on amino acid query files
     :param args: type ArgumentParser arguments
     """
-    log_str = f'Performing STEC allele discovery on amino acid sequences in {args.query_path} using amino' \
-              f' acid alleles in {args.aa_alleles}'
+    log_str = \
+        f'Performing STEC allele discovery on amino acid sequences in ' \
+        f'{args.query_path} using amino acid alleles in {args.aa_alleles}'
     logging.info(log_str)
     errors = []
     # Find errors for amino acid and query checks
     errors = common_allele_find_errors(
         args=args,
         errors=errors,
         amino_acid=True
@@ -582,46 +985,55 @@
 
 
 def allele_split(args):
     """
     Split files containing multiple alleles into individual files
     :param args: type ArgumentParser arguments
     """
-    logging.info('Splitting allele files in %s into individual files', args.query_path)
+    logging.info(
+        'Splitting allele files in %s into individual files', args.query_path
+    )
     errors = []
     allele_files = glob(os.path.join(args.query_path, '*.fasta'))
     # Query checks
     if not os.path.isdir(args.query_path):
-        errors.append(f'Could not find supplied nucleotide allele folder: {args.query_path}')
+        errors.append(
+            f'Could not find supplied nucleotide allele folder: '
+            f'{args.query_path}'
+        )
     else:
         if not allele_files:
             errors.append(
-                f'Could not locate sequence files in supplied allele folder: {args.query_path}'
+                f'Could not locate sequence files in supplied allele folder: '
+                f'{args.query_path}'
             )
     if errors:
         error_print(errors=errors)
     split_alleles(
         allele_files=allele_files,
         output_path=args.output_path
     )
 
 
 def allele_concatenate(args):
     """
-    Concatenate subunit files with linkers. Provide linkages between nucleotide and amino acid files
+    Concatenate subunit files with linkers. Provide linkages between
+    nucleotide and amino acid files
     :param args: type ArgumentParser arguments
     """
     logging.info('Concatenating allele subunits')
     errors = []
-    # Determine if the profile file, the allele folder, and the alleles all exist
+    # Determine if the profile file, the allele folder, and the alleles
+    # all exist
     errors = profile_allele_check(
         args=args,
         errors=errors
     )
-    # If there were any errors with the supplied arguments, print them, and exit
+    # If there were any errors with the supplied arguments, print them,
+    # and exit
     if errors:
         error_print(errors=errors)
     concatenate = AlleleConcatenate(
         nt_allele_path=args.nt_alleles,
         aa_allele_path=args.aa_alleles,
         nt_profile_file=args.nt_profile,
         aa_profile_file=args.aa_profile,
@@ -648,247 +1060,338 @@
         version=f'%(prog)s commit {__version__}'
         )
     parent_parser.add_argument(
         '-v', '--verbosity',
         choices=['debug', 'info', 'warning', 'error', 'critical'],
         metavar='verbosity',
         default='info',
-        help='Set the logging level. Options are debug, info, warning, error, and critical. '
-             'Default is info.'
+        help='Set the logging level. Options are debug, info, warning, error, '
+        'and critical. Default is info.'
     )
     profile_reduce_subparser = subparsers.add_parser(
         parents=[parent_parser],
         name='profile_reduce',
-        description='Reduce full wgMLST profile from Enterobase using genes of interest',
+        description='Reduce full wgMLST profile from Enterobase using genes '
+        'of interest',
         formatter_class=RawTextHelpFormatter,
-        help='Reduce full wgMLST profile from Enterobase using genes of interest'
+        help='Reduce full wgMLST profile from Enterobase using genes '
+        'of interest'
     )
     profile_reduce_subparser.add_argument(
         '-p', '--profile_file',
         metavar='profile_file',
         default='profiles.list',
-        help='Specify name and path of profile file. If not provided, the default '
-             '"profiles.list" in the current working directory will be used'
+        help='Specify name and path of profile file. If not provided, the '
+        'default "profiles.list" in the current working directory will be used'
         )
     profile_reduce_subparser.add_argument(
         '-g', '--gene_names',
         metavar='gene_names',
         default='genes.txt',
-        help='Name and path of text file containing gene names to use to filter the profile file '
-             '(one per line). If not provided, the default "genes.txt" in the current working '
-             'directory will be used. If the file does not exist, the program will attempt to '
-             'create a file using the .fasta files in the current working directory'
+        help='Name and path of text file containing gene names to use to '
+        'filter the profile file (one per line). If not provided, the default '
+        '"genes.txt" in the current working directory will be used. If the '
+        'file does not exist, the program will attempt to create a file using '
+        'the .fasta files in the current working directory'
     )
     profile_reduce_subparser.add_argument(
         '-o', '--output_folder',
         metavar='output_folder',
         default='nt_profile',
-        help='Name and path of folder into which the reduced profile and notes are to be placed. '
-             'If not provided, the default "nt_profile" folder in the current working directory '
-             'will be used'
+        help='Name and path of folder into which the reduced profile and notes'
+        ' are to be placed. If not provided, the default "nt_profile" folder '
+        'in the current working directory will be used'
     )
     profile_reduce_subparser.set_defaults(func=profile_reduce)
     # Create a subparser for allele translation and reduction
     allele_translate_reduce_subparser = subparsers.add_parser(
         parents=[parent_parser],
         name='allele_translate_reduce',
-        description='Translate allele files in nucleotide format to amino acid. Remove duplicates. Keep notes',
+        description='Translate allele files in nucleotide format to amino '
+        'acid. Remove duplicates. Keep notes',
         formatter_class=RawTextHelpFormatter,
         help='Translate allele files in nucleotide format to amino acid. '
              'Remove duplicates. Keep notes'
     )
     allele_translate_reduce_subparser.add_argument(
         '-a', '--allele_path',
         metavar='allele_path',
         default=os.path.join(os.getcwd(), 'nt_alleles'),
-        help='Specify name and path of folder containing allele files. If not provided, the '
-             'nt_alleles folder in the current working directory will be used by default'
+        help='Specify name and path of folder containing allele files. '
+        'If not provided, the nt_alleles folder in the current working '
+        'directory will be used by default'
     )
     allele_translate_reduce_subparser.add_argument(
         '-p', '--profile_file',
         metavar='profile_file',
         help='Optionally specify name and path of profile file. '
-             'Parse the nucleic acid profile, and create the corresponding reduced amino acid profile'
+             'Parse the nucleic acid profile, and create the corresponding '
+             'reduced amino acid profile'
         )
     allele_translate_reduce_subparser.add_argument(
         '-r', '--report_path',
         metavar='report_path',
         default=os.path.join(os.getcwd(), 'aa_profile'),
-        help='Specify the name and path of the folder into which outputs are to be placed. If not '
-              'provided, the aa_profile folder in the current working directory will be used'
+        help='Specify the name and path of the folder into which outputs are '
+        'to be placed. If not provided, the aa_profile folder in the current '
+        'working directory will be used'
     )
     allele_translate_reduce_subparser.add_argument(
         '-t', '--translated_path',
         metavar='translated_path',
         default=os.path.join(os.getcwd(), 'aa_alleles'),
-        help='Specify the name and path of the folder into which alleles are to be placed. If not '
-              'provided, the aa_alleles folder in the current working directory will be used'
+        help='Specify the name and path of the folder into which alleles are '
+        'to be placed. If not provided, the aa_alleles folder in the current '
+        'working directory will be used'
     )
     allele_translate_reduce_subparser.set_defaults(func=translate_reduce)
     # Create a subparser for allele discovery
     allele_find_subparser = subparsers.add_parser(
         parents=[parent_parser],
         name='allele_find',
-        description='Analyse sequences to determine allele complement. Update profiles and '
-        'databases. Keep notes',
+        description='Analyse sequences to determine allele complement. '
+        'Update profiles and databases. Keep notes',
         formatter_class=RawTextHelpFormatter,
-        help='Analyse sequences to determine allele complement. Update profiles and databases. '
-        'Keep notes'
+        help='Analyse sequences to determine allele complement. Update '
+        'profiles and databases. Keep notes'
     )
     allele_find_subparser.add_argument(
         '--nt_profile',
         metavar='nt_profile',
         default=os.path.join(os.getcwd(), 'nt_profile', 'profile.txt'),
-        help='Specify name and path of nucleotide profile file. If not provided, profile.txt in '
-             'the nt_profile folder in the current working directory will be used by default'
+        help='Specify name and path of nucleotide profile file. If not '
+        'provided, profile.txt in the nt_profile folder in the current '
+        'working directory will be used by default'
     )
     allele_find_subparser.add_argument(
         '--aa_profile',
         metavar='aa_profile',
         default=os.path.join(os.getcwd(), 'aa_profile', 'profile.txt'),
-        help='Specify name and path of amino acid profile file. If not provided, profile.txt in '
-             'the aa_profile folder in the current working directory will be used by default'
+        help='Specify name and path of amino acid profile file. If not '
+        'provided, profile.txt in the aa_profile folder in the current '
+        'working directory will be used by default'
     )
     allele_find_subparser.add_argument(
         '--nt_alleles',
         metavar='nt_alleles',
         default=os.path.join(os.getcwd(), 'nt_alleles'),
-        help='Specify name and path of folder containing nucleotide alleles. If not provided, the '
-             'nt_allele folder in the current working directory will be used by default'
+        help='Specify name and path of folder containing nucleotide alleles. '
+        'If not provided, the nt_allele folder in the current working '
+        'directory will be used by default'
     )
     allele_find_subparser.add_argument(
         '--aa_alleles',
         metavar='aa_alleles',
         default=os.path.join(os.getcwd(), 'aa_alleles'),
-        help='Specify name and path of folder containing amino acid alleles. If not provided, the '
-             'aa_allele folder in the current working directory will be used by default'
+        help='Specify name and path of folder containing amino acid alleles. '
+        'If not provided, the aa_allele folder in the current working '
+        'directory will be used by default'
     )
     allele_find_subparser.add_argument(
         '-r', '--report_path',
         metavar='report_path',
         default=os.path.join(os.getcwd(), 'reports'),
-        help='Specify name and path of folder into which reports are to be placed. If not '
-             'provided, the reports folder in the current working directory will be used'
+        help='Specify name and path of folder into which reports are to be '
+        'placed. If not provided, the reports folder in the current working '
+        'directory will be used'
     )
     allele_find_subparser.add_argument(
         '-q', '--query_path',
         metavar='query_path',
         default=os.path.join(os.getcwd(), 'query'),
-        help='Specify name and path of folder containing query files in FASTA format. '
-             'If not provided, the query folder in the current working directory will be used'
+        help='Specify name and path of folder containing query files in FASTA '
+        'format. If not provided, the query folder in the current working '
+        'directory will be used'
     )
     allele_find_subparser.set_defaults(func=allele_find)
-    # Create a subparser for allele discovery
+    # Create a subparser for allele discovery using nucleotide inputs against
+    # an amino acid database
+    allele_translate_find_subparser = subparsers.add_parser(
+        parents=[parent_parser],
+        name='allele_translate_find',
+        description='Analyse nucleotide sequences against an amino acid '
+        'database to determine allele complement. Update profiles and '
+        'databases. Keep notes',
+        formatter_class=RawTextHelpFormatter,
+        help='Analyse nucleotide sequences against an amino acid database to '
+        'determine allele complement. Update profiles and databases. '
+        'Keep notes'
+    )
+    allele_translate_find_subparser.add_argument(
+        '--nt_profile',
+        metavar='nt_profile',
+        default=os.path.join(os.getcwd(), 'nt_profile', 'profile.txt'),
+        required=False,
+        help='Specify name and path of nucleotide profile file. If not '
+        'provided, profile.txt in the nt_profile folder in the current '
+        'working directory will be used by default'
+    )
+    allele_translate_find_subparser.add_argument(
+        '--aa_profile',
+        metavar='aa_profile',
+        default=os.path.join(os.getcwd(), 'aa_profile', 'profile.txt'),
+        help='Specify name and path of amino acid profile file. If not '
+        'provided, profile.txt in the aa_profile folder in the current '
+        'working directory will be used by default'
+    )
+    allele_translate_find_subparser.add_argument(
+        '--nt_alleles',
+        metavar='nt_alleles',
+        default=os.path.join(os.getcwd(), 'nt_alleles'),
+        required=False,
+        help='Specify name and path of folder containing nucleotide alleles. '
+        'If not provided, the nt_allele folder in the current working '
+        'directory will be used by default'
+    )
+    allele_translate_find_subparser.add_argument(
+        '--aa_alleles',
+        metavar='aa_alleles',
+        default=os.path.join(os.getcwd(), 'aa_alleles'),
+        help='Specify name and path of folder containing amino acid alleles. '
+        'If not provided, the aa_allele folder in the current working '
+        'directory will be used by default'
+    )
+    allele_translate_find_subparser.add_argument(
+        '-r', '--report_path',
+        metavar='report_path',
+        default=os.path.join(os.getcwd(), 'reports'),
+        help='Specify name and path of folder into which reports are to be '
+        'placed. If not provided, the reports folder in the current '
+        'working directory will be used'
+    )
+    allele_translate_find_subparser.add_argument(
+        '-q', '--query_path',
+        metavar='query_path',
+        default=os.path.join(os.getcwd(), 'query'),
+        help='Specify name and path of folder containing query files in '
+        'FASTA format.  If not provided, the query folder in the current '
+        'working directory will be used'
+    )
+    allele_translate_find_subparser.set_defaults(func=allele_translate_find)
+    # Create a subparser for allele discovery using amino acid inputs against
+    # an amino acid database
     aa_allele_find_subparser = subparsers.add_parser(
         parents=[parent_parser],
         name='aa_allele_find',
-        description='Analyse amino acid sequences to determine allele complement. Update profiles and '
-                    'databases. Keep notes',
+        description='Analyse amino acid sequences to determine allele '
+        'complement. Update profiles and databases. Keep notes',
         formatter_class=RawTextHelpFormatter,
-        help='Analyse amino acid sequences to determine allele complement. Update profiles and databases. '
-             'Keep notes'
+        help='Analyse amino acid sequences to determine allele complement. '
+        'Update profiles and databases. Keep notes'
     )
     aa_allele_find_subparser.add_argument(
         '--aa_alleles',
         metavar='aa_alleles',
         default=os.path.join(os.getcwd(), 'aa_alleles'),
-        help='Specify name and path of folder containing amino acid alleles. If not provided, the '
-             'aa_allele folder in the current working directory will be used by default'
+        help='Specify name and path of folder containing amino acid alleles. '
+        'If not provided, the aa_allele folder in the current working '
+        'directory will be used by default'
     )
     aa_allele_find_subparser.add_argument(
         '-r', '--report_path',
         metavar='report_path',
         default=os.path.join(os.getcwd(), 'reports'),
-        help='Specify name and path of folder into which reports are to be placed. If not '
-             'provided, the reports folder in the current working directory will be used'
+        help='Specify name and path of folder into which reports are to be '
+        'placed. If not provided, the reports folder in the current '
+        'working directory will be used'
     )
     aa_allele_find_subparser.add_argument(
         '-q', '--query_path',
         metavar='query_path',
         default=os.path.join(os.getcwd(), 'query'),
-        help='Specify name and path of folder containing query files in FASTA format. '
-             'If not provided, the query folder in the current working directory will be used'
+        help='Specify name and path of folder containing query files in '
+        'FASTA format. If not provided, the query folder in the current '
+        'working directory will be used'
     )
     aa_allele_find_subparser.add_argument(
         '-c', '--cutoff',
         metavar='cutoff',
         default=90,
         choices=[percent for percent in range(90, 101)],
-        help='Specify the percent identity cutoff for matches. Allowed values are between 90 and 100. Default is 100'
+        help='Specify the percent identity cutoff for matches. Allowed values '
+        'are between 90 and 100. Default is 100'
     )
     aa_allele_find_subparser.set_defaults(func=aa_allele_find)
     # Create a subparser for splitting multi-FASTA files of alleles
     allele_split_subparser = subparsers.add_parser(
         parents=[parent_parser],
         name='allele_split',
         description='Split combined allele files into individual files',
         formatter_class=RawTextHelpFormatter,
         help='Split combined allele files into individual files'
     )
     allele_split_subparser.add_argument(
         '-q', '--query_path',
         metavar='query_path',
         default=os.path.join(os.getcwd(), 'query'),
-        help='Specify name and path of folder containing query files in FASTA format. '
-             'If not provided, the query folder in the current working directory will be used'
+        help='Specify name and path of folder containing query files in '
+        'FASTA format. If not provided, the query folder in the current '
+        'working directory will be used'
     )
     allele_split_subparser.add_argument(
         '-o', '--output_path',
         metavar='output_path',
         default=os.path.join(os.getcwd(), 'split_alleles'),
-        help='Specify name and path of folder into which the split allele files are to be written. '
-             'If not provided, the split_alleles folder in the current working directory will be used'
+        help='Specify name and path of folder into which the split allele '
+        'files are to be written. If not provided, the split_alleles folder '
+        'in the current working directory will be used'
     )
     allele_split_subparser.set_defaults(func=allele_split)
     # Create a subparser for concatenating stx subunits
     allele_concatenate_subparser = subparsers.add_parser(
         parents=[parent_parser],
         name='allele_concatenate',
         description='Concatenate stx toxin subunit alleles with linkers',
         formatter_class=RawTextHelpFormatter,
         help='Concatenate stx toxin subunit alleles with linkers'
     )
     allele_concatenate_subparser.add_argument(
         '--nt_profile',
         metavar='nt_profile',
         default=os.path.join(os.getcwd(), 'nt_profile', 'profile.txt'),
-        help='Specify name and path of nucleotide profile file. If not provided, profile.txt in '
-             'the nt_profile folder in the current working directory will be used by default'
+        help='Specify name and path of nucleotide profile file. If not '
+        'provided, profile.txt in the nt_profile folder in the current '
+        'working directory will be used by default'
     )
     allele_concatenate_subparser.add_argument(
         '--aa_profile',
         metavar='aa_profile',
         default=os.path.join(os.getcwd(), 'aa_profile', 'profile.txt'),
-        help='Specify name and path of amino acid profile file. If not provided, profile.txt in '
-             'the aa_profile folder in the current working directory will be used by default'
+        help='Specify name and path of amino acid profile file. If not '
+        'provided, profile.txt in the aa_profile folder in the current '
+        'working directory will be used by default'
     )
     allele_concatenate_subparser.add_argument(
         '--nt_alleles',
         metavar='nt_alleles',
         default=os.path.join(os.getcwd(), 'nt_alleles'),
-        help='Specify name and path of folder containing nucleotide alleles. If not provided, the '
-             'nt_allele folder in the current working directory will be used by default'
+        help='Specify name and path of folder containing nucleotide alleles. '
+        'If not provided, the nt_allele folder in the current working '
+        'directory will be used by default'
     )
     allele_concatenate_subparser.add_argument(
         '--aa_alleles',
         metavar='aa_alleles',
         default=os.path.join(os.getcwd(), 'aa_alleles'),
-        help='Specify name and path of folder containing amino acid alleles. If not provided, the '
-             'aa_allele folder in the current working directory will be used by default'
+        help='Specify name and path of folder containing amino acid alleles. '
+        'If not provided, the aa_allele folder in the current working '
+        'directory will be used by default'
     )
     allele_concatenate_subparser.add_argument(
         '-c', '--concatenate_path',
         metavar='concatenate_path',
         default=os.path.join(os.getcwd(), 'concatenated_alleles'),
-        help='Specify name and path of folder into which concatenated subunit files are to be placed. If not '
-             'provided, the concatenated_alleles folder in the current working directory will be used'
+        help='Specify name and path of folder into which concatenated subunit '
+        'files are to be placed. If not provided, the concatenated_alleles '
+        'folder in the current working directory will be used'
     )
     allele_concatenate_subparser.set_defaults(func=allele_concatenate)
     # Get the arguments into an object
     arguments = setup_arguments(parser=parser)
-    # Prevent the arguments being printed to the console (they are returned in order for the tests to work)
+    # Prevent the arguments being printed to the console (they are returned in
+    # order for the tests to work)
     sys.stderr = open(os.devnull, 'w', encoding='utf-8')
     return arguments
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `AlleleFinder-0.1.6/allele_tools/profile_reduce.py` & `allelefinder-0.1.7/allele_tools/profile_reduce.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 Reduce Enterobase wgMLST profiles with a supplied list of genes
 """
 
 # Standard imports
 from argparse import ArgumentParser
 from csv import DictReader
 import logging
-import sys
 import os
+import sys
+
 
 # Third-party imports
-from olctools.accessoryFunctions.accessoryFunctions import \
-    make_path, \
+from olctools.accessoryFunctions.accessoryFunctions import (
+    make_path,
     SetupLogging
+)
 from allele_tools.methods import pathfinder
 
 
 class ProfileReduce:
 
     """
     Reduce Enterobase wgMLST profiles
@@ -34,120 +36,164 @@
     def read_names(self):
         """
         Read in all the names of the genes of interest
         """
         logging.info('Reading names file')
         with open(self.name_file, 'r', encoding='utf-8') as names:
             self.names = sorted([name.rstrip() for name in names.readlines()])
-        logging.debug('Genes used to reduce profile are: %s', '\t'.join(self.names))
+        logging.debug(
+            'Genes used to reduce profile are: %s', '\t'.join(self.names)
+        )
 
     def read_profile(self):
         """
         Load, parse, and reduce the profile information
         """
         logging.info('Reducing profiles')
         with open(self.profile, 'r', encoding='utf-8') as profile:
             with open(self.reduced_profile, 'w', encoding='utf-8') as reduced:
                 with open(self.notes_file, 'w', encoding='utf-8') as notes:
                     # Write the header for the notes field
-                    notes.write('OriginalSequenceType\tReducedSequenceType\tNotes\n')
+                    notes.write(
+                        'OriginalSequenceType\tReducedSequenceType\tNotes\n'
+                    )
                     # Create the header for the reduced profile
                     gene_names = '\t'.join(self.names)
                     reduced_data = f'ST\t{gene_names}\n'
                     logging.info('Loading profile into memory')
                     # Use to DictReader to load the profile file
                     profile_dict = DictReader(profile, dialect='excel-tab')
-                    # Initialise a dictionary to store the string of allele numbers: sequence type
+                    # Initialise a dictionary to store the string of allele
+                    # numbers: sequence type
                     profile_st = {}
                     logging.info('Parsing profile')
                     # Iterate through all the sequence types in the profile
                     for allele_dict in profile_dict:
                         # Extract the sequence type from the 'ST' column
                         seq_type = allele_dict['ST']
-                        # Initialise variables to store the allele numbering information
+                        # Initialise variables to store the allele
+                        # numbering information
                         allele_list = []
                         allele_str = ''
                         # Iterate through all the genes of interest
                         for gene in self.names:
-                            try:
-                                allele_str += allele_dict[gene]
-                            # If an allele has been filtered based on length, the sequence type needs to be removed
-                            except TypeError:
-                                continue
-                            # Add the allele number to the list, and to the string
+                            # Add the allele to the string of alleles
+                            allele_str += allele_dict[gene]
+                            # Add the allele number to the list, and to
+                            # the string
                             allele_list.append(allele_dict[gene])
-                        # Check if the string of allele numbers is already in the dictionary
+                        # Check if the string of allele numbers is already
+                        # in the dictionary
                         if allele_str not in profile_st:
-                            # Update the dictionary with the string of alleles: sequence type
+                            # Update the dictionary with the string of
+                            # alleles: sequence type
                             profile_st[allele_str] = allele_dict[self.names[0]]
                             alleles = '\t'.join(allele_list)
-                            # Add the sequence type allele numbers for this sequence to the string
+                            # Add the sequence type allele numbers for this
+                            # sequence to the string
                             reduced_data += f'{seq_type}\t{alleles.rstrip()}\n'
-                            # Updated the notes with the sequence type linking information
+                            # Updated the notes with the sequence type
+                            # linking information
                             notes.write(f'{seq_type}\t{seq_type}\n')
                         # Reduced profile already exists
                         else:
-                            # Extract the original sequence type with this string of allele numbers
+                            # Extract the original sequence type with this
+                            # string of allele numbers
                             original_seq_type = profile_st[allele_str]
-                            # Write the sequence type linking information, making note of the fact
-                            # that this is a duplicate
-                            notes.write(f'{seq_type}\t{original_seq_type}\tduplicate\n')
+                            # Write the sequence type linking information,
+                            # making note of the fact that this is a duplicate
+                            notes.write(
+                                f'{seq_type}\t{original_seq_type}\tduplicate\n'
+                            )
                     # Write the reduced profile information to file
                     reduced.write(reduced_data)
 
-    def __init__(self, profile, names, output='profile'):
+    def __init__(
+            self,
+            profile: str,
+            names: str,
+            output: str = 'profile'):
+        """
+        Constructs all the necessary attributes for the MyClass object.
+
+        Parameters:
+        profile (str): Path to the profile file
+        names (str): Path to the file with gene names
+        output (str): Name of the output folder. Default is 'profile'
+        """
+
+        # Log welcome message
         logging.info('Welcome to profile reducer!')
+
+        # Set profile file
         self.profile = pathfinder(path=profile)
         try:
             assert os.path.isfile(self.profile)
         except AssertionError as exc:
-            logging.error('Cannot locate the specified profile file: %s', self.profile)
+            logging.error(
+                'Cannot locate the specified profile file: %s', self.profile
+            )
             raise SystemExit from exc
-        # Create the folder into which the reduced profile and notes are to be placed
+
+        # Create the folder into which the reduced profile and notes are
+        # to be placed
         self.report_path = os.path.join(os.path.dirname(self.profile), output)
         make_path(self.report_path)
+
+        # Set reduced profile and notes files
         self.reduced_profile = os.path.join(self.report_path, 'profile.txt')
         self.notes_file = os.path.join(self.report_path, 'reducing_notes.txt')
+
+        # Set name file
         self.name_file = pathfinder(path=names)
         try:
             assert os.path.isfile(self.name_file)
         except AssertionError as exc:
-            logging.error('Cannot find the supplied file with gene names: %s', self.name_file)
+            logging.error(
+                'Cannot find the supplied file with gene names: %s',
+                self.name_file
+            )
             raise SystemExit from exc
+
+        # Initialize other attributes
         self.names = []
         self.profile_dict = {}
         self.allele_dict = {}
 
 
 def cli():
     """
     Collect the arguments, create an object, and run the script
     """
     # Parser for arguments
-    parser = ArgumentParser(description='Extract the genes of interest from a profile file')
+    parser = ArgumentParser(
+        description='Extract the genes of interest from a profile file'
+    )
     parser.add_argument(
         '-p', '--profile',
         metavar='profile',
         required=True,
         help='Name and path of profile file.')
     parser.add_argument(
         '-n', '--names',
         metavar='names',
         required=True,
-        help='Name and path to a file containing the gene names (one per line) to be extracted '
-             'from the profile')
+        help='Name and path to a file containing the gene names '
+        '(one per line) to be extracted from the profile'
+    )
     # Get the arguments into an object
     arguments = parser.parse_args()
     SetupLogging(debug=True)
     reduce = ProfileReduce(
         profile=arguments.profile,
         names=arguments.names
     )
     reduce.main()
     logging.info('Profile reduction complete!')
-    # Prevent the arguments being printed to the console (they are returned in order for the tests to work)
+    # Prevent the arguments being printed to the console (they are returned
+    # in order for the tests to work)
     sys.stderr = open(os.devnull, 'w', encoding='utf-8')
     return arguments
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `AlleleFinder-0.1.6/allele_tools/methods.py` & `allelefinder-0.1.7/allele_tools/methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 # Third party inputs
 from olctools.accessoryFunctions.accessoryFunctions import (
     GenObject,
     make_path,
     MetadataObject,
     relative_symlink
  )
-from Bio.Blast.Applications import NcbiblastnCommandline, NcbiblastpCommandline
+from Bio.Blast.Applications import (
+    NcbiblastnCommandline,
+    NcbiblastpCommandline,
+    NcbiblastxCommandline
+)
 from Bio.Data.CodonTable import TranslationError
 from Bio.SeqRecord import SeqRecord
 from Bio.Seq import Seq
 from Bio import SeqIO
 import coloredlogs
 
 
@@ -43,73 +47,81 @@
             'bold': True, 'color': 'yellow'},
         'error': {
             'bold': True, 'color': 'red'},
         'critical': {
             'bold': True, 'background': 'red'}
 
     }
-    # Change the default log format to be the time prepended to the appropriately formatted 
-    # message string
+    # Change the default log format to be the time prepended to the
+    # appropriately formatted message string
     coloredlogs.DEFAULT_LOG_FORMAT = '%(asctime)s %(message)s'
     # Set the logging level
     coloredlogs.install(level=arguments.verbosity.upper())
 
 
 def setup_arguments(parser: ArgumentParser):
     """
-    Finalise setting up the ArgumentParser arguments into an object, and running subparser
-    functions, or displaying the help message
+    Finalise setting up the ArgumentParser arguments into an object,
+    and running subparser functions, or displaying the help message
     :param parser: type: ArgumentParser object
     :return: parsed ArgumentParser object
     """
     # Get the arguments into an object
     arguments = parser.parse_args()
     # Run the appropriate function for each sub-parser.
     if hasattr(arguments, 'func'):
         # Set up logging
         setup_logging(arguments=arguments)
         arguments.func(arguments)
-    # If the 'func' attribute doesn't exist, display the basic help for the appropriate subparser
-    # (if any)
+    # If the 'func' attribute doesn't exist, display the basic help for the
+    # appropriate subparser (if any)
     else:
         try:
-            # Determine which subparser was called by extracting it from the arguments.
-            # Note that this requires the use of the desc keyword when creating subparsers
+            # Determine which subparser was called by extracting it from the
+            # arguments.
+            # Note that this requires the use of the desc keyword when
+            # creating subparsers
             command = list(vars(arguments).keys())[0]
-            # If the extracted command exists, use the command-specific subparser help
+            # If the extracted command exists, use the command-specific
+            # subparser help
             if command:
                 parser.parse_args([command, '-h'])
             # Otherwise, use the basic help
             else:
                 parser.parse_args(['-h'])
-        # If there were no subparsers specified (the list of keys in the arguments is empty),
+        # If there were no subparsers specified (the list of keys in the
+        # arguments is empty),
         # use the basic help
         except IndexError:
             parser.parse_args(['-h'])
     return arguments
 
 
 def common_allele_find_errors(
         args: ArgumentParser.parse_args,
         errors: list,
         amino_acid: bool):
     """
     Perform checks for arguments shared between allele finding scripts
     :param args: type ArgumentParser arguments
     :param errors: List of errors with supplied arguments
-    :param amino_acid: Boolean of whether the query sequence is amino acid or nucleotide
+    :param amino_acid: Boolean of whether the query sequence is amino acid or
+    nucleotide
     :return: Updated list of errors
     """
     # Query folder checks
     if not os.path.isdir(args.query_path):
-        errors.append(f'Could not find supplied query folder: {args.query_path}')
+        errors.append(
+            f'Could not find supplied query folder: {args.query_path}'
+        )
     else:
         if not glob(os.path.join(args.query_path, '*.fasta')):
             errors.append(
-                f'Could not locate sequence files in supplied query folder: {args.query_path}'
+                f'Could not locate sequence files in supplied query folder: '
+                f'{args.query_path}'
             )
         else:
             if amino_acid:
                 errors = detect_protein(
                     query_path=args.query_path,
                     errors=errors
                 )
@@ -129,42 +141,56 @@
     :param args: type ArgumentParser arguments
     :param errors: List of errors with supplied arguments
     :return: Updated list of errors
     """
     # Nucleotide checks
     try:
         if not os.path.isdir(args.nt_alleles):
-            errors.append(f'Could not find supplied nucleic acid allele folder: {args.nt_alleles}')
+            errors.append(
+                f'Could not find supplied nucleic acid allele folder: '
+                f'{args.nt_alleles}'
+            )
         else:
             if not glob(os.path.join(args.nt_alleles, '*.fasta')):
                 errors.append(
-                    f'Could not locate sequence files in supplied nucleic acid allele folder: {args.nt_alleles}'
+                    f'Could not locate sequence files in supplied nucleic '
+                    f'acid allele folder: {args.nt_alleles}'
                 )
     # Allows for checks in analyses without nucleotide sequences
     except AttributeError:
         pass
     try:
         if not os.path.isfile(args.nt_profile):
-            errors.append(f'Could not locate supplied nucleic acid profile file: {args.nt_profile}')
+            errors.append(
+                f'Could not locate supplied nucleic acid profile '
+                f'file: {args.nt_profile}'
+            )
     except AttributeError:
         pass
     # Amino acid checks
     try:
         if not os.path.isdir(args.aa_alleles):
-            errors.append(f'Could not find supplied amino acid allele folder: {args.aa_alleles}')
+            errors.append(
+                f'Could not find supplied amino acid allele folder: '
+                f'{args.aa_alleles}'
+            )
         else:
             if not glob(os.path.join(args.aa_alleles, '*.fasta')):
                 errors.append(
-                    f'Could not locate sequence files in supplied amino acid allele folder: {args.aa_alleles}'
+                    f'Could not locate sequence files in supplied amino acid '
+                    f'allele folder: {args.aa_alleles}'
                 )
     except AttributeError:
         pass
     try:
         if not os.path.isfile(args.aa_profile):
-            errors.append(f'Could not locate supplied amino acid profile file: {args.aa_profile}')
+            errors.append(
+                f'Could not locate supplied amino acid profile '
+                f'file: {args.aa_profile}'
+            )
     except AttributeError:
         pass
     return errors
 
 
 def error_print(
         errors: list):
@@ -173,54 +199,64 @@
     :param errors: List of errors with supplied arguments
     """
     # Create variables to allow for grammatically correct error messages
     error_string = '\n'.join(errors)
     was_were = 'was' if len(errors) == 1 else 'were'
     correct = 'error' if len(errors) == 1 else 'errors'
     logging.error(
-        'There %s %s %s when attempting to run your command: \n%s', was_were, len(errors), correct, error_string)
+        'There %s %s %s when attempting to run your command: \n%s', was_were,
+        len(errors), correct, error_string
+    )
     raise SystemExit
 
 
 def detect_protein(
         query_path: str,
         errors: list):
     """
     Attempt to determine whether a supplied file contains protein sequence
-    :param query_path: String of absolute path to folder containing sequence files
+    :param query_path: String of absolute path to folder containing sequence
+    files
     :param errors: List of errors with supplied arguments
     :return: Updated list of errors
     """
     # Create a list of all the FASTA files in the query path
     seq_files = glob(os.path.join(query_path, '*.fasta'))
     # Iterate through all the files
     for seq_file in seq_files:
-        # Initialise a boolean to track whether the sequences appear to be amino acid or nucleotide
+        # Initialise a boolean to track whether the sequences appear to be
+        # amino acid or nucleotide
         aa = False
         for record in SeqIO.parse(seq_file, format='fasta'):
             # Convert the sequence object to a string
             seq = str(record.seq)
             # Create a set of all the characters in the string of the sequence
             seq_set = set(seq)
-            # Since there are only 4(5 with N, 6 with N and -) possible characters in DNA, but 20 in protein, I chose
-            # a length of 10 to allow for relatively low complexity protein sequences to pass, but DNA to fail
+            # Since there are only 4(5 with N, 6 with N and -) possible
+            # characters in DNA, but 20 in protein, I chose
+            # a length of 10 to allow for relatively low complexity protein
+            # sequences to pass, but DNA to fail
             if len(seq_set) > 10:
-                # Update the boolean - note that only a single sequence in the file needs to be considered protein for
+                # Update the boolean - note that only a single sequence in the
+                # file needs to be considered protein for
                 # the entire file to pass
                 aa = True
         # Update the errors if the file appears to be DNA
         if not aa:
-            errors.append(f'Query file {seq_file} does not appear to be protein')
+            errors.append(
+                f'Query file {seq_file} does not appear to be protein'
+            )
     return errors
 
 
 def pathfinder(path: str):
     """
     Create absolute path user-supplied path. Allows for tilde expansion from
-    :param path: String of path supplied by user. Could be relative, tilde expansion, or absolute
+    :param path: String of path supplied by user. Could be relative, tilde
+    expansion, or absolute
     :return: out_path: String of absolute path provided by user.
     """
     # Determine if the path requires path expansion
     if path.startswith('~'):
         # Create the absolute path of the tilde expanded path
         out_path = os.path.abspath(os.path.expanduser(os.path.join(path)))
     else:
@@ -231,17 +267,19 @@
 
 def query_prep(
         query_path: str,
         runmetadata: MetadataObject,
         clear_report=True):
     """
     Create MetadataObjects for each sample
-    :param query_path: String of absolute path to folder containing sequence files
+    :param query_path: String of absolute path to folder containing sequence
+    files
     :param runmetadata: MetadataObject with list of GenObjects for each query
-    :param clear_report: Boolean of whether to clear previous iterations of BLAST reports. Default is True
+    :param clear_report: Boolean of whether to clear previous iterations of
+    BLAST reports. Default is True
     :return runmetadata: MetadataObject updated with query information
     """
     logging.info('Preparing query files')
     # Find all the sequence files in the path
     fasta_files = sorted(glob(os.path.join(query_path, '*.fasta')))
     for fasta in fasta_files:
         name = os.path.splitext(os.path.basename(fasta))[0]
@@ -250,22 +288,24 @@
             metadata = MetadataObject()
             metadata.samples = []
             # Populate the MetadataObject with the required attributes
             metadata.name = name
             metadata.general = GenObject()
             metadata.commands = GenObject()
             metadata.alleles = GenObject()
-            metadata.alleles.outputdirectory = os.path.join(query_path, metadata.name)
+            metadata.alleles.outputdirectory = \
+                os.path.join(query_path, metadata.name)
             # Set the name of the BLAST output file
             metadata.alleles.blast_report = os.path.join(
                 metadata.alleles.outputdirectory,
                 f'{metadata.name}.tsv'
             )
-            # As the name and number of alleles can change over multiple iterations of the
-            # program, it's best to clear out any old reports before running again
+            # As the name and number of alleles can change over multiple
+            # iterations of the program, it's best to clear out any old
+            # reports before running again
             if clear_report:
                 try:
                     os.remove(metadata.alleles.blast_report)
                 except FileNotFoundError:
                     pass
             make_path(metadata.alleles.outputdirectory)
             # Create a symlink of the sequence file in its own subdirectory
@@ -284,23 +324,26 @@
         amino_acid: bool,
         combined_targets: str,
         cpus: int,
         outfmt: str):
     """
     Run the BLAST analyses on the query
     :param runmetadata: MetadataObject with list of GenObjects for each query
-    :param amino_acid: Boolean of whether the query sequence is amino acid or nucleotide
-    :param combined_targets: String of absolute path to file containing all sequences in other files in folder
+    :param amino_acid: Boolean of whether the query sequence is amino acid or
+    nucleotide
+    :param combined_targets: String of absolute path to file containing all
+    sequences in other files in folder
     :param cpus: Integer of number of threads to use for BLAST analyses
     :param outfmt: String of BLAST fields to include in the report
     """
     logging.info('Running BLAST analyses')
     # Iterate through the samples
     for sample in runmetadata.samples:
-        # Run the appropriate BLAST command BLASTN for nucleotide, BLASTP for protein
+        # Run the appropriate BLAST command BLASTN for nucleotide, BLASTP for
+        # protein
         if not amino_acid:
             blast = NcbiblastnCommandline(
                 db=os.path.splitext(combined_targets)[0],
                 query=sample.general.bestassemblyfile,
                 num_alignments=100000000,
                 evalue=0.001,
                 num_threads=cpus,
@@ -317,54 +360,87 @@
                 num_threads=cpus,
                 outfmt=outfmt,
                 out=sample.alleles.blast_report
             )
         blast()
 
 
+def blastx_alleles(
+        runmetadata: MetadataObject,
+        combined_targets: str,
+        cpus: int,
+        outfmt: str):
+    """
+    Run the BLAST analyses on the query
+    :param runmetadata: MetadataObject with list of GenObjects for each query
+    :param combined_targets: String of absolute path to file containing all
+    sequences in other files in folder
+    :param cpus: Integer of number of threads to use for BLAST analyses
+    :param outfmt: String of BLAST fields to include in the report
+    """
+    logging.info('Running BLAST analyses')
+    # Iterate through the samples
+    for sample in runmetadata.samples:
+        # Run the BLASTx command
+        blast = NcbiblastxCommandline(
+                query=sample.general.bestassemblyfile,
+                db=os.path.splitext(combined_targets)[0],
+                evalue=0.001,
+                num_alignments=100000000,
+                num_threads=cpus,
+                outfmt=outfmt,
+                out=sample.alleles.blast_report
+            )
+        blast()
+
+
 def create_gene_names(
         path=os.getcwd(),
         name='genes.txt'):
     """
-    Create a file with gene names to use in reducing a wgMLST profile by finding any .fasta files
+    Create a file with gene names to use in reducing a wgMLST profile by
+    finding any .fasta files
     in a folder and adding them to the file (one per line)
-    :param path: type: String of the path in which the genes file is to be created
+    :param path: type: String of the path in which the genes file is to be
+    created
     :param name: type: String of the name of the gene file
     """
     # Find all the .fasta files in the path
     fasta_files = glob(os.path.join(path, '*.fasta'))
     # Set the name and path of the gene file
     gene_file = os.path.join(path, name)
     # Open the gene file to write
     with open(gene_file, 'w', encoding='utf-8') as genes_file:
         for fasta in fasta_files:
             # Remove the path information and the file extension. Print to file
-            genes_file.write(os.path.basename(os.path.splitext(fasta)[0]) + '\n')
+            genes_file.write(
+                os.path.basename(os.path.splitext(fasta)[0]) + '\n'
+            )
             logging.debug(
                 'Adding %s to %s',
                 os.path.basename(os.path.splitext(fasta)[0]), gene_file
             )
     # Check to see if the file is empty
     if os.stat(gene_file).st_size == 0:
         # Log an error stating that the file could not be properly populated
         logging.error(
-            'Created gene file, %s, is empty. Please ensure that directory %s has files with '
-            '.fasta extensions', gene_file, path
+            'Created gene file, %s, is empty. Please ensure that directory %s '
+            'has files with .fasta extensions', gene_file, path
             )
         raise SystemExit
 
 
 def create_blast_dict(
         sample: MetadataObject,
         extended_fieldnames: list):
     """
     Use DictReader to open and read a BLAST report into a dictionary
     :param sample: MetadataObject with list of GenObjects for each query
-    :param extended_fieldnames: List of the BLAST fields used, as well as the additional percent
-    match in index 14
+    :param extended_fieldnames: List of the BLAST fields used, as well as the
+    additional percent match in index 14
     """
     # Open the BLAST report as a dictionary
     blastdict = DictReader(
         open(sample.alleles.blast_report,
              encoding='utf-8'),
         fieldnames=extended_fieldnames,
         dialect='excel-tab'
@@ -383,25 +459,28 @@
         report_path: str,
         overlap_range=50,
         cutoff=90):
     """
     Parse BLAST outputs. Ensure co-location of genes that must be co-located
     :param runmetadata: MetadataObject with list of GenObjects for each query
     :param fieldnames: List of the BLAST fields used
-    :param extended_fieldnames: List of the BLAST fields used, as well as the additional percent
-    match in index 14
+    :param extended_fieldnames: List of the BLAST fields used, as well as the
+    additional percent match in index 14
     :param amino_acid: Boolean of whether targets are protein
     :param gene_names: List of all gene names in the analysis
-    :param nt_allele_path: String of the absolute path to the folder containing nucleotide allele files
-    :param aa_allele_path: String of the absolute path to the folder containing amino acid allele files
-    :param report_path: String of the absolute path to the folder into which reports are to be written
-    :param overlap_range: Integer of the maximum distance allowed between two genes in order for
-    them to be considered co-located. Default is 50 bp
-    :param cutoff: Integer of the minimum percent identity between query and subject sequence.
-    Default is 100%
+    :param nt_allele_path: String of the absolute path to the folder
+    containing nucleotide allele files
+    :param aa_allele_path: String of the absolute path to the folder
+    containing amino acid allele files
+    :param report_path: String of the absolute path to the folder into which
+    reports are to be written
+    :param overlap_range: Integer of the maximum distance allowed between two
+    genes in order for them to be considered co-located. Default is 50 bp
+    :param cutoff: Integer of the minimum percent identity between query and
+    subject sequence. Default is 100%
     :return: runmetadata: Updated MetadataObjects
     :return: notes: List of contig:query_range-specific notes
     """
     logging.info('Parsing BLAST outputs')
     notes = {}
     for sample in runmetadata.samples:
         # Initialise GenObjects as required
@@ -423,109 +502,131 @@
                 continue
             target_id = row['subject_id']
             target_start = row['subject_start']
             target_end = row['subject_end']
             target_seq = row['query_sequence']
             high = max([int(row['query_start']), int(row['query_end'])])
             low = min([int(row['query_start']), int(row['query_end'])])
-            # Create a list of the properly ordered start and stop points of the match
+            # Create a list of the properly ordered start and stop points of
+            # the match
             query_range = [low, high]
             # Remove unwanted pipes added to the name
-            nt_allele = target_id.lstrip('gb|').rstrip('|') if '|' in target_id else \
-                target_id
+            nt_allele = target_id.lstrip('gb|').rstrip('|') if '|' in \
+                target_id else target_id
             # If the percent identity is equal to the cutoff
             if float(row['percent_match']) >= cutoff:
                 # Append the hit dictionary to the list
                 sample.alleles.blastlist.append(row)
-                # Determine if the orientation of the sequence is reversed compared to
-                # the reference sequence
+                # Determine if the orientation of the sequence is reversed
+                # compared to the reference sequence
                 if int(target_end) < int(target_start) and not amino_acid:
                     seq = Seq(target_seq)
                     # Calculate the reverse complement of the sequence
                     nt_querysequence = str(seq.reverse_complement())
-                # If the sequence is not reversed, use the sequence as it is in the output
+                # If the sequence is not reversed, use the sequence as it is
+                # in the output
                 else:
                     nt_querysequence = target_seq
                 # Create a variable to avoid unnecessary typing
                 contig = row['query_id']
-                # Create a boolean to track whether this contig:range combination has already been processed
+                # Create a boolean to track whether this contig:range
+                # combination has already been processed
                 processed = False
                 # Add the contig key to the dictionary as required
                 if contig not in processed_range_dict:
                     processed_range_dict[contig] = set()
-                # Check the processed range dictionary to see if the current range is present
+                # Check the processed range dictionary to see if the current
+                # range is present
                 if processed_range_dict[contig]:
                     for previous_range in processed_range_dict[contig]:
-                        # Allow a small overlap of five bases in case the range of one query is slightly different
-                        overlap = query_range[1] + 5 >= previous_range[0] and \
-                                  previous_range[1] + 5 >= query_range[0]
-                        # If the range is already present in the dictionary, update the tracking boolean
+                        # Allow a small overlap of ten bases in case the range
+                        # of one query is slightly different
+                        overlap = query_range[1] + 10 >= previous_range[0] \
+                            and previous_range[1] + 10 >= query_range[0]
+                        # If the range is already present in the dictionary,
+                        # update the tracking boolean
                         if overlap:
                             processed = True
-                # Add the range to the set if it is empty
-                else:
-                    processed_range_dict[contig].add(tuple(query_range))
-                # If range has already been processed, we can skip this iteration of it
+                # Add the range to the set
+                processed_range_dict[contig].add(tuple(query_range))
+                # If range has already been processed, we can skip this
+                # iteration of it
                 if processed:
                     continue
-                # Update the processed ranges dictionary with the current range
-                processed_range_dict[contig].add(tuple(query_range))
-                # Create a tuple of the query range list to allow it to be used as a dictionary key
+                # Create a tuple of the query range list to allow it to be
+                # used as a dictionary key
                 query_range_tuple = tuple(query_range)
                 # Add keys to the targetsequence dictionary as required
                 if contig not in sample.alleles.targetsequence:
                     sample.alleles.targetsequence[contig] = {}
-                if query_range_tuple not in sample.alleles.targetsequence[contig]:
-                    sample.alleles.targetsequence[contig][query_range_tuple] = {}
+                if query_range_tuple not in \
+                        sample.alleles.targetsequence[contig]:
+                    sample.alleles.targetsequence[contig][
+                        query_range_tuple] = {}
                 # Populate the percent match dictionary
                 if contig not in resultdict:
                     resultdict[contig] = {}
                 if query_range_tuple not in resultdict[contig]:
-                    resultdict[contig][query_range_tuple] = {nt_allele: row['percent_match']}
+                    resultdict[contig][query_range_tuple] = \
+                        {nt_allele: row['percent_match']}
                 # Populate the notes dictionary
                 if contig not in notes:
                     notes[contig] = {}
                 if query_range_tuple not in notes[contig]:
                     notes[contig][query_range_tuple] = []
-                # Determine the name of the gene corresponding to the allele e.g. if the allele
-                # ECs1206_138, the corresponding gene is ECs1206_
-                base_gene = [gene_name for gene_name in gene_names if gene_name in nt_allele][0]
+                # Determine the name of the gene corresponding to the allele
+                # e.g. if the allele Stx1A_1|315aa, the corresponding gene is
+                # stx1A
+                base_gene = [
+                    gene_name[0].lower() + gene_name[1:-1] +
+                    gene_name[-1].upper()
+                    for gene_name in gene_names
+                    if gene_name.lower() in nt_allele.lower()
+                ][0]
                 # Translate the query sequence to protein
                 aa_querysequence = translate_sequence(
                     nt_seq=nt_querysequence
                 )
                 # Find the amino acid allele corresponding to this sequence
                 returned = aa_allele_lookup(
                     aa_seq=aa_querysequence,
                     gene=base_gene,
                     aa_allele_path=aa_allele_path,
                     notes=notes[contig][query_range_tuple]
                 )
+
                 # Initialise a string to hold the amino acid allele identifier
                 aa_allele = str()
-                # Create a boolean to track whether the amino acid sequence fails the screen criteria
+                # Create a boolean to track whether the amino acid sequence
+                # fails the screening criteria
                 filtered = False
-                # If a perfect match to a previous allele was found, a string is returned
+                # If a perfect match to a previous allele was found, a string
+                # is returned
                 if isinstance(returned, str):
                     aa_allele = returned
-                # If not perfect match was found to a previous allele, a tuple of the updated filtered boolean, and
+                # If not perfect match was found to a previous allele, a tuple
+                # of the updated filtered boolean, and
                 # notes on the sequence are returned
                 else:
-                    filtered, notes[contig][query_range_tuple] = returned
+                    filtered, returned_notes = returned
+                    if returned_notes:
+                        notes[contig][query_range_tuple] = returned_notes
                 # Add unfiltered imperfect nt alleles to the database
                 if float(row['percent_match']) < 100 and not filtered:
                     # Find the next allele identifier for the database
                     nt_allele_id = find_next_allele(
                         gene=base_gene,
                         allele_path=nt_allele_path
                     )
                     # Add the base gene name to the allele identifier
-                    nt_allele = f'{base_gene}_{nt_allele_id}'
+                    nt_allele = \
+                        f'{base_gene}_{nt_allele_id}|{len(nt_querysequence)}nt'
                     # Update the allele database with the new allele
-                    notes[contig][query_range_tuple], nt_allele = update_allele_databases(
+                    notes[contig][query_range_tuple], nt_allele = \
+                        update_allele_databases(
                         query_sequence=nt_querysequence,
                         header=nt_allele,
                         filtered=filtered,
                         gene=base_gene,
                         report_path=report_path,
                         allele_path=nt_allele_path,
                         notes=notes[contig][query_range_tuple],
@@ -533,41 +634,48 @@
                     )
                 # Add unfiltered novel aa alleles to the database
                 if not aa_allele and not filtered:
                     aa_allele_id = find_next_allele(
                         gene=base_gene,
                         allele_path=aa_allele_path
                     )
-                    aa_allele = f'{base_gene}_{aa_allele_id}'
-                    notes[contig][query_range_tuple], aa_allele = update_allele_databases(
+                    aa_allele = \
+                        f'{base_gene}_{aa_allele_id}|{len(aa_querysequence)}aa'
+                    notes[contig][query_range_tuple], aa_allele = \
+                        update_allele_databases(
                         query_sequence=aa_querysequence,
                         header=aa_allele,
                         filtered=filtered,
                         gene=base_gene,
                         report_path=report_path,
                         allele_path=aa_allele_path,
                         notes=notes[contig][query_range_tuple],
                         molecule='Amino acid'
                     )
-                # Populate the targetsequence dictionary with information on the nt and aa alleles
-                if base_gene not in sample.alleles.targetsequence[contig][query_range_tuple]:
-                    sample.alleles.targetsequence[contig][query_range_tuple][base_gene] = {
+                # Populate the targetsequence dictionary with information on
+                # the nt and aa alleles
+                if base_gene not in sample.alleles.targetsequence[
+                        contig][query_range_tuple]:
+                    sample.alleles.targetsequence[contig][query_range_tuple][
+                        base_gene] = {
                         'nt': {
                             'allele': nt_allele,
                             'sequence': nt_querysequence
                         },
                         'aa': {
                             'allele': aa_allele,
                             'sequence': aa_querysequence
                         }
                     }
-                # Populate the co-location dictionary with the required keys as necessary
+                # Populate the co-location dictionary with the required keys
+                # as necessary
                 if contig not in colocation_dict:
                     colocation_dict[contig] = {}
-                # The query_ranges and target keys both correspond to lists of values
+                # The query_ranges and target keys both correspond to lists of
+                # values
                 if 'query_ranges' not in colocation_dict[contig]:
                     colocation_dict[contig] = {
                         'query_ranges': [query_range],
                         'target': [nt_allele]
                     }
                 # If the keys already exist, append to the lists
                 else:
@@ -584,16 +692,16 @@
             overlap_range=overlap_range
         )
     return runmetadata, notes
 
 
 def translate_sequence(nt_seq: str):
     """
-    Uses BioPython to translate a nucleotide sequence to protein, and trims it to the first stop
-    codon
+    Uses BioPython to translate a nucleotide sequence to protein, and trims it
+    to the first stop codon
     :param nt_seq: String of the nucleotide sequence
     :return aa_seq: String of the trimmed amino acid sequence
     """
     # Create a sequence object from the nucleotide sequence
     nt_seq_object = Seq(nt_seq)
     # Translate the sequence to protein
     try:
@@ -601,132 +709,147 @@
         aa_seq_object = nt_seq_object.translate()
     # BioPython cannot translate a sequence with gaps (-)
     except TranslationError:
         allele_seq = str(nt_seq_object).replace('-', '')
         seq = Seq(allele_seq)
         aa_seq_object = str(seq.translate())
     # Split the sting on stop codons, keep only the first part of the split
-    aa_seq = str(aa_seq_object).split('*', maxsplit=1)[0] + '*'
+    aa_seq = str(aa_seq_object).split('*', maxsplit=1)[0]
     return str(aa_seq)
 
 
 def aa_allele_lookup(
         aa_seq: str,
         gene: str,
         aa_allele_path: str,
         notes: list):
     """
-    Read in the amino acid allele file. Search for exact matches to the current sequence
+    Read in the amino acid allele file. Search for exact matches to the
+    current sequence
     :param aa_seq: String of the amino acid sequence
     :param gene: Sting of the gene name
-    :param aa_allele_path: String of the absolute path to the folder containing the amino acid
+    :param aa_allele_path: String of the absolute path to the folder
+    containing the amino acid
     allele files
     :param notes: List of notes for the current contig: query_range
-    :return record.id: Allele identifier corresponding to the sequence matching the aa_seq
+    :return record.id: Allele identifier corresponding to the sequence
+    matching the aa_seq
     if no matches:
-    :return filtered: Boolean of whether the amino acid sequence passes length thresholds
+    :return filtered: Boolean of whether the amino acid sequence passes length
+    thresholds
     :return notes: Populated notes
     """
-    # Set the name of the amino acid allele file by joining the allele folder path to the gene name
+    # Set the name of the amino acid allele file by joining the allele folder
+    # path to the gene name
     aa_allele_file = os.path.join(aa_allele_path, f'{gene}.fasta')
     # Iterate through all the alleles in the file
     for record in SeqIO.parse(aa_allele_file, 'fasta'):
-        # If the sequence in the file matches the current sequence, return the allele identifier
+        # If the sequence in the file matches the current sequence, return the
+        # allele identifier
         if aa_seq == str(record.seq):
             return record.id
-    # If no records match, evaluate whether the aa allele passes necessary length thresholds
-    filtered, notes = evaluate_translated_allele(
+    # If no records match, evaluate whether the aa allele passes necessary
+    # length thresholds
+    filtered, notes, aa_seq = evaluate_translated_allele(
         aa_seq=aa_seq,
         gene=gene,
         notes=notes
     )
     return filtered, notes
 
 
 def evaluate_translated_allele(
         aa_seq: str,
         gene: str,
-        notes: list,
-        aa=False):
+        notes: list):
     """
-    Evaluate whether an aa sequence passes the necessary length thresholds after trimming of an interior stop codons
+    Evaluate whether an aa sequence passes the necessary length thresholds
+    after trimming of an interior stop codons
     :param aa_seq: String of the amino acid sequence to evaluate
-    :param gene: String of the name of the gene (no allele information) being evaluated
+    :param gene: String of the name of the gene (no allele information) being
+    evaluated
     :param notes: List of notes for the current contig: query_range
-    :param aa: Boolean of whether the query sequence is amino acid. Triggers filtering if sequence doesn't end with a
-    stop codon
-    :return filtered: Boolean of whether the amino acid sequence passes length thresholds
+    :return filtered: Boolean of whether the amino acid sequence passes length
+    thresholds
     :return notes: Populated notes
     """
     # Dictionary of minimum acceptable lengths for each of the STEC genes
     length_dict = {
-        'ECs2973': 82,
         'stx1B': 82,
-        'ECs2974': 313,
         'stx1A': 313,
-        'ECs1205': 313,
         'stx2A': 313,
-        'ECs1206': 84,
         'stx2B': 84
     }
     filtered = False
-    if not aa_seq.endswith('*'):
-        notes.append(f'{gene} trimmed sequence did not end with a stop codon')
-        if aa:
-            filtered = True
-    # Remove all sequence after a stop codon (*)
-    aa_seq = aa_seq.split('*', maxsplit=1)[0] + '*'
+    # Remove stop codons and all sequence following it
+    aa_seq = aa_seq.split('*')[0]
     # Evaluate the translated length of the sequence
     filtered, notes = evaluate_translated_length(
         aa_seq=aa_seq,
         length_dict=length_dict,
         gene=gene,
         notes=notes,
         filtered=filtered
     )
-    return filtered, notes
+    return filtered, notes, aa_seq
 
 
 def update_allele_databases(
         query_sequence: SeqIO.parse,
         header: str,
         filtered: bool,
         gene: str,
         report_path: str,
         allele_path: str,
         notes: list,
         molecule: str):
     """
-    Update the appropriate allele file depending on quality filter status and molecule
+    Update the appropriate allele file depending on quality filter status and
+    molecule
     :param query_sequence: SEQIO sequence object of the novel allele
     :param header: String of the allele name (gene_allele ID)
     :param filtered: Boolean of whether the allele has been quality filtered
     :param gene: String of the name of the gene
-    :param report_path: String of the absolute path to the folder into which the reports are to be written
-    :param allele_path: String of the absolute path to the folder containing the allele database
+    :param report_path: String of the absolute path to the folder into which
+    the reports are to be written
+    :param allele_path: String of the absolute path to the folder containing
+    the allele database
     :param notes: List of notes on the alleles
-    :param molecule: String of the current molecule. Options are Nucleotide and Amino acid
+    :param molecule: String of the current molecule. Options are Nucleotide
+    and Amino acid
     :return: notes: Updated list of notes
     """
     # Create a SeqRecord of the allele using the novel allele name and sequence
     new_record = SeqRecord(
         seq=Seq(query_sequence),
         id=header,
         name='',
         description=''
     )
     # Create a string to prepend to allele file names
     molecule_str = 'nt' if molecule == 'Nucleotide' else 'aa'
     # Set the correct files depending on the filtering status
     if not filtered:
-        new_alleles = os.path.join(report_path, f'{molecule_str}_{gene}_novel_alleles.fasta')
-        allele_file = os.path.join(allele_path, f'{gene}.fasta')
+        new_alleles = os.path.join(
+            report_path,
+            f'{molecule_str}_{gene}_novel_alleles.fasta'
+        )
+        allele_file = os.path.join(
+            allele_path,
+            f'{gene}.fasta'
+        )
     else:
-        new_alleles = os.path.join(report_path, f'{molecule_str}_{gene}_filtered_alleles.fasta')
-        allele_file = os.path.join(allele_path, f'{gene}_filtered.txt')
+        new_alleles = os.path.join(
+            report_path,
+            f'{molecule_str}_{gene}_filtered_alleles.fasta'
+        )
+        allele_file = os.path.join(
+            allele_path,
+            f'{gene}_filtered.txt'
+        )
     records = []
     # Iterate through all the records in the allele database
     if os.path.isfile(allele_file):
         for record in SeqIO.parse(allele_file, 'fasta'):
             # Append all the records to the list
             records.append(record)
     # Check to see if the query sequence is novel in the database
@@ -735,140 +858,161 @@
         with open(new_alleles, 'a+', encoding='utf-8') as novel:
             SeqIO.write(
                 sequences=new_record,
                 handle=novel,
                 format='fasta'
             )
         records.append(new_record)
-        # Overwrite the existing allele database file with the updated list of records
+        # Overwrite the existing allele database file with the updated list of
+        # records
         with open(allele_file, 'w', encoding='utf-8') as alleles:
             SeqIO.write(
                 sequences=records,
                 handle=alleles,
                 format='fasta'
             )
         remove_combined_db_files(allele_path=allele_path)
         notes.append(f'{molecule} allele {header} is novel')
     # Non-novel sequences will have updated notes with the match
     else:
         for record in records:
             if str(query_sequence) == record.seq:
                 # Append the previous finding to the notes
-                notes.append(f'{molecule} matches previous result: {record.id}')
+                notes.append(
+                    f'{molecule} matches previous result: {record.id}'
+                )
                 # Set the header to the corresponding record.id on a match
                 header = record.id
     return notes, header
 
 
 def colocation_calculation(
         colocation_dict: dict,
         gene_names: list,
         overlap_range: int):
     """
     Determine if gene results are co-located on a contig
-    :param colocation_dict: Dictionary of contig: {'query_ranges': [query_range],
-    'target': [allele_id]}
+    :param colocation_dict: Dictionary of contig: {'query_ranges':
+    [query_range], 'target': [allele_id]}
     :param gene_names: List of all genes in the analysis
-    :param overlap_range: Integer of the maximum distance allowed between two separate hits before
-    they can no longer be considered co-located on a contig
-    :return overlap_dict: Dictionary of contig:full_range:gene_pair: {'overlap': overlap,
-    'allele': [allele_identifiers]}
+    :param overlap_range: Integer of the maximum distance allowed between two
+    separate hits before they cannot be considered co-located on a contig
+    :return overlap_dict: Dictionary of contig:full_range:gene_pair:
+    {'overlap': overlap, 'allele': [allele_identifiers]}
     """
     # Initialise a dictionary to store the details of any co-located sequences
     overlap_dict = {}
     # Iterate over all the contigs with hits
     for contig, info_dict in colocation_dict.items():
         # Update the overlap dictionary with the contig name as required
         if contig not in overlap_dict:
             overlap_dict[contig] = {}
         # Extract the query range and the allele identifiers from info_dict
         query_ranges = info_dict['query_ranges']
         targets = info_dict['target']
         # Iterate over all the query ranges with hits on the current contig
         for query_iterator, query_range in enumerate(query_ranges):
-            # Create a variable to track whether the current contig:query range combination has
-            # been added to the overlap dictionary
+            # Create a variable to track whether the current contig:query
+            # range combination has been added to the overlap dictionary
             processed = False
-            # Extract the name of the current allele from the list of all alleles in the range
+            # Extract the name of the current allele from the list of all
+            # alleles in the range
             current_allele = targets[query_iterator]
-            # Create a dictionary of tuple of other ranges present in the list of ranges: iterator
+            # Create a dictionary of tuple of other ranges present in the list
+            # of ranges: iterator
             other_ranges = {
-                tuple(other): j for j, other in enumerate(query_ranges) if other != query_range
+                tuple(other): j for j, other in enumerate(query_ranges) if
+                other != query_range
             }
             # Iterate over these other ranges
             for other_range, other_iterator in other_ranges.items():
-                # Calculate whether the current range overlaps with this other range
-                # e.g. query_range = (100, 500), other_range = (525, 1000), overlap_range = 50
-                # Check if 500 + 50 >= 525 and 1000 + 50 >= 100
-                overlap = query_range[1] + overlap_range >= other_range[0] and \
-                        other_range[1] + overlap_range >= query_range[0]
+                # Calculate whether the current range overlaps with this other
+                # range e.g. query_range = (100, 500), other_range =
+                # (525, 1000), overlap_range = 50. Check if 500 + 50 >= 525
+                # and 1000 + 50 >= 100
+                overlap = query_range[1] + overlap_range >= other_range[0] \
+                    and other_range[1] + overlap_range >= query_range[0]
                 # If these ranges overlap, populate the overlap dictionary
                 if overlap:
                     overlap_dict, processed = positive_overlap(
                         info_dict=info_dict,
                         other_iterator=other_iterator,
                         query_range=query_range,
                         other_range=other_range,
                         overlap_dict=overlap_dict,
                         current_allele=current_allele,
                         contig=contig,
                         gene_names=gene_names,
                         overlap=overlap
                     )
-            # If the current contig: range was not entered into the overlap dictionary, there were
-            # either no other hits, or the hits did not overlap
+            # If the current contig: range was not entered into the overlap
+            # dictionary, there were either no more hits, or the hits
+            # did not overlap
             if not processed:
                 # Create a tuple containing only the current range
                 tuple_range = tuple(query_range)
                 # Update the dictionary as required
                 if tuple_range not in overlap_dict[contig]:
                     overlap_dict[contig][tuple_range] = {}
                 # Extract the gene name corresponding to the allele identifier
-                # e.g. gene = ECs1206 allele = ECs1206_138 will create ECs1206
-                gene = [gene_name for gene_name in gene_names if gene_name in current_allele][0]
-                # Add the gene name to the dictionary, and update create the overlap and allele keys
+                # e.g. gene = stx1A allele = Stx1A_1|315aa will create stx1A
+                gene = [
+                    gene_name[0].lower() + gene_name[1:-1] +
+                    gene_name[-1].upper()
+                    for gene_name in gene_names
+                    if gene_name.lower() in current_allele.lower()
+                ][0]
+                # Add the gene name to the dictionary, and update create the
+                # overlap and allele keys
                 if gene not in overlap_dict[contig][tuple_range]:
                     overlap_dict[contig][tuple_range][gene] = {
                         'overlap': False,
                         'allele': []
                     }
                 # Append the current allele identifier to the list of alleles
-                overlap_dict[contig][tuple_range][gene]['allele'].append(current_allele)
+                overlap_dict[contig][tuple_range][gene]['allele'].append(
+                    current_allele
+                )
     return overlap_dict
 
 
 def positive_overlap(
         info_dict: dict,
         other_iterator: int,
         query_range: range,
         other_range: range,
         overlap_dict: dict,
         current_allele: str,
         contig: str,
         gene_names: list,
         overlap: bool):
     """
-    Determine the combined range of two overlapping ranges, extract gene names corresponding to
-    allele names, populate dictionary of range overlaps
-    :param info_dict: Dictionary of {'query_ranges': [query_range], 'target': [allele_id]}
-    :param other_iterator: Integer of the iterator corresponding to the current other_range from the
-    dictionary of other_range: iterator
-    :param query_range: Range of hit corresponding to current_allele in info_dict
-    e.g. info_dict['query_ranges'][query_iterator] and info_dict['target'][query_iterator]
-    :param other_range: Range of hit corresponding to non-current allele in info_dict
-    e.g. info_dict['query_ranges'][other_iterator] and info_dict['target'][other_iterator]
+    Determine the combined range of two overlapping ranges, extract gene names
+    corresponding to allele names, populate dictionary of range overlaps
+    :param info_dict: Dictionary of {'query_ranges': [query_range],
+    'target': [allele_id]}
+    :param other_iterator: Integer of the iterator corresponding to the
+    current other_range from the dictionary of other_range: iterator
+    :param query_range: Range of hit corresponding to current_allele in
+    info_dict e.g. info_dict['query_ranges'][query_iterator] and
+    info_dict['target'][query_iterator]
+    :param other_range: Range of hit corresponding to non-current allele in
+    info_dict e.g. info_dict['query_ranges'][other_iterator] and
+    info_dict['target'][other_iterator]
     :param overlap_dict: Dictionary of to be populated with overlap information
-    e.g. contig:full_range:gene_pair: {'overlap': overlap, 'allele': [allele_identifiers]}
-    :param current_allele: String of the name of the allele extracted from info_dict
-    e.g. info_dict['target'][query_iterator]
+    e.g. contig:full_range:gene_pair: {'overlap': overlap, 'allele':
+    [allele_identifiers]}
+    :param current_allele: String of the name of the allele extracted from
+    info_dict e.g. info_dict['target'][query_iterator]
     :param contig: Name of the contig within which the BLAST hits are located
     :param gene_names: List of all gene names in the analysis
     :param overlap: Boolean of whether query_range overlaps with other_range
     """
-    # Extract the name of the other allele from info_dict using the iterator of the other range
+    # Extract the name of the other allele from info_dict using the iterator
+    # of the other range
     other_allele = info_dict['target'][other_iterator]
     full_range = calculate_full_range(
         query_range=query_range,
         other_range=other_range
     )
     # Update the overlap dictionary with the full range as required
     if full_range not in overlap_dict[contig]:
@@ -876,41 +1020,47 @@
     # Create a sorted tuple of the allele names
     alleles = tuple(sorted([current_allele, other_allele]))
     # Create a set of all the genes with hits in the current overlap
     genes = set()
     # Iterate over all the alleles
     for allele in alleles:
         # Add the gene from the list of genes if it is present in the allele
-        # identifier e.g. gene = ECs1206 allele = ECs1206_138 will add ECs1206
-        genes.add([gene for gene in gene_names if gene in allele][0])
+        # identifier e.g. gene = stx1A allele = Stx1A_1|315aa will create stx1A
+        genes.add([
+            gene[0].lower() + gene[1:-1] + gene[-1].upper()
+            for gene in gene_names
+            if gene.lower() in allele.lower()
+        ][0])
     # Create a tuple of the sorted list of genes present in the set
     gene_pair = tuple(sorted(list(genes)))
     # Update the dictionary as required
     if gene_pair not in overlap_dict[contig][full_range]:
         overlap_dict[contig][full_range][gene_pair] = {
             'overlap': overlap,
             'allele': []
         }
     # Append the current allele to the overlap dictionary
-    overlap_dict[contig][full_range][gene_pair]['allele'].append(current_allele)
+    overlap_dict[contig][full_range][gene_pair]['allele'].append(
+        current_allele
+    )
     # Set processed to True to indicate that there was an overlap and that the
     # dictionary was populated
     processed = True
     return overlap_dict, processed
 
 
 def calculate_full_range(
         query_range: range,
         other_range: range):
     """
     Determine if two ranges overlap
     :param query_range: Range of hit corresponding to current_allele
     :param other_range: Range of hit corresponding to non-current allele
-    :return full_range: Tuple of minimum coordinate from both ranges, maximum coordinate from
-    both ranges
+    :return full_range: Tuple of minimum coordinate from both ranges, maximum
+    coordinate from both ranges
     """
     # Determine in the minimum and maximum coordinates of the two ranges
     # e.g. query_range = (100, 500), other_range = (525, 1000)
     # min_range = 100
     min_range = (min(query_range[0], other_range[0]))
     # max_range = 1000
     max_range = (max(query_range[1], other_range[1]))
@@ -923,321 +1073,408 @@
 def evaluate_translated_length(
         aa_seq: str,
         length_dict: dict,
         gene: str,
         notes: list,
         filtered: bool):
     """
-    Evaluate whether a translated sequence passes a length filter and starts with a methionine
-    residue
+    Evaluate whether a translated sequence passes a length filter and starts
+    with a methionine residue
     :param aa_seq: String of the amino acid sequence to evaluate
-    :param length_dict: Dictionary of minimum acceptable length for each gene in the analysis
+    :param length_dict: Dictionary of minimum acceptable length for each gene
+    in the analysis
     :param gene: String of the name of the gene
     :param notes: List of notes on the alleles
-    :param filtered: Boolean of whether the allele has been filtered based on length or content
+    :param filtered: Boolean of whether the allele has been filtered based on
+    length or content
     :return: filtered: Updated filtering boolean
     :return: notes: Updated list of notes
     """
     # Proper protein sequences must start with a methionine (M)
     if not aa_seq.startswith('M'):
         filtered = True
         notes.append(f'{gene} amino acid sequence does not start with M')
-    # The length of the sequence must also be greater than the minimum gene-specific length
+    # The length of the sequence must also be greater than the minimum
+    # gene-specific length
     if len(aa_seq) < length_dict[gene]:
         filtered = True
         notes.append(
-            f'{gene} amino acid sequence was {len(aa_seq)} amino acid residues. Minimum allowed '
-            f'length is {length_dict[gene]} amino acid residues')
+            f'{gene} amino acid sequence was {len(aa_seq)} amino acid '
+            f'residues. Minimum allowed length is {length_dict[gene]} '
+            f'amino acid residues'
+        )
     return filtered, notes
 
 
 def generic_evaluate_translated_length(
         aa_seq: str,
         sequence: str,
         gene: str,
         notes: list,
         filtered: bool,
         cutoff=0.95):
     """
-    Evaluate whether a translated sequence passes a generic length filter and starts with a methionine
-    residue
+    Evaluate whether a translated sequence passes a generic length filter and
+    starts with a methionine residue
     :param aa_seq: String of the amino acid sequence to evaluate
     :param sequence: String of untrimmed nucleotide sequence
     :param gene: String of the name of the gene
     :param notes: List of notes on the alleles
-    :param filtered: Boolean of whether the allele has been filtered based on length or content
-    :param cutoff: Float of minimum cutoff value to be used for filtering trimmed sequences. Default is 0.95
+    :param filtered: Boolean of whether the allele has been filtered based on
+    length or content
+    :param cutoff: Float of minimum cutoff value to be used for filtering
+    trimmed sequences. Default is 0.95
     :return: filtered: Updated filtering boolean
     :return: notes: Updated list of notes
     """
     # Proper protein sequences must start with a methionine (M)
     if not aa_seq.startswith('M'):
         filtered = True
         notes.append(f'{gene} amino acid sequence does not start with M')
-    # Minimum length of a trimmed amino acid allele permitted is 95% the length of the theoretical length of
-    # the translated nucleotide sequence e.g. a 99 bp nt sequence would be 33 amino acid residues, and 95% of
+    # Minimum length of a trimmed amino acid allele permitted is 95% the
+    # length of the theoretical length of the translated nucleotide sequence
+    # e.g. a 99 bp nt sequence would be 33 amino acid residues, and 95% of
     # that is 31.35 -> 31 (rounded down)
     minimum_length = math.floor(len(sequence) / 3 * cutoff)
     aa_seq_length = len(aa_seq)
     if aa_seq_length < minimum_length:
         filtered = True
         notes.append(
-            f'{gene} amino acid sequence was trimmed to {aa_seq_length} residues '
-            f'the minimum length allowed is {minimum_length} residues')
+            f'{gene} amino acid sequence was trimmed to {aa_seq_length} '
+            f'residues. The minimum length allowed is {minimum_length} '
+            'residues'
+        )
     return filtered, notes
 
 
 def find_next_allele(
         gene: str,
         allele_path: str,
         extension='.fasta'):
     """
     Update the allele database with the novel allele extracted above
     :param gene: Name of the current gene being examined
-    :param allele_path: Name and absolute path to folder containing allele files
+    :param allele_path: Name and absolute path to folder containing
+    allele files
     :param extension: String of the file extension. Default is .fasta
     :return: last_id: Number of the last alleles in the current database
     """
     # Find the allele database file
     allele_file = os.path.join(allele_path, f'{gene}{extension}')
-    # Initialise a variable to store the name of the last allele in the database file
+    # Initialise a variable to store the name of the last allele in the
+    # database file
     last_id = int()
     records = []
     if os.path.isfile(allele_file):
         # Iterate through all the records in the allele database
         for record in SeqIO.parse(allele_file, 'fasta'):
             # Update the last_id variable
-            last_id = int(record.id.split('_')[-1])
+            last_id = int(record.id.split('|')[0].split('_')[-1])
             records.append(record)
     else:
         last_id = 0
-    # Make it clear that these are novel profiles by starting at 1000000
-    if last_id < 1000000:
-        last_id = 999999
     return last_id + 1
 
 
 def remove_combined_db_files(allele_path: str):
     """
     Remove all the combined gene files used in BLAST analyses
-    :param allele_path: String of the absolute path to the folder containing the alleles
+    :param allele_path: String of the absolute path to the folder containing
+    the alleles
     """
     # Find all the files in the directory with the word combined in the name
     combined_files = glob(os.path.join(allele_path, 'combined*'))
     # Remove each of the files
     for file in combined_files:
         os.remove(file)
 
 
 def create_nt_allele_comprehension(
         runmetadata: MetadataObject,
-        gene_names: list):
+        gene_names: list,
+        translated: bool = False):
     """
-    Create gene: nucleotide allele ID comprehensions for each contig: range combination with hits
+    Create gene: nucleotide allele ID comprehensions for each contig: range
+    combination with hits
     :param runmetadata: MetadataObject with list of GenObjects for each query
     :param gene_names: List of all gene names in the analysis
-    :return: allele_comprehension: nucleotide allele comprehension. allele_comprehension[contig][full_range] =
-    {gene:allele}
+    :param translated: Boolean of whether the query is nucleotide against an
+    amino acid database
+    :return: allele_comprehension: nucleotide allele comprehension.
+    allele_comprehension[contig][full_range] = {gene:allele}
     """
     logging.info('Determining nucleotide allele profiles')
     # Initialise an empty allele comprehension dictionary
     allele_comprehension = {}
     # Iterate through all the samples
     for sample in runmetadata.samples:
-        # Extract hit information from the overlap dictionary
-        for contig, range_dict in sample.alleles.overlap_dict.items():
-            # Update the allele comprehension dictionary with the contig key as required
+        # Ensure that the proper dictionary is being evaluated. For nt samples
+        # against an aa database, sample.alleles.translated_overlap is used,
+        # as sample.alleles.overlap_dict has already been populated with
+        # the aa results
+        if translated:
+            try:
+                overlap_dict = sample.alleles.translated_overlap
+            except AttributeError:
+                overlap_dict = sample.alleles.overlap_dict
+        else:
+            overlap_dict = sample.alleles.overlap_dict
+        # Extract hit information from the dictionary
+        for contig, range_dict in overlap_dict.items():
+            # Update the allele comprehension dictionary with the contig key
+            # as required
             if contig not in allele_comprehension:
                 allele_comprehension[contig] = {}
             # Iterate through each query range with a hit in the current contig
             for query_range, gene_dict in range_dict.items():
                 # Update the dictionary with the query range key as required
                 if query_range not in allele_comprehension[contig]:
                     allele_comprehension[contig][query_range] = {}
-                # Iterate over each gene with a hit within this contig:query_range combination
+                # Iterate over each gene with a hit within this
+                # contig:query_range combination
                 for gene_pair, info_dict in gene_dict.items():
-                    # If the gene_pair variable is a string (instead of a tuple), there is only a single gene present
+                    # If the gene_pair variable is a string (instead of a
+                    # tuple), there is only a single gene present
                     if isinstance(gene_pair, str):
                         # Extract the gene_allele ID from the dictionary
                         corresponding_allele = info_dict['allele'][0]
-                        # Remove the gene name (and an underscore) from the corresponding_allele variable
-                        # (leaving only the allele ID)
-                        allele_number = corresponding_allele.replace(f'{gene_pair}_', '')
-                        # Update the allele comprehension dictionary with the gene name: alleleID
+                        # Extract the allele number
+                        allele_number = corresponding_allele.split('_')[-1]
+                        # Remove any metadata from the allele name
+                        if '|' in allele_number:
+                            allele_number = allele_number.split('|')[0]
+                        # Update the allele comprehension dictionary with the
+                        # gene name: alleleID
                         allele_comprehension[contig][query_range].update(
                             {gene_pair: allele_number}
                         )
-                        # Determine which gene(s) are missing from this contig:query_range
-                        missing = [other_gene for other_gene in gene_names if other_gene != gene_pair]
-                        # Populate the allele comprehension dictionary with the missing genes
+                        # Determine which gene(s) are missing from this
+                        # contig:query_range
+                        missing = [
+                            other_gene for other_gene in gene_names if
+                            other_gene.lower() != gene_pair.lower()
+                        ]
+                        # Populate the allele comprehension dictionary with
+                        # the missing genes
                         for missing_gene in missing:
-                            allele_comprehension[contig][query_range].update({missing_gene: '0'})
-                    # A tuple of gene names indicates that multiple co-located genes are present in this
-                    # contig:query_range combination
+                            missing_gene = missing_gene[0].lower() + \
+                                missing_gene[1:-1] + missing_gene[-1].upper()
+                            allele_comprehension[contig][query_range].update(
+                                {missing_gene: '0'}
+                            )
+                    # A tuple of gene names indicates that multiple co-located
+                    # genes are present in this contig:query_range combination
                     else:
                         # Iterate over each gene in the gene_pair tuple
                         for i, gene_name in enumerate(gene_pair):
-                            # Extract the gene_alleleID from the dictionary for this gene
+                            # Extract the gene_alleleID from the dictionary
+                            # for this gene
                             corresponding_allele = info_dict['allele'][i]
-                            # Remove the gene name information from the corresponding_allele variable
-
-                            if gene_name in corresponding_allele:
-                                allele_number = corresponding_allele.replace(f'{gene_name}_', '')
-                                # Update the dictionary with the new gene: allele number for the sample
-                                allele_comprehension[contig][query_range].update(
+                            # Remove the gene name information from the
+                            # corresponding_allele variable
+                            if gene_name.lower() in \
+                                    corresponding_allele.lower():
+                                allele_number = \
+                                    corresponding_allele.split('_')[-1]
+                                # Remove any metadata from the allele name
+                                if '|' in allele_number:
+                                    allele_number = allele_number.split('|')[0]
+                                # Update the dictionary with the new gene:
+                                # allele number for the sample
+                                allele_comprehension[contig][
+                                    query_range].update(
                                     {gene_name: allele_number}
                                 )
                             else:
-                                # Determine which gene(s) are not currently being examined
+                                # Determine which gene(s) are not currently
+                                # being examined
                                 corresponding_gene = [
-                                    other_gene for other_gene in gene_names if other_gene != gene_name
+                                    other_gene for other_gene in gene_names if
+                                    other_gene.lower() != gene_name.lower()
                                 ][0]
-                                allele_number = corresponding_allele.replace(f'{corresponding_gene}_', '')
-                                # Update the dictionary with the new gene: allele number for the sample
-                                allele_comprehension[contig][query_range].update(
-                                    {corresponding_gene: allele_number}
+                                corresponding_gene = \
+                                    corresponding_gene[0].lower() + \
+                                    corresponding_gene[1:-1] + \
+                                    corresponding_gene[-1].upper()
+                                allele_number = \
+                                    corresponding_allele.split('_')[-1]
+                                # Remove any metadata from the allele name
+                                if '|' in allele_number:
+                                    allele_number = allele_number.split('|')[0]
+                                # Update the dictionary with the new gene:
+                                # allele number for the sample
+                                allele_comprehension[contig][
+                                    query_range].update(
+                                    {
+                                        corresponding_gene: allele_number
+                                    }
                                 )
-        # If the allele_comprehension dictionary exists, it doesn't need to be further populated
+
+        # If the allele_comprehension dictionary exists, it doesn't need to be
+        # further populated
         if allele_comprehension:
             continue
         # Otherwise iterate through the targetsequence dictionary
-        for contig, range_dict in sample.alleles.targetsequence.items():
+        for contig in sample.alleles.targetsequence:
             # Update the allele comprehension dictionary as required
             if contig not in allele_comprehension:
                 allele_comprehension[contig] = {}
             # Iterate through all genes in the analysis
             for gene in gene_names:
                 # Set an 'empty' range as (0, 0)
                 full_range = (0, 0)
                 # Add the range to the dictionary as required
                 if full_range not in allele_comprehension[contig]:
                     allele_comprehension[contig][full_range] = {}
                 # Update the dictionary with the negative result
                 allele_comprehension[contig][full_range].update(
-                                {gene: '0'}
+                                {
+                                    gene: '0'
+                                }
                             )
     return allele_comprehension
 
 
 def create_aa_allele_comprehension(
         runmetadata: MetadataObject,
         gene_names: list):
     """
-    Create gene: amino acid allele ID comprehensions for each contig: range combination with hits
+    Create gene: amino acid allele ID comprehensions for each contig: range
+    combination with hits
     :param runmetadata: MetadataObject with list of GenObjects for each query
     :param gene_names: List of all gene names in the analysis
-    :return: allele_comprehension: amino acid allele comprehension. allele_comprehension[contig][full_range] =
-    {gene:allele}
+    :return: allele_comprehension: amino acid allele comprehension.
+    allele_comprehension[contig][full_range] = {gene:allele}
     """
     logging.info('Determining amino acid allele profiles')
     # Initialise a dictionary to store contig:query_range gene:alleleID results
     allele_comprehension = {}
     # Iterate through all the samples
     for sample in runmetadata.samples:
         # Iterate through all the contigs in the targetsequence dictionary
         for contig, range_dict in sample.alleles.targetsequence.items():
             # Update the dictionary as required
             if contig not in allele_comprehension:
                 allele_comprehension[contig] = {}
-            # If the current contig is not in the overlap dictionary, populate the allele comprehension with
-            # negative values
+            # If the current contig is not in the overlap dictionary, populate
+            # the allele comprehension with negative values
             if contig not in sample.alleles.overlap_dict:
                 # Iterate over every gene in the analysis
                 for gene in gene_names:
+                    gene = gene[0].lower() + gene[1:-1] + gene[-1].upper()
                     # Set the 'empty' value to (0, 0)
                     full_range = (0, 0)
                     # Update the dictionary with the negative values
                     if full_range not in allele_comprehension[contig]:
                         allele_comprehension[contig][full_range] = {}
                     allele_comprehension[contig][full_range].update(
                                     {gene: '0'}
                                 )
                 # The dictionary has been populated, so continue
                 continue
             # Extract all the ranges with hits in the overlap dictionary
             for full_range in sample.alleles.overlap_dict[contig]:
-                # Extract the query ranges with hits on the current contig in the targetsequence dictionary
+                # Extract the query ranges with hits on the current contig in
+                # the targetsequence dictionary
                 for query_range, gene_dict in range_dict.items():
                     # Determine if these two ranges have an overlap
-                    overlap = query_range[1] >= full_range[0] and full_range[1] >= query_range[0]
+                    overlap = query_range[1] >= full_range[0] and \
+                        full_range[1] >= query_range[0]
                     # If they do not overlap, they are not the same
                     if not overlap:
                         continue
                     # Update the dictionary as required
                     if full_range not in allele_comprehension[contig]:
                         allele_comprehension[contig][full_range] = {}
-                    # Create a list to store all genes in the analysis that do not have hits in the range
+                    # Create a list to store all genes in the analysis that do
+                    # not have hits in the range
                     missing_genes = []
                     # Iterate over all genes in the analysis
                     for gene in gene_names:
-                        # If the gene is not in the gene dictionary contained in the targetsequence dictionary,
-                        # add it to the list of missing genes
+                        # If the gene is not in the gene dictionary contained
+                        # in the targetsequence dictionary, add it to the list
+                        # of missing genes
                         if gene not in gene_dict:
                             missing_genes.append(gene)
                         # Otherwise, update the dictionary
                         else:
-                            # Extract the name of the gene:alleleID from gene_dict in the targetsequence dictionary
+                            # Extract the name of the gene:alleleID from
+                            # gene_dict in the targetsequence dictionary
                             full_allele = gene_dict[gene]['aa']['allele']
-                            # Remove the gene name information from the full_allele variable
-                            allele_number = full_allele.replace(f'{gene}_', '')
+                            # Extract the allele number
+                            allele_number = full_allele.split('_')[-1]
+                            # Remove any metadata from the allele name
+                            if '|' in allele_number:
+                                allele_number = allele_number.split('|')[0]
                             # Add the gene:alleleID to the dictionary
                             allele_comprehension[contig][full_range].update(
                                 {gene: allele_number}
                             )
-                    # Add any missing genes to the dictionary with negative values
+                    # Add any missing genes to the dictionary with negative
+                    # values
                     for gene in missing_genes:
-                        # Ensure that the gene isn't already present in the dictionary
-                        if gene not in allele_comprehension[contig][full_range]:
+                        gene = gene[0].lower() + gene[1:-1] + gene[-1].upper()
+                        # Ensure that the gene isn't already present in the
+                        # dictionary
+                        if gene not in \
+                                allele_comprehension[contig][full_range]:
                             allele_comprehension[contig][full_range].update(
                                     {gene: '0'}
                                 )
     return allele_comprehension
 
 
 def create_frozen_allele_comprehension(allele_comprehension: dict):
     """
     Freeze allele comprehension dictionaries
     :param allele_comprehension: Dictionary of contig:full_range: {gene:allele}
-    :return: frozen_allele_comprehension: Dictionary of contig:query_range: json.dumps({gene:allele}, sort_keys=True)
+    :return: frozen_allele_comprehension: Dictionary of contig:query_range:
+    json.dumps({gene:allele}, sort_keys=True)
     """
     # Initialise a dictionary to store the frozen allele comprehensions
     frozen_allele_comprehension = {}
     # Iterate over all the contigs with hits
     for contig, query_dict in allele_comprehension.items():
         # Update the frozen allele dictionary as required
         if contig not in frozen_allele_comprehension:
             frozen_allele_comprehension[contig] = {}
-        # Iterate over all the ranges and allele comprehensions on the current contig with hits
+        # Iterate over all the ranges and allele comprehensions on the current
+        # contig with hits
         for query_range, allele_dict in query_dict.items():
             # Freeze the allele comprehension
             frozen_allele_dict = json.dumps(allele_dict, sort_keys=True)
             # Update the dictionary with the range and the frozen allele string
             if query_range not in frozen_allele_comprehension[contig]:
-                frozen_allele_comprehension[contig][query_range] = frozen_allele_dict
+                frozen_allele_comprehension[contig][query_range] = \
+                    frozen_allele_dict
     return frozen_allele_comprehension
 
 
 def extract_novel_alleles(
         sample: MetadataObject,
         gene: str,
         genome_query: bool,
         amino_acid: bool,
         allele_path: str,
         report_path: str,
         cutoff=75):
     """
-    Extract the sequence of novel alleles from samples that do not have a 100% match
+    Extract the sequence of novel alleles from samples that do not have a
+    100% match
     :param sample: MetadataObject with list of GenObjects for each query
     :param gene: Name of current gene
-    :param genome_query: Boolean of whether the allele or the genome are the query
-    :param amino_acid: Variable indicating whether the current analyses are on DNA or
-    amino acid sequences
-    :param allele_path: Name and absolute path to folder containing allele files
-    :param report_path: Name and absolute path to folder in which reports are to be created
-    :param cutoff: The minimum percent identity cutoff to allow when considering the presence of a
+    :param genome_query: Bool of whether the allele or the genome are the query
+    :param amino_acid: Variable indicating whether the current analyses are on
+    DNA or amino acid sequences
+    :param allele_path: Name and absolute path to folder containing
+    allele files
+    :param report_path: Name and absolute path to folder in which reports are
+    to be created
+    :param cutoff: The minimum percent identity cutoff to allow when
+    considering the presence of a
     sequence in a query
     :return: sample: Updated sample
     :return: novel_allele: Name of novel alleles discovered
     :return: query_sequence: Sequence of novel alleles discovered
     """
     # Open the sequence profile file as a dictionary
     blastdict = DictReader(open(sample.alleles.blast_report, encoding='utf-8'),
@@ -1245,36 +1482,42 @@
     # Initialise the best hit value of 0
     best_hit = 0
     # Initialise strings to store the name and the sequence of novel alleles
     query_sequence = str()
     novel_allele = str()
     # Iterate through all the BLAST hits
     for row in blastdict:
-        # Extract the target id with the appropriate key depending on whether genome files
-        # are the query or the subject
+        # Extract the target id with the appropriate key depending on whether
+        # genome files are the query or the subject
         target_id = row['query_id'] if not genome_query else row['subject_id']
-        # Ensure that the gene name is present in the gene name + allele combination
+        # Ensure that the gene name is present in the gene name + allele
+        # combination
         if gene in target_id:
-            # Create a variable to store the value for percent identity, so it is easier to call
+            # Create a variable to store the value for percent identity, so
+            # it is easier to call
             perc_id = float(row['percent_match'])
-            # See if the percent identity for the current match is better than the previous best
-            # match, and is above the
-            # minimum cutoff threshold
+            # See if the percent identity for the current match is better than
+            # the previous best one, and is above the minimum cutoff threshold
             if perc_id > best_hit and perc_id >= cutoff:
-                # Set the start and end variables depending on whether genomes are the query
-                target_start = row['query_start'] if not genome_query else row['subject_start']
-                target_end = row['query_end'] if not genome_query else row['subject_end']
+                # Set the start and end variables depending on whether genomes
+                # are the query
+                target_start = row['query_start'] if not \
+                    genome_query else row['subject_start']
+                target_end = row['query_end'] if not genome_query else \
+                    row['subject_end']
                 target_seq = row['query_sequence']
-                # Determine if the orientation of the sequence is reversed compared to the reference
+                # Determine if the orientation of the sequence is reversed
+                # compared to the reference
                 if int(target_end) < int(target_start) and not amino_acid:
                     # Create a sequence object using BioPython
                     seq = Seq(target_seq)
                     # Calculate the reverse complement of the sequence
                     query_sequence = str(seq.reverse_complement())
-                # If the sequence is not reversed, use the sequence as it is in the output
+                # If the sequence is not reversed, use the sequence as it
+                # is in the output
                 else:
                     query_sequence = target_seq
                 best_hit = perc_id
 
     # If a query sequence was extracted, use it to update the allele database
     if query_sequence:
         novel_allele = update_allele_database(
@@ -1293,49 +1536,64 @@
         allele_path: str,
         report_path: str,
         amino_acid: bool):
     """
     Update the allele database with the novel allele extracted above
     :param gene: Name of the current gene being examined
     :param query_sequence: Sequence of the novel allele
-    :param allele_path: Name and absolute path to folder containing allele files
-    :param report_path: Name and absolute path to folder in which reports are to be created
-    :param amino_acid: Variable indicating whether the current analyses are on DNA or
-    amino acid sequences
+    :param allele_path: Name and absolute path to folder containing allele
+    files
+    :param report_path: Name and absolute path to folder in which reports are
+    to be created
+    :param amino_acid: Variable indicating whether the current analyses are on
+    DNA or amino acid sequences
     :return: novel_allele: Name of the novel allele entered into the database
     """
+    # Set the first character of the gene name to lowercase and the final
+    # character to uppercase
+    gene = gene[0].lower() + gene[1:-1] + gene[-1].upper()
     # Find the allele database file
-    allele_file = glob(os.path.join(allele_path, f'{gene}*.*fa*'))[0]
+    try:
+        allele_file = glob(os.path.join(allele_path, f'{gene}.*fa*'))[0]
+    except IndexError:
+        allele_file = os.path.join(allele_path, f'{gene}.fasta')
     # Set the appropriate molecule type based on the current analysis
     molecule = 'nt' if not amino_acid else 'aa'
     # Set the name of the novel allele file in the report path
-    new_alleles = os.path.join(report_path, f'{molecule}_{gene}_novel_alleles.fasta')
-    # Initialise a variable to store the name of the last allele in the database file
+    new_alleles = os.path.join(
+        report_path,
+        f'{molecule}_{gene}_novel_alleles.fasta'
+    )
+    # Initialise a variable to store the name of the last allele in the
+    # database file
     last_id = str()
     # Create a list to store all the allele records in the database
     records = []
-    # Iterate through all the records in the allele database
-    for record in SeqIO.parse(allele_file, 'fasta'):
-        # Add the records to the list
-        records.append(record)
-        # Update the last_id variable
-        last_id = record.id
-    # Try to separate the gene name from the allele e.g. MutS_1
     try:
+        # Iterate through all the records in the allele database
+        for record in SeqIO.parse(allele_file, 'fasta'):
+            # Add the records to the list
+            records.append(record)
+            # Update the last_id variable
+            last_id = record.id
+        # Try to separate the gene name from the allele e.g. MutS_1
         _, allele = last_id.rsplit('_', 1)
-    # If there is no allele, set the allele to 1
-    except ValueError:
+        # If there is no allele, set the allele to 1
+    except (FileNotFoundError, ValueError):
         allele = 1
-    # Typecase the variable to an integer
-    allele = int(allele)
-    # If the sequence type corresponds to an Enterobase number, use our local numbering scheme instead
-    if allele < 1000000:
-        allele = 999999
+    # Check if the allele is an integer. Otherwise, it will need to be cleaned
+    if not isinstance(allele, int):
+        # Clean up the allele name
+        allele = int(allele.split('|')[0])
     # Name the novel allele as the gene name _ allele number + 1
-    novel_allele = f'{gene}_{int(allele) + 1}'
+    novel_allele = f'{gene.capitalize()}_{allele + 1}'
+    if amino_acid:
+        novel_allele += f'|{len(query_sequence)}aa'
+    else:
+        novel_allele += f'|{len(query_sequence)}bp'
     # Create a SeqRecord of the allele using the novel allele name and sequence
     new_record = SeqRecord(
         seq=Seq(query_sequence),
         id=novel_allele,
         name='',
         description=''
     )
@@ -1344,15 +1602,16 @@
         SeqIO.write(
             sequences=new_record,
             handle=novel,
             format='fasta'
         )
     # Add the novel allele record to the list of all records
     records.append(new_record)
-    # Overwrite the existing allele database file with the updated list of records
+    # Overwrite the existing allele database file with the updated list
+    # of records
     with open(allele_file, 'w', encoding='utf-8') as alleles:
         SeqIO.write(
             sequences=records,
             handle=alleles,
             format='fasta'
         )
     return novel_allele
@@ -1364,29 +1623,31 @@
     :param runmetadata: MetadataObject with list of GenObjects for each query
     :return: Updated MetadataObject
     """
     logging.info('Translating allele sequences to amino acid')
     for sample in runmetadata.samples:
         # Initialise the dictionary to store the translated sequence
         sample.alleles.nt_alleles_translated = {}
-        for allele, allele_sequence_list in sample.alleles.targetsequence.items():
+        for allele, allele_sequence_list in \
+                sample.alleles.targetsequence.items():
             for allele_sequence in allele_sequence_list:
                 # Create a sequence object using BioPython
                 seq = Seq(allele_sequence)
                 try:
                     # Translate the sequence
                     aa_seq = str(seq.translate())
                 # BioPython cannot translate sequences with gaps (-)
                 except TranslationError:
                     # Remove all - from the sequence
                     allele_seq = allele_sequence.replace('-', '')
                     seq = Seq(allele_seq)
                     aa_seq = str(seq.translate())
-                # Ensure that the allele name exists (isn't an empty string) before adding
-                # allele name: translated sequence to the dictionary
+                # Ensure that the allele name exists (isn't an empty string)
+                # before adding allele name: translated sequence to
+                # the dictionary
                 if allele:
                     sample.alleles.nt_alleles_translated[allele] = aa_seq
     return runmetadata
 
 
 def match_profile(
         profile_data: dict,
@@ -1395,24 +1656,27 @@
         profile_file: str,
         genes: list,
         allele_comprehension: dict,
         molecule: str):
     """
     Match current profiles to any previously created profiles
     :param profile_data: Dictionary of seq_type: {gene name: allele ID}
-    :param frozen_allele_comprehension: Dictionary of json.dumps({gene name: allele ID}, sort_keys=True): seq_type
-    :param report_path: Name and absolute path to folder in which reports are to be created
+    :param frozen_allele_comprehension: Dictionary of json.dumps({gene name:
+    allele ID}, sort_keys=True): seq_type
+    :param report_path: Name and absolute path to folder in which reports are
+    to be created
     :param profile_file: Name and path of file containing reduced profiles
     :param genes: List of all genes in the analysis
     :param allele_comprehension: Dictionary of contig:full_range: {gene:allele}
-    :param molecule: String of the current molecule being processed. Options are "aa" and "nt"
+    :param molecule: String of the current molecule being processed. Options
+    are "aa" and "nt"
     :return: profile_matches: Dictionary of contig:query_range:seq_type_match
     """
-    # If the profile_data dictionary was not populated in the read_profiles methods,
-    # there is nothing to match
+    # If the profile_data dictionary was not populated in the read_profiles
+    # methods, there is nothing to match
     if not profile_data:
         return
     logging.info('Matching new %s profiles against profile file', molecule)
     profile_matches = {}
     # Extract all the profiles from the profile file (as a frozen string)
     frozen_profiles = freeze_profiles(
         profile_data=profile_data
@@ -1425,67 +1689,86 @@
                 # Extract the samples that match this profile
                 seq_type_match = frozen_profiles[frozen_allele_dict]
                 # Update the dictionary with the matching samples
                 if contig not in profile_matches:
                     profile_matches[contig] = {}
                 if query_range not in profile_matches[contig]:
                     profile_matches[contig][query_range] = seq_type_match
-            # The profile will not necessarily match any of the profiles found in the analysis
+            # The profile will not necessarily match any of the profiles
+            # found in the analysis
             except KeyError:
                 if contig not in profile_matches:
                     profile_matches[contig] = {}
                 # Update the profile file with this novel profile
                 profile_matches[contig][query_range] = update_profiles(
                     profile_file=profile_file,
                     report_path=report_path,
                     genes=genes,
                     allele_dict=allele_comprehension[contig][query_range],
                     molecule=molecule
                 )
                 # Update the profile_data dictionary with the new sequence type
-                profile_data[profile_matches[contig][query_range]] = allele_comprehension[contig][query_range]
+                profile_data[profile_matches[contig][query_range]] = \
+                    allele_comprehension[contig][query_range]
                 frozen_profiles = freeze_profiles(
                     profile_data=profile_data
                 )
     return profile_matches, frozen_profiles
 
 
 def freeze_profiles(profile_data: dict):
     """
-    Freeze profiles, so that the frozen {gene:allele} dictionary can be used as the key and the corresponding sequence
+    Freeze profiles, so that the frozen {gene:allele} dictionary can be used
+    as the key and the corresponding sequence
     type as the value
-    :param profile_data: Dictionary of all profiles in seq_type: {gene name: allele ID} format
-    :return: frozen_profiles: Dictionary of json.dumps({gene name: allele ID}, sort_keys=True): seq_type
+    :param profile_data: Dictionary of all profiles in seq_type: {gene name:
+    allele ID} format
+    :return: frozen_profiles: Dictionary of json.dumps({gene name: allele ID},
+    sort_keys=True): seq_type
     """
     # Initialise a dictionary to store the frozen profiles information
     frozen_profiles = {}
-    # Iterate over all the sequence type: {gene name: allele ID} pairs in the dictionary
+    # Iterate over all the sequence type: {gene name: allele ID} pairs in
+    # the dictionary
     for seq_type, allele_comprehension in profile_data.items():
+        if allele_comprehension is None:
+            continue
+        # Convert the gene allele dictionary to lower case
+        lower_comprehension = {}
+        for gene, allele in allele_comprehension.items():
+            lower_comprehension[gene.lower()] = allele
         # Freeze the allele comprehension
-        frozen_allele_comprehension = json.dumps(allele_comprehension, sort_keys=True)
+        frozen_allele_comprehension = json.dumps(
+            lower_comprehension,
+            sort_keys=True
+        )
         # Populate the dictionary with frozen_allele_comprehension: seq_type
         frozen_profiles[frozen_allele_comprehension] = seq_type
     return frozen_profiles
 
 
 def update_profiles(
         profile_file: str,
         report_path: str,
         genes: list,
         allele_dict: dict,
         molecule: str):
     """
-    Run methods to add novel profiles to the profile file. Determine the sequence type to use, and update the file
+    Run methods to add novel profiles to the profile file. Determine the
+    sequence type to use, and update the file
     :param profile_file: Name and path of file containing reduced profiles
-    :param report_path: Name and absolute path to folder in which reports are to be created
+    :param report_path: Name and absolute path to folder in which reports are
+    to be created
     :param genes: List of all genes in the analysis
-    :param allele_dict: Dictionary of a single allele comprehension. Extracted from
-    allele_comprehension[contig][query_range] = {gene: allele}
-    :param molecule: String of the current molecule being processed. Options are "aa" and "nt"
-    :return: next_seq_type: Integer of the sequence type assigned to the novel profile
+    :param allele_dict: Dictionary of a single allele comprehension. Extracted
+    from allele_comprehension[contig][query_range] = {gene: allele}
+    :param molecule: String of the current molecule being processed. Options
+    are "aa" and "nt"
+    :return: next_seq_type: Integer of the sequence type assigned to the
+    novel profile
     """
     # Extract the sequence type to use for the novel profile
     next_seq_type = return_next_seq_type(
         profile_file=profile_file
     )
     # Update the profile file
     created = update_profile_file(
@@ -1499,203 +1782,297 @@
     if not created:
         next_seq_type = 'N/A'
     return next_seq_type
 
 
 def return_next_seq_type(profile_file: str):
     """
-    Parse the profile file, and return the value for the next sequence type to be used. Local profiles will start at
-    1000000 in order to be distinct from Enterobase profiles
+    Parse the profile file, and return the value for the next sequence type
+    to be used.
     :param profile_file: Name and path of file containing reduced profiles
-    :return: last_seq_type + 1: Integer of the sequence type to be assigned to the novel profile
+    :return: last_seq_type + 1: Integer of the sequence type to be assigned
+    to the novel profile
     """
     # Open the profile file
     with open(profile_file, 'r', encoding='utf-8') as profile:
         # Create a list of all the lines in the file
         lines = profile.read().splitlines()
         # Extract the last value from the list of lines
         last_line = lines[-1]
-        # Split the line on tabs, and set the last_seq_type variable to the first entry e.g. 22\t3\t2\n yields a
+        # Split the line on tabs, and set the last_seq_type variable to the
+        # first entry e.g. 22\t3\t2\n yields a
         # sequence type of 22
         last_seq_type = last_line.split('\t')[0]
     # Typecase the variable to an integer
     int_last_seq_type = int(last_seq_type)
-    # If the sequence type corresponds to an Enterobase number, use our local numbering scheme instead
-    if int_last_seq_type < 1000000:
-        int_last_seq_type = 999999
     # Return the last sequence type + 1 to give the next sequence type
     return int_last_seq_type + 1
 
 
 def update_profile_file(
         profile_file: str,
         next_seq_type: int,
         allele_dict: dict,
         genes: list,
         report_path: str,
         molecule: str):
     """
-    Update the profile file with novel profile. Additionally, either create or update the novel_profiles.txt file
+    Update the profile file with novel profile. Additionally, either create or
+    update the novel_profiles.txt file
     with the same profile
     :param profile_file: Name and path of file containing reduced profiles
-    :param next_seq_type: Integer of the sequence type to be assigned to the novel profile
-    :param allele_dict: Dictionary of a single allele comprehension. Extracted from
-    allele_comprehension[contig][query_range] = {gene: allele}
+    :param next_seq_type: Integer of the sequence type to be assigned to the
+    novel profile
+    :param allele_dict: Dictionary of a single allele comprehension.
+    Extracted from allele_comprehension[contig][query_range] = {gene: allele}
     :param genes: List of all genes in the analysis
-    :param report_path: Name and absolute path to folder in which reports are to be created
-    :param molecule: String of the current molecule being processed. Options are "aa" and "nt"
+    :param report_path: Name and absolute path to folder in which reports are
+    to be created
+    :param molecule: String of the current molecule being processed. Options
+    are "aa" and "nt"
     :return bool: Boolean of whether the profile could be created or not
     """
-
-    # Initialise a string to store the profile information with the novel sequence type
+    # Initialise a variable to store whether the profile passes the filter
+    filter = False
+    # Initialise a string to store the profile information with the novel
+    # sequence type
     seq_type_str = f'{next_seq_type}'
     # Initialise a header to store 'ST  gene1   gene2.......geneX\n'
     header = 'ST'
     # Iterate over all the genes in the analysis
     for gene in genes:
         # Extract the allele ID for each gene in the analysis
         allele = allele_dict[gene]
-        # If the allele has been filtered return False, as a sequence type should not exist for filtered alleles
+        # If the allele has been filtered return False, as a sequence type
+        # should not exist for filtered alleles
         if not allele:
             return False
         # Check if the gene name is in the allele
-        if gene in allele:
+        if gene.lower() in allele.lower():
             # Extract the allele number
             allele = allele.split('_')[-1]
-
+        # Remove any metadata from the allele name
+        if '|' in allele:
+            allele = allele.split('|')[0]
+        # Check if the allele is 0, and if it is, set the filter variable
+        # to True
+        if allele == '0':
+            filter = True
         # Update the header with the gene
         header += f'\t{gene}'
         # Update the profile string with the allele ID
         seq_type_str += f'\t{allele}'
-    # Open the profile file (to update) and write the novel profile
-    with open(profile_file, 'a+', encoding='utf-8') as profile:
-        profile.write(seq_type_str + '\n')
-    # Set the name of the file containing novel profiles using the molecule variable ('aa' or 'nt')
-    novel_profile_file = os.path.join(report_path, f'{molecule}_novel_profiles.txt')
-    # Check to see if the novel profile file exists
-    if not os.path.isfile(novel_profile_file):
-        # If it does not exist, create it, and write the header line before the novel profile
-        with open(novel_profile_file, 'w', encoding='utf-8') as novel_profile:
-            novel_profile.write(header + '\n')
-            novel_profile.write(seq_type_str + '\n')
-    # Otherwise, update the existing file with the novel profile
+    # Check if last line in the file ends with a newline (or is an empty line)
+    with open(profile_file, 'r+', encoding='utf-8') as profile:
+        # Read all lines from the file into a list
+        lines = profile.readlines()
+        # Check if the list is not empty and the last line does not end with
+        # a newline
+        if lines and not lines[-1].endswith('\n'):
+            # If the last line does not end with a newline, append a newline
+            # character to it
+            lines[-1] += '\n'
+            # Move the file cursor to the beginning of the file
+            profile.seek(0)
+            # Write the lines back to the file
+            profile.writelines(lines)
+        # Check if the list is not empty and the last line is an empty line
+        elif lines and lines[-1] == '\n':
+            # If the last line is an empty line, remove it
+            lines = lines[:-1]
+            # Move the file cursor to the beginning of the file
+            profile.seek(0)
+            # Write the lines back to the file
+            profile.writelines(lines)
+    # Write filtered profiles to file
+    if filter:
+        # Set the name of the file containing filtered profiles using the
+        # molecule variable ('aa' or 'nt')
+        filtered_profile_file = os.path.join(
+            report_path,
+            f'{molecule}_filtered_profiles.txt'
+        )
+        # Check to see if the filtered profile file exists
+        if not os.path.isfile(filtered_profile_file):
+            with open(filtered_profile_file, 'w', encoding='utf-8') \
+                    as filtered_profile:
+                filtered_profile.write(header + '\n')
+                filtered_profile.write(seq_type_str + '\n')
+        else:
+            with open(filtered_profile_file, 'a+', encoding='utf-8') as \
+                    filtered_profile:
+                filtered_profile.write(seq_type_str + '\n')
+        return False
     else:
-        with open(novel_profile_file, 'a+', encoding='utf-8') as novel_profile:
-            novel_profile.write(seq_type_str + '\n')
-    return True
+        # Open the profile file (to update) and write the novel profile
+        with open(profile_file, 'a+', encoding='utf-8') as profile:
+            profile.write(seq_type_str + '\n')
+        # Set the name of the file containing novel profiles using the
+        # molecule variable ('aa' or 'nt')
+        novel_profile_file = os.path.join(
+            report_path,
+            f'{molecule}_novel_profiles.txt'
+        )
+        # Check to see if the novel profile file exists
+        if not os.path.isfile(novel_profile_file):
+            # If it does not exist, create it, and write the header line
+            # before the novel profile
+            with open(novel_profile_file, 'w', encoding='utf-8') as \
+                    novel_profile:
+                novel_profile.write(header + '\n')
+                novel_profile.write(seq_type_str + '\n')
+        # Otherwise, update the existing file with the novel profile
+        else:
+            with open(novel_profile_file, 'a+', encoding='utf-8') as \
+                    novel_profile:
+                novel_profile.write(seq_type_str + '\n')
+        return True
 
 
 def create_stec_report(
         runmetadata: MetadataObject,
         nt_profile_matches: dict,
         nt_alleles: dict,
         aa_profile_matches: dict,
         aa_alleles: dict,
         report_file: str,
         gene_names: list,
         aa_profile_path: str,
         notes: list):
     """
-    Create a STEC-specific report including the allele matches for each gene and sequence type for both nucleotide and
-    amino acid sequence information
+    Create a STEC-specific report including the allele matches for each gene
+    and sequence type for both nucleotide and amino acid sequence information
     :param runmetadata: MetadataObject with list of GenObjects for each query
-    :param nt_profile_matches: Dictionary of contig:query_range:nucleotide seq_type_match
-    :param nt_alleles: Dictionary of nucleotide contig:full_range:nucleotide seq_type_match
-    :param aa_profile_matches: Dictionary of contig:query_range:amino acid seq_type_match
-    :param aa_alleles: Dictionary of amino acid contig:full_range: {gene:allele}
+    :param nt_profile_matches: Dictionary of contig:query_range:nucleotide
+    seq_type_match
+    :param nt_alleles: Dictionary of nucleotide contig:full_range:nucleotide
+    seq_type_match
+    :param aa_profile_matches: Dictionary of contig:query_range:amino acid
+    seq_type_match
+    :param aa_alleles: Dictionary of amino acid contig:full_range:
+    {gene:allele}
     :param report_file: String of the name and path of the report file
     :param gene_names: List of all gene names in the analysis
-    :param aa_profile_path: String of the absolute path of the folder in which the amino acid profile file is located
+    :param aa_profile_path: String of the absolute path of the folder in which
+    the amino acid profile file is located
     :param notes: List of notes on the alleles
     """
     logging.info('Creating report')
-    # Set the appropriate order for the genes in the report (stx1 genes are not in numerical order)
+    # Set the appropriate order for the genes in the report
     gene_order = {
-        'stx1': ['ECs2974', 'ECs2973'],
-        'stx2': ['ECs1205', 'ECs1206']
+        'stx1': ['stx1A', 'stx1B'],
+        'stx2': ['stx2A', 'stx2B']
     }
     # Create a list to store the ordered genes
     ordered_genes = []
-    # Set the ordered genes according to the genes used in the current analysis (stx1 or stx2)
+    # Set the ordered genes according to the genes used in the current
+    # analysis (stx1 or stx2)
     for _, gene_list in gene_order.items():
-        # If the sorted list matches the list of genes in the analysis, use the unsorted list as the gene order
+        # If the sorted list matches the list of genes in the analysis, use
+        # the unsorted list as the gene order
         if sorted(gene_list) == gene_names:
             ordered_genes = gene_list
-    # Create a header for the report. Includes which alleles are present and the sequence type for both the nucleotide
+    # Create a header for the report. Includes which alleles are present and
+    # the sequence type for both the nucleotide
     # and amino acid sequences of the query and notes
-    header = f'Sample\tnt_{ordered_genes[0]}\tnt_{ordered_genes[1]}\tnt_seq_type\t' \
-             f'aa_{ordered_genes[0]}\taa_{ordered_genes[1]}\taa_seq_type\tnotes\n'
+    header = \
+        f'Sample\tnt_{ordered_genes[0]}\tnt_{ordered_genes[1]}\t' \
+        f'nt_seq_type\taa_{ordered_genes[0]}\taa_{ordered_genes[1]}\t' \
+        f'aa_seq_type\tnotes\n'
     # Create a string to store the query information
     data = str()
     # Iterate over the samples
     for sample in runmetadata.samples:
         # Iterate over all the contigs that had hits
         for contig, range_dict in nt_profile_matches.items():
-            # Iterate over the ranges: nucleotide profiles that had hits on this contig
+            # Iterate over the ranges: nucleotide profiles that had hits on
+            # this contig
             for query_range, nt_profile in range_dict.items():
                 # Update the data string with the sample name
                 data += f'{sample.name}\t'
-                # Extract the corresponding amino acid profile from aa_profile_matches
+                # Extract the corresponding amino acid profile from
+                # aa_profile_matches
                 aa_profile = aa_profile_matches[contig][query_range]
-                # Extract the allele dictionaries ({gene name: allele ID}) using the contig and query range
+                # Extract the allele dictionaries ({gene name: allele ID})
+                # using the contig and query range
                 nt_allele_dict = nt_alleles[contig][query_range]
                 aa_allele_dict = aa_alleles[contig][query_range]
-                # Iterate over the genes in the analysis to extract their corresponding nucleotide alleles
+                # Iterate over the genes in the analysis to extract their
+                # corresponding nucleotide alleles
                 for gene in ordered_genes:
                     # Update the string with the nucleotide allele ID
                     data += f'{nt_allele_dict[gene]}\t'
                 # Update the string with the nucleotide sequence type
                 data += f'{nt_profile}\t'
-                # Iterate over the genes in the analysis to extract their corresponding amino acid alleles
+                # Iterate over the genes in the analysis to extract their
+                # corresponding amino acid alleles
                 for gene in ordered_genes:
                     # Update the string with the amino acid allele ID
                     data += f'{aa_allele_dict[gene]}\t'
                 # Update the string with the amino acid sequence type
                 data += f'{aa_profile}\t'
-                # Create a list to store sample:contig:query_range-specific notes
+                # Create a list to store sample:contig:query_range-specific
+                # notes
                 note_list = []
-                # Determine if there are already notes for this contig in the notes dictionary
+                # Determine if there are already notes for this contig in the
+                # notes dictionary
                 if contig in notes:
-                    # Determine if there are already notes for this contig: range in the notes dictionary
+                    # Determine if there are already notes for this contig:
+                    # range in the notes dictionary
                     if query_range in notes[contig]:
-                        # Update the profile linking file. Use notes in the notes dictionary
+                        # Update the profile linking file. Use notes in the
+                        # notes dictionary
                         note_list = update_profile_link_file(
                             nt_seq_type=nt_profile,
                             aa_seq_type=aa_profile,
                             aa_profile_path=aa_profile_path,
                             note=notes[contig][query_range]
                         )
-                    # If there are no notes for the contig:range, create notes from scratch
+                    # If there are no notes for the contig:range, create notes
+                    # from scratch
                     else:
-                        # Update the profile linking file. Use notes in the notes_list list
+                        # Update the profile linking file. Use notes in the
+                        # notes_list list
                         note_list = update_profile_link_file(
                             nt_seq_type=nt_profile,
                             aa_seq_type=aa_profile,
                             aa_profile_path=aa_profile_path,
                             note=note_list
                         )
-                # If there are no notes for the contig, create notes from scratch
+                # If there are no notes for the contig, create notes from
+                # scratch
                 else:
-                    # Update the profile linking file. Use notes in the notes_list list
+                    # Update the profile linking file. Use notes in the
+                    # notes_list list
                     note_list = update_profile_link_file(
                         nt_seq_type=nt_profile,
                         aa_seq_type=aa_profile,
                         aa_profile_path=aa_profile_path,
                         note=note_list
                     )
                 # Join all the notes from the list with semicolons
-                note_str = '; '.join(note_list)
+                note_str = str()
+                for note in note_list:
+                    if isinstance(note, str):
+                        if note_str:
+                            note_str += f'; {note}'
+                        else:
+                            note_str += note
+                    else:
+                        note_str = '; '.join(note)
                 # Update the data string with the notes
                 data += f'{note_str}'
                 # Add a newline to the data string
                 data += '\n'
-        # If there were no hits for the sample, add negative values to the data string
+        # If there were no hits for the sample, add negative values to the
+        # data string
         if not data:
             data = f'{sample.name}\t0\t0\t1\t0\t0\t1\n'
-    # If the report file does not already exist, write the header and data strings
+    # If the report file does not already exist, write the header and data
+    # strings
     if not os.path.isfile(report_file):
         with open(report_file, 'w', encoding='utf-8') as report:
             report.write(header)
             report.write(data)
     # If the report already exists, write only the data string
     else:
         with open(report_file, 'a+', encoding='utf-8') as report:
@@ -1704,86 +2081,107 @@
 
 def update_profile_link_file(
         nt_seq_type: str,
         aa_seq_type: str,
         note: list,
         aa_profile_path: str):
     """
-    Update the file linking amino acid sequence type to the (multiple) corresponding nucleotide sequence type(s)
+    Update the file linking amino acid sequence type to the (multiple)
+    corresponding nucleotide sequence type(s)
     :param nt_seq_type: String of the nucleotide sequence type
     :param aa_seq_type: String of the amino acid sequence type
     :param note: List of notes on the alleles
-    :param aa_profile_path: String of the absolute path of the folder in which the amino acid profile file is located
+    :param aa_profile_path: String of the absolute path of the folder in which
+    the amino acid profile file is located
     :return: note: Update list of notes
     """
     # Set the name of the link file
     link_file = os.path.join(aa_profile_path, 'aa_nt_profile_links.tsv')
     # Create a dictionary of nucleotide sequence type matches
     nt_match = {}
-    # Initialise a boolean to track whether the amino acid sequence type is already present in the profile link file
+    # Initialise a boolean to track whether the amino acid sequence type is
+    # already present in the profile link file
     aa_match = False
     # Initialise a dictionary to store the aa_seq_type: nt_seq_type(s)
     links = {}
     # Initialise a list of all amino acid sequence types present the file
     records = []
+    # Ensure that the file exists
+    if not os.path.isfile(link_file):
+        # Create the file
+        with open(link_file, 'a', encoding='utf-8') as _:
+            pass
     # Open the profile link file to read in the contents
     with open(link_file, 'r', encoding='utf-8') as profile_link:
         for line in profile_link:
-            # Split the amino acid sequence type from the nucleotide sequence type(s)
-            # e.g 1 1 or 116 116;125;187;39973;92286;1000005
+            # Split the amino acid sequence type from the nucleotide sequence
+            # type(s) e.g 1 1 or 116 116;125;187;39973;92286;1000005
             aa_seq, nt_seq = line.split('\t')
-            # Check to see if the extracted amino acid sequence type matches the sequence type of the sample
+            # Check to see if the extracted amino acid sequence type matches
+            # the sequence type of the sample
             if aa_seq_type == aa_seq:
                 # Set the match boolean to True (there is a match)
                 aa_match = True
-                # Check to see if the nucleotide sequence type of sample is in the semicolon-separated list of
-                # nucleotide sequence types corresponding to the amino acid sequence type
+                # Check to see if the nucleotide sequence type of sample is in
+                # the semicolon-separated list of nucleotide sequence types
+                # corresponding to the amino acid sequence type
                 if nt_seq_type in nt_seq.rstrip().split(';'):
                     # Update the nucleotide sequence type match dictionary
                     nt_match[aa_seq] = nt_seq.rstrip()
             # Update the link dictionary
             links[aa_seq] = nt_seq.rstrip()
             # Add the amino acid sequence type to the list
             records.append(aa_seq)
     # Check if the amino acid of the sample matched a previous sequence type
     if aa_match:
         # Check if there was a match of the sample's nucleotide sequence type
         if not nt_match:
-            # Append the nucleotide sequence type to the string of nucleotide sequence type matches
+            # Append the nucleotide sequence type to the string of nucleotide
+            # sequence type matches
             links[aa_seq_type] += f';{nt_seq_type}'
             # Update the note
-            note.append(f'Novel nt_seq_type {nt_seq_type} links to aa_seq type {aa_seq_type}')
+            note.append(
+                f'Novel nt_seq_type {nt_seq_type} links to aa_seq '
+                f'type {aa_seq_type}'
+            )
     # If no match, this is a novel amino acid sequence type
     else:
-        # Update the link dictionary novel amino acid sequence type: novel nucleotide sequence type
+        # Update the link dictionary novel amino acid sequence type: novel
+        # nucleotide sequence type
         links[aa_seq_type] = nt_seq_type
         # Add the novel sequence type to the list
         records.append(aa_seq_type)
         # Update the notes
-        note.append(f'Novel nt_seq_type {nt_seq_type}, and aa_seq_type {aa_seq_type}')
+        note.append(
+            f'Novel nt_seq_type {nt_seq_type}, and aa_seq_type {aa_seq_type}'
+        )
     # Overwrite the profile link file with the updated links
     with open(link_file, 'w', encoding='utf-8') as profile_link:
         for record in records:
             profile_link.write(f'{record}\t{links[record]}\n')
     return note
 
 
 def split_alleles(
         allele_files: list,
         output_path: str):
     """
     Split FASTA files into individual sequences
-    :param allele_files: List of absolute path to FASTA-formatted allele sequence files
-    :param output_path: String of the absolute path into which the individual sequence files are to be written
+    :param allele_files: List of absolute path to FASTA-formatted allele
+    sequence files
+    :param output_path: String of the absolute path into which the individual
+    sequence files are to be written
     """
     # Create the output path if it doesn't already exist
     make_path(inpath=output_path)
     # Ensure that the path could be created
     if not os.path.isdir(output_path):
-        logging.error('Could not create desired output folder: %s', output_path)
+        logging.error(
+            'Could not create desired output folder: %s', output_path
+        )
         raise SystemExit
     # Iterate over all the allele files
     for allele_file in allele_files:
         # Use SeqIO to load all the records in the file
         for record in SeqIO.parse(allele_file, 'fasta'):
             # Set the name of the file to be the FASTA header
             output_file = os.path.join(output_path, f'{record.id}.fasta')
@@ -1800,140 +2198,434 @@
         notes: list,
         aa_allele_path: str,
         report_path: str,
         cutoff: int):
     """
     Parse amino acid BLAST results
     :param runmetadata: MetadataObject with list of GenObjects for each query
-    :param extended_fieldnames: List of the BLAST fields used, as well as the additional percent
-    match in index 14
+    :param extended_fieldnames: List of the BLAST fields used, as well as the
+    additional percent match in index 14
     :param fieldnames: List of the BLAST fields used
     :param gene_names: List of all gene names in the analysis
     :param notes: List of sample-specific notes
-    :param aa_allele_path: String of the absolute path to the folder containing amino acid allele files
-    :param report_path: String of the absolute path to the folder into which reports are to be written
-    them to be considered co-located. Default is 50 bp
-    :param cutoff: Integer of the minimum percent identity between query and subject sequence.
-    Default is 90
+    :param aa_allele_path: String of the absolute path to the folder
+    containing amino acid allele files
+    :param report_path: String of the absolute path to the folder into which
+    reports are to be written
+    :param cutoff: Integer of the minimum percent identity between query and
+    subject sequence. Default is 90
     :return: runmetadata: Updated MetadataObject
-    :return: filtered: Boolean of whether the sample fails quality/length checks
+    :return: filtered: Bool of whether the sample fails quality/length checks
     :return: notes: Updated list of sample-specific notes
     """
     logging.info('Parsing BLAST outputs')
     # Initialise a boolean to track if the sequence fails checks
     filtered = False
     for sample in runmetadata.samples:
         # Initialise GenObjects as required
         sample.alleles.blastlist = []
         sample.alleles.targetsequence = {}
         # Read the BLAST outputs into a dictionary
         blastdict = create_blast_dict(
             sample=sample,
             extended_fieldnames=extended_fieldnames
         )
-        # Initialise a boolean to track whether this contig:query_range has already been processed
-        processed = False
+        # Initialise dictionaries to store hit information
+        processed_range_dict = {}
+        colocation_dict = {}
         # Go through each BLAST result
         for row in blastdict:
+            aa_allele = str()
             # Ignore the headers
             if row['query_id'].startswith(fieldnames[0]):
                 continue
+            processed = False
             # Create variables to reduce extra typing and for extra clarity
             target_id = row['subject_id']
             percent_id = float(row['percent_match'])
+            contig = row['query_id']
+            high = max([int(row['query_start']), int(row['query_end'])])
+            low = min([int(row['query_start']), int(row['query_end'])])
+            # Create a list of the properly ordered start and stop points of
+            # the match
+            query_range = [low, high]
+            # Create a tuple of the query range list to allow it to be used as
+            # a dictionary key
+            query_range_tuple = tuple(query_range)
+            # Populate the notes dictionary
+            if contig not in notes:
+                notes[contig] = {}
+            if query_range_tuple not in notes[contig]:
+                notes[contig][query_range_tuple] = []
+            # Add the contig key to the dictionary as required
+            if contig not in processed_range_dict:
+                processed_range_dict[contig] = set()
+            # Check the processed range dictionary to see if the current range
+            # is present
+            if processed_range_dict[contig]:
+                for previous_range in processed_range_dict[contig]:
+                    # Allow a small overlap of five bases in case the range of
+                    # one query is slightly different
+                    overlap = query_range[1] + 5 >= previous_range[0] and \
+                              previous_range[1] + 5 >= query_range[0]
+                    # If the range is already present in the dictionary,
+                    # update the tracking boolean
+                    if overlap:
+                        processed = True
+            # Add the range to the set if it is empty
+            else:
+                processed_range_dict[contig].add(query_range_tuple)
+            # Do not evaluate this contig:query_range if it has already been
+            # processed
+            if processed:
+                continue
             # If the match is perfect
             if percent_id == 100:
                 # Add the name of the matching allele to the list
                 sample.alleles.blastlist.append(target_id)
-                # Update the processed boolean to indicate that this region has been processed
+                # Extract the allele number from the subject name e.g.
+                # Stx1A_1|315aa yields Stx1A_1
+                aa_allele = target_id.split('|')[0]
+                # Update the processed boolean to indicate that this region
+                # has been processed
                 processed = True
             # If the match is imperfect, but greater than the cutoff
-            elif cutoff < percent_id < 100 and not processed:
-                # Determine which gene is being processed by finding the match of the genes against the allele
-                gene = [gene for gene in gene_names if gene in target_id][0]
+            elif cutoff < percent_id < 100 and not processed and not filtered:
+                # Determine which gene is being processed by finding the match
+                # of the genes against the allele
+                gene = [
+                    gene for gene in gene_names if gene.lower() in
+                    target_id.lower()
+                ][0]
                 query_seq = row['query_sequence']
-                # Evaluate the sequence for length, as well as required start/stop codons
-                filtered, notes = evaluate_translated_allele(
+                # Evaluate the sequence for length, as well as required
+                # start/stop codons
+                filtered, notes[contig][query_range_tuple], query_seq = \
+                    evaluate_translated_allele(
                     aa_seq=query_seq,
                     gene=gene,
-                    notes=notes,
-                    aa=True
+                    notes=notes[contig][query_range_tuple]
                 )
                 # Find the next available allele identifier in the database
                 aa_allele_id = find_next_allele(
                     gene=gene,
                     allele_path=aa_allele_path
                 )
-                # Set the name of the allele as gene_alleleID
-                aa_allele = f'{gene}_{aa_allele_id}'
+                # Set the name of the allele depending on whether it was
+                # filtered
+                if not filtered:
+                    # Set the name of the allele as gene_alleleID
+                    aa_allele = f'{gene.capitalize()}_{aa_allele_id}|' \
+                        f'{len(query_seq)}aa'
+                else:
+                    aa_allele = f'Filtered_{gene.capitalize()}_' \
+                        f'{aa_allele_id}|{len(query_seq)}aa'
+                # Populate the notes dictionary
+                if contig not in notes:
+                    notes[contig] = {}
+                if query_range_tuple not in notes[contig]:
+                    notes[contig][query_range_tuple] = []
                 # Update the allele database with the novel allele
-                notes, aa_allele = update_allele_databases(
+                notes[contig][query_range_tuple], aa_allele = \
+                    update_allele_databases(
                     query_sequence=query_seq,
                     header=aa_allele,
                     filtered=filtered,
                     gene=gene,
                     report_path=report_path,
                     allele_path=aa_allele_path,
-                    notes=notes,
+                    notes=notes[contig][query_range_tuple],
                     molecule='Amino acid'
                 )
-                # If the allele passes the necessary checks, update the list of results
+                # If the allele passes the necessary checks, update the list
+                # of results
                 if not filtered:
                     sample.alleles.blastlist.append(aa_allele)
                 # Update the processed boolean
                 processed = True
+            # Do not process any sequences that are either already processed,
+            # or below the cutoff
+            if not processed:
+                continue
+            if filtered:
+                continue
+            # Create a list of the properly ordered start and stop points of
+            # the match
+            query_range = [low, high]
+            # Add the contig key to the dictionary as required
+            if contig not in processed_range_dict:
+                processed_range_dict[contig] = set()
+            # Update the processed ranges dictionary with the current range
+            processed_range_dict[contig].add(tuple(query_range))
+            # Create a tuple of the query range list to allow it to be used as
+            # a dictionary key
+            query_range_tuple = tuple(query_range)
+            # Add keys to the targetsequence dictionary as required
+            if contig not in sample.alleles.targetsequence:
+                sample.alleles.targetsequence[contig] = {}
+            if query_range_tuple not in sample.alleles.targetsequence[contig]:
+                sample.alleles.targetsequence[contig][query_range_tuple] = {}
+            # Determine the name of the gene corresponding to the allele e.g.
+            # gene = stx1A allele = Stx1A_1|315aa will create stx1A
+            base_gene = [
+                gene_name for gene_name in gene_names if gene_name.lower()
+                in target_id.lower()
+            ][0]
+            # Populate the targetsequence dictionary with information on the
+            # nt and aa alleles
+            if base_gene not in \
+                    sample.alleles.targetsequence[contig][query_range_tuple]:
+                sample.alleles.targetsequence[contig][
+                    query_range_tuple][base_gene] = {
+                    'nt': {
+                        'allele': '',
+                        'sequence': extract_nt_sequence(
+                            sample=sample,
+                            row=row
+                        )
+                    },
+                    'aa': {
+                        'allele': aa_allele,
+                        'sequence': row['query_sequence'].split('*')[0]
+                    }
+                }
+            # Populate the co-location dictionary with the required keys as
+            # necessary
+            if contig not in colocation_dict:
+                colocation_dict[contig] = {}
+            # The query_ranges and target keys both correspond to lists of
+            # values
+            if 'query_ranges' not in colocation_dict[contig]:
+                colocation_dict[contig] = {
+                    'query_ranges': [query_range],
+                    'target': [aa_allele]
+                }
+            # If the keys already exist, append to the lists
+            else:
+                colocation_dict[contig]['query_ranges'].append(query_range)
+                colocation_dict[contig]['target'].append(aa_allele)
+        sample.alleles.overlap_dict = colocation_calculation(
+            colocation_dict=colocation_dict,
+            gene_names=gene_names,
+            overlap_range=50
+        )
     return runmetadata, filtered, notes
 
 
+def extract_nt_sequence(
+        sample: GenObject,
+        row: dict):
+    """
+    Extract the nucleotide sequence from a file given the contig name as well
+    as the start and stop locations
+    :param sample: GenObject of current query
+    :param row: Dictionary from DictReader object created from BLAST outputs
+    :return nt_querysequence: String of extract nucleotide sequence
+    """
+    nt_querysequence = str()
+    for record in SeqIO.parse(sample.general.bestassemblyfile, 'fasta'):
+        # Ensure that the correct contig is being considered
+        if record.id == row['query_id']:
+            start = int(row['query_start'])
+            stop = int(row['query_end'])
+            # Ensure that the query sequence is returned in the proper
+            # orientation
+            if stop < start:
+                # Create a Seq object of the slice of the sequence
+                seq = Seq(record.seq[stop - 1:start])
+                # Calculate the reverse complement of the sequence
+                nt_querysequence = str(seq.reverse_complement())
+            else:
+                nt_querysequence = str(Seq(record.seq[start - 1:stop]))
+    return nt_querysequence
+
+
 def analyse_aa_alleles(
         runmetadata: MetadataObject,
         gene_names: list,
         notes: list):
     """
     Analyse supplied amino acid alleles to ensure that they pass quality checks
     :param runmetadata: MetadataObject with list of GenObjects for each query
     :param gene_names: List of all gene names in the analysis
     :param notes: List of sample-specific notes
     :return: runmetadata: Updated MetadataObject
     :return: notes: Updated list of sample-specific notes
     """
     # Iterate through all the samples
     for sample in runmetadata.samples:
-        # Iterate over all the records in the file (should only be one, as these files must be split with the
+        # Iterate over all the records in the file (should only be one, as
+        # these files must be split with the
         # split_alleles function)
-        for record in SeqIO.parse(sample.general.bestassemblyfile, 'fasta'):
-            # Determine to which gene the allele corresponds
-            gene = [gene for gene in gene_names if gene in record.id][0]
-            # Perform content/length checks
-            filtered, notes = evaluate_translated_allele(
-                aa_seq=record.seq,
-                gene=gene,
-                notes=notes,
-                aa=True
-            )
+        for contig, query_range_dict in sample.alleles.targetsequence.items():
+            if contig not in notes:
+                notes[contig] = {}
+            for query_range, base_gene_dict in query_range_dict.items():
+                if query_range not in notes[contig]:
+                    notes[contig][query_range] = []
+                for base_gene in base_gene_dict:
+                    # Perform content/length checks
+                    filtered, notes, seq = evaluate_translated_allele(
+                        aa_seq=sample.alleles.targetsequence[
+                            contig][query_range][base_gene]['aa']['sequence'],
+                        gene=base_gene,
+                        notes=notes[contig][query_range]
+                    )
     return runmetadata, notes
 
 
+def translated_update_nucleotide(
+        runmetadata: MetadataObject,
+        nt_allele_path: str,
+        report_path: str,
+        notes: dict,
+        gene_names: list,
+        filtered: bool,
+        overlap_range: int = 50):
+    """
+    Search nucleotide allele databases to determine whether the corresponding
+    allele already exists
+    :param runmetadata: MetadataObject with list of GenObjects for each query
+    :param nt_allele_path: Name and absolute path to folder containing
+    nucleotide alleles
+    :param report_path: String of the absolute path to the folder into which
+    reports are to be written
+    :param notes: List of sample-specific notes
+    :param gene_names: List of all gene names in the analysis
+    :param filtered: Boolean of whether the sample fails quality/length checks
+    :param overlap_range: Integer of the number of base pairs that must
+    overlap for two alleles to be considered
+    :return: runmetadata: Updated MetadataObject
+    :return: notes: Updated list of sample-specific notes
+    """
+    # Iterate through all the samples
+    colocation_dict = {}
+    for sample in runmetadata.samples:
+        for contig, range_dict in sample.alleles.targetsequence.items():
+            for query_range_tuple, gene_dict in range_dict.items():
+                for gene, molecule_dict in gene_dict.items():
+                    # for molecule, info_dict in molecule_dict.items():
+                    nt_length = len(molecule_dict['nt']['sequence'])
+                    aa_length = len(molecule_dict['aa']['sequence']) * 3
+                    # If the length of the nucleotide sequence is greater than
+                    # the length of the amino acid sequence
+                    if nt_length > aa_length:
+                        # Truncate the nucleotide sequence to the length of
+                        # the amino acid sequence
+                        molecule_dict['nt']['sequence'] = molecule_dict[
+                            'nt']['sequence'][:aa_length]
+                        # Update the length of the nucleotide sequence
+                        nt_length = len(molecule_dict['nt']['sequence'])
+
+                    # Get the nucleotide sequence
+                    nt_sequence = molecule_dict['nt']['sequence']
+
+                    # Look up the allele ID for the nucleotide sequence
+                    nt_allele_id = nt_allele_lookup(
+                        nt_seq=nt_sequence,
+                        gene=gene,
+                        nt_allele_path=nt_allele_path
+                    )
+
+                    # Find the next allele ID
+                    nt_allele_id = find_next_allele(
+                        gene=gene,
+                        allele_path=nt_allele_path
+                    )
+
+                    # Construct the allele name
+                    nt_allele = f'{gene.capitalize()}_{nt_allele_id}|' \
+                        f'{len(nt_sequence)}nt'
+
+                    # Update the allele databases and get the updated notes
+                    # and allele
+                    notes[contig][query_range_tuple], nt_allele = \
+                        update_allele_databases(
+                        query_sequence=nt_sequence,
+                        header=nt_allele,
+                        filtered=False,
+                        gene=gene,
+                        report_path=report_path,
+                        allele_path=nt_allele_path,
+                        notes=notes[contig][query_range_tuple],
+                        molecule='Nucleotide'
+                    )
+                    # Populate the co-location dictionary with the required
+                    # keys as necessary
+                    if contig not in colocation_dict:
+                        colocation_dict[contig] = {}
+                    # The query_ranges and target keys both correspond to
+                    # lists of values
+                    if 'query_ranges' not in colocation_dict[contig]:
+                        colocation_dict[contig] = {
+                            'query_ranges': [query_range_tuple],
+                            'target': [nt_allele]
+                        }
+                    # If the keys already exist, append to the lists
+                    else:
+                        colocation_dict[contig]['query_ranges'].append(
+                            query_range_tuple
+                        )
+                        colocation_dict[contig]['target'].append(nt_allele)
+                    # Populate the overlap dictionary
+                    sample.alleles.translated_overlap = colocation_calculation(
+                        colocation_dict=colocation_dict,
+                        gene_names=gene_names,
+                        overlap_range=overlap_range
+                    )
+    return runmetadata, notes
+
+
+def nt_allele_lookup(
+        nt_seq: str,
+        gene: str,
+        nt_allele_path: str):
+    """
+    Read in the nucleotide allele file. Search for exact matches to the
+    current sequence
+    :param nt_seq: String of the nucleotide sequence
+    :param gene: Sting of the gene name
+    :param nt_allele_path: String of the absolute path to the folder
+    containing the amino acid
+    allele files
+    :return record.id: Allele identifier corresponding to the sequence
+    matching the nt_seq
+    if no matches: return None
+    """
+    # Set the name of the amino acid allele file by joining the allele folder
+    # path to the gene name
+    nt_allele_file = os.path.join(nt_allele_path, f'{gene}.fasta')
+    # Iterate through all the alleles in the file
+    for record in SeqIO.parse(nt_allele_file, 'fasta'):
+        # If the sequence in the file matches the current sequence, return the
+        # allele identifier
+        if nt_seq == str(record.seq):
+            return record.id
+    return None
+
+
 def report_aa_alleles(
         runmetadata: MetadataObject,
         report_file: str,
         notes: list):
     """
-    Create an amino acid query-specific report with sample name, allele match, and notes
+    Create an amino acid query-specific report with sample name, allele match,
+    and notes
     :param runmetadata: MetadataObject with list of GenObjects for each query
     :param report_file: String of absolute path to the report file
     :param notes: List of sample-specific notes
     """
     # Initialise the header string
     header = 'Sample\tMatch\tNotes\n'
     # Create an empty string to store the sample-specific results
     data = str()
     # Iterate over all the samples
     for sample in runmetadata.samples:
-        # Extract the list of hits from the MetadataObject, and join with semicolons
+        # Extract the list of hits from the MetadataObject, and join with
+        # semicolons
         matches = ';'.join(sample.alleles.blastlist)
         # Join the list of notes with
         note = ';'.join(notes)
         # Populate the data string with the matches and notes
         data += f'{sample.name}\t{matches}\t{note}\n'
     # If the report doesn't already exist write the header and data string
     if not os.path.isfile(report_file):
@@ -1950,27 +2642,31 @@
         allele_path: str,
         allele_order: dict):
     """
     Use SeqIO to read in allele files
     :param str allele_path: Name and path of folder containing allele files
     :param dict allele_order: Dictionary of stx gene name: allele order to use
     :return: str stx_gene: Name of stx gene (stx1 or stx2) being concatenated
-    :return: dict allele_dict: Dictionary of stx gene name: allele name: allele sequence
+    :return: dict allele_dict: Dictionary of stx gene name: allele name:
+    allele sequence
     """
-    # Initialise variable to store the stx gene name being analysed and the sequence of the alleles
+    # Initialise variable to store the stx gene name being analysed and the
+    # sequence of the alleles
     stx_gene = None
     allele_dict = {}
     # Find all the allele files in the folder
     allele_files = glob(os.path.join(allele_path, '*.fasta'))
     for allele_file in allele_files:
-        # Set the name of the subunit by splitting off the path information and the file extension from the file
+        # Set the name of the subunit by splitting off the path information
+        # and the file extension from the file
         allele_name = os.path.splitext(os.path.basename(allele_file))[0]
         # Determine which stx gene is being processed
         for gene_name, alleles in allele_order.items():
-            # The name of the current subunit is present in the list of subunits linked to the stx gene
+            # The name of the current subunit is present in the list of
+            # subunits linked to the stx gene
             if allele_name in alleles:
                 stx_gene = gene_name
         # Initialise the subunit name in the dictionary as required
         if allele_name not in allele_dict:
             allele_dict[allele_name] = {}
         # Use SeqIO to read in the allele file
         for record in SeqIO.parse(handle=allele_file, format='fasta'):
@@ -1984,67 +2680,80 @@
         allele_dict: dict,
         allele_order: dict,
         stx_gene: str,
         linker_length_dict: dict,
         molecule: str):
     """
 
-    :param profile_data: Dictionary of all profiles in seq_type: {gene name: allele ID} format
-    :param allele_dict: Dictionary of stx gene name: allele name: allele sequence
+    :param profile_data: Dictionary of all profiles in seq_type: {gene name:
+    allele ID} format
+    :param allele_dict: Dictionary of stx gene name: allele name:
+    allele sequence
     :param dict allele_order: Dictionary of stx gene name: allele order to use
     :param str stx_gene: Name of stx gene (stx1 or stx2) being concatenated
-    :param dict linker_length_dict: Dictionary of gene name: length of linker sequence to use
-    :param str molecule: String of the current molecule. Options are "nt" (nucleotide) and "aa" (amino acid)
-    :return: concatenated_sequences: List of SeqRecords for all concatenated sequences
+    :param dict linker_length_dict: Dictionary of gene name: length of linker
+    sequence to use
+    :param str molecule: String of the current molecule. Options are "nt"
+    (nucleotide) and "aa" (amino acid)
+    :return: concatenated_sequences: List of SeqRecords for all
+    concatenated sequences
     """
     # Create a list to store SeqRecords of the concatenated sequences
     concatenated_sequences = []
     # Iterate over all the sequence type: profile pairs in profile_data
     for seq_type, profile in profile_data.items():
         # Initialise a string to store the concatenated sequences
         concatenated_seq = str()
-        # Create a boolean to store if one (or both) of the allele subunits is missing
+        # Create a boolean to store if one (or both) of the allele subunits
+        # is missing
         complete = True
         # Create a variable to store the name of the concatenated allele
         concatenated_name = str()
         # Iterate over the subunits in order from the allele_order dictionary
         for subunit in allele_order[stx_gene]:
-            # Extract the allele number from the profile dictionary using the subunit as the key
+            # Extract the allele number from the profile dictionary using the
+            # subunit as the key
             allele_number = profile[subunit]
-            # If the allele number is 0, the subunit is absent, and the concatenated sequence will not be created
+            # If the allele number is 0, the subunit is absent, and the
+            # concatenated sequence will not be created
             if allele_number == '0':
                 complete = False
                 continue
-            # Set the full allele name by joining the subunit with the allele number
+            # Set the full allele name by joining the subunit with the
+            # allele number
             full_allele_name = f'{subunit}_{allele_number}'
-            # Extract the string of the allele sequence from the allele dictionary
+            # Extract the string of the allele sequence from the allele
+            # dictionary
             allele_seq = allele_dict[subunit][full_allele_name]
-            # If the first subunit is already present, simply append the second subunit to the string
+            # If the first subunit is already present, simply append the
+            # second subunit to the string
             if concatenated_seq:
                 concatenated_seq += allele_seq
             # Otherwise the linker sequence must be created
             else:
                 # Extract the gene-specific linker length from the dictionary
                 linker_length = linker_length_dict[stx_gene]
                 # Nucleotide sequences will use N as the linker sequence
                 if molecule == 'nt':
                     linker = 'N' * linker_length
-                # Amino acid sequences will use X as the linker sequence, and will be reduced by a factor of three
+                # Amino acid sequences will use X as the linker sequence,
+                # and will be reduced by a factor of three
                 else:
                     linker = 'X' * int(linker_length / 3)
                 concatenated_seq += f'{allele_seq}{linker}'
             # Update the name of the concatenated sequence
             if concatenated_name:
                 concatenated_name += f'_{allele_number}'
             else:
                 concatenated_name = allele_number
         # Do not add incomplete sequences to the list
         if not complete:
             continue
-        # Create a SeqRecord of the allele using the novel allele name and sequence
+        # Create a SeqRecord of the allele using the novel allele name
+        # and sequence
         concatenated_sequences.append(
             SeqRecord(
                 seq=Seq(concatenated_seq),
                 id=concatenated_name,
                 name='',
                 description=''
             )
@@ -2055,21 +2764,26 @@
 def write_concatenated_sequences(
         concatenated_sequences: list,
         concatenate_path: str,
         file_name: str,
         molecule: str):
     """
     Write the concatenated sequences to file
-    :param list concatenated_sequences: List of all SeqRecord objects for the concatenated sequences
-    :param str concatenate_path: Name and absolute path of the folder into which the FASTA files of the concatenated
+    :param list concatenated_sequences: List of all SeqRecord objects for the
+    concatenated sequences
+    :param str concatenate_path: Name and absolute path of the folder into
+    which the FASTA files of the concatenated
     sequences are to be written
-    :param str file_name: File name to use. 'ECs2974_ECs2973' (stx1) and 'ECs1205_ECs1206' (stx2)
-    :param str molecule: String of the current molecule. Options are "nt" (nucleotide) and "aa" (amino acid)
+    :param str file_name: File name to use. 'stx1A_stx1B' (stx1) and
+    'stx2A_stx2B' (stx2)
+    :param str molecule: String of the current molecule. Options are "nt"
+    (nucleotide) and "aa" (amino acid)
     """
-    # Set the name of the output path by adding the molecule to the supplied path
+    # Set the name of the output path by adding the molecule to the
+    # supplied path
     output_path = os.path.join(concatenate_path, molecule)
     make_path(inpath=output_path)
     # Clear out any previous iterations of this script
     previous_fastas = glob(os.path.join(output_path, '*.fasta'))
     for fasta in previous_fastas:
         os.remove(fasta)
     # Set the name of the file to use
```

### Comparing `AlleleFinder-0.1.6/allele_tools/allele_updater.py` & `allelefinder-0.1.7/allele_tools/allele_updater.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 #!/usr/bin/env python
 
 """
-Determine allele complement and profile of sequences. Update profiles and databases as necessary
+Determine allele complement and profile of sequences. Update profiles and
+databases as necessary
 """
 
 # Standard imports
 from argparse import ArgumentParser
-import multiprocessing
 from glob import glob
 import logging
 import json
+import multiprocessing
 import os
 
 
 # Third-party imports
-from olctools.accessoryFunctions.accessoryFunctions import \
-    make_path, \
-    MetadataObject, \
-    SetupLogging
 from Bio import SeqIO
+from olctools.accessoryFunctions.accessoryFunctions import (
+    make_path,
+    MetadataObject,
+    SetupLogging
+)
 
 # Local imports
-from allele_tools.allele_profiler import \
-    allele_prep, \
-    append_profiles, \
-    clear_alleles, \
-    create_profile, \
-    match_profile, \
-    parse_results, \
-    parseable_blast_outputs, \
-    profile_alleles, \
-    read_profile, \
+from allele_tools.allele_profiler import (
+    allele_prep,
+    append_profiles,
+    clear_alleles,
+    create_profile,
+    match_profile,
+    parse_results,
+    parseable_blast_outputs,
+    profile_alleles,
+    read_profile,
     sequence_typer
-from allele_tools.methods import \
-    update_allele_database, \
-    translate, \
-    query_prep, \
-    blast_alleles, \
+)
+from allele_tools.methods import (
+    update_allele_database,
+    translate,
+    query_prep,
+    blast_alleles,
     pathfinder
+)
 
 __author__ = 'adamkoziol'
 
 
 class Updater:
-
     """
-    Determine allele complement and profile of sequences. Update profiles and databases as
-    necessary
+    Determine allele complement and profile of sequences. Update profiles
+    and databases as necessary
     """
 
     # pylint: disable=too-many-instance-attributes
 
     def main(self):
         """
         Run the appropriate methods in the correct order
@@ -190,15 +193,17 @@
                 aa_profile_dict, aa_profile_set = self.aa_allele_match(
                     runmetadata=sample,
                     profile_dict={},
                     profile_set=[],
                     gene_names=gene_names,
                     amino_acid=True
                 )
-                aa_profile_data = read_profile(profile_file=self.aa_profile_file)
+                aa_profile_data = read_profile(
+                    profile_file=self.aa_profile_file
+                )
                 aa_profile_matches = match_profile(
                     profile_data=aa_profile_data,
                     profile_dict=aa_profile_dict,
                     profile_matches={}
                 )
                 aa_profile_matches, aa_profile_data, aa_new_profiles = \
                     create_profile(
@@ -225,49 +230,67 @@
                     data=self.data,
                     novel_profiles=True,
                     profile_path=self.aa_profile_path,
                     gene_names=self.gene_names
                 )
                 self.aa_notes(runmetadata=sample)
                 clear_alleles(
-                    combined_targets_db=glob(os.path.join(self.allele_path, 'combinedtargets*')),
+                    combined_targets_db=glob(
+                        os.path.join(
+                            self.allele_path,
+                            'combinedtargets*'
+                        )
+                    ),
                     custom_targets=os.path.join(self.allele_path, 'custom.tfa')
                 )
 
     def aa_allele_prep(self):
         """
         Create (first time only) and read the amino acid allele database file
         """
         # Create the amino acid allele database file path as required
         make_path(self.aa_allele_path)
         # Iterate through all the gene in the analysis
         for gene in self.gene_names:
             # Attempt to find the database file
             try:
-                allele_file = glob(os.path.join(self.aa_allele_path, f'{gene}*.*fa*'))[0]
+                allele_file = glob(
+                    os.path.join(
+                        self.aa_allele_path,
+                        f'{gene}*.*fa*'
+                    )
+                )[0]
             # Create the file if it doesn't exist
             except IndexError:
                 allele_file = self.initialise_aa_alleles(gene=gene)
-            # Read in and store all the amino acid records in the allele database file
+            # Read in and store all the amino acid records in the allele
+            # database file
             for record in SeqIO.parse(allele_file, 'fasta'):
                 self.aa_allele_dict[record.id] = str(record.seq)
 
     def initialise_aa_alleles(self, gene):
         """
         Create a gene-specific amino acid allele database file
         :param gene: Name of current gene being analysed
         :return: Name and absolute path to the created database file
         """
         # Find the corresponding gene-specific nucleotide database file
-        nt_allele_file = glob(os.path.join(self.allele_path, f'{gene}*.*fa*'))[0]
+        nt_allele_file = glob(
+            os.path.join(
+                self.allele_path,
+                f'{gene}*.*fa*'
+            )
+        )[0]
         # Set the name of the amino acid database file
-        aa_allele_file = os.path.join(self.aa_allele_path, f'{gene}_alleles.fasta')
-        # Initialise a dictionary to store str(amino acid sequence): allele name to be used
-        # in finding duplicate
-        # translated alleles
+        aa_allele_file = os.path.join(
+            self.aa_allele_path,
+            f'{gene}_alleles.fasta'
+        )
+        # Initialise a dictionary to store str(amino acid sequence): allele
+        # name to be used in finding duplicate translated alleles
         allele_dict = {}
         for record in SeqIO.parse(nt_allele_file, 'fasta'):
             # Replace and dashes in the record.id with underscores
             record.id = record.id.replace('-', '_')
             record_id = record.id
             # Translate the sequence to amino acid
             record = record.translate()
@@ -283,312 +306,474 @@
                 # Update the dictionary with the sequence: allele
                 allele_dict[str(record.seq)] = record.id
                 # Update the dictionary with gene: allele
                 if not self.aa_nt_allele_link_dict[gene]:
                     self.aa_nt_allele_link_dict[gene][record.id] = record.id
                 if allele_id == '1':
                     # Write the translated target sequence to file
-                    with open(aa_allele_file, 'a+', encoding='utf-8') as aa_targets:
+                    with open(
+                            aa_allele_file,
+                            'a+',
+                            encoding='utf-8') as aa_targets:
                         SeqIO.write(record, aa_targets, 'fasta')
             else:
                 if not self.aa_nt_allele_link_dict[gene]:
-                    self.aa_nt_allele_link_dict[gene][record.id] = allele_dict[str(record.seq)]
+                    self.aa_nt_allele_link_dict[gene][record.id] = \
+                        allele_dict[str(record.seq)]
         return aa_allele_file
 
-    def aa_allele_match(self, runmetadata, profile_dict, profile_set, gene_names, amino_acid):
+    def aa_allele_match(
+            self,
+            runmetadata: list,
+            profile_dict: dict,
+            profile_set: list,
+            gene_names: list,
+            amino_acid: str):
         """
         Find match the alleles in the current sample to alleles in the database
         :param runmetadata: List of metadata objects for the current sample
-        :param profile_dict: Dictionary to store gene:allele profile for each sample
+        :param profile_dict: Dictionary to store gene:allele profile for
+        each sample
         :param profile_set: List of all unique profiles
         :param gene_names: List of all gene names in the analysis
-        :param amino_acid: Variable indicating whether the current analyses are on DNA or
+        :param amino_acid: Variable indicating whether the current analyses
+        are on DNA or
         amino acid sequences
-        :return: profile_dict and profile_set updated with the results from the current sample
+        :return: profile_dict and profile_set updated with the results from
+        the current sample
         """
         for sample in runmetadata.samples:
-            # Initialise a dictionary to store the gene:allele combinations for each sample
+            # Initialise a dictionary to store the gene:allele combinations
+            # for each sample
             allele_comprehension = {}
-            for allele, allele_seq in sorted(sample.alleles.nt_alleles_translated.items()):
+            for allele, allele_seq in sorted(
+                    sample.alleles.nt_alleles_translated.items()):
                 present = False
-                # Strip off the allele number from the allele e.g. adk_1 yields adk, while EC042_RS26480_2 yields
+                # Strip off the allele number from the allele e.g. adk_1
+                # yields adk, while EC042_RS26480_2 yields
                 # EC042_RS26480
                 try:
                     gene, _ = allele.rsplit('_', 1)
+                    gene = gene[0].lower() + gene[1:-1] + gene[-1].upper()
                 except ValueError:
                     gene = str()
-                for record_id, record_seq in sorted(self.aa_allele_dict.items()):
+                for record_id, record_seq in sorted(
+                        self.aa_allele_dict.items()):
                     if allele_seq == record_seq:
-                        # Update the dictionary with the new gene: allele number for the sample
-                        allele_comprehension.update({gene: record_id.split('_')[-1]})
+                        # Update the dictionary with the new gene: allele
+                        # number for the sample
+                        allele_comprehension.update(
+                            {
+                                gene: record_id.split('_')[-1]
+                            }
+                        )
                         present = True
-                # If, after iterating through all the BLAST outputs, the gene is not present in the sample, update
-                # the gene: allele to reflect this absence
+                # If, after iterating through all the BLAST outputs, the gene
+                # is not present in the sample, update the gene: allele to
+                # reflect this absence
                 if not present:
                     novel_allele = update_allele_database(
                         gene=gene,
                         query_sequence=allele_seq,
                         allele_path=self.aa_allele_path,
                         report_path=self.report_path,
                         amino_acid=amino_acid
                     )
                     if novel_allele:
-                        allele_comprehension.update({gene: novel_allele.split('_')[-1]})
+                        allele_comprehension.update(
+                            {
+                                gene: novel_allele.split('_')[-1].split('|')[0]
+                            }
+                        )
                     else:
                         allele_comprehension.update({gene: '0'})
-            profile_dict, profile_set, allele_comprehension = self.profile_dict_set_populate(
-                gene_names=gene_names,
-                allele_comprehension=allele_comprehension,
-                profile_dict=profile_dict,
-                sample=sample,
-                profile_set=profile_set
-            )
+            profile_dict, profile_set, allele_comprehension = \
+                self.profile_dict_set_populate(
+                    gene_names=gene_names,
+                    allele_comprehension=allele_comprehension,
+                    profile_dict=profile_dict,
+                    sample=sample,
+                    profile_set=profile_set
+                )
         return profile_dict, profile_set
 
     @staticmethod
-    def profile_dict_set_populate(gene_names, allele_comprehension, profile_dict, sample, profile_set):
+    def profile_dict_set_populate(
+            gene_names: list,
+            allele_comprehension: dict,
+            profile_dict: dict,
+            sample: MetadataObject,
+            profile_set: list):
         """
-        Update the profile dictionary, profile set, and allele comprehension for each gene
+        Update the profile dictionary, profile set, and allele comprehension
+        for each gene
         :param gene_names: List of all gene names in the analysis
-        :param allele_comprehension: Dictionary of the gene:allele combinations for each sample
-        :param profile_dict: Dictionary to store gene:allele profile for each sample
+        :param allele_comprehension: Dictionary of the gene:allele
+        combinations for each sample
+        :param profile_dict: Dictionary to store gene:allele profile for
+        each sample
         :param sample: Metadata objects of current genome
         :param profile_set: List of all unique profiles
         """
         # Iterate through all the genes
         for gene_name in gene_names:
             if gene_name not in allele_comprehension:
+                gene_name = gene_name[0].lower() + \
+                    gene_name[1:-1] + \
+                    gene_name[-1].upper()
                 allele_comprehension.update({gene_name: '0'})
-            # In order to hash the dictionary, use JSON, with sorted keys to freeze it
-            frozen_allele_comprehension = json.dumps(allele_comprehension, sort_keys=True)
+            # In order to hash the dictionary, use JSON, with sorted keys to
+            # freeze it
+            frozen_allele_comprehension = json.dumps(
+                allele_comprehension,
+                sort_keys=True
+            )
             # Update the dictionary of profiles with the hash of the
             # frozen dictionary: list of samples with that hash
             if hash(frozen_allele_comprehension) not in profile_dict:
                 profile_dict[hash(frozen_allele_comprehension)] = [sample.name]
             else:
-                profile_dict[hash(frozen_allele_comprehension)].append(sample.name)
-            # Add the 'regular' dictionary to the list of all profiles as required
+                profile_dict[hash(frozen_allele_comprehension)].append(
+                    sample.name
+                )
+            # Add the 'regular' dictionary to the list of all profiles
+            # as required
             if allele_comprehension not in profile_set:
                 profile_set.append(allele_comprehension)
         return profile_dict, profile_set, allele_comprehension
 
-    def aa_notes(self, runmetadata):
-        """
-        Create (first time only), and update the profile and alleles notes files. These files
-        link amino acid profile(s) and allele(s), respectively, to the corresponding nucleotide
-        profile, and allele
+    def aa_notes(
+            self,
+            runmetadata: list):
+        """
+        Create (first time only), and update the profile and alleles notes
+        files. These files link amino acid profile(s) and allele(s),
+        respectively, to the corresponding nucleotide profile, and allele
         :param runmetadata: List of metadata objects for the current sample
         """
         logging.info('Creating/Updating notes')
         # Read in the profile notes file
         allele_profile_dict = self.read_aa_profile_notes()
         for sample in runmetadata.samples:
-            # Check if the nucleotide sequence type has previously been encountered
+            # Check if the nucleotide sequence type has previously
+            # been encountered
             try:
-                # Extract all the previously encountered amino acid sequence types corresponding
+                # Extract all the previously encountered amino acid sequence
+                # types corresponding
                 # to the nucleotide st
-                known_allele_profiles = allele_profile_dict[sample.alleles.nt_st]
-                # Determine whether the current amino acid st is already in the list of aa
+                known_allele_profiles = allele_profile_dict[
+                    sample.alleles.nt_st
+                ]
+                # Determine whether the current amino acid st is already in
+                # the list of aa
                 # sequence types
                 if sample.alleles.aa_st not in known_allele_profiles:
-                    # If the current st is novel, update the list of profiles, and use the
-                    # list to update the
-                    # notes file
-                    allele_profile_dict[sample.alleles.nt_st].append(sample.alleles.aa_st)
-                    self.update_aa_profile_notes(aa_profile_dict=allele_profile_dict)
-            # If the current nucleotide sequence type is novel, add it to the dictionary
+                    # If the current st is novel, update the list of profiles,
+                    # and use the list to update the notes file
+                    allele_profile_dict[sample.alleles.nt_st].append(
+                        sample.alleles.aa_st
+                    )
+                    self.update_aa_profile_notes(
+                        aa_profile_dict=allele_profile_dict
+                    )
+            # If the current nucleotide sequence type is novel, add it to
+            # the dictionary
             except KeyError:
-                allele_profile_dict[sample.alleles.nt_st] = [sample.alleles.aa_st]
+                allele_profile_dict[sample.alleles.nt_st] = \
+                    [sample.alleles.aa_st]
                 # Use the dictionary to update the notes file
-                self.update_aa_profile_notes(aa_profile_dict=allele_profile_dict)
+                self.update_aa_profile_notes(
+                    aa_profile_dict=allele_profile_dict
+                )
             # Process the allele file
             for gene, allele in sample.alleles.nt_profile.items():
+                gene = gene[0].lower() + gene[1:-1] + gene[-1].upper()
                 # Attempt to read in the previous allele notes file
                 allele_notes_dict = self.read_aa_allele_notes(gene=gene)
+                # Clean up the allele name
+                allele = int(allele.split('|')[0])
                 # Check if the nucleotide allele is present in the dictionary
                 try:
                     # Extract the list of all amino acid alleles corresponding
                     # to the nucleotide allele
                     try:
-                        known_aa_alleles = allele_notes_dict[int(allele)]
+                        known_aa_alleles = allele_notes_dict[allele]
                     # Initialise an empty list if allele_notes_dict is empty
                     except ValueError:
                         known_aa_alleles = list()
-                    # Set the aa_allele variable to save typing the long attribute
+                    # Set the aa_allele variable to save typing the
+                    # long attribute
                     aa_allele = sample.alleles.aa_profile[gene]
-                    # Check to see if the amino acid allele has already been encountered
+                    # Check to see if the amino acid allele has already
+                    # been encountered
                     if aa_allele not in known_aa_alleles:
                         # Make sure that the allele isn't missing 'ND'
                         if aa_allele != '0':
                             # Add the allele to the list
-                            allele_notes_dict[int(allele)].append(aa_allele)
+                            allele_notes_dict[allele].append(aa_allele)
                             # Update the notes file with the
                             self.update_aa_allele_notes(
                                 gene=gene,
                                 allele_notes_dict=allele_notes_dict
                             )
                 # If the nucleotide allele is novel, add it to the dictionary
                 except KeyError:
                     aa_allele = sample.alleles.aa_profile[gene]
                     if aa_allele != '0':
-                        allele_notes_dict[int(allele)] = [aa_allele]
+                        allele_notes_dict[allele] = [aa_allele]
                         self.update_aa_allele_notes(
                             gene=gene,
                             allele_notes_dict=allele_notes_dict
                         )
 
-    def read_aa_profile_notes(self):
+    def read_aa_profile_notes(self) -> dict:
         """
         Read in all the notes from the profile file (if it exists)
-        :return: aa_profile_dict: Dictionary of nucleotide seq type: amino acid sequence type(s)
+        :return: aa_profile_dict: Dictionary of nucleotide seq type:
+        amino acid sequence type(s)
         """
         aa_profile_dict = dict()
         try:
             with open(self.aa_profile_notes, 'r', encoding='utf-8') as profile:
                 # Ignore the header
                 _ = profile.readline()
                 # Read in all the lines
                 for line in profile:
-                    # Split the nucleotide sequence type from the amino acid sequence type(s)
+                    # Split the nucleotide sequence type from the amino
+                    # acid sequence type(s)
                     nt_profile, aa_profiles = line.rstrip().split('\t')
                     # Create a list of all the amino acid sequence types
                     aa_profile_dict[nt_profile] = aa_profiles.split(';')
         except FileNotFoundError:
             pass
         return aa_profile_dict
 
-    def update_aa_profile_notes(self, aa_profile_dict):
+    def update_aa_profile_notes(
+            self,
+            aa_profile_dict: dict):
         """
         Update the profile file with a novel entry
-        :param aa_profile_dict: Dictionary of nucleotide sequence type: amino acid sequence type(s)
+        :param aa_profile_dict: Dictionary of nucleotide sequence type:
+        amino acid sequence type(s)
         """
         # Overwrite the previous notes file
         with open(self.aa_profile_notes, 'w', encoding='utf-8') as profile:
             # Create the header for the profile file
             profile.write('nt_profile\taa_profile(s)\n')
             # Iterate through all the sequence type entries in the dictionary
             for nt_profile, aa_profiles in aa_profile_dict.items():
-                aa_profiles = ';'.join([str(profile) for profile in aa_profiles])
+                aa_profiles = ';'.join(
+                    [str(profile) for profile in aa_profiles]
+                )
                 # Write each nucleotide profile: aa_profile link
                 profile.write(f'{nt_profile}\t{aa_profiles}\n')
 
-    def read_aa_allele_notes(self, gene):
+    def read_aa_allele_notes(
+            self,
+            gene: str) -> dict:
         """
         Read in the allele notes file. If it doesn't exist, create it
         :param gene: Name of the current gene being analysed
-        :return: Dictionary of nucleotide allele: list of corresponding amino acid alleles
+        :return: Dictionary of nucleotide allele: list of corresponding
+        amino acid alleles
         """
         allele_notes_dict = {}
         # Set the name of the notes file
-        notes_file = os.path.join(self.aa_notes_path, f'{gene}_allele_notes.tsv')
+        notes_file = os.path.join(
+            self.aa_notes_path,
+            f'{gene}_allele_notes.tsv'
+        )
         # Attempt to read the notes file
         try:
             with open(notes_file, 'r', encoding='utf-8') as notes:
                 # Ignore the header
                 _ = notes.readline()
-                # Extract the nt allele, ';'-separated list of amino acid alleles from the line
+                # Extract the nt allele, ';'-separated list of amino acid
+                # alleles from the line
                 for line in notes:
                     nt_allele, aa_alleles = line.rstrip().split('\t')
                     # Create a list of all the amino acid alleles
                     allele_notes_dict[int(nt_allele)] = aa_alleles.split(';')
         # Create the file if it doesn't exist
         except FileNotFoundError:
-            # Iterate through all the entries in the dictionary of gene name: nt allele: aa allele
+            # Iterate through all the entries in the dictionary of gene name:
+            # nt allele: aa allele
             for _, allele_dict in self.aa_nt_allele_link_dict.items():
                 for nt_allele, aa_allele in allele_dict.items():
                     # Split the entries on underscores
                     _, nt_allele_number = nt_allele.rsplit('_', 1)
                     _, aa_allele_number = aa_allele.rsplit('_', 1)
-                    # Update the notes dictionary with int(nt allele): list(aa allele)
-                    allele_notes_dict[int(nt_allele_number)] = [aa_allele_number]
+                    # Update the notes dictionary with int(nt allele):
+                    # list(aa allele)
+                    allele_notes_dict[int(nt_allele_number)] = \
+                        [aa_allele_number]
         return allele_notes_dict
 
-    def update_aa_allele_notes(self, gene, allele_notes_dict):
+    def update_aa_allele_notes(
+            self,
+            gene: str,
+            allele_notes_dict: dict):
         """
         Update the amino acid allele notes file with the novel alleles
         :param gene: Current gene being analysed
-        :param allele_notes_dict: Dictionary of nucleotide allele: list of corresponding amino 
-        acid alleles
+        :param allele_notes_dict: Dictionary of nucleotide allele: list of
+        corresponding amino acid alleles
         """
         # Set the name and path of the notes file
-        notes_file = os.path.join(self.aa_notes_path, f'{gene}_allele_notes.tsv')
+        notes_file = os.path.join(
+            self.aa_notes_path,
+            f'{gene}_allele_notes.tsv'
+        )
         with open(notes_file, 'w', encoding='utf-8') as notes:
             # Create the header for the notes file
             notes.write('nt_allele\taa_alleles\n')
             for nt_allele, aa_alleles in sorted(allele_notes_dict.items()):
-                # Write the nucleotide allele and list of corresponding amino acid alleles
+                # Write the nucleotide allele and list of corresponding amino
+                # acid alleles
                 aa_alleles = ';'.join(str(allele) for allele in aa_alleles)
                 notes.write(f'{str(nt_allele)}\t{aa_alleles}\n')
 
-    def __init__(self, path, amino_acid):
+    def __init__(
+            self,
+            path: str,
+            amino_acid: bool):
+        """
+        Constructs all the necessary attributes for the Updater object.
+
+        Parameters:
+        path (str): Path to the file
+        amino_acid (bool): Flag to indicate if the target is an amino acid
+        """
+
+        # Set paths
         self.path = pathfinder(path=path)
         self.allele_path = os.path.join(self.path, 'nt_alleles')
         self.aa_allele_path = os.path.join(self.path, 'aa_alleles')
         self.profile_path = os.path.join(self.path, 'nt_profile')
         self.aa_profile_path = os.path.join(self.path, 'aa_profile')
+
+        # Create profile path
         make_path(self.profile_path)
+
+        # Set profile files
         self.profile_file = os.path.join(self.profile_path, 'profile.txt')
-        self.aa_profile_file = os.path.join(self.aa_profile_path, 'profile.txt')
+        self.aa_profile_file = os.path.join(
+            self.aa_profile_path,
+            'profile.txt'
+        )
+
+        # Set query and report paths
         self.query_path = os.path.join(self.path, 'query')
         self.report_path = os.path.join(self.path, 'reports')
+
+        # Create report path
         make_path(self.report_path)
+
+        # Remove novel alleles
         novel_alleles = glob(os.path.join(self.report_path, '*.fasta'))
         for novel_allele in novel_alleles:
             os.remove(novel_allele)
-        self.aa_notes_path = os.path.join(self.path, 'aa_notes')
+
+        # Set notes path and file
+        self.aa_notes_path = os.path.join(
+            self.path,
+            'aa_notes'
+        )
         make_path(self.aa_notes_path)
-        self.aa_profile_notes = os.path.join(self.aa_notes_path, 'aa_profile_notes.tsv')
+        self.aa_profile_notes = os.path.join(
+            self.aa_notes_path,
+            'aa_profile_notes.tsv'
+        )
+
+        # Set amino acid flag
         self.amino_acid = amino_acid
+
+        # Set combined targets
         if not self.amino_acid:
-            self.combined_targets = os.path.join(self.allele_path, 'combinedtargets.fasta')
+            self.combined_targets = os.path.join(
+                self.allele_path,
+                'combinedtargets.fasta'
+            )
         else:
-            self.combined_targets = os.path.join(self.aa_allele_path, 'combinedtargets.fasta')
+            self.combined_targets = os.path.join(
+                self.aa_allele_path,
+                'combinedtargets.fasta'
+            )
+
+        # Initialize other attributes
         self.gene_names = []
         self.runmetadata = MetadataObject()
         self.runmetadata.samples = []
         self.cpus = multiprocessing.cpu_count() - 1
-        self.profile_report = os.path.join(self.report_path, 'nt_profiles.tsv')
-        self.aa_profile_report = os.path.join(self.report_path, 'aa_profiles.tsv')
+        self.profile_report = os.path.join(
+            self.report_path,
+            'nt_profiles.tsv'
+        )
+        self.aa_profile_report = os.path.join(
+            self.report_path,
+            'aa_profiles.tsv'
+        )
+
+        # Remove profile report if it exists
         try:
             os.remove(self.profile_report)
         except FileNotFoundError:
             pass
-        # Fields used for custom outfmt 6 BLAST output:
-        self.fieldnames = ['query_id', 'subject_id', 'identical', 'mismatches', 'gaps',
-                           'evalue', 'bit_score', 'query_length', 'subject_length', 'alignment_length',
-                           'query_start', 'query_end', 'subject_start', 'subject_end',
-                           'query_sequence', 'subject_sequence']
+
+        # Set field names for BLAST output
+        self.fieldnames = [
+            'query_id',
+            'subject_id',
+            'identical',
+            'mismatches',
+            'gaps',
+            'evalue',
+            'bit_score',
+            'query_length',
+            'subject_length',
+            'alignment_length',
+            'query_start',
+            'query_end',
+            'subject_start',
+            'subject_end',
+            'query_sequence',
+            'subject_sequence'
+        ]
         self.extended_fieldnames = self.fieldnames.copy()
         self.extended_fieldnames.insert(14, 'percent_match')
-        self.outfmt = '6 qseqid sseqid nident mismatch gaps evalue bitscore qlen slen length ' \
-                      'qstart qend sstart send qseq sseq'
-        # A string of the header to use for formatting the profile file, and the report headers
+        self.outfmt = '6 qseqid sseqid nident mismatch gaps evalue bitscore ' \
+            'qlen slen length qstart qend sstart send qseq sseq'
+
+        # Initialize data and dictionaries
         self.data = str()
         self.aa_allele_dict = {}
         self.aa_nt_allele_link_dict = {}
 
 
 def cli():
     """
     Collect the arguments, create an object, and run the script
     """
     # Parser for arguments
     parser = ArgumentParser(
-        description='Determines profiles of strains against previously calculated allele database '
-                    'and profile. Creates and/or updates both the database of allele definitions '
-                    'and the profile based on novel alleles and/or profiles discovered'
+        description='Determines profiles of strains against previously '
+        'calculated allele database and profile. Creates and/or updates both '
+        'the database of allele definitions and the profile based on novel '
+        'alleles and/or profiles discovered'
     )
     parser.add_argument(
         '-p', '--path',
         required=True,
-        help='Specify path. Note that due to code reuse, the query sequence files must be in the '
-             '"query" sub-folder, nucleotide alleles must be in the "nt_alleles" sub-folder, the nucleotide profile '
-             'must be named profile.txt and be located in the "nt_profile" sub-folder, amino acid alleles must be in '
-             'the "aa_allele" sub-folder, and the amino acid profile must be named profile.txt and be located in the'
-             '"aa_profile" sub-folder '
+        help='Specify path. Note that due to code reuse, the query sequence '
+        'files must be in the "query" sub-folder, nucleotide alleles must be '
+        'in the "nt_alleles" sub-folder, the nucleotide profile must be named '
+        'profile.txt and be located in the "nt_profile" sub-folder, amino '
+        'acid alleles must be in the "aa_allele" sub-folder, and the '
+        'amino acid profile must be named profile.txt and be located in the '
+        '"aa_profile" sub-folder '
     )
     parser.add_argument(
         '-aa', '--amino_acid',
         action='store_true',
         help='The query sequences are protein.'
     )
     # Get the arguments into an object
```

### Comparing `AlleleFinder-0.1.6/allele_tools/allele_translate_reduce.py` & `allelefinder-0.1.7/allele_tools/allele_translate_reduce.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 Translate nucleotide alleles to amino acid, and remove duplicates
 """
 
 # Standard imports
 from argparse import ArgumentParser
 from glob import glob
 import logging
+import os
 import shutil
 import sys
-import os
+from typing import TextIO
 
 # Third-party imports
-from olctools.accessoryFunctions.accessoryFunctions import make_path, SetupLogging
+from olctools.accessoryFunctions.accessoryFunctions import (
+    make_path,
+    SetupLogging
+)
 from Bio.SeqRecord import SeqRecord
 from Bio import SeqIO
 
 # Local imports
 from allele_tools.allele_profiler import read_profile
 from allele_tools.profile_reduce import ProfileReduce
-from allele_tools.methods import \
-    evaluate_translated_length, \
-    generic_evaluate_translated_length, \
-    remove_combined_db_files, \
+from allele_tools.methods import (
+    evaluate_translated_length,
+    generic_evaluate_translated_length,
+    remove_combined_db_files,
     pathfinder
+)
 
 
 class Translate:
 
     """
     Translate and reduce alleles
     """
@@ -39,26 +44,30 @@
         """
         # Read in all the allele files
         self.load_alleles()
         # Parse the alleles
         self.parse_alleles(length_dict=self.length_dict)
         # If a profile file has been provided, run the profiling methods
         if self.profile_file:
-            # Extract seq_type:allele comprehensions from the nucleotide profile file
+            # Extract seq_type:allele comprehensions from the nucleotide
+            # profile file
             self.profile_data = read_profile(profile_file=self.profile_file)
             # Create the amino acid profiles
             self.aa_profile()
             # Remove duplicate profiles
             reduce = ProfileReduce(
                 profile=self.aa_profile_file,
                 names=self.gene_name_file
             )
             reduce.main()
-            # Read in the profile data again now that the profile file has been updated
-            self.aa_profile_data = read_profile(profile_file=self.aa_profile_file)
+            # Read in the profile data again now that the profile file has
+            # been updated
+            self.aa_profile_data = read_profile(
+                profile_file=self.aa_profile_file
+            )
             # Find linkages between nucleotide and amino acid profiles
             self.profile_link()
             # Write profile links to file
             self.link_file()
             # Copy and rename the reduced profile file
             self.copy_profile()
 
@@ -66,126 +75,155 @@
         """
         Use SeqIO to read in all the gene sequences
         """
         for allele_file in self.sequence_files:
             gene_name = os.path.splitext(os.path.basename(allele_file))[0]
             # Add the gene name to the set of names
             self.gene_names.add(gene_name)
-            self.allele_dict[gene_name] = SeqIO.to_dict(SeqIO.parse(allele_file, 'fasta'))
+            self.allele_dict[gene_name] = SeqIO.to_dict(
+                SeqIO.parse(allele_file, 'fasta')
+            )
 
-    def parse_alleles(self, length_dict=None):
-        """
-        Parse the allele files to translate the amino acid sequence using BioPython. Write the
-        amino acid sequence to file. Store the allele name in the notes. Find duplicates, and link
-        the nucleotide allele name to the amino acid allele name
-        :param length_dict: Dictionary of gene name: minimum acceptable length of translated sequence
+    def parse_alleles(
+            self,
+            length_dict: dict = None):
+        """
+        Parse the allele files to translate the amino acid sequence using
+        BioPython. Write the amino acid sequence to file. Store the allele
+        name in the notes. Find duplicates, and link the nucleotide allele
+        name to the amino acid allele name
+        :param length_dict: Dictionary of gene name: minimum acceptable
+        length of translated sequence
         """
         logging.info('Translating and parsing alleles')
         for gene_name, allele_dict in self.allele_dict.items():
-            # Initialise the dictionary to store the links between the nt alleles and the aa
-            # alleles with the name of the gene
+            # Initialise the dictionary to store the links between the nt
+            # alleles and the aa alleles with the name of the gene
             self.allele_links[gene_name] = {}
-            #  Initialise a set of allele that do not pass the required filters, and
-            # must be removed from the database
+            #  Initialise a set of allele that do not pass the required
+            # filters, and must be removed from the database
             remove_list = set()
             logging.info('Processing %s', gene_name)
-            # Initialise a dictionary to store the translated allele sequence: allele name
+            # Initialise a dictionary to store the translated allele
+            # sequence: allele name
             seq_allele = {}
             # Set the name and path of the allele and notes files
-            allele_file = os.path.join(self.translated_path, f'{gene_name}.fasta')
-            notes_file = os.path.join(self.notes_path, f'{gene_name}_notes.txt')
+            allele_file = os.path.join(
+                self.translated_path,
+                f'{gene_name}.fasta'
+            )
+            notes_file = os.path.join(
+                self.notes_path,
+                f'{gene_name}_notes.txt'
+            )
             # Open the file to store the translated alleles
             with open(allele_file, 'w', encoding='utf-8') as aa_alleles:
                 # Open the notes file
                 with open(notes_file, 'w', encoding='utf-8') as notes:
                     # Create the header for the notes file
                     notes.write('nt_allele\taa_allele\tnote\n')
                     # Iterate through all the alleles in the dictionary
                     for allele, details in allele_dict.items():
                         # Create a list to store notes
                         note = []
-                        # Create a boolean to track whether the sequence is filtered
+                        # Create a boolean to track whether the sequence
+                        # is filtered
                         filtered = False
-                        # Create a string to store the untrimmed nucleotide sequence
+                        # Create a string to store the untrimmed nucleotide
+                        # sequence
                         original_nt_sequence = str(details.seq)
                         # Calculate the translated sequence
                         translated_allele = details.seq.translate()
                         # Remove all sequence after a stop codon (*)
                         split_allele = translated_allele.split('*')
                         # Create a string to hold the trimmed sequence
                         trimmed_seq = str()
-                        # If there are multiple stop codons in the sequence, trim to the first one
+                        # If there are multiple stop codons in the sequence,
+                        # trim to the first one
                         if len(split_allele) > 2:
                             if split_allele[1]:
                                 for trimmed in split_allele[1:]:
-                                    trimmed_seq += f'*{trimmed}'
+                                    trimmed_seq += trimmed
                             else:
                                 for trimmed in split_allele[2:]:
-                                    trimmed_seq += f'*{trimmed}'
+                                    trimmed_seq += trimmed
                             note.append(f'Trimmed {trimmed_seq} from end')
                         elif len(split_allele) == 1:
                             pass
                         else:
-                            if split_allele[-1] and not str(translated_allele).endswith('*'):
+                            if split_allele[-1] and not \
+                                    str(translated_allele).endswith('*'):
                                 trimmed_seq += split_allele[-1]
                                 note.append(f'Trimmed {trimmed_seq} from end')
-                        # Create a dictionary to store the allele nt sequences to check to see if
-                        # any are duplicates following trimming
+                        # Create a dictionary to store the allele nt sequences
+                        # to check to see if any are duplicates following
+                        # trimming
                         nt_sequences = {}
-                        filtered, note, nt_sequences, translated_allele = Translate.trim_alleles(
-                            note=note,
-                            allele=allele,
-                            sequence=details,
-                            gene_name=gene_name,
-                            nt_allele_path=self.path,
-                            trim_length=len(trimmed_seq),
-                            length_dict=length_dict,
-                            filtered=filtered,
-                            nt_sequences=nt_sequences,
-                            original_nt_sequence=original_nt_sequence
-                        )
-                        # If the allele has not been filtered through the trim_alleles
+                        filtered, note, nt_sequences, translated_allele = \
+                            Translate.trim_alleles(
+                                note=note,
+                                allele=allele,
+                                sequence=details,
+                                gene_name=gene_name,
+                                nt_allele_path=self.path,
+                                trim_length=len(trimmed_seq),
+                                length_dict=length_dict,
+                                filtered=filtered,
+                                nt_sequences=nt_sequences,
+                                original_nt_sequence=original_nt_sequence
+                            )
+                        # If the allele has not been filtered through the
+                        # trim_alleles
                         if not filtered:
                             # Determine if this amino acid allele is new
                             if str(translated_allele) not in seq_allele:
-                                # Add the string of the amino acid sequence to the dictionary
+                                # Add the string of the amino acid sequence to
+                                # the dictionary
                                 seq_allele[str(translated_allele)] = allele
                                 # Create a SeqRecord of the translated allele
                                 seq_record = SeqRecord(
                                     seq=translated_allele,
                                     id=allele,
                                     name=str(),
                                     description=str()
                                 )
                                 # Write the SeqRecord to file
                                 SeqIO.write(
                                     sequences=seq_record,
                                     handle=aa_alleles,
                                     format='fasta'
                                 )
-                                # Update the notes with the allele naming information
-                                notes.write(f'{allele}\t{allele}\t{";".join(note)}\n')
-                                # Populate the linking dictionary with the nt allele: aa allele
-                                self.allele_links[gene_name][allele.split('_')[-1]] = \
+                                # Update the notes with the allele naming
+                                # information
+                                notes.write(
+                                    f'{allele}\t{allele}\t{";".join(note)}\n'
+                                )
+                                # Populate the linking dictionary with the nt
+                                # allele: aa allele
+                                self.allele_links[
+                                    gene_name][allele.split('_')[-1]] = \
                                     allele.split('_')[-1]
                             # Amino acid allele already exists
                             else:
-                                # Extract the allele name corresponding to the translated sequence
+                                # Extract the allele name corresponding to the
+                                # translated sequence
                                 aa_allele = seq_allele[str(translated_allele)]
-                                # Update the notes, including that this allele is a duplicate, and a
-                                # pointer to the original
+                                # Update the notes, including that this allele
+                                # is a duplicate, and a pointer to the original
                                 notes.write(
                                     f'{allele}\t{aa_allele}\tDuplicate'
                                 )
                                 if not note:
                                     notes.write('\n')
                                 else:
                                     notes.write(f'; {";".join(note)}\n')
-                                # Populate the linking dictionary with the nt allele: aa allele
-                                self.allele_links[gene_name][allele.split('_')[-1]] = \
+                                # Populate the linking dictionary with the nt
+                                # allele: aa allele
+                                self.allele_links[
+                                    gene_name][allele.split('_')[-1]] = \
                                     aa_allele.split('_')[-1]
                                 self.allele_links[gene_name]['0'] = '0'
                         # Filtered alleles must be removed from the database
                         else:
                             Translate.write_filtered_allele_notes(
                                 notes=notes,
                                 allele=allele,
@@ -195,58 +233,79 @@
                             # Create a SeqRecord of the translated allele
                             seq_record = SeqRecord(
                                 seq=translated_allele,
                                 id=allele,
                                 name=str(),
                                 description=str()
                             )
-                            # Write the filtered alleles to the filtered alleles file
+                            # Write the filtered alleles to the filtered
+                            # alleles file
                             Translate.create_or_update_filtered_files(
                                 gene=gene_name,
                                 allele_path=self.translated_path,
                                 records_filter=[seq_record]
                             )
             # Remove the filtered sequences from the database
             Translate.remove_filtered_alleles_from_db(
                 gene_name=gene_name,
                 allele_list=remove_list,
                 nt_allele_path=self.path,
             )
             self.load_alleles()
 
     @staticmethod
-    def trim_alleles(note, allele, sequence, gene_name, nt_allele_path, trim_length, length_dict, filtered,
-                     nt_sequences, original_nt_sequence):
-        """
-        Trim the alleles based on location of stop codons and whether the sequence is a multiple of three nucleotides.
-        Evaluate the trimmed sequence based on length and contents.
+    def trim_alleles(
+            note: list,
+            allele: str,
+            sequence: SeqIO,
+            gene_name: str,
+            nt_allele_path: str,
+            trim_length: int,
+            length_dict: dict,
+            filtered: bool,
+            nt_sequences: dict,
+            original_nt_sequence: str):
+        """
+        Trim the alleles based on location of stop codons and whether the
+        sequence is a multiple of three nucleotides. Evaluate the trimmed
+        sequence based on length and contents.
         :param note: List of sequence-specific notes
         :param allele: String of the allele identifier
         :param sequence: SeqIO sequence object of nucleotide sequence
-        :param gene_name: String of the gene name to which the allele corresponds
-        :param nt_allele_path: String of the absolute path to the folder in which the nucleotide alleles are located
-        :param trim_length: Integer of the number of nucleotides to be trimmed (due to internal stop codons)
-        :param length_dict: Dictionary of minimum acceptable length for each gene in the analysis
-        :param filtered: Boolean to track whether the sequence fails the quality/length checks
+        :param gene_name: String of the gene name to which the
+        allele corresponds
+        :param nt_allele_path: String of the absolute path to the folder in
+        which the nucleotide alleles are located
+        :param trim_length: Integer of the number of nucleotides to be trimmed
+        (due to internal stop codons)
+        :param length_dict: Dictionary of minimum acceptable length for each
+        gene in the analysis
+        :param filtered: Boolean to track whether the sequence fails the
+        quality/length checks
         :param nt_sequences: Dictionary of allele: sequence
-        :param original_nt_sequence: String of the untrimmed nucleotide sequence of the allele
-        :return: filtered: Updated boolean of whether the sequence fails quality/length checks
+        :param original_nt_sequence: String of the untrimmed nucleotide
+        sequence of the allele
+        :return: filtered: Updated boolean of whether the sequence fails
+        quality/length checks
         :return: note: Update list of sequence-specific notes
         :return: nt_sequences: Updated dictionary of allele: sequence
-        :return: translated_allele: SeqIO sequence object of trimmed, translated allele
+        :return: translated_allele: SeqIO sequence object of trimmed,
+        translated allele
         """
         # Determine the length of sequence to trim from the end of the sequence
-        # Multiply the number of amino acid residues to trim by three to get the number of nucleotides
-        # Add the modulo three of the sequence to yield a final length divisible by three
+        # Multiply the number of amino acid residues to trim by three to get
+        # the number of nucleotides. Add the modulo three of the sequence to
+        # yield a final length divisible by three
         nt_to_trim = 3 * trim_length + len(sequence) % 3
         # Check if trimming is required
         if nt_to_trim:
             # Slice the string by the number of required bases at the end
             sequence = sequence[:-nt_to_trim]
-            # Update the nucleotide sequence in the database with the trimmed version
+            # Update the nucleotide sequence in the database with the trimmed
+            # version
             Translate.update_allele_db(
                 nt_allele_path=nt_allele_path,
                 gene=gene_name,
                 allele=allele,
                 nt_sequence=sequence
             )
         # Translate the sequence to amino acid
@@ -273,118 +332,147 @@
         filtered, note, nt_sequences = Translate.find_duplicates(
             nt_sequences=nt_sequences,
             nt_sequence=sequence,
             allele=allele,
             filtered=filtered,
             note=note
         )
-        # Update the notes if the sequence does not end with a stop codon
-        if not str(translated_allele).endswith('*'):
-            note.append('Trimmed sequence did not end with a stop codon')
         return filtered, note, nt_sequences, translated_allele
-    
+
     @staticmethod
-    def update_allele_db(nt_allele_path, gene, allele, nt_sequence):
+    def update_allele_db(
+            nt_allele_path: str,
+            gene: str,
+            allele: str,
+            nt_sequence: SeqIO):
         """
         Update nucleotide allele files with newly trimmed sequences
-        :param nt_allele_path: String of the absolute path to the folder containing the nucleotide allele database
+        :param nt_allele_path: String of the absolute path to the folder
+        containing the nucleotide allele database
         :param gene: String of the name of the current gene
         :param allele: String of the allele header (geneName_alleleID)
         :param nt_sequence: SeqIO object of the nucleotide sequence
         """
-        # Set the name of the allele database file to update by joining the allele path and the gene name
+        # Set the name of the allele database file to update by joining the
+        # allele path and the gene name
         nt_allele_file = os.path.join(nt_allele_path, f'{gene}.fasta')
         # Create a list to store all database records (including modified ones)
         updated_records = []
         # Iterate over all the sequences in the nucleotide allele file
         for record in SeqIO.parse(handle=nt_allele_file, format='fasta'):
-            # Check if the header of the database sequence matches the header of the query sequence
+            # Check if the header of the database sequence matches the header
+            # of the query sequence
             if record.id == allele:
                 # Update the record to be the query allele sequence object
                 record = nt_sequence
             # Append the record to the list of records
             updated_records.append(record)
         # Overwrite the allele file with the records
         SeqIO.write(updated_records, handle=nt_allele_file, format='fasta')
-    
+
     @staticmethod
-    def find_duplicates(nt_sequences, nt_sequence, allele, filtered, note):
+    def find_duplicates(
+            nt_sequences: dict,
+            nt_sequence: SeqIO,
+            allele: str,
+            filtered: bool,
+            note: list):
         """
-        Match a query amino acid sequence against the protein allele database file
+        Match a query amino acid sequence against the protein allele
+        database file
         :param nt_sequences: Dictionary of allele: sequence
-        :param nt_sequence: SeqIO sequence object of the trimmed nucleotide sequence
+        :param nt_sequence: SeqIO sequence object of the trimmed
+        nucleotide sequence
         :param allele: String of the allele header (geneName_alleleID)
-        :param filtered: Boolean of whether the sequence passes content/length filters
+        :param filtered: Boolean of whether the sequence passes
+        content/length filters
         :param note: List of sequence-specific notes
-        :return: filtered: Updated boolean of sequence-specific content/length filtering results
+        :return: filtered: Updated boolean of sequence-specific
+        content/length filtering results
         :return: note: Updated list of sequence-specific notes
         :return: nt_sequences: Updated list of allele: sequence
         """
         # Initialise a list to store any matches
         matches = []
         # Iterate over allele header, sequence in the dictionary
         for prev_allele, nt_seq in nt_sequences.items():
             # Check if the current nucleotide sequence matches a previous entry
-            if nt_sequence == nt_seq:
+            if nt_sequence.seq == nt_seq.seq:  # Compare sequence strings
                 # Append matches to the list
                 matches.append(prev_allele)
         # Check if the list has been populated with matches
         if not matches:
             # If no matches, update the dictionary with the novel sequence
-            nt_sequences[allele] = nt_sequences
+            nt_sequences[allele] = nt_sequence
             return filtered, note, nt_sequences
         # If there are matches
         for match in matches:
-            # Set the filtering boolean to True (this is not a novel sequence, so do not update the database)
+            # Set the filtering boolean to True (this is not a novel sequence,
+            # so do not update the database)
             filtered = True
             # Update the note
-            note.append(f'Trimmed nt sequence matches previous allele sequence: {match}')
+            note.append(
+                f'Trimmed nt sequence matches previous '
+                f'allele sequence: {match}'
+            )
         return filtered, note, nt_sequences
 
     @staticmethod
-    def write_filtered_allele_notes(notes, allele, note):
+    def write_filtered_allele_notes(
+            notes: TextIO,
+            allele: str,
+            note: list):
         """
         Write notes for filtered sequences to file
-        :param notes: Filehandle for notes file
+        :param notes: File handle for notes file
         :param allele: String of the allele header (geneName_alleleID)
         :param note: List of sequence-specific notes
         """
-        # Write the allele \t ND (because the sequence is filtered,there is no amino acid allele) \t
+        # Write the allele \t ND (because the sequence is filtered,there is
+        # no amino acid allele) \t
         notes.write(f'{allele}\tND\tFiltered: {"; ".join(note)}\n')
 
     @staticmethod
-    def remove_filtered_alleles_from_db(gene_name, allele_list, nt_allele_path):
+    def remove_filtered_alleles_from_db(
+            gene_name: str,
+            allele_list: list,
+            nt_allele_path: str):
         """
         Remove filtered sequences from the allele database file
         :param gene_name: String of the gene name currently being analysed
         :param allele_list: List of alleles to be removed from the database
-        :param nt_allele_path: String of the absolute path to the folder containing the nucleotide allele database
+        :param nt_allele_path: String of the absolute path to the folder
+        containing the nucleotide allele database
         """
-        # Remove the combinedtargets.fasta and BLAST database files from the folder
+        # Remove the combinedtargets.fasta and BLAST database files from
+        # the folder
         remove_combined_db_files(
             allele_path=nt_allele_path
         )
         # Set the name and path of the allele file
         nt_allele_file = os.path.join(nt_allele_path, f'{gene_name}.fasta')
         # Create a list of all the records in the database file using SeqIO
         records = SeqIO.parse(nt_allele_file, 'fasta')
         # Initialise a list to store unfiltered records
         records_keep = []
         # Initialise a list to store filtered records
         records_filter = []
         # Iterate over all the records in the database
         for record in records:
-            # Check if the allele header matches any of the headers of alleles to be filtered
+            # Check if the allele header matches any of the headers of alleles
+            # to be filtered
             if record.id not in allele_list:
                 # If the record is not to be filtered, add it to the keep list
                 records_keep.append(record)
-            # If the record header matches any of the alleles to be filtered, add it to the filtered list
+            # If the record header matches any of the alleles to be filtered,
+            # add it to the filtered list
             else:
                 records_filter.append(record)
-        # Overwrite the nucleotide allele database file with all the unfiltered records
+        # Overwrite the nucleotide allele database file with all the
+        # unfiltered records
         with open(nt_allele_file, 'w', encoding='utf-8') as allele_file:
             for record in records_keep:
                 SeqIO.write(
                     sequences=record,
                     handle=allele_file,
                     format='fasta'
                 )
@@ -393,68 +481,88 @@
             Translate.create_or_update_filtered_files(
                 gene=gene_name,
                 allele_path=nt_allele_path,
                 records_filter=records_filter
             )
 
     @staticmethod
-    def create_or_update_filtered_files(gene, allele_path, records_filter):
+    def create_or_update_filtered_files(
+            gene: str,
+            allele_path: str,
+            records_filter: list):
         """
         Write the filtered alleles to the filtered alleles file
         :param gene: String of the gene name currently being analysed
-        :param allele_path: String of the absolute path to the folder containing the allele database
-        :param records_filter: List of SeqIO sequence objects for alleles to be added to the filtered alleles file
+        :param allele_path: String of the absolute path to the folder
+        containing the allele database
+        :param records_filter: List of SeqIO sequence objects for alleles to
+        be added to the filtered alleles file
         """
         # Set the name and path of the filtered alleles file
-        filtered_allele_file = os.path.join(allele_path, f'{gene}_filtered.txt')
+        filtered_allele_file = os.path.join(
+            allele_path,
+            f'{gene}_filtered.txt'
+        )
         # Append the filtered alleles to the file
-        with open(filtered_allele_file, 'a+', encoding='utf-8') as filtered_alleles:
+        with open(
+                filtered_allele_file,
+                'a+',
+                encoding='utf-8') as filtered_alleles:
+            # Iterate and write all the records in the list of filtered records
             for record in records_filter:
                 SeqIO.write(
                     sequences=record,
                     handle=filtered_alleles,
                     format='fasta'
                 )
 
     def aa_profile(self):
         """
         Create the amino acid profile
         """
-        # Create a list to store profiles containing alleles that have been quality filtered
+        # Create a list to store profiles containing alleles that have been
+        # quality filtered
         filtered_list = set()
         # Initialise a dictionary to store sequenceType:geneName_alleleID
         filtered_dict = {}
         # Initialise a string to hold the profile
         profile_str = ''
         # Iterate through all the sequence types in the profile_data dictionary
         for seq_type in sorted(int(st) for st in self.profile_data):
             # Create a string to store the allele information
             allele_string = str()
-            # Iterate through all the gene: allele entries in the nested dictionary
+            # Iterate through all the gene: allele entries in the nested
+            # dictionary
             for gene_name, allele in self.profile_data[str(seq_type)].items():
                 try:
                     # Extract the linked amino acid allele from the dictionary
-                    allele_string += self.allele_links[gene_name][str(allele)] + '\t'
-                # If the gene name + allele ID is not in the allele link dictionary, add the sequence type to the set
+                    allele_string += self.allele_links[
+                        gene_name][str(allele)] + '\t'
+                # If the gene name + allele ID is not in the allele link
+                # dictionary, add the sequence type to the set
                 except KeyError:
                     filtered_list.add(seq_type)
-                    # Initialise the sequence type key in the filtered dictionary as required
+                    # Initialise the sequence type key in the filtered
+                    # dictionary as required
                     if seq_type not in filtered_dict:
                         filtered_dict[seq_type] = []
-                    # Update the dictionary with the filtered geneName_alleleIdentifier
+                    # Update the dictionary with the filtered
+                    # geneName_alleleIdentifier
                     filtered_dict[seq_type].append(f'{gene_name}_{allele}')
             if allele_string:
                 # Add the sequence type to the profile string
                 profile_str += f'{str(seq_type)}\t{allele_string}'
-                # Remove trailing whitespace and add a newline for proper formatting
+                # Remove trailing whitespace and add a newline for proper
+                # formatting
                 profile_str = profile_str.rstrip()
                 profile_str += '\n'
         # Create the amino acid profile file
         with open(self.aa_profile_file, 'w', encoding='utf-8') as aa_profile:
-            # Create a string of tab-delimited gene names to be used in the header
+            # Create a string of tab-delimited gene names to be used in
+            # the header
             names = '\t'.join(sorted(list(self.gene_names)))
             # Write the header string
             aa_profile.write(f'ST\t{names.rstrip()}\n')
             # Write the tab-delimited profile string
             aa_profile.write(profile_str)
         # Create the names file
         with open(self.gene_name_file, 'w', encoding='utf-8') as gene_file:
@@ -472,17 +580,20 @@
                 filtered_list=filtered_list,
                 filtered_dict=filtered_dict,
                 profile_path=os.path.dirname(self.profile_file)
             )
             self.profile_data = read_profile(profile_file=self.profile_file)
 
     @staticmethod
-    def filter_profiles(filtered_list, profile_file):
+    def filter_profiles(
+            filtered_list: set,
+            profile_file: str):
         """
-        Remove filtered profiles from the profile file. Write them to the filtered profile file
+        Remove filtered profiles from the profile file. Write them to the
+        filtered profile file
         :param filtered_list: Set of filtered sequence types
         :param profile_file: String of the absolute path to the profile file
         """
         # Initialise a list to store the filtered sequence types
         filtered_rows = []
         # Initialise a list to store the unfiltered sequence types
         keep_rows = []
@@ -492,207 +603,285 @@
             for row in profiles:
                 # Extract the sequence type from the row
                 seq_type = row.split('\t')[0]
                 # Check if it is the header, which starts with 'ST'
                 if seq_type == 'ST':
                     # Filter the header
                     filtered_rows.append(row)
-                # Check to see if the sequence type of the row is present in the list of filtered sequence types
-                if str(seq_type) in [str(filtered) for filtered in filtered_list]:
+                # Check to see if the sequence type of the row is present in
+                # the list of filtered sequence types
+                if str(seq_type) in [
+                        str(filtered) for filtered in filtered_list]:
                     # Add the row to the list of filtered rows
                     filtered_rows.append(row)
                 # Unfiltered rows are added to the list of unfiltered rows
                 else:
                     keep_rows.append(row)
-        # Extract the absolute path of the folder in which the profile file is located
+        # Extract the absolute path of the folder in which the profile file
+        # is located
         profile_path = os.path.dirname(profile_file)
         # Overwrite the profile file with the unfiltered profiles
-        with open(os.path.join(profile_path, 'profile.txt'), 'w', encoding='utf-8') as updated_profile:
+        with open(os.path.join(
+                profile_path,
+                'profile.txt'
+                ), 'w', encoding='utf-8') as updated_profile:
             updated_profile.write(''.join(keep_rows))
         # Overwrite the filtered profile file with the filtered profiles
-        with open(os.path.join(profile_path, 'filtered_profiles.txt'), 'w', encoding='utf-8') as filtered_profiles:
+        with open(os.path.join(
+                profile_path,
+                'filtered_profiles.txt'
+                ), 'w', encoding='utf-8') as filtered_profiles:
             filtered_profiles.write(''.join(filtered_rows))
 
     @staticmethod
-    def filter_notes(filtered_list, filtered_dict, profile_path):
+    def filter_notes(
+            filtered_list: set,
+            filtered_dict: dict,
+            profile_path: str):
         """
         Write the notes regarding profile filtering to file
         :param filtered_list: Set of filtered sequence types
         :param filtered_dict: Dictionary of sequenceType:geneName_alleleID
-        :param profile_path: String of the absolute path to the folder containing the profile file
-        :return:
+        :param profile_path: String of the absolute path to the folder
+        containing the profile file
         """
-        # Set the absolute path of the file containing the profile filtering notes
+        # Set the absolute path of the file containing the profile filtering
+        # notes
         filtered_notes = os.path.join(profile_path, 'filtering_notes.txt')
         # Write the notes to file
         with open(filtered_notes, 'w', encoding='utf-8') as notes:
             # Create the header
             notes.write('SequenceType\tFilteringNote\n')
             # Create a new line for each filtered profile
             for seq_type in filtered_list:
-                # Create a sting of the list of filtered alleles present in this profile
+                # Create a sting of the list of filtered alleles present in
+                # this profile
                 gene_allele = ';'.join(filtered_dict[seq_type])
-                # Write the sequence type and all the missing alleles to the note
+                # Write the sequence type and all the missing alleles to the
+                # note
                 notes.write(f'{seq_type}\t{gene_allele} missing\n')
-    
+
     def profile_link(self):
         """
         Link nucleotide and amino profiles
         """
-        # Initialise a dictionary to store to number of matches between a query profile and the profiles in the database
+        # Initialise a dictionary to store to number of matches between a
+        # query profile and the profiles in the database
         match_score = {}
         # Iterate over all the profiles in the profile file
         for seq_type, gene_dict in self.profile_data.items():
             # Initialise the seq_type key in the dictionary
             self.profile_matches[seq_type] = set()
             match_score[seq_type] = {}
-            # Iterate over all the gene name, allele ID combinations in the profile dictionary
+            # Iterate over all the gene name, allele ID combinations in the
+            # profile dictionary
             for gene, allele in gene_dict.items():
                 # Iterate over all the profiles in the amino acid profile file
                 for aa_st, aa_gene_dict in self.aa_profile_data.items():
-                    # Use the gene name to extract the amino acid allele ID from the profile file.
-                    # Also extract the amino acid allele ID from the linking dictionary with the gene name and
+                    # Use the gene name to extract the amino acid allele ID
+                    # from the profile file.
+                    # Also extract the amino acid allele ID from the linking
+                    # dictionary with the gene name and
                     # nucleotide allele ID. Check if they match
                     if aa_gene_dict[gene] == self.allele_links[gene][allele]:
-                        # Initialise the amino acid sequence type in the dictionary
+                        # Initialise the amino acid sequence type in
+                        # the dictionary
                         if aa_st not in match_score[seq_type]:
                             match_score[seq_type][aa_st] = 0
                         # Increment the number of matches to the profile
                         match_score[seq_type][aa_st] += 1
         # Iterate over all the matches to the profiles in the profile file
         for seq_type, aa_st_dict in match_score.items():
             # Iterate over the amino acid sequence type matches
             for aa_st, matches, in aa_st_dict.items():
-                # Check if the number of matches observed is equal to the required number of matches (one for each gene)
+                # Check if the number of matches observed is equal to the
+                # required number of matches (one for each gene)
                 if matches == len(self.gene_names):
-                    # Update the dictionary of matches with the amino acid sequence type: nucleotide sequence type
+                    # Update the dictionary of matches with the amino acid
+                    # sequence type: nucleotide sequence type
                     self.profile_matches[aa_st].add(seq_type)
 
     def link_file(self):
         """
-        Write linking details between nucleotide and amino acid profiles to file
+        Write linking details between nucleotide and amino acid profiles
+        to file
         """
-        #
+        # Open the profile link file
         with open(self.aa_nt_profile_link_file, 'w', encoding='utf-8') as link:
             # Write the header information
             link.write('aa_seq_type\tnt_seq_types\n')
             # Iterate over all the profile matches in the dictionary
             for seq_type, match_set in self.profile_matches.items():
                 # Check the length of the match
                 if len(match_set) == 1:
                     # With a single match, convert the set to a string
                     nt_st = ''.join(match_set)
                     link.write(f'{seq_type}\t{nt_st}\n')
                 # Multiple profile matches
                 else:
-                    # Semicolon-join the set of matches. Since they are strings, first typecase to int for proper
-                    # sorting before converting back to strings
-                    nt_st = ';'.join(str(nt_st) for nt_st in sorted(int(nt_st) for nt_st in match_set))
+                    # Semicolon-join the set of matches. Since they are
+                    # strings, first typecase to int for proper sorting before
+                    # converting back to strings
+                    nt_st = ';'.join(
+                        str(nt_st) for nt_st in sorted(
+                            int(nt_st) for nt_st in match_set
+                        )
+                    )
                     link.write(f'{seq_type}\t{nt_st}\n')
 
     def copy_profile(self):
         """
-        Copy the reduced profile file from the profile folder to the base aa_profile folder
+        Copy the reduced profile file from the profile folder to the base
+        aa_profile folder
         """
-        # Use shutil to copy and rename the profile file to the root of the report path
+        # Use shutil to copy and rename the profile file to the root of
+        # the report path
         shutil.copyfile(
             src=os.path.join(self.report_path, 'profile', 'profile.txt'),
             dst=os.path.join(self.report_path, 'profile.txt')
         )
 
-    def __init__(self, path, profile, report_path=os.path.join(os.getcwd(), 'aa_profile'),
-                 translated_path=os.path.join(os.getcwd(), 'aa_alleles'), length_dict=None):
+    def __init__(
+            self,
+            path: str,
+            profile: str,
+            report_path: str = os.path.join(os.getcwd(), 'aa_profile'),
+            translated_path: str = os.path.join(os.getcwd(), 'aa_alleles'),
+            length_dict: dict = None):
+        """
+        Constructs all the necessary attributes for the Translate object.
+
+        Parameters:
+        path (str): Path to the file
+        profile (str): Profile file. If not provided, it will look for
+        'nt_profile/profile.txt' in the path
+        report_path (str): Path to the report. Default is 'aa_profile' in
+        the current working directory
+        translated_path (str): Path to the translated file. Default is
+        'aa_alleles' in the current working directory
+        length_dict (dict): Dictionary of lengths. Default is None
+        """
 
         logging.info('Welcome to the allele translator!')
         self.path = pathfinder(path=path)
+
+        # Set profile file
         if profile:
             if not os.path.isfile(profile):
-                self.profile_file = os.path.join(self.path, 'nt_profile', 'profile.txt')
+                self.profile_file = os.path.join(
+                    self.path,
+                    'nt_profile',
+                    'profile.txt'
+                )
             else:
                 self.profile_file = profile
             try:
                 assert os.path.isfile(self.profile_file)
             except AssertionError as exc:
                 logging.error(
-                    'Cannot locate the required profile file: %s. Please ensure that '
-                    'the file name and path of your file is correct', self.profile_file
+                    'Cannot locate the required profile file: %s. '
+                    'Please ensure that the file name and path of your file '
+                    'is correct', self.profile_file
                 )
                 raise SystemExit from exc
         else:
             self.profile_file = None
+
+        # Set sequence files
         self.sequence_files = glob(os.path.join(self.path, '*.fasta'))
         try:
             assert self.sequence_files
         except AssertionError as exc:
-            logging.error('Could not locate alleles in provided allele path: %s', self.path)
+            logging.error(
+                'Could not locate alleles in provided allele path: %s',
+                self.path
+            )
             raise SystemExit from exc
+
+        # Set report path
         self.report_path = pathfinder(path=report_path)
         make_path(inpath=self.report_path)
+
+        # Set translated path
         self.translated_path = pathfinder(path=translated_path)
         make_path(inpath=self.translated_path)
+
+        # Set notes path
         self.notes_path = os.path.join(self.translated_path, 'notes')
         make_path(inpath=self.notes_path)
+
+        # Initialize other attributes
         self.length_dict = length_dict
         self.allele_dict = {}
         self.profile_data = {}
         self.allele_links = {}
-        self.aa_profile_file = os.path.join(self.report_path, 'aa_full_profile.txt')
+        self.aa_profile_file = os.path.join(
+            self.report_path,
+            'aa_full_profile.txt'
+        )
         self.gene_names = set()
-        self.gene_name_file = os.path.join(self.report_path, 'gene_names.txt')
+        self.gene_name_file = os.path.join(
+            self.report_path, 'gene_names.txt'
+        )
         self.aa_profile_data = {}
         self.profile_matches = {}
         self.aa_nt_profile_link_file = os.path.join(
             self.report_path,
             'aa_nt_profile_links.tsv'
         )
 
 
 def cli():
     """
     Collect the arguments, create an object, and run the script
     """
     # Parser for arguments
     parser = ArgumentParser(
-        description='Translate allele files in nucleotide format to amino acid. '
-                    'Remove duplicates. Keep notes.'
+        description='Translate allele files in nucleotide format to '
+        'amino acid. Remove duplicates. Keep notes.'
     )
     parser.add_argument(
         '-p', '--path',
         required=True,
         help='Specify path containing allele files.'
     )
     parser.add_argument(
         '--profile',
         action='store_true',
-        help='Optionally parse the nucleic acid profile, and create the corresponding reduced '
-             'amino acid profile. The profile must be named profile.txt and be located in nt_profile folder in the path'
+        help='Optionally parse the nucleic acid profile, and create the '
+        'corresponding reduced amino acid profile. The profile must be named '
+        'profile.txt and be located in nt_profile folder in the path'
     )
     parser.add_argument(
         '--report_path',
         default=os.path.join(os.getcwd(), 'aa_profile'),
-        help='Optionally provide the name (and path, if desired) of the folder into which the amino acid profile '
-             'and related files are to be written. Default folder is "aa_profile" in your current working directory'
+        help='Optionally provide the name (and path, if desired) of the '
+        'folder into which the amino acid profile and related files are to be '
+        'written. Default folder is "aa_profile" in your current '
+        'working directory'
     )
     parser.add_argument(
         '--translated_path',
         default=os.path.join(os.getcwd(), 'aa_alleles'),
-        help='Optionally provide the name (and path, if desired) of the folder into which the amino acid alleles '
-             'and notes are to be written. Default folder is "aa_alleles" in your current working directory'
+        help='Optionally provide the name (and path, if desired) of the '
+        'folder into which the amino acid alleles and notes are to be written.'
+        ' Default folder is "aa_alleles" in your current working directory'
     )
     # Get the arguments into an object
     arguments = parser.parse_args()
     SetupLogging(debug=True)
     translate = Translate(
         path=arguments.path,
         profile=arguments.profile,
         report_path=arguments.report_path,
         translated_path=arguments.translated_path
     )
     translate.main()
     logging.info('Allele translation complete!')
-    # Prevent the arguments being printed to the console (they are returned in order for the tests to work)
+    # Prevent the arguments being printed to the console (they are returned in
+    # order for the tests to work)
     sys.stderr = open(os.devnull, 'w', encoding='utf-8')
     return arguments
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `AlleleFinder-0.1.6/tests/test_0_profile_reduce.py` & `allelefinder-0.1.7/tests/test_6_stec_aa_allele_find.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,119 @@
 #!/usr/bin/env python
 
 """
-Unit and integration tests for allele_tools/profile_reduce.py
+Unit and integration tests for allele_tools/stec.py Only testing the
+allele_find functionality
 """
 
-# Standard imports
-from unittest.mock import patch
+# Standard library imports
 import argparse
-import shutil
 import os
+from unittest.mock import patch
 
-# Third-party imports
+# Third party imports
 import pytest
 
-# Local imports
-from allele_tools.profile_reduce import \
+# Local application imports
+from allele_tools.stec import (
+    aa_allele_find,
     cli
+)
+from .test_2_allele_updater import (
+    clean_outputs,
+    prepare_files,
+    setup
+)
 
-
-@pytest.fixture(name='variables', scope='module')
-def setup():
-    class Variables:
-        def __init__(self):
-            # Extract the connection string prior to running tests
-            self.test_path = os.path.abspath(os.path.dirname(__file__))
-            self.file_path = os.path.join(self.test_path, 'test_files', 'profile_reduce')
-            self.profile = os.path.join(self.file_path, 'profiles.list')
-            self.names = os.path.join(self.file_path, 'genes.txt')
-            self.output_path = os.path.join(self.file_path, 'profile')
-            self.output_profiles = os.path.join(self.file_path, 'profile', 'profile.txt')
-            self.output_notes = os.path.join(self.file_path, 'profile', 'reducing_notes.txt')
-
-    return Variables()
+# Ensure the setup function is correctly named
+assert vars(setup)['_pytestfixturefunction'].name == 'variables'
 
 
 @patch('argparse.ArgumentParser.parse_args')
-def test_profile_reduce_missing_tilde_profile(mock_args, variables):
-    mock_args.return_value = argparse.Namespace(
-        profile='~/fake_file_profiles.list',
-        names=variables.names
-    )
+def test_allele_find_integration_missing_files(mock_args, variables):
+    """
+    Test the integration of the allele find functionality when files
+    are missing.
+
+    :param mock_args: A mock object for the command line arguments.
+    :param variables: An instance of the Variables class.
+    """
     with pytest.raises(SystemExit):
-        cli()
+        # Mock the command line arguments for the allele find functionality
+        mock_args.return_value = argparse.Namespace(
+            aa_alleles=variables.aa_allele_path,
+            query_path=variables.query_path,
+            report_path=variables.report_path,
+            cutoff=90,
+        )
 
+        # Run the command line interface and get the arguments
+        arguments = cli()
 
-@patch('argparse.ArgumentParser.parse_args')
-def test_profile_reduce_missing_tilde_names(mock_args, variables):
-    mock_args.return_value = argparse.Namespace(
-        profile=variables.profile,
-        names='~/fake_file_genes.txt'
-    )
-    with pytest.raises(SystemExit):
-        cli()
+        # Run the allele find functionality with the arguments
+        aa_allele_find(args=arguments)
 
 
 @patch('argparse.ArgumentParser.parse_args')
-def test_profile_reduce_integration(mock_args, variables):
-    mock_args.return_value = argparse.Namespace(
-        profile=variables.profile,
-        names=variables.names
+def test_allele_find_integration(mock_args, variables):
+    """
+    Test the integration of the allele find functionality.
+
+    :param mock_args: A mock object for the command line arguments.
+    :param variables: An instance of the Variables class.
+    """
+    # Prepare the necessary files for the test
+    prepare_files(
+        variables=variables,
+        nucleotide=False,
+        links=True
     )
-    cli()
-    assert os.path.isfile(variables.output_profiles)
-
-
-def test_output_profile_header(variables):
-    variables.profiles = open(variables.output_profiles, 'r', encoding='utf-8').readlines()
-    assert variables.profiles[0] == 'ST	ECs1205	ECs1206\n'
-
-
-def test_output_profile_sequence_type(variables):
-    assert variables.profiles[1] == '1	0	0\n'
-
-
-def test_output_notes_header(variables):
-    variables.notes = open(variables.output_notes, 'r', encoding='utf-8').readlines()
-    assert variables.notes[0] == 'OriginalSequenceType	ReducedSequenceType	Notes\n'
-
-
-def test_output_notes_novel(variables):
-    assert variables.notes[1] == '1	1\n'
 
+    # Mock the command line arguments for the allele find functionality
+    mock_args.return_value = argparse.Namespace(
+        aa_alleles=variables.aa_allele_path,
+        query_path=variables.query_path,
+        report_path=variables.report_path,
+        cutoff=90,
+    )
 
-def test_output_notes_duplicate(variables):
-    assert variables.notes[2] == '2	0	duplicate\n'
+    # Run the command line interface and get the arguments
+    arguments = cli()
 
+    # Run the allele find functionality with the arguments
+    aa_allele_find(args=arguments)
 
-def test_output_notes_length(variables):
-    assert len(variables.notes) == 10
+    # Check if the allele report file exists
+    variables.allele_report = os.path.join(
+        variables.report_path,
+        'allele_report.tsv'
+    )
+    assert os.path.isfile(variables.allele_report)
 
 
-def test_output_clean_up(variables):
-    shutil.rmtree(variables.output_path)
-    assert not os.path.isfile(variables.output_path)
+def test_report_contents(variables):
+    """
+    Test the contents of the report.
+
+    :param variables: An instance of the Variables class.
+    """
+    # Read the contents of the allele report file
+    variables.report_contents = open(
+        variables.allele_report,
+        'r',
+        encoding='utf-8'
+    ).readlines()
+
+    # Check the contents of the allele report file
+    assert variables.report_contents[3] == 'stx2A_1388\t\t\n'
+    assert variables.report_contents[12] == \
+           'stx2A_9\tStx2a_868|319aa\tAmino acid allele Stx2a_868|319aa ' \
+           'is novel\n'
+
+
+def test_clean(variables):
+    """
+    Test the clean up of the outputs.
+
+    :param variables: An instance of the Variables class.
+    """
+    clean_outputs(variables=variables)
```

### Comparing `AlleleFinder-0.1.6/tests/test_2_allele_updater.py` & `allelefinder-0.1.7/tests/test_5_stec_allele_find.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,197 +1,213 @@
 #!/usr/bin/env python
 
 """
-Unit and integration tests for allele_tools/allele_translate_reduce.py
+Unit and integration tests for allele_tools/stec.py Only testing the
+allele_find functionality
 """
 
-# Standard imports
-from unittest.mock import patch
-from glob import glob
+# Standard library imports
 import argparse
-import shutil
+from glob import glob
 import os
+from unittest.mock import patch
 
-# Third-party imports
-from Bio import SeqIO
+# Third party imports
 import pytest
 
-# Local imports
-from allele_tools.allele_updater import \
-    Updater, \
+# Local application imports
+from allele_tools.stec import (
+    allele_find,
     cli
+)
+from .test_2_allele_updater import (
+    clean_outputs,
+    prepare_files
+)
 
 
 @pytest.fixture(name='variables', scope='module')
 def setup():
+    """
+    Pytest fixture for setting up the test environment.
+    This fixture is named 'variables' and has module scope.
+    """
     class Variables:
         def __init__(self):
             # Extract the connection string prior to running tests
             self.test_path = os.path.abspath(os.path.dirname(__file__))
-            self.file_path = os.path.join(self.test_path, 'test_files', 'allele_updater')
-            self.original_files_path = os.path.join(self.file_path, 'original_files')
-            self.original_nt_allele_files = glob(os.path.join(self.original_files_path, 'nt_alleles', 'ECs12*'))
-            self.original_nt_profile_file = os.path.join(self.original_files_path, 'nt_profile', 'profile.txt')
-            self.original_nt_query_files = glob(os.path.join(self.original_files_path, 'nt_query', '*.fasta'))
-            self.original_aa_allele_files = glob(os.path.join(self.original_files_path, 'aa_alleles', 'ECs12*'))
-            self.original_aa_profile_path = os.path.join(self.original_files_path, 'aa_profile')
-            self.original_aa_profile_file = os.path.join(self.original_aa_profile_path, 'profile.txt')
-            self.original_aa_query_files = glob(os.path.join(self.original_files_path, 'aa_query', '*.fasta'))
-            self.nt_allele_path = os.path.join(self.file_path, 'nt_alleles')
-            self.nt_profile_file = os.path.join(self.file_path, 'nt_profile', 'profile.txt')
-            self.nt_profile_path = os.path.join(self.file_path, 'nt_profile')
-            self.aa_allele_path = os.path.join(self.file_path, 'aa_alleles')
-            self.aa_profile_path = os.path.join(self.file_path, 'aa_profile')
-            self.aa_profile_file = os.path.join(self.aa_profile_path, 'profile.txt')
-            self.aa_notes_path = os.path.join(self.file_path, 'aa_notes')
-            self.query_path = os.path.join(self.file_path, 'query')
-            self.report_path = os.path.join(self.file_path, 'reports')
-            self.aa_report_file = os.path.join(self.report_path, 'aa_profiles.tsv')
 
-            self.report_file = os.path.join(self.report_path, 'nt_profiles.tsv')
+            # Define file paths for testing
+            self.file_path = os.path.join(
+                self.test_path, 'test_files', 'stec_allele_find'
+            )
+            self.original_files_path = os.path.join(
+                self.file_path, 'original_files'
+            )
+            self.original_nt_allele_files = glob(os.path.join(
+                self.original_files_path, 'nt_alleles', 'stx2*'
+            ))
+            self.original_nt_profile_file = os.path.join(
+                self.original_files_path, 'nt_profile', 'profile.txt'
+            )
+            self.original_nt_query_files = glob(os.path.join(
+                self.original_files_path, 'nt_query', '*.fasta'
+            ))
+            self.original_aa_allele_files = glob(os.path.join(
+                self.original_files_path, 'aa_alleles', 'stx2*'
+            ))
+            self.original_aa_profile_path = os.path.join(
+                self.original_files_path, 'aa_profile'
+            )
+            self.original_aa_profile_file = os.path.join(
+                self.original_aa_profile_path, 'profile.txt'
+            )
+            self.original_aa_query_files = glob(os.path.join(
+                self.original_files_path, 'aa_query', '*.fasta'
+            ))
+            self.nt_allele_path = os.path.join(
+                self.file_path, 'nt_alleles'
+            )
+            self.nt_profile_file = os.path.join(
+                self.file_path, 'nt_profile', 'profile.txt'
+            )
+            self.nt_profile_path = os.path.join(
+                self.file_path, 'nt_profile'
+            )
+            self.aa_allele_path = os.path.join(
+                self.file_path, 'aa_alleles'
+            )
+            self.aa_profile_path = os.path.join(
+                self.file_path, 'aa_profile'
+            )
+            self.aa_profile_file = os.path.join(
+                self.aa_profile_path, 'profile.txt'
+            )
+            self.aa_notes_path = os.path.join(
+                self.file_path, 'aa_notes'
+            )
+            self.aa_reports_path = os.path.join(
+                self.file_path, 'aa_reports'
+            )
+            self.aa_report_file = os.path.join(
+                self.aa_reports_path, 'aa_profiles.tsv'
+            )
+            self.query_path = os.path.join(
+                self.file_path, 'query'
+            )
+            self.report_path = os.path.join(
+                self.file_path, 'reports'
+            )
+            self.report_file = os.path.join(
+                self.report_path, 'profiles.tsv'
+            )
+
+            # Define length dictionary for testing
             self.length_dict = {
-                'ECs2973': 82,
-                'ECs2974': 313,
-                'ECs1205': 313,
-                'ECs1206': 84
+                'stx1B': 82,
+                'stx1A': 313,
+                'stx2A': 313,
+                'stx2B': 84
             }
+
+            # Define a fake path for testing
             self.fake_path = os.path.join('~', 'completely_fake_path')
 
     return Variables()
 
 
-def clean_outputs(variables):
-    if os.path.isdir(variables.nt_allele_path):
-        shutil.rmtree(variables.nt_allele_path)
-    if os.path.isdir(variables.nt_profile_path):
-        shutil.rmtree(variables.nt_profile_path)
-    if os.path.isdir(variables.aa_allele_path):
-        shutil.rmtree(variables.aa_allele_path)
-    if os.path.isdir(variables.aa_profile_path):
-        shutil.rmtree(variables.aa_profile_path)
-    if os.path.isdir(variables.query_path):
-        shutil.rmtree(variables.query_path)
-    if os.path.isdir(variables.report_path):
-        shutil.rmtree(variables.report_path)
-    if os.path.isdir(variables.aa_notes_path):
-        shutil.rmtree(variables.aa_notes_path)
-
-
-def prepare_files(variables, nucleotide=True, links=False):
-    if not os.path.isdir(variables.nt_allele_path):
-        os.makedirs(name=variables.nt_allele_path)
-    for nt_allele in variables.original_nt_allele_files:
-        shutil.copyfile(
-            src=nt_allele,
-            dst=os.path.join(variables.nt_allele_path, os.path.basename(nt_allele))
-        )
-    if not os.path.isdir(variables.nt_profile_path):
-        os.makedirs(name=variables.nt_profile_path)
-    shutil.copyfile(
-        src=variables.original_nt_profile_file,
-        dst=os.path.join(variables.nt_profile_path, os.path.basename(variables.original_nt_profile_file))
-    )
-    if not os.path.isdir(variables.aa_allele_path):
-        os.makedirs(name=variables.aa_allele_path)
-    for aa_allele in variables.original_aa_allele_files:
-        shutil.copyfile(
-            src=aa_allele,
-            dst=os.path.join(variables.aa_allele_path, os.path.basename(aa_allele))
-        )
-    if not os.path.isdir(variables.aa_profile_path):
-        os.makedirs(name=variables.aa_profile_path)
-    shutil.copyfile(
-        src=variables.original_aa_profile_file,
-        dst=os.path.join(variables.aa_profile_path, os.path.basename(variables.original_aa_profile_file))
-    )
-    if links:
-        link_file = 'aa_nt_profile_links.tsv'
-        shutil.copyfile(
-            src=os.path.join(variables.original_aa_profile_path, link_file),
-            dst=os.path.join(variables.aa_profile_path, link_file)
-        )
-    os.makedirs(name=variables.query_path)
-    if nucleotide:
-        for nt_query in variables.original_nt_query_files:
-            shutil.copyfile(
-                src=nt_query,
-                dst=os.path.join(variables.query_path, os.path.basename(nt_query))
-            )
-    else:
-        for aa_query in variables.original_aa_query_files:
-            shutil.copyfile(
-                src=aa_query,
-                dst=os.path.join(variables.query_path, os.path.basename(aa_query))
-            )
-
-
 @patch('argparse.ArgumentParser.parse_args')
-def test_allele_updater_integration(mock_args, variables):
-    prepare_files(variables=variables)
-    mock_args.return_value = argparse.Namespace(
-        path=variables.file_path,
-        amino_acid=False,
-    )
-    cli()
-    assert os.path.isfile(variables.report_file)
-
-
-def test_report_contents(variables):
-    variables.report_contents = open(variables.report_file, 'r', encoding='utf-8').readlines()
-    assert variables.report_contents[1] == '2013-SEQ-0039	259156	6	8\n'
-
-
-def test_novel_alleles(variables):
-    novel_allele_file = os.path.join(variables.report_path, 'nt_ECs1205_novel_alleles.fasta')
-    novel_alleles = open(novel_allele_file, 'r', encoding='utf-8').readlines()
-    assert novel_alleles[0] == '>ECs1205_1000000\n'
-    clean_outputs(variables=variables)
+def test_allele_find_integration_no_files(mock_args, variables):
+    """
+    Test the integration of the allele find functionality when no files
+    are provided.
+
+    :param mock_args: A mock object for the command line arguments.
+    :param variables: An instance of the Variables class.
+    """
+    with pytest.raises(SystemExit):
+        # Mock the command line arguments for the allele find functionality
+        mock_args.return_value = argparse.Namespace(
+            nt_profile=variables.nt_profile_file,
+            aa_profile=variables.aa_profile_file,
+            nt_alleles=variables.nt_allele_path,
+            aa_alleles=variables.aa_allele_path,
+            query_path=variables.query_path,
+            report_path=variables.report_path
+        )
 
+        # Run the command line interface and get the arguments
+        arguments = cli()
 
-def test_tilde_path(variables):
-    Updater(
-        path=variables.fake_path,
-        amino_acid=False
-    )
-    abs_path = os.path.abspath(os.path.expanduser(os.path.join(variables.fake_path)))
-    assert os.path.isdir(abs_path)
-    shutil.rmtree(abs_path)
+        # Run the allele find functionality with the arguments
+        allele_find(args=arguments)
 
 
 @patch('argparse.ArgumentParser.parse_args')
-def test_allele_updater_integration_aa_query(mock_args, variables):
+def test_allele_find_integration(mock_args, variables):
+    """
+    Test the integration of the allele find functionality.
+
+    :param mock_args: A mock object for the command line arguments.
+    :param variables: An instance of the Variables class.
+    """
+    # Prepare the necessary files for the test
     prepare_files(
         variables=variables,
-        nucleotide=False
+        links=True
     )
+
+    # Mock the command line arguments for the allele find functionality
     mock_args.return_value = argparse.Namespace(
-        path=variables.file_path,
-        amino_acid=True,
+        nt_profile=variables.nt_profile_file,
+        aa_profile=variables.aa_profile_file,
+        nt_alleles=variables.nt_allele_path,
+        aa_alleles=variables.aa_allele_path,
+        query_path=variables.query_path,
+        report_path=variables.report_path
+    )
+
+    # Run the command line interface and get the arguments
+    arguments = cli()
+
+    # Run the allele find functionality with the arguments
+    allele_find(args=arguments)
+
+    # Check if the allele report file exists
+    variables.allele_report = os.path.join(
+        variables.report_path,
+        'stec_report.tsv'
     )
-    cli()
-    assert os.path.isfile(variables.aa_report_file)
-
-
-def test_aa_report_contents(variables):
-    aa_report_contents = open(variables.aa_report_file, 'r', encoding='utf-8').readlines()
-    assert aa_report_contents[2] == 'ECs1205_11\t175\t11\t0\n'
-    clean_outputs(variables=variables)
+    assert os.path.isfile(variables.allele_report)
 
 
-@patch('argparse.ArgumentParser.parse_args')
-def test_allele_updater_integration_new_aa_files(mock_args, variables):
-    prepare_files(variables=variables)
-    shutil.rmtree(variables.aa_allele_path)
-    mock_args.return_value = argparse.Namespace(
-        path=variables.file_path,
-        amino_acid=False,
-    )
-    cli()
-    assert os.path.isfile(variables.report_file)
+def test_report_contents(variables):
+    """
+    Test the contents of the report.
 
+    :param variables: An instance of the Variables class.
+    """
+    # Read the contents of the allele report file
+    variables.report_contents = open(
+        variables.allele_report,
+        'r',
+        encoding='utf-8'
+    ).readlines()
+
+    # Check the contents of the allele report file
+    assert variables.report_contents[1] == \
+        '2013-SEQ-0039\t6\t9\t259156\t868\t137\t259156\tNovel nt_seq_type ' \
+        '259156, and aa_seq_type 259156\n'
+    assert variables.report_contents[16] == \
+        '2017-SEQ-0617	0	2	N/A	0		N/A	stx2B amino acid ' \
+        'sequence does not start with M; ' \
+        'stx2B amino acid sequence was 13 amino acid residues. ' \
+        'Minimum allowed length is 84 amino acid residues\n'
+
+
+def test_clean(variables):
+    """
+    Test the clean up of the outputs.
 
-def test_novel_aa_alleles(variables):
-    novel_aa_allele_file = os.path.join(variables.aa_allele_path, 'ECs1206_alleles.fasta')
-    records = list(SeqIO.parse(novel_aa_allele_file, 'fasta'))
-    assert records[0].seq == \
-           'MKKMFMAVLFALASVNAMAADCAKGKIEFSKYNEDDTFTVKVDGKEYWTSRWNLQPLLQSAQLTGMTVTIKSSTCESGSGFAEVQFNND*'
+    :param variables: An instance of the Variables class.
+    """
     clean_outputs(variables=variables)
```

