# Comparing `tmp/autodft-1.0.1.tar.gz` & `tmp/autodft-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodft-1.0.1.tar", last modified: Sat Apr 20 03:45:28 2024, max compression
+gzip compressed data, was "autodft-1.0.2.tar", last modified: Sun Apr 28 22:07:21 2024, max compression
```

## Comparing `autodft-1.0.1.tar` & `autodft-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-20 03:45:28.519139 autodft-1.0.1/
--rw-r--r--   0 sting    (144291) shenvi   (10405)    35821 2024-04-20 02:50:10.000000 autodft-1.0.1/LICENSE.txt
--rw-r--r--   0 sting    (144291) shenvi   (10405)    10556 2024-04-20 03:45:28.518312 autodft-1.0.1/PKG-INFO
--rw-r--r--   0 sting    (144291) shenvi   (10405)    10358 2024-04-20 02:50:09.000000 autodft-1.0.1/README.md
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-20 03:45:28.501861 autodft-1.0.1/autodft/
--rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-20 02:50:49.000000 autodft-1.0.1/autodft/__init__.py
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-20 03:45:28.507260 autodft-1.0.1/autodft/config/
--rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-20 02:50:50.000000 autodft-1.0.1/autodft/config/__init__.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     1185 2024-04-20 02:50:50.000000 autodft-1.0.1/autodft/config/config.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     2610 2024-04-20 03:44:12.000000 autodft-1.0.1/autodft/config/default_parameters.yaml
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-20 03:45:28.510472 autodft-1.0.1/autodft/helpers/
--rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-20 02:50:50.000000 autodft-1.0.1/autodft/helpers/__init__.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     7402 2024-04-20 02:50:50.000000 autodft-1.0.1/autodft/helpers/crest_job.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)    11913 2024-04-20 02:50:50.000000 autodft-1.0.1/autodft/helpers/gaussian_inputfile.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     3660 2024-04-20 02:50:50.000000 autodft-1.0.1/autodft/helpers/gaussian_manager.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)    15776 2024-04-20 02:50:50.000000 autodft-1.0.1/autodft/helpers/user_input.py
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-20 03:45:28.512949 autodft-1.0.1/autodft/utils/
--rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-20 02:50:51.000000 autodft-1.0.1/autodft/utils/__init__.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     4269 2024-04-20 02:50:51.000000 autodft-1.0.1/autodft/utils/autodft_utils.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     2168 2024-04-20 02:50:51.000000 autodft-1.0.1/autodft/utils/files.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     5077 2024-04-20 02:50:51.000000 autodft-1.0.1/autodft/utils/gaussian_output.py
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-20 03:45:28.517379 autodft-1.0.1/autodft.egg-info/
--rw-r--r--   0 sting    (144291) shenvi   (10405)    10556 2024-04-20 03:45:27.000000 autodft-1.0.1/autodft.egg-info/PKG-INFO
--rw-r--r--   0 sting    (144291) shenvi   (10405)      747 2024-04-20 03:45:27.000000 autodft-1.0.1/autodft.egg-info/SOURCES.txt
--rw-r--r--   0 sting    (144291) shenvi   (10405)        1 2024-04-20 03:45:27.000000 autodft-1.0.1/autodft.egg-info/dependency_links.txt
--rw-r--r--   0 sting    (144291) shenvi   (10405)        1 2024-04-20 03:45:27.000000 autodft-1.0.1/autodft.egg-info/not-zip-safe
--rw-r--r--   0 sting    (144291) shenvi   (10405)       57 2024-04-20 03:45:27.000000 autodft-1.0.1/autodft.egg-info/requires.txt
--rw-r--r--   0 sting    (144291) shenvi   (10405)        8 2024-04-20 03:45:27.000000 autodft-1.0.1/autodft.egg-info/top_level.txt
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-20 03:45:28.516677 autodft-1.0.1/scripts/
--rw-r--r--   0 sting    (144291) shenvi   (10405)     2282 2024-04-20 02:50:52.000000 autodft-1.0.1/scripts/autodft_flow.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     2295 2024-04-20 02:50:52.000000 autodft-1.0.1/scripts/autodft_flow_xyz.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     9216 2024-04-20 02:50:52.000000 autodft-1.0.1/scripts/compile_results.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     4975 2024-04-20 02:50:52.000000 autodft-1.0.1/scripts/gstatus.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)      500 2024-04-20 02:50:52.000000 autodft-1.0.1/scripts/run_autodft.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)      630 2024-04-20 02:50:52.000000 autodft-1.0.1/scripts/run_autodft_xyz.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)       38 2024-04-20 03:45:28.519357 autodft-1.0.1/setup.cfg
--rw-r--r--   0 sting    (144291) shenvi   (10405)     1065 2024-04-20 03:44:21.000000 autodft-1.0.1/setup.py
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:07:21.047680 autodft-1.0.2/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    35821 2024-04-28 22:04:45.000000 autodft-1.0.2/LICENSE.txt
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    11185 2024-04-28 22:07:21.046657 autodft-1.0.2/PKG-INFO
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    10989 2024-04-28 22:04:45.000000 autodft-1.0.2/README.md
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:07:21.023176 autodft-1.0.2/autodft/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:04:46.000000 autodft-1.0.2/autodft/__init__.py
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:07:21.031140 autodft-1.0.2/autodft/config/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:04:49.000000 autodft-1.0.2/autodft/config/__init__.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     1185 2024-04-28 22:04:49.000000 autodft-1.0.2/autodft/config/config.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     3041 2024-04-28 22:04:49.000000 autodft-1.0.2/autodft/config/default_parameters.yaml
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:07:21.035920 autodft-1.0.2/autodft/helpers/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/helpers/__init__.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     7402 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/helpers/crest_job.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    11913 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/helpers/gaussian_inputfile.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     3660 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/helpers/gaussian_manager.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    15776 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/helpers/user_input.py
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:07:21.039384 autodft-1.0.2/autodft/utils/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/utils/__init__.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     4269 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/utils/autodft_utils.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     2261 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/utils/files.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     5077 2024-04-28 22:04:50.000000 autodft-1.0.2/autodft/utils/gaussian_output.py
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:07:21.045431 autodft-1.0.2/autodft.egg-info/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    11185 2024-04-28 22:07:20.000000 autodft-1.0.2/autodft.egg-info/PKG-INFO
+-rw-r--r--   0 sting    (144291) shenvi   (10405)      747 2024-04-28 22:07:20.000000 autodft-1.0.2/autodft.egg-info/SOURCES.txt
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        1 2024-04-28 22:07:20.000000 autodft-1.0.2/autodft.egg-info/dependency_links.txt
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        1 2024-04-28 22:07:20.000000 autodft-1.0.2/autodft.egg-info/not-zip-safe
+-rw-r--r--   0 sting    (144291) shenvi   (10405)       57 2024-04-28 22:07:20.000000 autodft-1.0.2/autodft.egg-info/requires.txt
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        8 2024-04-28 22:07:20.000000 autodft-1.0.2/autodft.egg-info/top_level.txt
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-28 22:07:21.044498 autodft-1.0.2/scripts/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     2282 2024-04-28 22:04:47.000000 autodft-1.0.2/scripts/autodft_flow.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     2295 2024-04-28 22:04:47.000000 autodft-1.0.2/scripts/autodft_flow_xyz.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     9216 2024-04-28 22:04:47.000000 autodft-1.0.2/scripts/compile_results.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     4975 2024-04-28 22:04:47.000000 autodft-1.0.2/scripts/gstatus.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)      500 2024-04-28 22:04:47.000000 autodft-1.0.2/scripts/run_autodft.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)      630 2024-04-28 22:04:47.000000 autodft-1.0.2/scripts/run_autodft_xyz.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)       38 2024-04-28 22:07:21.047959 autodft-1.0.2/setup.cfg
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     1065 2024-04-28 22:04:45.000000 autodft-1.0.2/setup.py
```

### Comparing `autodft-1.0.1/LICENSE.txt` & `autodft-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/PKG-INFO` & `autodft-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodft
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automated conformer searching and DFT calculations
 Home-page: https://github.com/shenvilab/autodft
 Author: Shenvi Lab
 Author-email: sting@scripps.edu
 License: GPL-v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -209,60 +209,62 @@
 which can ultimately lead to invalid structures. Pay attention to any ChemDraw warnings:
 
 ![stereo_example3](images/stereo_example3.png)
 
 ### Custom settings
 If you would like, you can specify custom AutoDFT settings to use (including
 DFT level of theory). This is recommended if you routinely preform calculations
-at a different level of theory. To do this, copy/paste the below text, modify
-as desired, and save it as a file named ```config.yaml```. The text following
-the '#' symbols are descriptive comments and do not affect the settings.
+at a different level of theory. To do this, copy/paste the below text, which
+contains the default AutoDFT settings. Then, modify as desired, and save 
+as a new file named ```config.yaml```. The text following the '#' symbols are
+descriptive comments and do not affect the settings.
 
 Upload your ```config.yaml``` file to the computing cluster. When running
 AutoDFT in the future, you can respond ```n``` to the prompt about using the
-default settings for CREST, resources, etc. Then, provide the name of
-your ```config.yaml``` file when prompted (make sure you are in the folder
-containing the ```config.yaml``` file).
+default settings for CREST, resources, etc. Then, type ```config.yaml``` 
+when prompted (make sure you are in the folder containing the ```config.yaml``` file).
+
 
 ```
-autodft_flow:                          # Settings for 'chaperone' job
-  mem: 256mb                           # Memory
-  processors: 1                        # Number of processors
-  time: '30:00:00'                     # Wall time. Should be at least the sum of wall times for the CREST and Gaussian jobs
-  
+autodft_flow:                           # Settings for 'chaperone' job
+  mem: 128mb                            # Memory
+  processors: 1                         # Number of processors
+  time: '30:00:00'                      # Wall time (should be at least the sum of wall times for the CREST and Gaussian jobs)
+
 crest:
-  mem: 12gb                            # Memory
-  method: gfn2                         # Method
-  nprocshared: 16                      # Number of processors
-  rm_extra_files: true                 # Remove extra CREST files
-  solvent: ''                          # Solvent (do not include --gbsa flag)
-  time: '6:00:00'                      # Wall time
-  keywords: ''                         # Additional keywords
+  method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
+  solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
+  mem: 2gb                              # Memory
+  nprocshared: 12                       # Number of processors
+  time: '6:00:00'                       # Wall time
+  rm_extra_files: true                  # Remove extra CREST files  
+  keywords: ''                          # Additional keywords (see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
 
 gaussian_input:
-  version: '16'                        # Gaussian version (09 or 16)
-  maxjobs: 10                          # Maximum number of jobs to submit
-  mem: 12gb                            # Memory per job
-  nprocshared: 12                      # Processors per job
-  time: '24:00:00'                     # Wall time per job
-  write_chk: false                     # Whether to write and keep .chk files (Always written with linked jobs but this decides whether they are kept)
-
-gaussian_jobs:                         # Dashes indicate beginning of each job (can add or remove jobs as desired)
-- functional: B3LYP                    # Functional
-  basisset: GENECP                     # Basis set
-  route: Opt Freq SCF=XQC              # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
-  ecp_basisset_heavy: SDD              # For split basis sets, the basis set for heavy atoms (write null if not applicable)
-  ecp_basisset_light: 6-31G(d)         # For split basis sets, the basis set for light atoms (write null if not applicable)
-  ecp_cutoff: 36                       # For split basis sets, the maximum atomic number for light atoms  (write null if not applicable)
+  version: '16'                         # Version of Gaussian (09 or 16)
+  maxjobs: 10                           # Maximum number of jobs to submit
+  mem: 2gb                              # Memory per job
+  nprocshared: 12                       # Processors per job
+  time: '24:00:00'                      # Wall time per job
+  write_chk: false                      # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
+
+gaussian_jobs:                          # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
+- functional: B3LYP                     # Functional (for options, see: https://gaussian.com/dft/)
+  basisset: GENECP                      # Basis set (for options, see: https://gaussian.com/basissets/) (write GENECP for split basis set) 
+  route: Opt Freq SCF=XQC               # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
+  ecp_basisset_light: 6-31G(d)          # For split basis sets, the basis set for light atoms (write null if not applicable)
+  ecp_basisset_heavy: SDD               # For split basis sets, the basis set for heavy atoms (write null if not applicable)
+  ecp_cutoff: 36                        # For split basis sets, the maximum atomic number for light atoms (write null if not applicable)
 - functional: M062X
   basisset: def2TZVP
   route: ''
-  ecp_basisset_heavy: null
   ecp_basisset_light: null
+  ecp_basisset_heavy: null
   ecp_cutoff: null
-
+  
 goodvibes:
-  conc: '1'                            # Concentration (mol/L; 1 mol/L is solution phase standard state)
-  f_cutoff: '100'                      # Frequency cutoff (cm-1)
-  qs: truhlar                          # Quasiharmonic oscillator approximation method
-  keywords: ''                         # Additional keywords
+  conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
+  f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
+  qs: truhlar                           # Quasiharmonic oscillator approximation method
+  keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
+
 ```
```

### Comparing `autodft-1.0.1/README.md` & `autodft-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -192,60 +192,62 @@
 which can ultimately lead to invalid structures. Pay attention to any ChemDraw warnings:
 
 ![stereo_example3](images/stereo_example3.png)
 
 ### Custom settings
 If you would like, you can specify custom AutoDFT settings to use (including
 DFT level of theory). This is recommended if you routinely preform calculations
-at a different level of theory. To do this, copy/paste the below text, modify
-as desired, and save it as a file named ```config.yaml```. The text following
-the '#' symbols are descriptive comments and do not affect the settings.
+at a different level of theory. To do this, copy/paste the below text, which
+contains the default AutoDFT settings. Then, modify as desired, and save 
+as a new file named ```config.yaml```. The text following the '#' symbols are
+descriptive comments and do not affect the settings.
 
 Upload your ```config.yaml``` file to the computing cluster. When running
 AutoDFT in the future, you can respond ```n``` to the prompt about using the
-default settings for CREST, resources, etc. Then, provide the name of
-your ```config.yaml``` file when prompted (make sure you are in the folder
-containing the ```config.yaml``` file).
+default settings for CREST, resources, etc. Then, type ```config.yaml``` 
+when prompted (make sure you are in the folder containing the ```config.yaml``` file).
+
 
 ```
-autodft_flow:                          # Settings for 'chaperone' job
-  mem: 256mb                           # Memory
-  processors: 1                        # Number of processors
-  time: '30:00:00'                     # Wall time. Should be at least the sum of wall times for the CREST and Gaussian jobs
-  
+autodft_flow:                           # Settings for 'chaperone' job
+  mem: 128mb                            # Memory
+  processors: 1                         # Number of processors
+  time: '30:00:00'                      # Wall time (should be at least the sum of wall times for the CREST and Gaussian jobs)
+
 crest:
-  mem: 12gb                            # Memory
-  method: gfn2                         # Method
-  nprocshared: 16                      # Number of processors
-  rm_extra_files: true                 # Remove extra CREST files
-  solvent: ''                          # Solvent (do not include --gbsa flag)
-  time: '6:00:00'                      # Wall time
-  keywords: ''                         # Additional keywords
+  method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
+  solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
+  mem: 2gb                              # Memory
+  nprocshared: 12                       # Number of processors
+  time: '6:00:00'                       # Wall time
+  rm_extra_files: true                  # Remove extra CREST files  
+  keywords: ''                          # Additional keywords (see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
 
 gaussian_input:
-  version: '16'                        # Gaussian version (09 or 16)
-  maxjobs: 10                          # Maximum number of jobs to submit
-  mem: 12gb                            # Memory per job
-  nprocshared: 12                      # Processors per job
-  time: '24:00:00'                     # Wall time per job
-  write_chk: false                     # Whether to write and keep .chk files (Always written with linked jobs but this decides whether they are kept)
-
-gaussian_jobs:                         # Dashes indicate beginning of each job (can add or remove jobs as desired)
-- functional: B3LYP                    # Functional
-  basisset: GENECP                     # Basis set
-  route: Opt Freq SCF=XQC              # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
-  ecp_basisset_heavy: SDD              # For split basis sets, the basis set for heavy atoms (write null if not applicable)
-  ecp_basisset_light: 6-31G(d)         # For split basis sets, the basis set for light atoms (write null if not applicable)
-  ecp_cutoff: 36                       # For split basis sets, the maximum atomic number for light atoms  (write null if not applicable)
+  version: '16'                         # Version of Gaussian (09 or 16)
+  maxjobs: 10                           # Maximum number of jobs to submit
+  mem: 2gb                              # Memory per job
+  nprocshared: 12                       # Processors per job
+  time: '24:00:00'                      # Wall time per job
+  write_chk: false                      # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
+
+gaussian_jobs:                          # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
+- functional: B3LYP                     # Functional (for options, see: https://gaussian.com/dft/)
+  basisset: GENECP                      # Basis set (for options, see: https://gaussian.com/basissets/) (write GENECP for split basis set) 
+  route: Opt Freq SCF=XQC               # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
+  ecp_basisset_light: 6-31G(d)          # For split basis sets, the basis set for light atoms (write null if not applicable)
+  ecp_basisset_heavy: SDD               # For split basis sets, the basis set for heavy atoms (write null if not applicable)
+  ecp_cutoff: 36                        # For split basis sets, the maximum atomic number for light atoms (write null if not applicable)
 - functional: M062X
   basisset: def2TZVP
   route: ''
-  ecp_basisset_heavy: null
   ecp_basisset_light: null
+  ecp_basisset_heavy: null
   ecp_cutoff: null
-
+  
 goodvibes:
-  conc: '1'                            # Concentration (mol/L; 1 mol/L is solution phase standard state)
-  f_cutoff: '100'                      # Frequency cutoff (cm-1)
-  qs: truhlar                          # Quasiharmonic oscillator approximation method
-  keywords: ''                         # Additional keywords
+  conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
+  f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
+  qs: truhlar                           # Quasiharmonic oscillator approximation method
+  keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
+
 ```
```

### Comparing `autodft-1.0.1/autodft/config/config.py` & `autodft-1.0.2/autodft/config/config.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/autodft/config/default_parameters.yaml` & `autodft-1.0.2/autodft/config/default_parameters.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-autodft_flow:                                 # Settings for 'chaperone' job
-  mem: 128mb                                  # Memory
-  processors: 1                               # Number of processors
-  time: '30:00:00'                            # Wall time (should be at least the sum of wall times for the CREST and Gaussian jobs)
+autodft_flow:                           # Settings for 'chaperone' job
+  mem: 128mb                            # Memory
+  processors: 1                         # Number of processors
+  time: '30:00:00'                      # Wall time (should be at least the sum of wall times for the CREST and Gaussian jobs)
 
 crest:
-  method: gfn2                                # Method
-  solvent: ''                                 # Solvent (do not include --gbsa flag)
-  mem: 2gb                                    # Memory
-  nprocshared: 12                             # Number of processors
-  time: '6:00:00'                             # Wall time
-  rm_extra_files: true                        # Remove extra CREST files  
-  keywords: ''                                # Additional keywords
+  method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
+  solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
+  mem: 2gb                              # Memory
+  nprocshared: 12                       # Number of processors
+  time: '6:00:00'                       # Wall time
+  rm_extra_files: true                  # Remove extra CREST files  
+  keywords: ''                          # Additional keywords (see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
 
 gaussian_input:
-  version: '16'                               # Version of Gaussian (09 or 16)
-  maxjobs: 10                                 # Maximum number of jobs to submit
-  mem: 2gb                                    # Memory per job
-  nprocshared: 12                             # Processors per job
-  time: '24:00:00'                            # Wall time per job
-  write_chk: false                            # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
+  version: '16'                         # Version of Gaussian (09 or 16)
+  maxjobs: 10                           # Maximum number of jobs to submit
+  mem: 2gb                              # Memory per job
+  nprocshared: 12                       # Processors per job
+  time: '24:00:00'                      # Wall time per job
+  write_chk: false                      # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
 
-gaussian_jobs:                                # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
-- functional: B3LYP                           # Functional
-  basisset: GENECP                            # Basis set
-  route: Opt Freq SCF=XQC                     # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
-  ecp_basisset_light: 6-31G(d)                # For split basis sets, the basis set for light atoms
-  ecp_basisset_heavy: SDD                     # For split basis sets, the basis set for heavy atoms
-  ecp_cutoff: 36                              # For split basis sets, the maximum atomic number for light atoms
+gaussian_jobs:                          # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
+- functional: B3LYP                     # Functional (for options, see: https://gaussian.com/dft/)
+  basisset: GENECP                      # Basis set (for options, see: https://gaussian.com/basissets/) (write GENECP for split basis set) 
+  route: Opt Freq SCF=XQC               # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
+  ecp_basisset_light: 6-31G(d)          # For split basis sets, the basis set for light atoms (write null if not applicable)
+  ecp_basisset_heavy: SDD               # For split basis sets, the basis set for heavy atoms (write null if not applicable)
+  ecp_cutoff: 36                        # For split basis sets, the maximum atomic number for light atoms (write null if not applicable)
 - functional: M062X
   basisset: def2TZVP
   route: ''
   ecp_basisset_light: null
   ecp_basisset_heavy: null
   ecp_cutoff: null
   
 goodvibes:
-  conc: '1'                                   # Concentration (mol/L; 1 mol/L is solution phase standard state)
-  f_cutoff: '100'                             # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
-  qs: truhlar                                 # Quasiharmonic oscillator approximation method
-  keywords: ''                                # Additional keywords
+  conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
+  f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
+  qs: truhlar                           # Quasiharmonic oscillator approximation method
+  keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
```

### Comparing `autodft-1.0.1/autodft/helpers/crest_job.py` & `autodft-1.0.2/autodft/helpers/crest_job.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,21 @@
         logger.info('Submitting CREST job to SLURM...')
         subprocess.run(['sbatch', '-W', CREST_SCRIPT])
         
 
     def cleanup(self) -> None:
         """Organizes files after completion of the CREST job"""
 
+        # Check for normal termination of CREST job
+        with open(f'{self.molname}_crest.out') as f:
+            last_line = f.readlines()[-1]
+            if 'CREST terminated normally.' not in last_line:
+                raise CRESTAbnormalTerminationError()
+        logger.info('CREST terminated normally.')
+
         # Remove unnecessary files
         if self.rm_extra_files:
             to_keep = [f'{self.molname}.out',
                        f'{self.molname}_crest.out',
                        'crest_conformers.xyz',
                        f'autodft_{self.molname}.json',
                        'autodft_parameters.yaml']
@@ -119,21 +126,14 @@
                 except OSError:
                     print(f'Unable to delete: {f}')
 
         # Rename output file
         os.rename('crest_conformers.xyz',
                   f'{self.molname}_crest_conformers.xyz')
 
-        # Check for normal termination of CREST job
-        with open(f'{self.molname}_crest.out') as f:
-            last_line = f.readlines()[-1]
-            if 'CREST terminated normally.' not in last_line:
-                raise CRESTAbnormalTerminationError()
-        logger.info('CREST terminated normally.')
-
     def get_conf_cartesians(self) -> None:
         """Returns cartesian coordinates for each conformer generated by CREST.
         The conformers are ordered starting with the lowest energy."""
 
         xyz_blocks = []
 
         with open(self.molname + '_crest_conformers.xyz') as f:
```

### Comparing `autodft-1.0.1/autodft/helpers/gaussian_inputfile.py` & `autodft-1.0.2/autodft/helpers/gaussian_inputfile.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/autodft/helpers/gaussian_manager.py` & `autodft-1.0.2/autodft/helpers/gaussian_manager.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/autodft/helpers/user_input.py` & `autodft-1.0.2/autodft/helpers/user_input.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/autodft/utils/autodft_utils.py` & `autodft-1.0.2/autodft/utils/autodft_utils.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/autodft/utils/files.py` & `autodft-1.0.2/autodft/utils/files.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import glob
 import os
 import sys
 
+from autodft.utils.gaussian_output import is_gaussian_logfile
+
 
 # CONSTANTS
 INDENT = ' ' * 3
 
 
 def print_indent(msg: str) -> None:
     """Prints an indented message"""
@@ -14,25 +16,26 @@
         print(INDENT + line)
     if msg.endswith('\n'):
         print('')
 
 
 def log_files(dirs: list[str] = None) -> list[str]:
     """Takes a sequence of directory names and returns a dictionary of
-    directories to .log files. If no directories are given, the current
-    directory is used (denoted as '.')"""
+    directories to Gaussian .log files. If no directories are given, the
+    current directory is used (denoted as '.')"""
 
     dirs = ['.'] if not dirs else [d for d in dirs if os.path.isdir(d)]
     logfile_dict = {}
 
     for d in dirs:
-        logfiles_in_dir = [x for x in os.listdir(d) if x.endswith('.log')]
+        logfiles_in_dir = [x for x in os.listdir(d) if is_gaussian_logfile(f'{d}/{x}')]
         logfiles_in_dir.sort(key=lambda x: (molname_from_log(x), filenum(x)))
         if logfiles_in_dir:
             logfile_dict[d] = logfiles_in_dir
+    
     if not logfile_dict:
         print('\n  No .log files in the specified directory(s)\n')
         sys.exit()
     logfile_dict = dict(sorted(logfile_dict.items()))
     return logfile_dict
```

### Comparing `autodft-1.0.1/autodft/utils/gaussian_output.py` & `autodft-1.0.2/autodft/utils/gaussian_output.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/autodft.egg-info/PKG-INFO` & `autodft-1.0.2/autodft.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodft
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automated conformer searching and DFT calculations
 Home-page: https://github.com/shenvilab/autodft
 Author: Shenvi Lab
 Author-email: sting@scripps.edu
 License: GPL-v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -209,60 +209,62 @@
 which can ultimately lead to invalid structures. Pay attention to any ChemDraw warnings:
 
 ![stereo_example3](images/stereo_example3.png)
 
 ### Custom settings
 If you would like, you can specify custom AutoDFT settings to use (including
 DFT level of theory). This is recommended if you routinely preform calculations
-at a different level of theory. To do this, copy/paste the below text, modify
-as desired, and save it as a file named ```config.yaml```. The text following
-the '#' symbols are descriptive comments and do not affect the settings.
+at a different level of theory. To do this, copy/paste the below text, which
+contains the default AutoDFT settings. Then, modify as desired, and save 
+as a new file named ```config.yaml```. The text following the '#' symbols are
+descriptive comments and do not affect the settings.
 
 Upload your ```config.yaml``` file to the computing cluster. When running
 AutoDFT in the future, you can respond ```n``` to the prompt about using the
-default settings for CREST, resources, etc. Then, provide the name of
-your ```config.yaml``` file when prompted (make sure you are in the folder
-containing the ```config.yaml``` file).
+default settings for CREST, resources, etc. Then, type ```config.yaml``` 
+when prompted (make sure you are in the folder containing the ```config.yaml``` file).
+
 
 ```
-autodft_flow:                          # Settings for 'chaperone' job
-  mem: 256mb                           # Memory
-  processors: 1                        # Number of processors
-  time: '30:00:00'                     # Wall time. Should be at least the sum of wall times for the CREST and Gaussian jobs
-  
+autodft_flow:                           # Settings for 'chaperone' job
+  mem: 128mb                            # Memory
+  processors: 1                         # Number of processors
+  time: '30:00:00'                      # Wall time (should be at least the sum of wall times for the CREST and Gaussian jobs)
+
 crest:
-  mem: 12gb                            # Memory
-  method: gfn2                         # Method
-  nprocshared: 16                      # Number of processors
-  rm_extra_files: true                 # Remove extra CREST files
-  solvent: ''                          # Solvent (do not include --gbsa flag)
-  time: '6:00:00'                      # Wall time
-  keywords: ''                         # Additional keywords
+  method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
+  solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
+  mem: 2gb                              # Memory
+  nprocshared: 12                       # Number of processors
+  time: '6:00:00'                       # Wall time
+  rm_extra_files: true                  # Remove extra CREST files  
+  keywords: ''                          # Additional keywords (see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
 
 gaussian_input:
-  version: '16'                        # Gaussian version (09 or 16)
-  maxjobs: 10                          # Maximum number of jobs to submit
-  mem: 12gb                            # Memory per job
-  nprocshared: 12                      # Processors per job
-  time: '24:00:00'                     # Wall time per job
-  write_chk: false                     # Whether to write and keep .chk files (Always written with linked jobs but this decides whether they are kept)
-
-gaussian_jobs:                         # Dashes indicate beginning of each job (can add or remove jobs as desired)
-- functional: B3LYP                    # Functional
-  basisset: GENECP                     # Basis set
-  route: Opt Freq SCF=XQC              # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
-  ecp_basisset_heavy: SDD              # For split basis sets, the basis set for heavy atoms (write null if not applicable)
-  ecp_basisset_light: 6-31G(d)         # For split basis sets, the basis set for light atoms (write null if not applicable)
-  ecp_cutoff: 36                       # For split basis sets, the maximum atomic number for light atoms  (write null if not applicable)
+  version: '16'                         # Version of Gaussian (09 or 16)
+  maxjobs: 10                           # Maximum number of jobs to submit
+  mem: 2gb                              # Memory per job
+  nprocshared: 12                       # Processors per job
+  time: '24:00:00'                      # Wall time per job
+  write_chk: false                      # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
+
+gaussian_jobs:                          # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
+- functional: B3LYP                     # Functional (for options, see: https://gaussian.com/dft/)
+  basisset: GENECP                      # Basis set (for options, see: https://gaussian.com/basissets/) (write GENECP for split basis set) 
+  route: Opt Freq SCF=XQC               # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
+  ecp_basisset_light: 6-31G(d)          # For split basis sets, the basis set for light atoms (write null if not applicable)
+  ecp_basisset_heavy: SDD               # For split basis sets, the basis set for heavy atoms (write null if not applicable)
+  ecp_cutoff: 36                        # For split basis sets, the maximum atomic number for light atoms (write null if not applicable)
 - functional: M062X
   basisset: def2TZVP
   route: ''
-  ecp_basisset_heavy: null
   ecp_basisset_light: null
+  ecp_basisset_heavy: null
   ecp_cutoff: null
-
+  
 goodvibes:
-  conc: '1'                            # Concentration (mol/L; 1 mol/L is solution phase standard state)
-  f_cutoff: '100'                      # Frequency cutoff (cm-1)
-  qs: truhlar                          # Quasiharmonic oscillator approximation method
-  keywords: ''                         # Additional keywords
+  conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
+  f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
+  qs: truhlar                           # Quasiharmonic oscillator approximation method
+  keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
+
 ```
```

### Comparing `autodft-1.0.1/autodft.egg-info/SOURCES.txt` & `autodft-1.0.2/autodft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/scripts/autodft_flow.py` & `autodft-1.0.2/scripts/autodft_flow.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/scripts/autodft_flow_xyz.py` & `autodft-1.0.2/scripts/autodft_flow_xyz.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/scripts/compile_results.py` & `autodft-1.0.2/scripts/compile_results.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/scripts/gstatus.py` & `autodft-1.0.2/scripts/gstatus.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/scripts/run_autodft_xyz.py` & `autodft-1.0.2/scripts/run_autodft_xyz.py`

 * *Files identical despite different names*

### Comparing `autodft-1.0.1/setup.py` & `autodft-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description=f.read()
 
 setup(
     name='autodft',
-    version='1.0.1',
+    version='1.0.2',
     author='Shenvi Lab',
     author_email='sting@scripps.edu',
     url='https://github.com/shenvilab/autodft',
     description='Automated conformer searching and DFT calculations',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

