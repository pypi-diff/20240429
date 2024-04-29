# Comparing `tmp/nwb4fp-0.6.0.9.tar.gz` & `tmp/nwb4fp-0.6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.0.9.tar", last modified: Mon Apr 29 11:05:37 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.1.0.tar", last modified: Mon Apr 29 13:36:23 2024, max compression
```

## Comparing `nwb4fp-0.6.0.9.tar` & `nwb4fp-0.6.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:38.101150 nwb4fp-0.6.0.9/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.0.9/LICENSE
--rw-rw-rw-   0        0        0     5746 2024-04-29 11:05:38.095140 nwb4fp-0.6.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 11:05:38.115139 nwb4fp-0.6.0.9/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-04-29 11:05:33.000000 nwb4fp-0.6.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:37.376144 nwb4fp-0.6.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:37.501146 nwb4fp-0.6.0.9/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.0.9/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:37.592141 nwb4fp-0.6.0.9/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.0.9/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.0.9/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:37.797140 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17085 2024-04-29 10:32:35.000000 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    13220 2024-04-26 10:54:41.000000 nwb4fp-0.6.0.9/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:37.987141 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     7290 2024-04-29 11:05:13.000000 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.9/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:37.396147 nwb4fp-0.6.0.9/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:37.999140 nwb4fp-0.6.0.9/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.0.9/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1425 2024-04-28 10:02:22.000000 nwb4fp-0.6.0.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.0.9/src/nwb4fp/test/run_scripts/test.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:05:37.570141 nwb4fp-0.6.0.9/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5746 2024-04-29 11:05:37.000000 nwb4fp-0.6.0.9/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2024-04-29 11:05:37.000000 nwb4fp-0.6.0.9/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:05:37.000000 nwb4fp-0.6.0.9/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2892 2024-04-29 11:05:37.000000 nwb4fp-0.6.0.9/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-29 11:05:37.000000 nwb4fp-0.6.0.9/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.772516 nwb4fp-0.6.1.0/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5746 2024-04-29 13:36:23.760513 nwb4fp-0.6.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 13:36:23.793513 nwb4fp-0.6.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-04-29 13:36:19.000000 nwb4fp-0.6.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.115515 nwb4fp-0.6.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.240519 nwb4fp-0.6.1.0/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.1.0/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.325518 nwb4fp-0.6.1.0/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.1.0/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.1.0/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.497514 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17085 2024-04-29 10:32:35.000000 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    13220 2024-04-26 10:54:41.000000 nwb4fp-0.6.1.0/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.635514 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8152 2024-04-29 13:34:38.000000 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.0/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.141524 nwb4fp-0.6.1.0/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.731514 nwb4fp-0.6.1.0/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.1.0/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1425 2024-04-28 10:02:22.000000 nwb4fp-0.6.1.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.1.0/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.1.0/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:36:23.293514 nwb4fp-0.6.1.0/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5746 2024-04-29 13:36:22.000000 nwb4fp-0.6.1.0/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1040 2024-04-29 13:36:22.000000 nwb4fp-0.6.1.0/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 13:36:22.000000 nwb4fp-0.6.1.0/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2892 2024-04-29 13:36:22.000000 nwb4fp-0.6.1.0/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-29 13:36:22.000000 nwb4fp-0.6.1.0/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.0.9/LICENSE` & `nwb4fp-0.6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/PKG-INFO` & `nwb4fp-0.6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.0.9
+Version: 0.6.1.0
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.0.9/README.md` & `nwb4fp-0.6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/setup.py` & `nwb4fp-0.6.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.0.9',
+    version='0.6.1.0',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.1.0/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.1.0/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.1.0/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.1.0/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.1.0/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.1.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.1.0/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.1.0/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.1.0/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pynwb import NWBHDF5IO
 import numpy as np
 from pynwb.ecephys import LFP, ElectricalSeries
 #from preprocess.down_sample_lfp import down_sample_lfp
 import numpy as np
 import pandas as pd
 import spikeinterface.preprocessing as spre
-
+import spikeinterface as si
 
 def main():
     print(main)
 
 def down_sample_lfp(file_path,raw_path):
     #raw_path = r'S:\Sachuriga/Ephys_Recording/CR_CA1/65409/65409_2023-12-04_15-42-35_A'
     stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-100.Rhythm Data'
@@ -85,26 +85,47 @@
     
     # lfp_slice=lfp.channel_slice(channel_ids=['CH4', 'CH9', 'CH25',
     #                                          'CH17', 'CH11', 'CH2',
     #                                          'CH32', 'CH16', 'CH14',
     #                                          'CH59', 'CH54', 'CH51',
     #                                          'CH53', 'CH58', 'CH64',
     #                                          'CH47', 'CH36', 'CH56'])
+    origin = recording_prb.get_property('channel_name')
+    new = recording_good_channels_f.get_property('channel_name')
+    region = []
+    for id in new:
+        region.append(np.int32(np.where(origin==id)[0])[0])
 
-    print("get_traces() shape:")
-    np_lfp_car = lfp_car.get_traces()
-    np_lfp = lfp.get_traces()
     path_iron = Path(file_path)
+    np_lfp_car = load_lfp2mem(lfp_car)
+    np.save(path_iron / fr'lfp_car.npy',  np_lfp_car.get_traces(return_scaled=True))
+    del np_lfp_car
+
+    np_lfp = load_lfp2mem(lfp)
+    np.save(path_iron / fr'lfp_raw.npy',  np_lfp.get_traces(return_scaled=True))
+    del np_lfp 
+
     np.save(path_iron / 'lfp_times.npy', lfp_times) # type: ignore
-    np.save(path_iron / 'lfp_car.npy',  np_lfp_car)
-    np.save(path_iron / 'lfp_raw.npy', np_lfp)  # Save the LFP data
+    # np.save(path_iron / 'lfp_car.npy',  np_lfp_car)
+    # np.save(path_iron / 'lfp_raw.npy', np_lfp)  # Save the LFP data
     # print(f"shape {np_lfp.shape}")
     # print(f"descriptions{lfp.get_binary_description()}")
     # print(np_lfp)
-    return bad_channel_ids
+    return region
+
+def load_lfp2mem(lfp):
+    from pathlib import Path
+    job_kwargs = dict(n_jobs=40,
+                              chunk_duration="5s",
+                              progress_bar=True)
+    base_folder = Path(".")
+    preprocessed = "_" + "preprocessed_temp"
+    lfp.save(folder=base_folder / preprocessed, overwrite=True, **job_kwargs)
+    recording_rec = si.load_extractor(base_folder / preprocessed)
+    return recording_rec
 
 def add_lfp2nwb(filename,channel2selec,folder1_path):
 
     with NWBHDF5IO(filename, "r+") as io:
         read_nwbfile = io.read()
         region=channel2selec
         # create a TimeSeries and add it to the file under the acquisition group
@@ -117,15 +138,15 @@
         lfp_times = np.load(fr"{folder1_path}/lfp_times.npy")
         lfp_raw = np.load(fr"{folder1_path}/lfp_raw.npy")
         lfp_car = np.load(fr"{folder1_path}/lfp_car.npy")
         lfp_electrical_series = ElectricalSeries(
             name="lfp_raw",
             data=lfp_raw,
             electrodes=regions,
-            starting_time=np.float64(lfp_times[0]),
+            # starting_time=np.float64(lfp_times[0]),
             rate=1000.0)
         lfp = LFP(electrical_series=lfp_electrical_series)
         ecephys_module = read_nwbfile.create_processing_module(name="lfp_raw", 
                                                         description="1-475Hz, 1000Hz sampling rate, raw extracellular electrophysiology data")
         ecephys_module.add(lfp)
         
         #np_lfp = read_nwbfile.modules["ecephys_raw"].data_interfaces['LFP']['lfp_raw']
@@ -135,15 +156,15 @@
         ecephys_car_module = read_nwbfile.create_processing_module(name="lfp_car", 
                                                         description="1-475Hz, 1000Hz sampling rate, common average reference extracellular electrophysiology data")
 
         lfp_car_electrical_series = ElectricalSeries(
             name="lfp_car",
             data=lfp_car,
             electrodes=regions,
-            starting_time=np.float64(lfp_times[0]),
+            #starting_time=np.float64(lfp_times[0]),
             rate=1000.0)
         lfp_car = LFP(electrical_series=lfp_car_electrical_series)
         ecephys_car_module.add(lfp_car)
         
         #np_lfp_car = read_nwbfile.modules["ecephys_car"].data_interfaces['LFP']['lfp_car']
         #ch_car = np_lfp_car.electrodes.to_dataframe()['channel_name'].tolist()
         #df = pd.DataFrame(np_lfp.data, columns = ch_car)
```

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.1.0/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.1.0/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.1.0/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.1.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.1.0/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.0.9
+Version: 0.6.1.0
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.1.0/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 src/nwb4fp/preprocess/down_sample_lfp.py
 src/nwb4fp/preprocess/extract_lfp.py
 src/nwb4fp/preprocess/get_path.py
 src/nwb4fp/preprocess/load_data.py
 src/nwb4fp/preprocess/run_phy.py
 src/nwb4fp/test/run_scripts/readnwb.py
 src/nwb4fp/test/run_scripts/readnwb_09PC.py
-src/nwb4fp/test/run_scripts/test.py
+src/nwb4fp/test/run_scripts/test.py
+src/nwb4fp/test/run_scripts/test_lfp.py
```

### Comparing `nwb4fp-0.6.0.9/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.1.0/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

