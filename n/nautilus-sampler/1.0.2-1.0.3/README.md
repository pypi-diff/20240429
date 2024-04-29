# Comparing `tmp/nautilus_sampler-1.0.2.tar.gz` & `tmp/nautilus_sampler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautilus_sampler-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nautilus_sampler-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nautilus_sampler-1.0.2.tar` & `nautilus_sampler-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11603 2024-02-15 21:31:29.615389 nautilus_sampler-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-08-09 17:54:21.525684 nautilus_sampler-1.0.2/LICENSE
--rw-r--r--   0        0        0     3830 2024-02-15 19:17:21.229117 nautilus_sampler-1.0.2/README.md
--rw-r--r--   0        0        0      218 2024-02-15 22:45:31.123772 nautilus_sampler-1.0.2/nautilus/__init__.py
--rw-r--r--   0        0        0      316 2023-08-09 17:54:21.524684 nautilus_sampler-1.0.2/nautilus/bounds/__init__.py
--rw-r--r--   0        0        0    22470 2024-02-15 19:17:21.231117 nautilus_sampler-1.0.2/nautilus/bounds/basic.py
--rw-r--r--   0        0        0    18248 2024-02-15 22:36:30.247825 nautilus_sampler-1.0.2/nautilus/bounds/neural.py
--rw-r--r--   0        0        0    15036 2024-02-15 19:17:21.232117 nautilus_sampler-1.0.2/nautilus/bounds/union.py
--rw-r--r--   0        0        0     5757 2024-02-15 19:17:21.232117 nautilus_sampler-1.0.2/nautilus/neural.py
--rw-r--r--   0        0        0     1169 2024-02-15 19:57:08.746459 nautilus_sampler-1.0.2/nautilus/pool.py
--rw-r--r--   0        0        0     5967 2023-08-09 17:54:21.524684 nautilus_sampler-1.0.2/nautilus/prior.py
--rw-r--r--   0        0        0    51735 2024-02-15 22:36:54.898661 nautilus_sampler-1.0.2/nautilus/sampler.py
--rw-r--r--   0        0        0      668 2024-02-15 19:17:21.233116 nautilus_sampler-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5583 2024-02-15 19:17:21.233116 nautilus_sampler-1.0.2/tests/test_blobs.py
--rw-r--r--   0        0        0    14845 2024-02-15 19:17:21.234116 nautilus_sampler-1.0.2/tests/test_bounds.py
--rw-r--r--   0        0        0     5377 2024-02-15 19:17:21.234116 nautilus_sampler-1.0.2/tests/test_io.py
--rw-r--r--   0        0        0      486 2023-11-06 20:24:00.822972 nautilus_sampler-1.0.2/tests/test_neural.py
--rw-r--r--   0        0        0     1117 2024-02-15 19:17:21.234116 nautilus_sampler-1.0.2/tests/test_pool.py
--rw-r--r--   0        0        0     3714 2023-11-06 20:24:00.825972 nautilus_sampler-1.0.2/tests/test_prior.py
--rw-r--r--   0        0        0    11594 2024-02-15 22:41:16.562193 nautilus_sampler-1.0.2/tests/test_sampler.py
--rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 nautilus_sampler-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11962 2024-04-29 17:19:11.567390 nautilus_sampler-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2024-04-25 16:48:30.243642 nautilus_sampler-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3830 2024-04-25 16:48:30.243642 nautilus_sampler-1.0.3/README.md
+-rw-r--r--   0        0        0      218 2024-04-29 17:26:00.109579 nautilus_sampler-1.0.3/nautilus/__init__.py
+-rw-r--r--   0        0        0      316 2024-04-25 16:48:30.251642 nautilus_sampler-1.0.3/nautilus/bounds/__init__.py
+-rw-r--r--   0        0        0    22470 2024-04-25 16:48:30.251642 nautilus_sampler-1.0.3/nautilus/bounds/basic.py
+-rw-r--r--   0        0        0    18248 2024-04-25 16:48:30.251642 nautilus_sampler-1.0.3/nautilus/bounds/neural.py
+-rw-r--r--   0        0        0    15036 2024-04-25 16:48:30.251642 nautilus_sampler-1.0.3/nautilus/bounds/union.py
+-rw-r--r--   0        0        0     5757 2024-04-25 16:48:30.251642 nautilus_sampler-1.0.3/nautilus/neural.py
+-rw-r--r--   0        0        0     1169 2024-04-25 16:48:30.251642 nautilus_sampler-1.0.3/nautilus/pool.py
+-rw-r--r--   0        0        0     5967 2024-04-25 16:48:30.251642 nautilus_sampler-1.0.3/nautilus/prior.py
+-rw-r--r--   0        0        0    52903 2024-04-29 17:18:56.371458 nautilus_sampler-1.0.3/nautilus/sampler.py
+-rw-r--r--   0        0        0      755 2024-04-25 16:48:30.252642 nautilus_sampler-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5583 2024-04-25 16:48:30.252642 nautilus_sampler-1.0.3/tests/test_blobs.py
+-rw-r--r--   0        0        0    14845 2024-04-25 16:48:30.252642 nautilus_sampler-1.0.3/tests/test_bounds.py
+-rw-r--r--   0        0        0     5377 2024-04-25 16:48:30.252642 nautilus_sampler-1.0.3/tests/test_io.py
+-rw-r--r--   0        0        0      486 2024-04-25 16:48:30.252642 nautilus_sampler-1.0.3/tests/test_neural.py
+-rw-r--r--   0        0        0     1117 2024-04-25 16:48:30.252642 nautilus_sampler-1.0.3/tests/test_pool.py
+-rw-r--r--   0        0        0     3714 2024-04-25 16:48:30.252642 nautilus_sampler-1.0.3/tests/test_prior.py
+-rw-r--r--   0        0        0    12203 2024-04-29 17:18:56.371458 nautilus_sampler-1.0.3/tests/test_sampler.py
+-rw-r--r--   0        0        0     4479 1970-01-01 00:00:00.000000 nautilus_sampler-1.0.3/PKG-INFO
```

### Comparing `nautilus_sampler-1.0.2/CHANGELOG.md` & `nautilus_sampler-1.0.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 # Changelog
 
 All notable changes to nautilus will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.3] - 2023-04-29
+
+### Added
+- The user can now specify a timeout interval for the sampler. If that time is exceeded, the sampler will not start new calculations. (#46)
+- The sampler now returns whether it finished normally or stopped because the timeout or maximum number of likelihood computations was reached. (#46)
+
 ## [1.0.2] - 2023-02-15
 
 ### Changed
 - Further improved the way the sampler handles plateaus. For example, if the lowest-likelihood point in the live set is part of a plateau, the sampler will jump past the plateau if enough live points with higher likelihood exist. The sampler also behaves reasonably if most or all points are part of a plateau. This leads to less freezes and better performance.
 
 ## [1.0.1] - 2023-02-12
 
 ### Fixed
 - Fixed a crash when multiple blobs per likelihood call are returned as a single array.
 
 ## [1.0.0] - 2023-02-12
 
+### Added
+- The user can now specify a maximum number of likelihood calls. If that number is exceeded, the sampler will automatically stop. (#23)
+
 ### Changed
 - Updated the terminal output to be more compact and more friendly for log files. This also removes the dependency on `tqdm`. (#36)
-- The user can now specify a maximum number of likelihood calls. If that number is exceeded, the sampler will automatically stop. (#23)
 - By default, the batch size is now dynamically determined at the start based on the pool size. This should prevent issues for new users parallelizing over a large number of CPUs.
 
 ### Fixed
 - Fixed a crash when returning the posterior as a dictionary and with equal weight.
 - Fixed a potential crash when `n_update` is extremely low.
 
 ### Depcrecated
@@ -60,38 +68,42 @@
 ## [0.7.1] - 2023-07-07
 
 ### Fixed
 - Parallelization with MPIPoolExecutor should now work correctly.
 
 ## [0.7.0] - 2023-06-20
 
+### Added
+- Added the function `sampler.asymptotic_sampling_efficiency` which returns an estimate of the sampling efficiency in the sampling phase.
+
 ### Changed
 - One can now change whether to discard points in the exploration phase after calling `run` by changing the `discard_exploration` argument of the sampler. To achieve this, information about points in the exploration phase is never dropped. Consequently, the sampler does not create a backup of the end of the exploration stage under "filename_exp.hdf5", anymore.
 - The computational overhead was slightly reduced when new bounds are rejected. Also, the output now specifically mentions when adding a new bound failed because the volume increased.
-- Added the function `sampler.asymptotic_sampling_efficiency` which returns an estimate of the sampling efficiency in the sampling phase.
 
 ### Fixed
 - Likelihoods with large plateaus shouldn't crash, anymore.
 - Information updates about bounds are now written during the sampling phase. Previously, if computations were interrupted and restarted during the sampling phase, the volume estimates were noisier than necessary, and some points may have been proposed twice.
 
 ### Removed
 - The `n_jobs` keyword argument for the sampler has been removed. The pool used for likelihood calls is now also used for sampler parallelization, by default. To use independent pools for likelihood calls and sampler calculations, pass a tuple to `pool`.
 - The `random_state` keyword argument for the sampler has been removed. Use `seed`, instead.
 - The `enlarge` keyword argument has been removed. Use `enlarge_per_dim`, instead.
 
 ## [0.6.0] - 2023-04-22
 
+### Added
+- Added the keyword arguments `n_points_min` and `split_threshold` to the sampler. Previously, they were not accessible.
+- Sampling new points can now be parallelized using the `n_jobs` keyword argument.
+
 ### Changed
 - The code now uses the more modern `numpy.random.Generator` framework instead of `numpy.random.RandomState`.
-- Added the keyword arguments `n_points_min` and `split_threshold` to the sampler. Previously, they were not accessible.
 - The default value for `n_points_min` is now the number of dimensions plus 50. Previously, it was hard-coded to be the number of dimensions plus 1.
 - The multi-ellipsoidal decomposition has been tweaked with the goal of reducing computational overhead for high-dimensional problems.
 - The default number of parallel processes has been changed to one. By default, the sampler will not use parallelization.
 - Multi-ellipsoidal decomposition now uses Gaussian mixture modeling instead of K-Means. The former typically results in better performance, i.e., smaller boundaries with fewer ellipsoids.
-- Sampling new points can now be parallelized using the `n_jobs` keyword argument.
 
 ### Fixed
 - The sampler now correctly writes the random number generator in the sampling phase.
 - The keyword argument `n_jobs` is now being correctly passed when training networks. Previously, all cores were used regardless of `n_jobs`.
 - The sampler doesn't crash when setting `verbose=True`and `n_networks=0`.
 
 ### Deprecated
```

### Comparing `nautilus_sampler-1.0.2/LICENSE` & `nautilus_sampler-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/README.md` & `nautilus_sampler-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/nautilus/bounds/basic.py` & `nautilus_sampler-1.0.3/nautilus/bounds/basic.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/nautilus/bounds/neural.py` & `nautilus_sampler-1.0.3/nautilus/bounds/neural.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/nautilus/bounds/union.py` & `nautilus_sampler-1.0.3/nautilus/bounds/union.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/nautilus/neural.py` & `nautilus_sampler-1.0.3/nautilus/neural.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/nautilus/pool.py` & `nautilus_sampler-1.0.3/nautilus/pool.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/nautilus/prior.py` & `nautilus_sampler-1.0.3/nautilus/prior.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/nautilus/sampler.py` & `nautilus_sampler-1.0.3/nautilus/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from functools import partial
 from multiprocessing import Pool
 from pathlib import Path
 from scipy.special import logsumexp
 from shutil import get_terminal_size
 from threadpoolctl import threadpool_limits
+from time import time
 from warnings import warn
 
 from .bounds import UnitCube, NautilusBound
 from .pool import initialize_worker, likelihood_worker, pool_size
 
 
 class Sampler():
@@ -364,52 +365,72 @@
                 self.bounds = [
                     UnitCube.read(fstream['bound_0'], rng=self.rng), ]
                 for i in range(1, len(self.shell_n)):
                     self.bounds.append(NautilusBound.read(
                         fstream['bound_{}'.format(i)], rng=self.rng))
 
     def run(self, f_live=0.01, n_shell=1, n_eff=10000, n_like_max=np.inf,
-            discard_exploration=False, verbose=False):
+            discard_exploration=False, timeout=np.inf, verbose=False):
         """Run the sampler until convergence.
 
         Parameters
         ----------
         f_live : float, optional
             Maximum fraction of the evidence contained in the live set before
             building the initial shells terminates. Default is 0.01.
         n_shell : int, optional
             Minimum number of points in each shell. The algorithm will sample
             from the shells until this is reached. Default is 1.
         n_eff : float, optional
             Minimum effective sample size. The algorithm will sample from the
             shells until this is reached. Default is 10000.
         n_like_max : int, optional
-            Maximum number of likelihood evaluations. Regardless of progress,
-            the sampler will stop if this value is reached. Default is
-            infinity.
+            Maximum total (accross multiple runs) number of likelihood
+            evaluations. Regardless of progress, the sampler will not start new
+            likelihood computations if this value is reached. Note that this
+            value includes likelihood calls from previous runs, if applicable.
+            Default is infinity.
         discard_exploration : bool, optional
             Whether to discard points drawn in the exploration phase. This is
             required for a fully unbiased posterior and evidence estimate.
             Default is False.
+        timeout : float, optional
+            Timeout interval in seconds. The sampler will not start new
+            likelihood computations if this limit is reached. Unlike for
+            `n_like_max`, this maximum only refers to the current function
+            call. Default is infinity.
         verbose : bool, optional
             If True, print information about sampler progress. Default is
             False.
 
+        Returns
+        -------
+        success : bool
+            Whether the run finished successfully without stopping prematurely.
+            False if the run finished because the `n_like_max` or `timeout`
+            limits were reached and True otherwise.
+
         """
+        t_start = time()
+
         if verbose:
             print('Starting the nautilus sampler...')
             print('Please report issues at github.com/johannesulf/nautilus.')
             self.print_status(header=True)
 
         if len(self.bounds) == 0:
             self.add_bound()
             self.n_update_iter = -self.n_live
             self.n_like_iter = 0
 
-        while self.n_like < n_like_max:
+        success = (self.explored and np.all(self.shell_n >= n_shell) and
+                   self.n_eff >= n_eff)
+
+        while ((self.n_like < n_like_max) and (time() - t_start < timeout) and
+               not success):
 
             if not self.explored:
 
                 if ((self.n_update_iter >= self.n_update or
                      self.n_like_iter >= self.n_like_new_bound) and
                         np.sum(self.shell_n) > self.n_live):
                     self.add_bound(verbose=verbose)
@@ -463,19 +484,24 @@
                 shell = np.argmax(self.shell_log_l + self.shell_log_v -
                                   0.5 * np.log(self.shell_n) -
                                   0.5 * np.log(self.shell_n_eff))
                 self.add_samples(shell, verbose=verbose)
                 if self.filepath is not None:
                     self.write_shell_update(self.filepath, shell)
 
-            else:
-                break
+            success = (self.explored and np.all(self.shell_n >= n_shell) and
+                       self.n_eff >= n_eff)
 
         if verbose:
-            self.print_status('Finished')
+            if success:
+                self.print_status('Finished')
+            else:
+                self.print_status('Stopped')
+
+        return success
 
     @property
     def discard_exploration(self):
         """Return whether the exploration phase is discarded.
 
         Returns
         -------
```

### Comparing `nautilus_sampler-1.0.2/tests/test_blobs.py` & `nautilus_sampler-1.0.3/tests/test_blobs.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/tests/test_bounds.py` & `nautilus_sampler-1.0.3/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/tests/test_io.py` & `nautilus_sampler-1.0.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/tests/test_pool.py` & `nautilus_sampler-1.0.3/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/tests/test_prior.py` & `nautilus_sampler-1.0.3/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-1.0.2/tests/test_sampler.py` & `nautilus_sampler-1.0.3/tests/test_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,21 +234,40 @@
         return -np.linalg.norm(x - 0.5)**2 * 0.001
 
     sampler_a = Sampler(prior, likelihood, n_dim=2, n_networks=0, seed=0)
     sampler_b = Sampler(prior, likelihood, n_dim=2, n_networks=0, seed=0)
 
     sampler_a.run(verbose=True)
     for n_like_max in range(sampler_a.n_like + 1):
-        sampler_b.run(n_like_max=n_like_max, verbose=True)
+        success = sampler_b.run(n_like_max=n_like_max, verbose=True)
         assert sampler_b.n_like <= n_like_max + sampler_b.n_batch
+        assert not success if sampler_a.n_like != sampler_b.n_like else success
 
     assert sampler_a.log_z == sampler_b.log_z
     assert sampler_a.n_eff == sampler_b.n_eff
 
 
+def test_sampler_timeout():
+    # Test that the sampler correctly stops when reaching the timeout limits.
+
+    def prior(x):
+        return x
+
+    def likelihood(x):
+        return -np.linalg.norm(x - 0.5)**2 * 0.001
+
+    sampler = Sampler(prior, likelihood, n_dim=10, n_networks=0, seed=0)
+    # The sampler shouldn't finish within 1 second.
+    success = sampler.run(verbose=True, timeout=1)
+    assert not success
+
+    # We should be able to continue afterwards.
+    success = sampler.run(verbose=True, timeout=5)
+
+
 def test_sampler_funnel():
     # Test the sampler on a funnel distribution. This is a great, challenging
     # distribution. Also, the nature of the likelihood leads to nautilus
     # boundaries that are not strictly nested, unlike for simpler
     # distributions.
 
     def prior(x):
```

### Comparing `nautilus_sampler-1.0.2/PKG-INFO` & `nautilus_sampler-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: nautilus-sampler
-Version: 1.0.2
+Version: 1.0.3
 Summary: Neural Network-Boosted Importance Sampling for Bayesian Statistics
 Author-email: "Johannes U. Lange" <julange.astro@pm.me>
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: threadpoolctl
-Requires-Dist: h5py ; extra == "checkpointing"
-Requires-Dist: h5py ; extra == "tests"
+Requires-Dist: numpy>=1.18.0
+Requires-Dist: scipy>=1.4.0
+Requires-Dist: scikit-learn>=0.22.0
+Requires-Dist: threadpoolctl>=3.0.0
+Requires-Dist: h5py>=3.0.0 ; extra == "checkpointing"
+Requires-Dist: h5py>=3.0.0 ; extra == "tests"
 Project-URL: Home, https://nautilus-sampler.readthedocs.io
 Provides-Extra: checkpointing
 Provides-Extra: tests
 
 ![Logo](https://raw.githubusercontent.com/johannesulf/nautilus/main/docs/nautilus_text_image.png "Logo")
 
 [![Unit Testing Status](https://img.shields.io/github/actions/workflow/status/johannesulf/nautilus/tests.yml?branch=main&label=tests)](https://github.com/johannesulf/nautilus/actions)
```

