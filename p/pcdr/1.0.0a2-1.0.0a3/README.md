# Comparing `tmp/pcdr-1.0.0a2.tar.gz` & `tmp/pcdr-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdr-1.0.0a2.tar", last modified: Tue Apr 23 15:55:17 2024, max compression
+gzip compressed data, was "pcdr-1.0.0a3.tar", last modified: Mon Apr 29 11:49:20 2024, max compression
```

## Comparing `pcdr-1.0.0a2.tar` & `pcdr-1.0.0a3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/
--rw-r--r--   0 j         (1000) j         (1000)    35149 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/LICENSE
--rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     1191 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/README.md
--rw-r--r--   0 j         (1000) j         (1000)      613 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/pyproject.toml
--rw-r--r--   0 j         (1000) j         (1000)       38 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/setup.cfg
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.992619 pcdr-1.0.0a2/src/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.992619 pcdr-1.0.0a2/src/pcdr/
--rw-r--r--   0 j         (1000) j         (1000)      781 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/__init__.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.996619 pcdr-1.0.0a2/src/pcdr/_beta/
--rw-r--r--   0 j         (1000) j         (1000)     3106 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_beta/gnuradio_receiver.py
--rw-r--r--   0 j         (1000) j         (1000)     7098 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_beta/gnuradio_sendlike.py
--rw-r--r--   0 j         (1000) j         (1000)     1774 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     3866 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     9152 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_flow_impl.py
--rw-r--r--   0 j         (1000) j         (1000)     2766 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_helpers.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.996619 pcdr-1.0.0a2/src/pcdr/_internal/
--rw-r--r--   0 j         (1000) j         (1000)     3989 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/basictermplot.py
--rw-r--r--   0 j         (1000) j         (1000)     1565 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/fileio.py
--rw-r--r--   0 j         (1000) j         (1000)    16005 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/misc.py
--rw-r--r--   0 j         (1000) j         (1000)     7650 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/our_GR_blocks.py
--rw-r--r--   0 j         (1000) j         (1000)     2456 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/queue_to_guisink_flowgraph.py
--rwxr-xr-x   0 j         (1000) j         (1000)     5357 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/queue_to_waterfall_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)      657 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/types_and_contracts.py
--rw-r--r--   0 j         (1000) j         (1000)     3013 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/vector_to_guisink_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     3471 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/vector_tx_flowgraphs.py
--rw-r--r--   0 j         (1000) j         (1000)     1451 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/wrapped_GR_blocks.py
--rw-r--r--   0 j         (1000) j         (1000)     5185 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_modulators.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.996619 pcdr-1.0.0a2/src/pcdr/_queue/
--rw-r--r--   0 j         (1000) j         (1000)       51 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_queue/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     6343 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_queue/sink.py
--rw-r--r--   0 j         (1000) j         (1000)     1199 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_queue/source.py
--rw-r--r--   0 j         (1000) j         (1000)    46825 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_wavegen.py
--rw-r--r--   0 j         (1000) j         (1000)      141 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/flow.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/src/pcdr.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     1189 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       40 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        5 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/top_level.txt
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/tests/
--rw-r--r--   0 j         (1000) j         (1000)      838 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_gnuradio_vector_tx_flowgraphs.py
--rw-r--r--   0 j         (1000) j         (1000)      939 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_gnuradio_write_file_and_read_file.py
--rw-r--r--   0 j         (1000) j         (1000)      308 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_helpers.py
--rw-r--r--   0 j         (1000) j         (1000)     2988 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_multiple.py
--rw-r--r--   0 j         (1000) j         (1000)     5648 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_other__blocks_for_testing.py
--rw-r--r--   0 j         (1000) j         (1000)     2498 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_our_GR_blocks.py
--rw-r--r--   0 j         (1000) j         (1000)     1705 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_simple.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-29 11:49:20.525245 pcdr-1.0.0a3/
+-rw-r--r--   0 j         (1000) j         (1000)    35149 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/LICENSE
+-rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-29 11:49:20.525245 pcdr-1.0.0a3/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1191 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/README.md
+-rw-r--r--   0 j         (1000) j         (1000)      613 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/pyproject.toml
+-rw-r--r--   0 j         (1000) j         (1000)       38 2024-04-29 11:49:20.525245 pcdr-1.0.0a3/setup.cfg
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-29 11:49:20.521246 pcdr-1.0.0a3/src/
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-29 11:49:20.521246 pcdr-1.0.0a3/src/pcdr/
+-rw-r--r--   0 j         (1000) j         (1000)      781 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/__init__.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-29 11:49:20.525245 pcdr-1.0.0a3/src/pcdr/_beta/
+-rw-r--r--   0 j         (1000) j         (1000)     3106 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_beta/gnuradio_receiver.py
+-rw-r--r--   0 j         (1000) j         (1000)     7098 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_beta/gnuradio_sendlike.py
+-rw-r--r--   0 j         (1000) j         (1000)     1774 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     3866 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     9266 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_flow_impl.py
+-rw-r--r--   0 j         (1000) j         (1000)     2766 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_helpers.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-29 11:49:20.525245 pcdr-1.0.0a3/src/pcdr/_internal/
+-rw-r--r--   0 j         (1000) j         (1000)     3989 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/basictermplot.py
+-rw-r--r--   0 j         (1000) j         (1000)     1565 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/fileio.py
+-rw-r--r--   0 j         (1000) j         (1000)    16005 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/misc.py
+-rw-r--r--   0 j         (1000) j         (1000)     7650 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/our_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     2456 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/queue_to_guisink_flowgraph.py
+-rwxr-xr-x   0 j         (1000) j         (1000)     5357 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/queue_to_waterfall_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)      791 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/types_and_contracts.py
+-rw-r--r--   0 j         (1000) j         (1000)     3013 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/vector_to_guisink_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     3471 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/vector_tx_flowgraphs.py
+-rw-r--r--   0 j         (1000) j         (1000)     1451 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_internal/wrapped_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     5185 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_modulators.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-29 11:49:20.525245 pcdr-1.0.0a3/src/pcdr/_queue/
+-rw-r--r--   0 j         (1000) j         (1000)       51 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_queue/__init__.py
+-rw-r--r--   0 j         (1000) j         (1000)     6343 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_queue/sink.py
+-rw-r--r--   0 j         (1000) j         (1000)     1199 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_queue/source.py
+-rw-r--r--   0 j         (1000) j         (1000)    46825 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/_wavegen.py
+-rw-r--r--   0 j         (1000) j         (1000)      132 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/src/pcdr/flow.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-29 11:49:20.525245 pcdr-1.0.0a3/src/pcdr.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-29 11:49:20.000000 pcdr-1.0.0a3/src/pcdr.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1189 2024-04-29 11:49:20.000000 pcdr-1.0.0a3/src/pcdr.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2024-04-29 11:49:20.000000 pcdr-1.0.0a3/src/pcdr.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       40 2024-04-29 11:49:20.000000 pcdr-1.0.0a3/src/pcdr.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        5 2024-04-29 11:49:20.000000 pcdr-1.0.0a3/src/pcdr.egg-info/top_level.txt
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-29 11:49:20.525245 pcdr-1.0.0a3/tests/
+-rw-r--r--   0 j         (1000) j         (1000)      838 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/tests/test_gnuradio_vector_tx_flowgraphs.py
+-rw-r--r--   0 j         (1000) j         (1000)      939 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/tests/test_gnuradio_write_file_and_read_file.py
+-rw-r--r--   0 j         (1000) j         (1000)      308 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/tests/test_helpers.py
+-rw-r--r--   0 j         (1000) j         (1000)     2988 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/tests/test_multiple.py
+-rw-r--r--   0 j         (1000) j         (1000)     5648 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/tests/test_other__blocks_for_testing.py
+-rw-r--r--   0 j         (1000) j         (1000)     2498 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/tests/test_our_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     1718 2024-04-29 11:49:12.000000 pcdr-1.0.0a3/tests/test_simple.py
```

### Comparing `pcdr-1.0.0a2/LICENSE` & `pcdr-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/PKG-INFO` & `pcdr-1.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdr
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: GNU Radio-based transmit and receive wrappers and more
 Author: james-pcdr
 Project-URL: Homepage, https://github.com/python-can-define-radio/pcdr
 Project-URL: Bug Tracker, https://github.com/python-can-define-radio/pcdr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pcdr-1.0.0a2/README.md` & `pcdr-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/pyproject.toml` & `pcdr-1.0.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pcdr"
-version = "1.0.0a2"
+version = "1.0.0a3"
 authors = [
   { name="james-pcdr" },
 ]
 description = "GNU Radio-based transmit and receive wrappers and more"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["numpy", "termcolor", "typeguard", "attrs>=21.3.0"]
```

### Comparing `pcdr-1.0.0a2/src/pcdr/__init__.py` & `pcdr-1.0.0a3/src/pcdr/__init__.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_beta/gnuradio_receiver.py` & `pcdr-1.0.0a3/src/pcdr/_beta/gnuradio_receiver.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_beta/gnuradio_sendlike.py` & `pcdr-1.0.0a3/src/pcdr/_beta/gnuradio_sendlike.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py` & `pcdr-1.0.0a3/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py` & `pcdr-1.0.0a3/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_flow_impl.py` & `pcdr-1.0.0a3/src/pcdr/_flow_impl.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,25 +15,26 @@
     Startable, StopAndWaitable, Waitable, IFGainSettable,
     BBGainSettable, CenterFrequencySettable, ProbeReadable
 )
 from pcdr._internal.types_and_contracts import HasWorkFunc
 
 
 
-class OsmosdrSingleFreqReceiver(Startable, StopAndWaitable, IFGainSettable, BBGainSettable):
-    """A simplified interface to the Osmosdr Source
-    which measures the strength of only the specified frequency.
+class OsmoSingleFreqReceiver(Startable, StopAndWaitable, IFGainSettable, BBGainSettable):
+    """Measures the strength of only the specified frequency.
+    
     Example usage:
     
     ```python3
-    import pcdr.simple
-    receiver = pcdr.simple.OsmosdrReceiver("hackrf=0", 103.9e6)
+    from pcdr.flow import OsmoSingleFreqReceiver
+    receiver = OsmoSingleFreqReceiver("hackrf=0", 103.9e6)
     recevier.start()
     strength = receiver.get_strength()
     print(strength)
+    recevier.stop_and_wait()
     ```
     """
     @typechecked
     def __init__(self, device_args: str, freq: float):
         """
         `device_args`: For example, "hackrf=0", etc. See the osmocom docs for a full list.
         `freq`: The frequency which the device will tune to. See note on `set_freq` for more info.
@@ -48,15 +49,15 @@
         self.__stream_to_vec = blocks.stream_to_vector(gr.sizeof_gr_complex, fft_size)
         self.__streng = Blk_strength_at_freq(self._osmoargs.samp_rate, self.__freq_offset, fft_size)
         self._tb.connect(self._osmo, self.__stream_to_vec, self.__streng)
         
     @typechecked
     def get_strength(self, block: bool = True, timeout: float = 2.0) -> float:
         """Get the signal strength at the current frequency.
-        The frequency is specified when the `OsmosdrReceiver` is created,
+        The frequency is specified when the `OsmoSingleFreqReceiver` is created,
         and can be changed using `set_freq`.
         """
         return self.__streng._reading.get(block, timeout)
     
     @typechecked
     def set_freq(self, freq: float, seconds: float = 0.5):
         """
@@ -74,26 +75,25 @@
         true_freq = freq - self.__freq_offset
         self._osmoargs.center_freq = true_freq
         retval = self._osmo.set_center_freq(true_freq)
         time.sleep(seconds)
         return retval
 
 
-class OsmosdrSingleFreqTransmitter(Startable, StopAndWaitable,
+class OsmoSingleFreqTransmitter(Startable, StopAndWaitable,
                          IFGainSettable, BBGainSettable,
                          CenterFrequencySettable):
-    """A simplified interface to the Osmosdr Sink
-    which transmits a pure sine wave on the specified frequency.
+    """Transmits a pure sine wave on the specified frequency.
     
     Example usage:
     
     ```python3
-    import pcdr.simple
+    from pcdr.flow import OsmoSingleFreqTransmitter
     import time
-    transmitter = pcdr.simple.OsmosdrTransmitter("hackrf=0", 2.45e9)
+    transmitter = OsmoSingleFreqTransmitter("hackrf=0", 2.45e9)
     transmitter.start()
     transmitter.set_if_gain(37)
     time.sleep(1)
     transmitter.set_center_freq(2.4501e9)
     time.sleep(1)
     transmitter.set_center_freq(2.4502e9)
     time.sleep(1)
@@ -169,24 +169,26 @@
         elif location == "audio_sink":
             # this is the feeder block for the audio sink
             src_blk = self.__source  
             type_ = np.float32
         self._probe = connect_probe_common(self._tb, src_blk, type_, vecsize)
 
 
-class OsmosdrWBFMTransmitter(Startable, StopAndWaitable, CenterFrequencySettable,
+class OsmoWBFMTransmitter(Startable, StopAndWaitable, CenterFrequencySettable,
                              IFGainSettable, BBGainSettable, Waitable):
     """
+    Transmits Wide-Band Frequency Modulated audio on the specified frequency.
+    
     ```python3
-    import pcdr.simple
+    from pcdr.flow import OsmoWBFMTransmitter
     import time
-    transmitter = pcdr.simple.OsmosdrWBFMTransmitter("hackrf=0", 2.45e9, "pulse_monitor")
+    transmitter = OsmoWBFMTransmitter("hackrf=0", 2.45e9, "pulse_monitor")
     transmitter.start()
     transmitter.set_if_gain(37)
-    time.sleep(10)
+    time.sleep(10)  # During this time, the transmitter is transmitting.
     transmitter.stop_and_wait()
     ```
     """
     @typechecked
     def __init__(self, device_args: str, freq: float, *,
                  audio_device: Optional[str] = None,
                  wavfile: Optional[Union[str, Path]] = None,
```

### Comparing `pcdr-1.0.0a2/src/pcdr/_helpers.py` & `pcdr-1.0.0a3/src/pcdr/_helpers.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/basictermplot.py` & `pcdr-1.0.0a3/src/pcdr/_internal/basictermplot.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/fileio.py` & `pcdr-1.0.0a3/src/pcdr/_internal/fileio.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/misc.py` & `pcdr-1.0.0a3/src/pcdr/_internal/misc.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/our_GR_blocks.py` & `pcdr-1.0.0a3/src/pcdr/_internal/our_GR_blocks.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/queue_to_guisink_flowgraph.py` & `pcdr-1.0.0a3/src/pcdr/_internal/queue_to_guisink_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/queue_to_waterfall_flowgraph.py` & `pcdr-1.0.0a3/src/pcdr/_internal/queue_to_waterfall_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/vector_to_guisink_flowgraph.py` & `pcdr-1.0.0a3/src/pcdr/_internal/vector_to_guisink_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/vector_tx_flowgraphs.py` & `pcdr-1.0.0a3/src/pcdr/_internal/vector_tx_flowgraphs.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_internal/wrapped_GR_blocks.py` & `pcdr-1.0.0a3/src/pcdr/_internal/wrapped_GR_blocks.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_modulators.py` & `pcdr-1.0.0a3/src/pcdr/_modulators.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_queue/sink.py` & `pcdr-1.0.0a3/src/pcdr/_queue/sink.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_queue/source.py` & `pcdr-1.0.0a3/src/pcdr/_queue/source.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr/_wavegen.py` & `pcdr-1.0.0a3/src/pcdr/_wavegen.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/src/pcdr.egg-info/PKG-INFO` & `pcdr-1.0.0a3/src/pcdr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdr
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: GNU Radio-based transmit and receive wrappers and more
 Author: james-pcdr
 Project-URL: Homepage, https://github.com/python-can-define-radio/pcdr
 Project-URL: Bug Tracker, https://github.com/python-can-define-radio/pcdr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pcdr-1.0.0a2/src/pcdr.egg-info/SOURCES.txt` & `pcdr-1.0.0a3/src/pcdr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/tests/test_gnuradio_vector_tx_flowgraphs.py` & `pcdr-1.0.0a3/tests/test_gnuradio_vector_tx_flowgraphs.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/tests/test_gnuradio_write_file_and_read_file.py` & `pcdr-1.0.0a3/tests/test_gnuradio_write_file_and_read_file.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/tests/test_multiple.py` & `pcdr-1.0.0a3/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/tests/test_other__blocks_for_testing.py` & `pcdr-1.0.0a3/tests/test_other__blocks_for_testing.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a2/tests/test_our_GR_blocks.py` & `pcdr-1.0.0a3/tests/test_our_GR_blocks.py`

 * *Files identical despite different names*

