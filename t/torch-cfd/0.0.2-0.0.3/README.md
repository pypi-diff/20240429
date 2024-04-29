# Comparing `tmp/torch_cfd-0.0.2.tar.gz` & `tmp/torch_cfd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_cfd-0.0.2.tar", last modified: Tue Apr 23 16:11:02 2024, max compression
+gzip compressed data, was "torch_cfd-0.0.3.tar", last modified: Mon Apr 29 03:55:24 2024, max compression
```

## Comparing `torch_cfd-0.0.2.tar` & `torch_cfd-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 16:03:17.000000 torch_cfd-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 16:03:17.000000 torch_cfd-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 16:10:57.000000 torch_cfd-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/torch_cfd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/equations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/fast_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/finite_differences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/forcings.py
--rw-r--r--   0 runner    (1001) docker     (127)    41005 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/torch_cfd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 03:55:20.000000 torch_cfd-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/torch_cfd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/fast_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/finite_differences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/forcings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41005 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-29 03:53:51.000000 torch_cfd-0.0.3/torch_cfd/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:55:24.193568 torch_cfd-0.0.3/torch_cfd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 03:55:24.000000 torch_cfd-0.0.3/torch_cfd.egg-info/top_level.txt
```

### Comparing `torch_cfd-0.0.2/LICENSE` & `torch_cfd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.2/PKG-INFO` & `torch_cfd-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-cfd
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyTorch CFD
 Home-page: https://github.com/scaomath/torch-cfd
 Author: Shuhao Cao
 Author-email: scao.math@gmail.com
 License: Apache-2.0
 Keywords: pytorch,cfd,pde,spectral
 Classifier: Development Status :: 4 - Beta
```

### Comparing `torch_cfd-0.0.2/README.md` & `torch_cfd-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.2/setup.py` & `torch_cfd-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'torch-cfd',
   packages=find_packages(include=['torch_cfd', 'torch_cfd.*']),
-  version='0.0.2',
+  version='0.0.3',
   license='Apache-2.0',
   description = 'PyTorch CFD',
   long_description='PyTorch Computational Fluid Dynamics Library',
   long_description_content_type="text/markdown",
   author = 'Shuhao Cao',
   author_email = 'scao.math@gmail.com',
   url = 'https://github.com/scaomath/torch-cfd',
```

### Comparing `torch_cfd-0.0.2/torch_cfd/equations.py` & `torch_cfd-0.0.3/torch_cfd/equations.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Modifications copyright (C) 2024 S.Cao
 # ported Google's Jax-CFD functional template to PyTorch's tensor ops
 
-from typing import Callable, Dict, Optional
+from typing import Tuple, Callable, Dict, Optional
 
 import torch
 import torch.nn as nn
 import torch.fft as fft
 from . import grids
 from tqdm.auto import tqdm
 
@@ -144,15 +144,15 @@
         u,
         dt=dt,
         params=params,
         equation=equation,
     )
 
 
-class NavierStokes2D(nn.Module):
+class NavierStokes2DSpectral(nn.Module):
     """Breaks the Navier-Stokes equation into implicit and explicit parts.
 
     Implicit parts are the linear terms and explicit parts are the non-linear
     terms.
 
     Attributes:
       viscosity: strength of the diffusion term
@@ -197,22 +197,32 @@
         n, _ = grid.shape
         filter_ = torch.zeros((n, n // 2 + 1))
         filter_[: int(2 / 3 * n) // 2, : int(2 / 3 * (n // 2 + 1))] = 1
         filter_[-int(2 / 3 * n) // 2 :, : int(2 / 3 * (n // 2 + 1))] = 1
         return filter_
 
     @staticmethod
-    def spectral_curl_2d(mesh, velocity_hat):
-        """Computes the 2D curl in the Fourier basis."""
-        kx, ky = mesh
-        uhat, vhat = velocity_hat
+    def spectral_curl_2d(vhat, rfft_mesh):
+        r"""
+        Computes the 2D curl in the Fourier basis.
+        det [d_x d_y \\ u v]
+        """
+        uhat, vhat = vhat
+        kx, ky = rfft_mesh
         return 2j * torch.pi * (vhat * kx - uhat * ky)
 
     @staticmethod
-    def vorticity_to_velocity(grid: Grid, w_hat: Array):
+    def spectral_grad_2d(vhat, rfft_mesh):
+        kx, ky = rfft_mesh
+        return 2j * torch.pi * kx * vhat, 2j * torch.pi * ky * vhat
+
+    @staticmethod
+    def vorticity_to_velocity(
+        grid: Grid, w_hat: Array, rfft_mesh: Optional[Tuple[Array, Array]] = None
+    ):
         """Constructs a function for converting vorticity to velocity, both in Fourier domain.
 
         Solves for the stream function and then uses the stream function to compute
         the velocity. This is the standard approach. A quick sketch can be found in
         [1].
 
         Args:
@@ -225,45 +235,50 @@
         Reference:
             [1] Z. Yin, H.J.H. Clercx, D.C. Montgomery, An easily implemented task-based
             parallel scheme for the Fourier pseudospectral solver applied to 2D
             Navier-Stokes turbulence, Computers & Fluids, Volume 33, Issue 4, 2004,
             Pages 509-520, ISSN 0045-7930,
             https://doi.org/10.1016/j.compfluid.2003.06.003.
         """
-        device = w_hat.device
-        kx, ky = grid.rfft_mesh()
-        kx, ky = kx.to(device), ky.to(device)
+        kx, ky = rfft_mesh if rfft_mesh is not None else grid.rfft_mesh()
         two_pi_i = 2 * torch.pi * 1j
         laplace = two_pi_i**2 * (abs(kx) ** 2 + abs(ky) ** 2)
         laplace[0, 0] = 1
         psi_hat = -1 / laplace * w_hat
         vxhat = two_pi_i * ky * psi_hat
         vyhat = -two_pi_i * kx * psi_hat
         return vxhat, vyhat
+    
+    def residual(self,
+        vort_hat: Array,
+        vort_t_hat: Array,
+    ):
+        residual = vort_t_hat -  self.explicit_terms(vort_hat) - self.viscosity *  self.implicit_terms(vort_hat)
+        return residual
 
     def _explicit_terms(self, vort_hat):
-        vxhat, vyhat = self.vorticity_to_velocity(self.grid, vort_hat)
+        vxhat, vyhat = self.vorticity_to_velocity(self.grid, vort_hat, (self.kx, self.ky))
         vx, vy = fft.irfft2(vxhat), fft.irfft2(vyhat)
 
         grad_x_hat = 2j * torch.pi * self.kx * vort_hat
         grad_y_hat = 2j * torch.pi * self.ky * vort_hat
         grad_x, grad_y = fft.irfft2(grad_x_hat), fft.irfft2(grad_y_hat)
 
         advection = -(grad_x * vx + grad_y * vy)
         advection_hat = fft.rfft2(advection)
 
-        if self.smooth is not None:
+        if self.smooth:
             advection_hat *= self.filter
 
         terms = advection_hat
 
         if self.forcing_fn is not None:
             fx, fy = self.forcing_fn(self.grid, (vx, vy))
             fx_hat, fy_hat = fft.rfft2(fx.data), fft.rfft2(fy.data)
-            terms += self.spectral_curl_2d((self.kx, self.ky), (fx_hat, fy_hat))
+            terms += self.spectral_curl_2d((fx_hat, fy_hat), (self.kx, self.ky))
 
         return terms
 
     def explicit_terms(self, vort_hat):
         return self._explicit_terms(vort_hat)
 
     def implicit_terms(self, vort_hat):
@@ -272,27 +287,29 @@
     def implicit_solve(self, vort_hat, dt):
         return 1 / (1 - dt * self.linear_term) * vort_hat
 
     def get_trajectory(
         self,
         w0: Array,
         dt: float,
-        time_steps: int,
+        T: float,
         record_every_steps=1,
         pbar=False,
         pbar_desc="",
         require_grad=False,
     ):
         """
         vorticity stacked in the time dimension
         """
         w_all = []
         v_all = []
         dwdt_all = []
+        res_all = []
         w = w0
+        time_steps = int(T / dt)
         update_iters = time_steps // TQDM_ITERS
         with tqdm(total=time_steps) as pbar:
             for t in range(time_steps):
                 w, dwdt = self.forward(w, dt=dt)
                 w.requires_grad_(require_grad)
                 dwdt.requires_grad_(require_grad)
 
@@ -300,22 +317,26 @@
                     pbar.set_description(pbar_desc)
                     pbar.update(update_iters)
 
                 if t % record_every_steps == 0:
                     w_ = w.detach().clone()
                     dwdt_ = dwdt.detach().clone()
                     v = self.vorticity_to_velocity(self.grid, w_)
+                    res = self.residual(w_, dwdt_)
+
                     v = torch.stack(v, dim=0)
                     w_all.append(w_)
                     v_all.append(v)
                     dwdt_all.append(dwdt_)
+                    res_all.append(res)
+
         result = {
             var_name: torch.stack(var, dim=0)
             for var_name, var in zip(
-                ["vorticity", "velocity", "vort_t"], [w_all, v_all, dwdt_all]
+                ["vorticity", "velocity", "vort_t", "residual"], [w_all, v_all, dwdt_all, res_all]
             )
         }
         return result
 
     def step(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
```

### Comparing `torch_cfd-0.0.2/torch_cfd/fast_diagonalization.py` & `torch_cfd-0.0.3/torch_cfd/fast_diagonalization.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.2/torch_cfd/finite_differences.py` & `torch_cfd-0.0.3/torch_cfd/finite_differences.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.2/torch_cfd/grids.py` & `torch_cfd-0.0.3/torch_cfd/grids.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.2/torch_cfd/initial_conditions.py` & `torch_cfd-0.0.3/torch_cfd/initial_conditions.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,15 +135,20 @@
     return GridArray(pinv, rhs.offset, rhs.grid)
 
 
 def projection(
     v: GridVariableVector,
     solve: Callable = solve_fast_diag,
 ) -> GridVariableVector:
-    """Apply pressure projection to make a velocity field divergence free."""
+    """
+    Apply pressure projection (a discrete Helmholtz decomposition)
+    to make a velocity field divergence free.
+    
+    Note: this will have a non-negligible error in fp32.
+    """
     grid = grids.consistent_grid(*v)
     pressure_bc = grids.get_pressure_bc_from_velocity(v)
 
     q0 = GridArray(torch.zeros(grid.shape), grid.cell_center, grid)
     q0 = pressure_bc.impose_bc(q0)
 
     q = solve(v, q0, pressure_bc)
@@ -186,18 +191,14 @@
 
     # Log normal distribution peaked at `peak_wavenumber`. Note that we have to
     # divide by `k ** (ndim - 1)` to account for the volume of the
     # `ndim - 1`-sphere of values with wavenumber `k`.
     def spectral_density(k):
         return _log_normal_pdf(k, peak_wavenumber) / k ** (grid.ndim - 1)
 
-    # TODO(b/156601712): Switch back to the vmapped implementation of filtering:
-    # noise = jax.random.normal(rng_key, (grid.ndim,) + grid.shape)
-    # filtered = wrap_velocities(jax.vmap(spectral.filter, (None, 0, None))(
-    #     spectral_density, noise, grid), grid)
     random_states = [random_state + i for i in range(grid.ndim)]
     rng = torch.Generator()
     velocity_components = []
     boundary_conditions = []
     for k in random_states:
         rng.manual_seed(k)
         noise = torch.randn(grid.shape, generator=rng)
```

### Comparing `torch_cfd-0.0.2/torch_cfd/tensor_utils.py` & `torch_cfd-0.0.3/torch_cfd/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.2/torch_cfd.egg-info/PKG-INFO` & `torch_cfd-0.0.3/torch_cfd.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-cfd
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyTorch CFD
 Home-page: https://github.com/scaomath/torch-cfd
 Author: Shuhao Cao
 Author-email: scao.math@gmail.com
 License: Apache-2.0
 Keywords: pytorch,cfd,pde,spectral
 Classifier: Development Status :: 4 - Beta
```

