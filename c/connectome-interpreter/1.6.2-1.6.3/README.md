# Comparing `tmp/connectome_interpreter-1.6.2.tar.gz` & `tmp/connectome_interpreter-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.6.2.tar", last modified: Sun Apr 28 19:50:37 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.6.3.tar", last modified: Mon Apr 29 17:26:03 2024, max compression
```

## Comparing `connectome_interpreter-1.6.2.tar` & `connectome_interpreter-1.6.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 19:50:37.692154 connectome_interpreter-1.6.2/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     1095 2024-04-28 19:50:37.692154 connectome_interpreter-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 19:50:37.667269 connectome_interpreter-1.6.2/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.2/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.6.2/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    21563 2024-04-28 18:29:19.000000 connectome_interpreter-1.6.2/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.6.2/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.2/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 19:50:37.686540 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1095 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 19:50:37.692154 connectome_interpreter-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1702 2024-04-28 19:48:44.000000 connectome_interpreter-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 19:50:37.690161 connectome_interpreter-1.6.2/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.2/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:26:03.766310 connectome_interpreter-1.6.3/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0     1095 2024-04-29 17:26:03.764225 connectome_interpreter-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 17:26:03.673426 connectome_interpreter-1.6.3/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.3/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    33835 2024-04-29 17:22:56.000000 connectome_interpreter-1.6.3/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    21563 2024-04-28 18:29:19.000000 connectome_interpreter-1.6.3/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.6.3/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.3/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:26:03.726660 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1095 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:26:03.767307 connectome_interpreter-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     2218 2024-04-29 17:23:50.000000 connectome_interpreter-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:26:03.762095 connectome_interpreter-1.6.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.3/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.3/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.6.2/LICENSE` & `connectome_interpreter-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.2/PKG-INFO` & `connectome_interpreter-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.6.2
+Version: 1.6.3
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
-Requires-Dist: torch>=1.7.1
+Requires-Dist: torch==2.2.0
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
```

### Comparing `connectome_interpreter-1.6.2/README.md` & `connectome_interpreter-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.2/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.6.3/connectome_interpreter/activation_maximisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,102 +10,112 @@
 
 from .compress_paths import result_summary
 from .utils import adjacency_df_to_el, get_activations
 
 
 class MultilayeredNetwork(nn.Module):
     """
-    A PyTorch module representing a multilayered neural network model. 
-    This network architecture is designed to process temporal sequences of sensory data 
-    through multiple layers, with the initial layer handling sensory inputs and subsequent 
+    A PyTorch module representing a multilayered neural network model.
+    This network architecture is designed to process temporal sequences of sensory data
+    through multiple layers, with the initial layer handling sensory inputs and subsequent
     layers processing sensory + non-sensory input.
 
-    The forward pass of the network unrolls the connectome through time, with each layer 
-    receiving its own time-specific sensory input. 
+    The forward pass of the network unrolls the connectome through time, with each layer
+    receiving its own time-specific sensory input.
 
     Attributes:
-        all_weights (torch.nn.Parameter): The connectome. Input neurons are in the columns. 
-        sensory_indices (list[int]): Indices indicating which rows/columns in the all_weights matrix 
+        all_weights (torch.nn.Parameter): The connectome. Input neurons are in the columns.
+        sensory_indices (list[int]): Indices indicating which rows/columns in the all_weights matrix
             correspond to sensory neurons.
         num_layers (int): The number of layers in the network.
         threshold (float): The activation threshold for neurons in the network.
-        activations (list[torch.Tensor]): A list storing the activations of each layer 
-            after the forward pass.
+        activations (numpy.ndarray): A 2D array storing the activations of all neurons (rows) across time steps (columns).
 
     Args:
         all_weights (torch.Tensor): The connectome. Input neurons are in the columns.
-        sensory_indices (list[int]): A list indicating the indices of sensory neurons 
+        sensory_indices (list[int]): A list indicating the indices of sensory neurons
             within the network.
-        num_layers (int, optional): The number of temporal layers to unroll the network through. 
+        num_layers (int, optional): The number of temporal layers to unroll the network through.
             Defaults to 2.
         threshold (float, optional): The threshold for activation of neurons. Defaults to 0.01.
     """
 
     def __init__(self, all_weights, sensory_indices, num_layers=2, threshold=0.01, tanh_steepness=5):
         super(MultilayeredNetwork, self).__init__()
 
         self.all_weights = torch.nn.parameter.Parameter(all_weights)
         self.sensory_indices = torch.tensor(sensory_indices)
         self.num_layers = num_layers
         self.threshold = threshold
         self.tanh_steepness = tanh_steepness
-        self.activations = []  # List for activations of middle layers
+        self.activations = []
 
     def forward(self, inthroughtime):
         """
         Processes the input through the multilayered neural network, applying thresholding
         and tanh activation functions. This method sequentially processes the input through
         each layer of the network, considering both sensory and non-sensory neurons, to produce
         the final activations.
 
         Args:
             inthroughtime (torch.Tensor): A 2D tensor representing the input to the network
                 across different time steps. Each column corresponds to a different time step,
                 and each row corresponds to different sensory inputs.
 
         Returns:
-            torch.Tensor: A 2D tensor of activations for all neurons across all layers and
+            numpy.ndarray: A 2D array of activations for all neurons across all layers and
                 time steps. Each column represents the activations for a specific time step,
                 while each row corresponds to different neurons.
 
         This method first applies a threshold ReLU to the input, setting all values below
         the threshold to zero. It then limits the range of activations between 0 and 1 using
         a tanh function. The activation of all neurons is then calculated, based on the input and the weights. The activation of input neurons at layer n is the sum of: input from the previous layer (input neurons are allowed to connect with each other), and freshly fed-in external input.
         The process accounts for the model's threshold and `tanh_steepness` to modulate
         the activations. The final activations are stored in the `activations` attribute
         of the model, with each entry corresponding to the activations for a specific layer.
         """
 
         self.activations = []  # Clear activations list at each forward pass
 
+        # thresholded relu
         inthroughtime = torch.where(inthroughtime >= self.threshold,
-                                    inthroughtime, 0)  # Thresholded ReLU
+                                    inthroughtime, 0)
         # Limit the range between 0 and 1
         inthroughtime = torch.tanh(inthroughtime)
 
         # Initial activations are based only on sensory inputs for the first time step
         x = self.all_weights[:, self.sensory_indices] @ inthroughtime[:, 0]
-        x = torch.where(x >= self.threshold, x, 0)  # Thresholded ReLU
+        # thresholded relu
+        x = torch.where(x >= self.threshold, x, 0)
+
         # Limit the range between 0 and 1
         x = torch.tanh(self.tanh_steepness*x)
-        self.activations.append(x)
+        self.activations.append(x.cpu().detach().numpy())
 
         # Process remaining layers
         for i in range(1, self.num_layers):
             x = self.all_weights @ x
             # add inthroughtime[:, i] to the sensory neurons
             x[self.sensory_indices] += inthroughtime[:, i]
+            # thresholded relu
+            x = torch.where(x >= self.threshold, x, 0)
 
-            x = torch.where(x >= self.threshold, x, 0)  # Thresholded ReLU
             # Limit the range between 0 and 1
             x = torch.tanh(self.tanh_steepness*x)
 
-            self.activations.append(x)
+            self.activations.append(x.cpu().detach().numpy())
 
-        self.activations = torch.stack(self.activations, dim=1)
+        # free up memory as much as possible
+        del inthroughtime
+        del x
+        torch.cuda.empty_cache()
+
+        # stack the numpy activations together
+        self.activations = np.stack(self.activations, axis=1)
+        # self.activations = torch.stack(self.activations, dim=1)
         return self.activations
 
 
 def activation_maximisation(
         model, selected_neurons_per_layer: Dict[int, List[int]],
         input_tensor=None,
         num_iterations=100, learning_rate=0.4,
@@ -143,15 +153,15 @@
         wandb (bool, optional): Whether to log optimization details to Weights & Biases. Defaults to True. Requires wandb to be installed.
 
     Returns:
         A tuple containing:
         The optimized `input_tensor` as a numpy array.
         The output of the model after optimization as a numpy array.
         A list of input activation losses over iterations.
-        A list of output activation losses over iterations. 
+        A list of output activation losses over iterations.
         A list of input activation regularization losses over iterations.
         A list of output activation regularization losses over iterations.
         A list of input tensor snapshots taken during optimization.
 
     Raises:
         ImportError: If `wandb` is True and wandb is not installed.
     """
@@ -214,59 +224,68 @@
         for layer_index, neuron_indices in selected_neurons_per_layer.items():
             # Ensure layer index is valid
             if layer_index < model.activations.shape[1]:
                 # Get activations for this layer
                 layer_activations = model.activations[:, layer_index]
                 # Negative sign because we want to maximize activation
                 # Only select activations from specified neurons
-                activation_loss -= torch.mean(
+                # layer_activations is now a numpy array
+                activation_loss -= np.mean(
                     layer_activations[neuron_indices])
         # in the end, activation loss is the sum of mean activation across layers.
 
-        out_regularisation_loss = out_regularisation_lambda * torch.mean(
+        out_regularisation_loss = out_regularisation_lambda * np.mean(
             model.activations)
         # Apply custom regularisation
         in_regularisation_loss = in_regularisation_lambda * custom_in_regularisation(
             input_tensor)
         loss = activation_loss + in_regularisation_loss + out_regularisation_loss
         losses.append(loss.item())
 
         if early_stopping and (iteration > n_runs):
             # when the difference between the max and the min < stopping_threshold
             if np.max(losses[-n_runs:]) - np.min(losses[-n_runs:]) < stopping_threshold:
                 break
 
         if wandb:
-            dct = {"activation_loss": activation_loss.item(
-            ), "in_regularisation_loss": in_regularisation_loss.item(),
-                'out_regularisation_loss': out_regularisation_loss.item(),
-                "loss": loss.item()}
+            dct = {"activation_loss": activation_loss.item(),
+                   "in_regularisation_loss": in_regularisation_loss.item(),
+                   'out_regularisation_loss': out_regularisation_loss.item(),
+                   "loss": loss.item()}
             wandb.log(dct)
 
         act_loss.append(activation_loss.item())
         out_reg_loss.append(out_regularisation_loss.item())
         in_reg_loss.append(in_regularisation_loss.item())
 
         # Backward pass and optimization
         loss.backward()
         optimizer.step()
 
         # Optional: Print information about the optimization process
         if print_output and iteration % 10 == 0:  # Print every 10 iterations
             print(
                 f"Iteration {iteration}: Activation Loss = {activation_loss.item()}, Input regularization Loss = {in_regularisation_loss.item()}, Output regularization Loss = {out_regularisation_loss.item()}")
+            # print(f'Memory after optimization {iteration}:', torch.cuda.memory_allocated(
+            #     device) / 1e9, 'GB')
+
+        torch.cuda.empty_cache()
 
     output_after = model(input_tensor)
-    input_tensor = torch.where(input_tensor >= model.threshold,
-                               input_tensor, 0)  # Thresholded ReLU
+    # first bring to cpu to save gpu memory
+    input_tensor = input_tensor.cpu().detach().numpy()
+    input_tensor = np.where(input_tensor >= model.threshold,
+                            input_tensor, 0)
     # Limit the range between 0 and 1
-    input_tensor = torch.tanh(input_tensor)
+    input_tensor = np.tanh(input_tensor)
+
+    # print('Memory after optimization:',
+    #       torch.cuda.memory_allocated(device) / 1e9, 'GB')
 
-    return (input_tensor.cpu().detach().numpy(),
-            output_after.cpu().detach().numpy(),
+    return (input_tensor, output_after,
             act_loss, out_reg_loss, in_reg_loss, input_snapshots)
 
 
 # # implementation where there are no connections between sensory neurons:
 # class MultilayeredNetwork(nn.Module):
 #     """
 #     A PyTorch module representing a multilayered neural network model.
@@ -548,15 +567,15 @@
 def activations_to_df(inprop, opt_in, out, sensory_indices, inidx_mapping=None, outidx_mapping=None, activation_threshold=0, connectivity_threshold=0):
     """
     Generates a dataframe representing the paths in a layered plot, filtering by activation and connectivity thresholds.
 
     This function takes the direct connectivity matrix (inprop), optimal input neuron activity, output neuron activity, indices for sensory neurons, and mapping between input and output indices to groups. It generates a dataframe that represents the paths through the network layers.
 
     Args:
-        inprop (scipy.sparse matrix or numpy.ndarray): Matrix representing the synaptic strengths 
+        inprop (scipy.sparse matrix or numpy.ndarray): Matrix representing the synaptic strengths
             between neurons, can be dense or sparse. Presynaptic is in the rows, postsynaptic in the columns.
         opt_in (numpy.ndarray): A 2D array representing optimal input to the network.
         out (numpy.ndarray): A 2D array representing the output from the network. The second dimension represents timepoints.
         sensory_indices (list of int): A list of indices corresponding to sensory neurons in `inprop`.
         inidx_mapping (dict, optional): A dictionary mapping indices in `inprop` to new indices. If None, indices are not remapped.
                                        Defaults to None.
         outidx_mapping (dict, optional): A dictionary mapping indices in `out` to new indices. If None, `inidx_mapping` is used for
```

### Comparing `connectome_interpreter-1.6.2/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.6.3/connectome_interpreter/compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.2/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.6.3/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.2/connectome_interpreter/utils.py` & `connectome_interpreter-1.6.3/connectome_interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.2/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.6.3/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.6.2
+Version: 1.6.3
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
-Requires-Dist: torch>=1.7.1
+Requires-Dist: torch==2.2.0
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
```

### Comparing `connectome_interpreter-1.6.2/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.6.3/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.2/setup.py` & `connectome_interpreter-1.6.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,42 @@
 from setuptools import setup, find_packages
+import pkg_resources
+
+# Function to check if PyTorch is already installed
+
+
+def get_torch_version():
+    try:
+        return pkg_resources.get_distribution('torch').version
+    except pkg_resources.DistributionNotFound:
+        return None
+
+
+# Specify a PyTorch version requirement only if it's not installed
+torch_version = get_torch_version()
+if torch_version is None:
+    torch_requirement = 'torch>=1.7.1'
+else:
+    torch_requirement = f'torch=={torch_version}'
+
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.6.2',
+    version='1.6.3',
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here
         'numpy',
         'pandas',
         'scipy',
-        'torch>=1.7.1',
+        # 'torch>=1.7.1',
+        torch_requirement,
         'tqdm',
         'plotly',
         'matplotlib',
         'networkx',
         'seaborn',
         'ipywidgets',
         'IPython',
```

### Comparing `connectome_interpreter-1.6.2/tests/test_compress_paths.py` & `connectome_interpreter-1.6.3/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.2/tests/test_utils.py` & `connectome_interpreter-1.6.3/tests/test_utils.py`

 * *Files identical despite different names*

