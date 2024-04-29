# Comparing `tmp/GraphSL-0.8.tar.gz` & `tmp/GraphSL-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSL-0.8.tar", last modified: Fri Apr  5 01:28:38 2024, max compression
+gzip compressed data, was "GraphSL-0.9.tar", last modified: Mon Apr 29 16:32:46 2024, max compression
```

## Comparing `GraphSL-0.8.tar` & `GraphSL-0.9.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.762250 GraphSL-0.8/
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.693724 GraphSL-0.8/GraphSL/
--rw-rw-rw-   0        0        0      628 2024-04-02 03:37:06.000000 GraphSL-0.8/GraphSL/Evaluation.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.711631 GraphSL-0.8/GraphSL/GNN/
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.719314 GraphSL-0.8/GraphSL/GNN/GCNSI/
--rw-rw-rw-   0        0        0       41 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/GNN/GCNSI/__init__.py
--rw-rw-rw-   0        0        0    10598 2024-04-04 22:13:16.000000 GraphSL-0.8/GraphSL/GNN/GCNSI/main.py
--rw-rw-rw-   0        0        0     2842 2024-04-03 23:42:30.000000 GraphSL-0.8/GraphSL/GNN/GCNSI/model.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.742178 GraphSL-0.8/GraphSL/GNN/IVGD/
--rw-rw-rw-   0        0        0      185 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/GNN/IVGD/__init__.py
--rw-rw-rw-   0        0        0     1592 2024-04-03 23:40:52.000000 GraphSL-0.8/GraphSL/GNN/IVGD/correction.py
--rw-rw-rw-   0        0        0     4000 2024-03-30 18:14:05.000000 GraphSL-0.8/GraphSL/GNN/IVGD/earlystopping.py
--rw-rw-rw-   0        0        0     6267 2024-04-03 23:40:52.000000 GraphSL-0.8/GraphSL/GNN/IVGD/i_deepis.py
--rw-rw-rw-   0        0        0    16718 2024-04-04 22:13:43.000000 GraphSL-0.8/GraphSL/GNN/IVGD/main.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.746256 GraphSL-0.8/GraphSL/GNN/IVGD/model/
--rw-rw-rw-   0        0        0     4840 2024-03-21 02:09:16.000000 GraphSL-0.8/GraphSL/GNN/IVGD/model/MLP.py
--rw-rw-rw-   0        0        0       18 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/GNN/IVGD/model/__init__.py
--rw-rw-rw-   0        0        0     2780 2024-03-30 20:31:33.000000 GraphSL-0.8/GraphSL/GNN/IVGD/preprocessing.py
--rw-rw-rw-   0        0        0    16726 2024-03-30 21:24:24.000000 GraphSL-0.8/GraphSL/GNN/IVGD/training.py
--rw-rw-rw-   0        0        0     3985 2024-04-05 00:03:14.000000 GraphSL-0.8/GraphSL/GNN/IVGD/validity_net.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.755664 GraphSL-0.8/GraphSL/GNN/SLVAE/
--rw-rw-rw-   0        0        0       41 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/GNN/SLVAE/__init__.py
--rw-rw-rw-   0        0        0    16056 2024-04-04 22:14:01.000000 GraphSL-0.8/GraphSL/GNN/SLVAE/main.py
--rw-rw-rw-   0        0        0    13014 2024-04-03 23:43:48.000000 GraphSL-0.8/GraphSL/GNN/SLVAE/model.py
--rw-rw-rw-   0        0        0        0 2024-03-24 17:30:45.000000 GraphSL-0.8/GraphSL/GNN/__init__.py
--rw-rw-rw-   0        0        0    22346 2024-04-04 22:12:39.000000 GraphSL-0.8/GraphSL/Prescribed.py
--rw-rw-rw-   0        0        0       52 2024-04-05 00:09:46.000000 GraphSL-0.8/GraphSL/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.760193 GraphSL-0.8/GraphSL/data/
--rw-rw-rw-   0        0        0       20 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/data/__init__.py
--rw-rw-rw-   0        0        0     7110 2024-04-04 22:33:31.000000 GraphSL-0.8/GraphSL/data/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.709948 GraphSL-0.8/GraphSL.egg-info/
--rw-rw-rw-   0        0        0      732 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2024-04-02 03:37:06.000000 GraphSL-0.8/LICENSE
--rw-rw-rw-   0        0        0      732 2024-04-05 01:28:38.763307 GraphSL-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     9089 2024-04-03 23:13:28.000000 GraphSL-0.8/README.md
--rw-rw-rw-   0        0        0       86 2024-04-05 01:28:38.764241 GraphSL-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1729 2024-04-05 01:28:15.000000 GraphSL-0.8/setup.py
+drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-29 16:32:46.987569 GraphSL-0.9/
+drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-29 16:32:46.987569 GraphSL-0.9/GraphSL/
+-rw-r--r--   0 junwang   (8726) dsss      (5100)      598 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/Evaluation.py
+drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-29 16:32:46.987569 GraphSL-0.9/GraphSL/GNN/
+drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-29 16:32:46.987569 GraphSL-0.9/GraphSL/GNN/GCNSI/
+-rw-r--r--   0 junwang   (8726) dsss      (5100)       40 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/GCNSI/__init__.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)    10470 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/GCNSI/main.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     2756 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/GCNSI/model.py
+drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-29 16:32:46.987569 GraphSL-0.9/GraphSL/GNN/IVGD/
+-rw-r--r--   0 junwang   (8726) dsss      (5100)      179 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/__init__.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     1548 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/correction.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     3882 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/earlystopping.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     6069 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/i_deepis.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)    16466 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/main.py
+drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-29 16:32:46.987569 GraphSL-0.9/GraphSL/GNN/IVGD/model/
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     4743 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/model/MLP.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)       18 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/model/__init__.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     2686 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/preprocessing.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)    16243 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/training.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     3866 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/IVGD/validity_net.py
+drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-29 16:32:46.987569 GraphSL-0.9/GraphSL/GNN/SLVAE/
+-rw-r--r--   0 junwang   (8726) dsss      (5100)       40 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/SLVAE/__init__.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)    15740 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/SLVAE/main.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)    12548 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/SLVAE/model.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)        0 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/GNN/__init__.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)    22079 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/Prescribed.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)       72 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/__init__.py
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     6725 2024-04-29 15:43:57.000000 GraphSL-0.9/GraphSL/utils.py
+drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-29 16:32:46.987569 GraphSL-0.9/GraphSL.egg-info/
+-rw-r--r--   0 junwang   (8726) dsss      (5100)      851 2024-04-29 16:32:46.000000 GraphSL-0.9/GraphSL.egg-info/PKG-INFO
+-rw-r--r--   0 junwang   (8726) dsss      (5100)      770 2024-04-29 16:32:46.000000 GraphSL-0.9/GraphSL.egg-info/SOURCES.txt
+-rw-r--r--   0 junwang   (8726) dsss      (5100)        1 2024-04-29 16:32:46.000000 GraphSL-0.9/GraphSL.egg-info/dependency_links.txt
+-rw-r--r--   0 junwang   (8726) dsss      (5100)       62 2024-04-29 16:32:46.000000 GraphSL-0.9/GraphSL.egg-info/requires.txt
+-rw-r--r--   0 junwang   (8726) dsss      (5100)        8 2024-04-29 16:32:46.000000 GraphSL-0.9/GraphSL.egg-info/top_level.txt
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     1070 2024-04-29 15:43:57.000000 GraphSL-0.9/LICENSE
+-rw-r--r--   0 junwang   (8726) dsss      (5100)      851 2024-04-29 16:32:46.987569 GraphSL-0.9/PKG-INFO
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     9516 2024-04-29 15:43:57.000000 GraphSL-0.9/README.md
+-rw-r--r--   0 junwang   (8726) dsss      (5100)       79 2024-04-29 16:32:46.991570 GraphSL-0.9/setup.cfg
+-rw-r--r--   0 junwang   (8726) dsss      (5100)     1700 2024-04-29 15:54:37.000000 GraphSL-0.9/setup.py
```

### Comparing `GraphSL-0.8/GraphSL/GNN/GCNSI/main.py` & `GraphSL-0.9/GraphSL/GNN/GCNSI/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,263 +1,271 @@
-import torch
-from scipy.sparse import csgraph,coo_matrix
-import copy
-import numpy as np
-from GraphSL.GNN.GCNSI.model import GCNSI_model
-from GraphSL.Prescribed import LPSI
-from sklearn.metrics import roc_auc_score,f1_score,accuracy_score,precision_score,recall_score
-from GraphSL.Evaluation import Metric
-class GCNSI:
-    """
-    Implement the Graph Convolutional Networks based Source Identification (GCNSI).
-
-    Dong, Ming, et al. "Multiple rumor source detection with graph convolutional networks." Proceedings of the 28th ACM international conference on information and knowledge management. 2019.
-    """
-
-    def __init__(self):
-        """
-        Initializes the GCNSI module.
-        """
-
-    def train(self, adj, train_dataset, alpha=0.01, thres_list=[0.1,0.3,0.5,0.7,0.9],lr=0.001, num_epoch=50,print_epoch=10, weight=torch.tensor([1.0,3.0])):
-        """
-        Train the GCNSI model.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): Adjacency matrix of the graph.
-
-        - train_dataset (torch.utils.data.dataset.Subset): the training dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
-        
-        - alpha (float): The fraction of label information that a node gets from its neighbors (between 0 and 1) to try.
-        
-        - thres_list (list): List of threshold values to try.
-
-        - lr (float): Learning rate.
-        
-        - num_epoch (int): Number of training epochs.
-        
-        - print_epoch (int): Number of epochs every time to print loss.
-
-        - weight (torch.Tensor): Weight tensor for loss computation, the first and second values are loss weights for non-seed and seed, respectively.
-
-        Returns:
-
-        - gcnsi_model (GCNSI_model): GCNSI model.
-
-        - opt_thres (float): Optimal threshold value.
-
-        - train_auc (float): Training AUC score.
-
-        - opt_f1 (float): Optimal F1 score.
-
-        - opt_pred (numpy.ndarray): Predicted seed vector of the training set, every column is the prediction of every simulation. It is used to adjust thres_list.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.GNN.GCNSI.main import GCNSI
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        gcnsi = GCNSI()
-
-        gcnsi_model, thres, auc, f1, pred =gcnsi.train(adj, train_dataset)
-
-        print("GCNSI:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-        """
-        # Compute Laplacian matrix
-        S = csgraph.laplacian(adj, normed=True)
-        S = np.array(coo_matrix.todense(S))
-        num_node = adj.shape[0]
-        train_num = len(train_dataset)
-        # Convert adjacency matrix to edge index tensor
-        coo = adj.tocoo()
-        row = torch.from_numpy(coo.row.astype(np.int64)).to(torch.long)
-        col = torch.from_numpy(coo.col.astype(np.int64)).to(torch.long)
-        edge_index = torch.stack([row, col], dim=0)
-        # Iterate over alpha values
-        gcnsi_model = GCNSI_model()
-        optimizer = torch.optim.Adam(gcnsi_model.parameters(), lr=lr)
-        criterion = torch.nn.CrossEntropyLoss(weight=weight)
-        # Augmented features by LPSI
-
-        lpsi = LPSI()  # Initializing LPSI module
-        lpsi_input = np.zeros((train_num,num_node,4))
-
-        for i, influ_mat in enumerate(train_dataset):
-            diff_vec = influ_mat[:, -1]
-            V3 = copy.deepcopy(diff_vec)
-            V4 = copy.deepcopy(diff_vec)
-            V3[diff_vec < 0.5] = 0.5
-            V4[diff_vec >= 0.5] = 0.5
-            d1 = copy.deepcopy(diff_vec)
-            d1 = d1[:, np.newaxis]
-            d2 = lpsi.predict(S, num_node,alpha, diff_vec)
-            d2 = d2[:, np.newaxis]
-            d3 = lpsi.predict(S, num_node,alpha, V3)
-            d3 = d3[:, np.newaxis]
-            d4 = lpsi.predict(S, num_node,alpha, V4)
-            d4 = d4[:, np.newaxis]
-            lpsi_input[i,:,:] = np.concatenate((d1, d2, d3, d4), axis=1)
-        # Training loop
-        for epoch in range(num_epoch):
-            optimizer.zero_grad()
-            total_loss = 0
-            for i, influ_mat in enumerate(train_dataset):
-                seed_vec = influ_mat[:, 0].unsqueeze(-1)
-                seed_vec_onehot =torch.concat((1-seed_vec,seed_vec),dim=1)
-                diff_vec = influ_mat[:, -1]
-                pred = gcnsi_model(lpsi_input[i,:,:], edge_index)
-                loss = criterion(pred, seed_vec_onehot)
-                total_loss += loss
-                loss.backward()
-                optimizer.step()
-            average_loss =total_loss/train_num
-            if epoch%print_epoch==0:
-                print(f"epoch = {epoch}, loss = {average_loss:.3f}")
-        train_auc = 0
-        # Compute AUC score on training data
-        for i,influ_mat in enumerate(train_dataset):
-            seed_vec = influ_mat[:, 0]
-            seed_vec = seed_vec.squeeze(-1).long()
-            pred = gcnsi_model(lpsi_input[i,:,:], edge_index)
-            pred = torch.softmax(pred,dim=1)
-            pred = pred[:, 1].squeeze(-1).detach().numpy()
-            train_auc += roc_auc_score(seed_vec, pred)
-        train_auc = train_auc / train_num
-        print(f"train_auc = {train_auc:.3f}")
-        
-        opt_pred = np.zeros((num_node,train_num))
-        seed_all = np.zeros((num_node,train_num))
-        for i,influ_mat in enumerate(train_dataset):
-                seed_all[:,i] = influ_mat[:, 0]
-                diff_vec = influ_mat[:, -1]
-                pred = gcnsi_model(lpsi_input[i,:,:], edge_index)
-                pred = torch.softmax(pred, dim=1)
-                pred = pred[:, 1].squeeze(-1).detach().numpy()
-                opt_pred[:,i] = pred
-
-        opt_f1 = 0
-        # Find optimal threshold and F1 score
-        for thres in thres_list:
-            train_f1 = 0
-            for i in range(train_num):
-                train_f1 += f1_score(seed_all[:,i], opt_pred[:,i] >= thres)
-            train_f1 = train_f1 / train_num
-            print(f"thres = {thres:.3f}, train_f1 = {train_f1:.3f}")
-            if train_f1 > opt_f1:
-                opt_f1 = train_f1
-                opt_thres = thres
-
-        return gcnsi_model, opt_thres, train_auc, opt_f1, opt_pred
-
-    def test(self, adj, test_dataset, gcnsi_model, thres, alpha = 0.01):
-        """
-        Test the GCNSI model.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): Adjacency matrix of the graph.
-
-        - test_dataset (torch.utils.data.dataset.Subset): the test dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
-
-        - gcnsi_model (GCNSI_model): Trained GCNSI model.
-
-        - thres (float): Threshold value.
-
-        - alpha (float): The fraction of label information that a node gets from its neighbors (between 0 and 1).
-
-
-        Returns:
-
-        - metric (Metric): Evaluation metric containing accuracy, precision, recall, F1 score, and AUC score.
-
-        Example:
-
-        from data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GNN.GCNSI.main import GCNSI
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        gcnsi = GCNSI()
-
-        gcnsi_model, thres, auc, f1, pred =gcnsi.train(adj, train_dataset)
-
-        print("GCNSI:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-
-        metric = gcnsi.test(adj, test_dataset, gcnsi_model, thres)
-
-        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-        """
-        # Compute Laplacian matrix
-        S = csgraph.laplacian(adj, normed=True)
-        S = np.array(coo_matrix.todense(S))
-        num_node = adj.shape[0]
-        test_num = len(test_dataset)
-        # Convert adjacency matrix to edge index tensor
-        coo = adj.tocoo()
-        row = torch.from_numpy(coo.row.astype(np.int64)).to(torch.long)
-        col = torch.from_numpy(coo.col.astype(np.int64)).to(torch.long)
-        edge_index = torch.stack([row, col], dim=0)
-
-        lpsi = LPSI()  # Initializing LPSI module
-        lpsi_input = np.zeros((test_num,num_node,4))
-
-        for i, influ_mat in enumerate(test_dataset):
-            diff_vec = influ_mat[:, -1]
-            V3 = copy.deepcopy(diff_vec)
-            V4 = copy.deepcopy(diff_vec)
-            V3[diff_vec < 0.5] = 0.5
-            V4[diff_vec >= 0.5] = 0.5
-            d1 = copy.deepcopy(diff_vec)
-            d1 = d1[:, np.newaxis]
-            d2 = lpsi.predict(S, num_node,alpha, diff_vec)
-            d2 = d2[:, np.newaxis]
-            d3 = lpsi.predict(S, num_node,alpha, V3)
-            d3 = d3[:, np.newaxis]
-            d4 = lpsi.predict(S, num_node,alpha, V4)
-            d4 = d4[:, np.newaxis]
-            lpsi_input[i,:,:] = np.concatenate((d1, d2, d3, d4), axis=1)
-        test_acc = 0
-        test_pr = 0
-        test_re = 0
-        test_f1 = 0
-        test_auc = 0
-        # Evaluate on test data
-        for influ_mat in test_dataset:
-            seed_vec = influ_mat[:, 0]
-            diff_vec = influ_mat[:, -1]
-            pred = gcnsi_model(lpsi_input[i,:,:], edge_index)
-            pred = torch.softmax(pred, dim=1)
-            pred = pred[:, 1].squeeze(-1).detach().numpy()
-            test_acc += accuracy_score(seed_vec, pred >= thres)
-            test_pr += precision_score(seed_vec, pred >= thres, zero_division = 1)
-            test_re += recall_score(seed_vec, pred >= thres, zero_division = 1)
-            test_f1 += f1_score(seed_vec, pred >= thres, zero_division = 1)
-            test_auc += roc_auc_score(seed_vec, pred)
-
-        test_acc = test_acc / test_num
-        test_pr = test_pr / test_num
-        test_re = test_re / test_num
-        test_f1 = test_f1 / test_num
-        test_auc = test_auc / test_num
-        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
-        return metric
+import torch
+from scipy.sparse import csgraph,coo_matrix
+import copy
+import numpy as np
+from GraphSL.GNN.GCNSI.model import GCNSI_model
+from GraphSL.Prescribed import LPSI
+from sklearn.metrics import roc_auc_score,f1_score,accuracy_score,precision_score,recall_score
+from GraphSL.Evaluation import Metric
+class GCNSI:
+    """
+    Implement the Graph Convolutional Networks based Source Identification (GCNSI).
+
+    Dong, Ming, et al. "Multiple rumor source detection with graph convolutional networks." Proceedings of the 28th ACM international conference on information and knowledge management. 2019.
+    """
+
+    def __init__(self):
+        """
+        Initializes the GCNSI module.
+        """
+
+    def train(self, adj, train_dataset, alpha=0.01, thres_list=[0.1,0.3,0.5,0.7,0.9],lr=0.001, num_epoch=50,print_epoch=10, weight=torch.tensor([1.0,3.0])):
+        """
+        Train the GCNSI model.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): Adjacency matrix of the graph.
+
+        - train_dataset (torch.utils.data.dataset.Subset): the training dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
+        
+        - alpha (float): The fraction of label information that a node gets from its neighbors (between 0 and 1) to try.
+        
+        - thres_list (list): List of threshold values to try.
+
+        - lr (float): Learning rate.
+        
+        - num_epoch (int): Number of training epochs.
+        
+        - print_epoch (int): Number of epochs every time to print loss.
+
+        - weight (torch.Tensor): Weight tensor for loss computation, the first and second values are loss weights for non-seed and seed, respectively.
+
+        Returns:
+
+        - gcnsi_model (GCNSI_model): GCNSI model.
+
+        - opt_thres (float): Optimal threshold value.
+
+        - train_auc (float): Training AUC score.
+
+        - opt_f1 (float): Optimal F1 score.
+
+        - opt_pred (numpy.ndarray): Predicted seed vector of the training set, every column is the prediction of every simulation. It is used to adjust thres_list.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.GNN.GCNSI.main import GCNSI
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        gcnsi = GCNSI()
+
+        gcnsi_model, thres, auc, f1, pred =gcnsi.train(adj, train_dataset)
+
+        print("GCNSI:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+        """
+        # Compute Laplacian matrix
+        S = csgraph.laplacian(adj, normed=True)
+        S = np.array(coo_matrix.todense(S))
+        num_node = adj.shape[0]
+        train_num = len(train_dataset)
+        # Convert adjacency matrix to edge index tensor
+        coo = adj.tocoo()
+        row = torch.from_numpy(coo.row.astype(np.int64)).to(torch.long)
+        col = torch.from_numpy(coo.col.astype(np.int64)).to(torch.long)
+        edge_index = torch.stack([row, col], dim=0)
+        # Iterate over alpha values
+        gcnsi_model = GCNSI_model()
+        optimizer = torch.optim.Adam(gcnsi_model.parameters(), lr=lr)
+        criterion = torch.nn.CrossEntropyLoss(weight=weight)
+        # Augmented features by LPSI
+
+        lpsi = LPSI()  # Initializing LPSI module
+        lpsi_input = np.zeros((train_num,num_node,4))
+
+        for i, influ_mat in enumerate(train_dataset):
+            diff_vec = influ_mat[:, -1]
+            V3 = copy.deepcopy(diff_vec)
+            V4 = copy.deepcopy(diff_vec)
+            V3[diff_vec < 0.5] = 0.5
+            V4[diff_vec >= 0.5] = 0.5
+            d1 = copy.deepcopy(diff_vec)
+            d1 = d1[:, np.newaxis]
+            d2 = lpsi.predict(S, num_node,alpha, diff_vec)
+            d2 = d2[:, np.newaxis]
+            d3 = lpsi.predict(S, num_node,alpha, V3)
+            d3 = d3[:, np.newaxis]
+            d4 = lpsi.predict(S, num_node,alpha, V4)
+            d4 = d4[:, np.newaxis]
+            lpsi_input[i,:,:] = np.concatenate((d1, d2, d3, d4), axis=1)
+        # Training loop
+        for epoch in range(num_epoch):
+            optimizer.zero_grad()
+            total_loss = 0
+            for i, influ_mat in enumerate(train_dataset):
+                seed_vec = influ_mat[:, 0].unsqueeze(-1)
+                seed_vec_onehot =torch.concat((1-seed_vec,seed_vec),dim=1)
+                diff_vec = influ_mat[:, -1]
+                pred = gcnsi_model(lpsi_input[i,:,:], edge_index)
+                loss = criterion(pred, seed_vec_onehot)
+                total_loss += loss
+                loss.backward()
+                optimizer.step()
+            average_loss =total_loss/train_num
+            if epoch%print_epoch==0:
+                print(f"epoch = {epoch}, loss = {average_loss:.3f}")
+        train_auc = 0
+        # Compute AUC score on training data
+        for i,influ_mat in enumerate(train_dataset):
+            seed_vec = influ_mat[:, 0]
+            seed_vec = seed_vec.squeeze(-1).long()
+            pred = gcnsi_model(lpsi_input[i,:,:], edge_index)
+            pred = torch.softmax(pred,dim=1)
+            pred = pred[:, 1].squeeze(-1).detach().numpy()
+            train_auc += roc_auc_score(seed_vec, pred)
+        train_auc = train_auc / train_num
+        print(f"train_auc = {train_auc:.3f}")
+        
+        opt_pred = np.zeros((num_node,train_num))
+        seed_all = np.zeros((num_node,train_num))
+        for i,influ_mat in enumerate(train_dataset):
+                seed_all[:,i] = influ_mat[:, 0]
+                diff_vec = influ_mat[:, -1]
+                pred = gcnsi_model(lpsi_input[i,:,:], edge_index)
+                pred = torch.softmax(pred, dim=1)
+                pred = pred[:, 1].squeeze(-1).detach().numpy()
+                opt_pred[:,i] = pred
+
+        opt_f1 = 0
+        # Find optimal threshold and F1 score
+        for thres in thres_list:
+            train_f1 = 0
+            for i in range(train_num):
+                train_f1 += f1_score(seed_all[:,i], opt_pred[:,i] >= thres)
+            train_f1 = train_f1 / train_num
+            print(f"thres = {thres:.3f}, train_f1 = {train_f1:.3f}")
+            if train_f1 > opt_f1:
+                opt_f1 = train_f1
+                opt_thres = thres
+
+        return gcnsi_model, opt_thres, train_auc, opt_f1, opt_pred
+
+    def test(self, adj, test_dataset, gcnsi_model, thres, alpha = 0.01):
+        """
+        Test the GCNSI model.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): Adjacency matrix of the graph.
+
+        - test_dataset (torch.utils.data.dataset.Subset): the test dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
+
+        - gcnsi_model (GCNSI_model): Trained GCNSI model.
+
+        - thres (float): Threshold value.
+
+        - alpha (float): The fraction of label information that a node gets from its neighbors (between 0 and 1).
+
+
+        Returns:
+
+        - metric (Metric): Evaluation metric containing accuracy, precision, recall, F1 score, and AUC score.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from data.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GNN.GCNSI.main import GCNSI
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        gcnsi = GCNSI()
+
+        gcnsi_model, thres, auc, f1, pred =gcnsi.train(adj, train_dataset)
+
+        print("GCNSI:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+
+        metric = gcnsi.test(adj, test_dataset, gcnsi_model, thres)
+
+        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+        """
+        # Compute Laplacian matrix
+        S = csgraph.laplacian(adj, normed=True)
+        S = np.array(coo_matrix.todense(S))
+        num_node = adj.shape[0]
+        test_num = len(test_dataset)
+        # Convert adjacency matrix to edge index tensor
+        coo = adj.tocoo()
+        row = torch.from_numpy(coo.row.astype(np.int64)).to(torch.long)
+        col = torch.from_numpy(coo.col.astype(np.int64)).to(torch.long)
+        edge_index = torch.stack([row, col], dim=0)
+
+        lpsi = LPSI()  # Initializing LPSI module
+        lpsi_input = np.zeros((test_num,num_node,4))
+
+        for i, influ_mat in enumerate(test_dataset):
+            diff_vec = influ_mat[:, -1]
+            V3 = copy.deepcopy(diff_vec)
+            V4 = copy.deepcopy(diff_vec)
+            V3[diff_vec < 0.5] = 0.5
+            V4[diff_vec >= 0.5] = 0.5
+            d1 = copy.deepcopy(diff_vec)
+            d1 = d1[:, np.newaxis]
+            d2 = lpsi.predict(S, num_node,alpha, diff_vec)
+            d2 = d2[:, np.newaxis]
+            d3 = lpsi.predict(S, num_node,alpha, V3)
+            d3 = d3[:, np.newaxis]
+            d4 = lpsi.predict(S, num_node,alpha, V4)
+            d4 = d4[:, np.newaxis]
+            lpsi_input[i,:,:] = np.concatenate((d1, d2, d3, d4), axis=1)
+        test_acc = 0
+        test_pr = 0
+        test_re = 0
+        test_f1 = 0
+        test_auc = 0
+        # Evaluate on test data
+        for influ_mat in test_dataset:
+            seed_vec = influ_mat[:, 0]
+            diff_vec = influ_mat[:, -1]
+            pred = gcnsi_model(lpsi_input[i,:,:], edge_index)
+            pred = torch.softmax(pred, dim=1)
+            pred = pred[:, 1].squeeze(-1).detach().numpy()
+            test_acc += accuracy_score(seed_vec, pred >= thres)
+            test_pr += precision_score(seed_vec, pred >= thres, zero_division = 1)
+            test_re += recall_score(seed_vec, pred >= thres, zero_division = 1)
+            test_f1 += f1_score(seed_vec, pred >= thres, zero_division = 1)
+            test_auc += roc_auc_score(seed_vec, pred)
+
+        test_acc = test_acc / test_num
+        test_pr = test_pr / test_num
+        test_re = test_re / test_num
+        test_f1 = test_f1 / test_num
+        test_auc = test_auc / test_num
+        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
+        return metric
```

### Comparing `GraphSL-0.8/GraphSL/GNN/GCNSI/model.py` & `GraphSL-0.9/GraphSL/GNN/GCNSI/model.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import torch
-from torch_geometric.nn import MessagePassing
-from torch_geometric.utils import add_self_loops, degree
-import torch.nn.functional as F
-class GCNConv(MessagePassing):
-    """
-    Define a Graph Convolutional Network (GCN) layer.
-    """
-
-    def __init__(self, in_channels, out_channels):
-        """
-        Initialize the GCNConv layer with input and output channel dimensions.
-
-        Args:
-
-        - in_channels (int): Number of input channels.
-
-        - out_channels (int): Number of output channels.
-        """
-        super(GCNConv, self).__init__(aggr='add')  # Setting the aggregation method for message passing
-        self.lin = torch.nn.Linear(in_channels, out_channels)  # Initializing a linear transformation
-
-    def forward(self, x, edge_index):
-        """
-        Perform the forward pass of the GCNConv layer.
-
-        Args:
-
-        - x (torch.Tensor): Input node features.
-
-        - edge_index (torch.Tensor): Edge indices representing connectivity.
-
-        Returns:
-
-        - torch.Tensor: Tensor after the GCN layer computation.
-        """
-        # Step 1: Add self-loops
-        edge_index, _ = add_self_loops(edge_index, num_nodes=x.size(0))
-
-        # Step 2: Multiply with weights
-        x = self.lin(x)
-
-        # Step 3: Calculate the normalization
-        row, col = edge_index
-        deg = degree(row, x.size(0), dtype=x.dtype)
-        deg_inv_sqrt = deg.pow(-0.5)
-        norm = deg_inv_sqrt[row] * deg_inv_sqrt[col]
-
-        # Step 4: Propagate the embeddings to the next layer
-        return self.propagate(edge_index, size=(x.size(0), x.size(0)), x=x, norm=norm)
-
-class GCNSI_model(torch.nn.Module):
-    """
-    Define the model of Graph Convolutional Networks based Source Identification (GCNSI).
-    """
-
-    def __init__(self):
-        super(GCNSI_model, self).__init__()
-        self.conv1 = GCNConv(4, 32)  # Initializing the first GCN layer
-        self.conv2 = GCNConv(32, 32)  # Initializing the second GCN layer
-        self.fc = torch.nn.Linear(32, 2)  # Initializing a linear transformation layer
-        #self.softmax=torch.nn.Softmax(dim=1)
-
-    def forward(self, x, edge_index):
-        """
-        Performs the forward pass of the GCNSI model.
-
-        Args:
-
-        - x (numpy.ndarray): The input features augmented by LPSI.
-
-        - edge_index (torch.Tensor): Edge indices representing connectivity.
-
-        Returns:
-
-        - x (torch.Tensor): A tensor representing identified source nodes.
-        """
-        
-        x = torch.tensor(x, dtype=torch.float)
-        x = self.conv1(x, edge_index)
-        x = F.relu(x)
-        x = F.dropout(x, training=self.training)
-        x = self.conv2(x, edge_index)
-        x = self.fc(x)
-        #x = self.softmax(x)
-        return x
+import torch
+from torch_geometric.nn import MessagePassing
+from torch_geometric.utils import add_self_loops, degree
+import torch.nn.functional as F
+class GCNConv(MessagePassing):
+    """
+    Define a Graph Convolutional Network (GCN) layer.
+    """
+
+    def __init__(self, in_channels, out_channels):
+        """
+        Initialize the GCNConv layer with input and output channel dimensions.
+
+        Args:
+
+        - in_channels (int): Number of input channels.
+
+        - out_channels (int): Number of output channels.
+        """
+        super(GCNConv, self).__init__(aggr='add')  # Setting the aggregation method for message passing
+        self.lin = torch.nn.Linear(in_channels, out_channels)  # Initializing a linear transformation
+
+    def forward(self, x, edge_index):
+        """
+        Perform the forward pass of the GCNConv layer.
+
+        Args:
+
+        - x (torch.Tensor): Input node features.
+
+        - edge_index (torch.Tensor): Edge indices representing connectivity.
+
+        Returns:
+
+        - torch.Tensor: Tensor after the GCN layer computation.
+        """
+        # Step 1: Add self-loops
+        edge_index, _ = add_self_loops(edge_index, num_nodes=x.size(0))
+
+        # Step 2: Multiply with weights
+        x = self.lin(x)
+
+        # Step 3: Calculate the normalization
+        row, col = edge_index
+        deg = degree(row, x.size(0), dtype=x.dtype)
+        deg_inv_sqrt = deg.pow(-0.5)
+        norm = deg_inv_sqrt[row] * deg_inv_sqrt[col]
+
+        # Step 4: Propagate the embeddings to the next layer
+        return self.propagate(edge_index, size=(x.size(0), x.size(0)), x=x, norm=norm)
+
+class GCNSI_model(torch.nn.Module):
+    """
+    Define the model of Graph Convolutional Networks based Source Identification (GCNSI).
+    """
+
+    def __init__(self):
+        super(GCNSI_model, self).__init__()
+        self.conv1 = GCNConv(4, 32)  # Initializing the first GCN layer
+        self.conv2 = GCNConv(32, 32)  # Initializing the second GCN layer
+        self.fc = torch.nn.Linear(32, 2)  # Initializing a linear transformation layer
+        #self.softmax=torch.nn.Softmax(dim=1)
+
+    def forward(self, x, edge_index):
+        """
+        Performs the forward pass of the GCNSI model.
+
+        Args:
+
+        - x (numpy.ndarray): The input features augmented by LPSI.
+
+        - edge_index (torch.Tensor): Edge indices representing connectivity.
+
+        Returns:
+
+        - x (torch.Tensor): A tensor representing identified source nodes.
+        """
+        
+        x = torch.tensor(x, dtype=torch.float)
+        x = self.conv1(x, edge_index)
+        x = F.relu(x)
+        x = F.dropout(x, training=self.training)
+        x = self.conv2(x, edge_index)
+        x = self.fc(x)
+        #x = self.softmax(x)
+        return x
```

### Comparing `GraphSL-0.8/GraphSL/GNN/IVGD/correction.py` & `GraphSL-0.9/GraphSL/GNN/IVGD/correction.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import torch
-import torch.nn.functional as F
-
-class correction(torch.nn.Module):
-    """
-    Define an error correction module.
-    """
-
-    def __init__(self):
-        """
-        Initializes the error correction module.
-        """
-        super(correction, self).__init__()
-        number_of_neurons = 1000
-        # Define the fully connected layers
-        self.fc1 = torch.nn.Linear(2, number_of_neurons)
-        self.fc2 = torch.nn.Linear(number_of_neurons, number_of_neurons)
-        self.fc3 = torch.nn.Linear(number_of_neurons, 2)
-
-    def forward(self, x):
-        """
-        Define the forward pass of the error correction module.
-
-        Args:
-
-        - x (torch.Tensor): Prediction of the seed vector from invertible graph residual net.
-
-        Returns:
-
-        - temp (torch.Tensor): Corrected prediction of the seed vector.
-        """
-        # Concatenate the input tensor with its complement along the second dimension
-        x = torch.cat((1 - x, x), dim=1)
-        # Apply the first fully connected layer followed by ReLU activation
-        temp = F.relu(self.fc1(x))
-        # Apply the second fully connected layer followed by ReLU activation
-        temp = F.relu(self.fc2(temp))
-        # Apply the third fully connected layer
-        temp = self.fc3(temp)
-        # Add the input tensor to the output tensor
-        temp = (temp + x)
-        # Clip the values of the output tensor between 0 and 1
-        temp = torch.minimum(torch.maximum(torch.zeros(temp.shape), temp), torch.ones(temp.shape))
-        return temp
+import torch
+import torch.nn.functional as F
+
+class correction(torch.nn.Module):
+    """
+    Define an error correction module.
+    """
+
+    def __init__(self):
+        """
+        Initializes the error correction module.
+        """
+        super(correction, self).__init__()
+        number_of_neurons = 1000
+        # Define the fully connected layers
+        self.fc1 = torch.nn.Linear(2, number_of_neurons)
+        self.fc2 = torch.nn.Linear(number_of_neurons, number_of_neurons)
+        self.fc3 = torch.nn.Linear(number_of_neurons, 2)
+
+    def forward(self, x):
+        """
+        Define the forward pass of the error correction module.
+
+        Args:
+
+        - x (torch.Tensor): Prediction of the seed vector from invertible graph residual net.
+
+        Returns:
+
+        - temp (torch.Tensor): Corrected prediction of the seed vector.
+        """
+        # Concatenate the input tensor with its complement along the second dimension
+        x = torch.cat((1 - x, x), dim=1)
+        # Apply the first fully connected layer followed by ReLU activation
+        temp = F.relu(self.fc1(x))
+        # Apply the second fully connected layer followed by ReLU activation
+        temp = F.relu(self.fc2(temp))
+        # Apply the third fully connected layer
+        temp = self.fc3(temp)
+        # Add the input tensor to the output tensor
+        temp = (temp + x)
+        # Clip the values of the output tensor between 0 and 1
+        temp = torch.minimum(torch.maximum(torch.zeros(temp.shape), temp), torch.ones(temp.shape))
+        return temp
```

### Comparing `GraphSL-0.8/GraphSL/GNN/IVGD/earlystopping.py` & `GraphSL-0.9/GraphSL/GNN/IVGD/earlystopping.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from typing import List
-import copy
-import operator
-from enum import Enum, auto
-import numpy as np
-from torch.nn import Module
-
-
-class StopVariable(Enum):
-    """
-    Enum class representing stopping criteria variables.
-    """
-    LOSS = auto()
-    ACCURACY = auto()
-    NONE = auto()
-
-
-class Best(Enum):
-    """
-    Enum class representing best stopping criteria.
-    """
-    RANKED = auto()
-    ALL = auto()
-
-
-stopping_args = dict(
-    stop_varnames=[StopVariable.LOSS],
-    patience=30, max_epochs=1000, remember=Best.RANKED)
-
-
-class EarlyStopping:
-    """
-    Class for implementing early stopping in model training.
-    """
-
-    def __init__(
-            self, model: Module, stop_varnames: List[StopVariable],
-            patience: int = 30, max_epochs: int = 1000, remember: Best = Best.ALL):
-        """
-        Initializes the EarlyStopping object.
-
-        Args:
-
-        - model (Module): The neural network model.
-
-        - stop_varnames (List[StopVariable]): List of stopping criteria variables.
-
-        - patience (int): Number of epochs to wait after reaching the best model before stopping.
-
-        - max_epochs (int): Maximum number of epochs for training.
-
-        - remember (Best): Specifies how to remember the best model.
-        """
-        self.model = model
-        self.comp_ops = []
-        self.stop_vars = []
-        self.best_vals = []
-        for stop_varname in stop_varnames:
-            if stop_varname is StopVariable.LOSS:
-                self.stop_vars.append('loss')
-                self.comp_ops.append(operator.le)
-                self.best_vals.append(np.inf)
-            elif stop_varname is StopVariable.ACCURACY:
-                self.stop_vars.append('acc')
-                self.comp_ops.append(operator.ge)
-                self.best_vals.append(-np.inf)
-        self.remember = remember
-        self.remembered_vals = copy.copy(self.best_vals)
-        self.max_patience = patience
-        self.patience = self.max_patience
-        self.max_epochs = max_epochs
-        self.best_epoch = None
-        self.best_state = None
-
-    def check(self, values: List[np.floating], epoch: int) -> bool:
-        """
-        Checks if early stopping criteria are met.
-
-        Args:
-
-        - values (List[np.floating]): List of evaluation metric values.
-
-        - epoch (int): Current epoch number.
-
-        Returns:
-
-        - bool: True if early stopping criteria are met, False otherwise.
-        """
-        checks = [self.comp_ops[i](val, self.best_vals[i])
-                  for i, val in enumerate(values)]
-        if any(checks):
-            self.best_vals = np.choose(checks, [self.best_vals, values])
-            self.patience = self.max_patience
-
-            comp_remembered = [
-                    self.comp_ops[i](val, self.remembered_vals[i])
-                    for i, val in enumerate(values)]
-            if self.remember is Best.ALL:
-                if all(comp_remembered):
-                    self.best_epoch = epoch
-                    self.remembered_vals = copy.copy(values)
-                    self.best_state = {
-                            key: value.cpu() for key, value
-                            in self.model.state_dict().items()}
-            elif self.remember is Best.RANKED:
-                for i, comp in enumerate(comp_remembered):
-                    if comp:
-                        if not(self.remembered_vals[i] == values[i]):
-                            self.best_epoch = epoch
-                            self.remembered_vals = copy.copy(values)
-                            self.best_state = {
-                                    key: value.cpu() for key, value
-                                    in self.model.state_dict().items()}
-                            break
-                    else:
-                        break
-        else:
-            self.patience -= 1
+from typing import List
+import copy
+import operator
+from enum import Enum, auto
+import numpy as np
+from torch.nn import Module
+
+
+class StopVariable(Enum):
+    """
+    Enum class representing stopping criteria variables.
+    """
+    LOSS = auto()
+    ACCURACY = auto()
+    NONE = auto()
+
+
+class Best(Enum):
+    """
+    Enum class representing best stopping criteria.
+    """
+    RANKED = auto()
+    ALL = auto()
+
+
+stopping_args = dict(
+    stop_varnames=[StopVariable.LOSS],
+    patience=30, max_epochs=1000, remember=Best.RANKED)
+
+
+class EarlyStopping:
+    """
+    Class for implementing early stopping in model training.
+    """
+
+    def __init__(
+            self, model: Module, stop_varnames: List[StopVariable],
+            patience: int = 30, max_epochs: int = 1000, remember: Best = Best.ALL):
+        """
+        Initializes the EarlyStopping object.
+
+        Args:
+
+        - model (Module): The neural network model.
+
+        - stop_varnames (List[StopVariable]): List of stopping criteria variables.
+
+        - patience (int): Number of epochs to wait after reaching the best model before stopping.
+
+        - max_epochs (int): Maximum number of epochs for training.
+
+        - remember (Best): Specifies how to remember the best model.
+        """
+        self.model = model
+        self.comp_ops = []
+        self.stop_vars = []
+        self.best_vals = []
+        for stop_varname in stop_varnames:
+            if stop_varname is StopVariable.LOSS:
+                self.stop_vars.append('loss')
+                self.comp_ops.append(operator.le)
+                self.best_vals.append(np.inf)
+            elif stop_varname is StopVariable.ACCURACY:
+                self.stop_vars.append('acc')
+                self.comp_ops.append(operator.ge)
+                self.best_vals.append(-np.inf)
+        self.remember = remember
+        self.remembered_vals = copy.copy(self.best_vals)
+        self.max_patience = patience
+        self.patience = self.max_patience
+        self.max_epochs = max_epochs
+        self.best_epoch = None
+        self.best_state = None
+
+    def check(self, values: List[np.floating], epoch: int) -> bool:
+        """
+        Checks if early stopping criteria are met.
+
+        Args:
+
+        - values (List[np.floating]): List of evaluation metric values.
+
+        - epoch (int): Current epoch number.
+
+        Returns:
+
+        - bool: True if early stopping criteria are met, False otherwise.
+        """
+        checks = [self.comp_ops[i](val, self.best_vals[i])
+                  for i, val in enumerate(values)]
+        if any(checks):
+            self.best_vals = np.choose(checks, [self.best_vals, values])
+            self.patience = self.max_patience
+
+            comp_remembered = [
+                    self.comp_ops[i](val, self.remembered_vals[i])
+                    for i, val in enumerate(values)]
+            if self.remember is Best.ALL:
+                if all(comp_remembered):
+                    self.best_epoch = epoch
+                    self.remembered_vals = copy.copy(values)
+                    self.best_state = {
+                            key: value.cpu() for key, value
+                            in self.model.state_dict().items()}
+            elif self.remember is Best.RANKED:
+                for i, comp in enumerate(comp_remembered):
+                    if comp:
+                        if not(self.remembered_vals[i] == values[i]):
+                            self.best_epoch = epoch
+                            self.remembered_vals = copy.copy(values)
+                            self.best_state = {
+                                    key: value.cpu() for key, value
+                                    in self.model.state_dict().items()}
+                            break
+                    else:
+                        break
+        else:
+            self.patience -= 1
         return self.patience == 0
```

### Comparing `GraphSL-0.8/GraphSL/GNN/IVGD/i_deepis.py` & `GraphSL-0.9/GraphSL/GNN/IVGD/i_deepis.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-import torch
-import torch.nn as nn
-import numpy as np
-import scipy.sparse as sp
-
-
-class Identity(nn.Module):
-    """
-    Identity module to select specific elements from input tensor.
-    """
-
-    def __init__(self):
-        super(Identity, self).__init__()
-
-    def forward(self, preds, idx):
-        """
-        Forward pass to select specific elements from input tensor.
-
-        Args:
-
-        - preds (torch.Tensor): Input tensor.
-
-        - idx (torch.Tensor): Indices of elements to select.
-
-        Returns:
-
-        - torch.Tensor: Selected elements from input tensor.
-        """
-        return preds[idx]
-
-
-class DiffusionPropagate(nn.Module):
-    """
-    Module for diffusion propagation.
-    """
-
-    def __init__(self, prob_matrix, niter):
-        """
-        Initializes the DiffusionPropagate module.
-
-        Args:
-
-        - prob_matrix (torch.Tensor): Probability matrix for diffusion.
-
-        - niter (int): Number of iterations for diffusion propagation.
-        """
-        super(DiffusionPropagate, self).__init__()
-        self.niter = niter
-        if sp.isspmatrix(prob_matrix):
-            prob_matrix = prob_matrix.toarray()
-        self.register_buffer('prob_matrix', torch.FloatTensor(prob_matrix))
-
-    def forward(self, preds, seed_idx, idx):
-        """
-        Performs forward pass for diffusion propagation.
-
-        Args:
-
-        - preds (torch.Tensor): Input tensor of predictions.
-
-        - seed_idx (torch.Tensor): Indices of seed nodes.
-
-        - idx (torch.Tensor): Indices of nodes to propagate to.
-
-        Returns:
-
-        - torch.Tensor: Resulting propagated predictions.
-        """
-        temp = preds
-        temp = temp.flatten()
-        device = preds.device
-        for i in range(self.niter):
-            P2 = self.prob_matrix.T * preds.view((1, -1)).expand(self.prob_matrix.shape)
-            P3 = torch.ones(self.prob_matrix.shape).to(device) - P2
-            preds = torch.ones((self.prob_matrix.shape[0],)).to(device) - torch.prod(P3, dim=1)
-            #preds[seed_idx] = 1
-        preds = (preds + temp) / 2
-        return preds[idx]
-
-    def backward(self, preds):
-        """
-        Perform backward pass for diffusion propagation.
-
-        Args:
-
-        - preds (torch.Tensor):  Prediction of diffusion.
-
-        Returns:
-
-        - res (torch.Tensor): Prediction of seeds.
-        """
-        device = preds.device
-        res = preds
-        temp = preds
-        for j in range(10):
-            for i in range(self.niter):
-                P2 = self.prob_matrix.T * res.view((1, -1)).expand(self.prob_matrix.shape)
-                P3 = torch.ones(self.prob_matrix.shape).to(device) - P2
-                temp = torch.ones((self.prob_matrix.shape[0],)).to(device) - torch.prod(P3, dim=1)
-                #temp[preds == 1] = 1
-            res = 2 * preds - temp
-            res = torch.maximum(torch.minimum(res, torch.tensor(1)), torch.tensor(0))
-        return res
-
-
-class i_DeepIS(nn.Module):
-    """
-    Invertible Deep Influence Spread (i_DeepIS) module for graph source localization.
-    """
-
-    def __init__(self, gnn_model: nn.Module, propagate: nn.Module):
-        """
-        Initializes the i_DeepIS module.
-
-        Args:
-
-        - gnn_model (nn.Module): Graph neural network model.
-
-        - propagate (nn.Module): Propagation module for diffusion.
-        """
-        super(i_DeepIS, self).__init__()
-        self.gnn_model = gnn_model
-        self.propagate = propagate
-
-        self.reg_params = list(filter(lambda x: x.requires_grad, self.gnn_model.parameters()))
-
-    def forward(self, idx: torch.LongTensor):
-        """
-        Forward pass for i_DeepIS module.
-
-        Args:
-
-        - idx (torch.LongTensor): Indices of nodes to fetch predictions for.
-
-        Returns:
-
-        - torch.Tensor: Predictions for selected nodes.
-        """
-        device = next(self.gnn_model.parameters()).device
-        total_node_nums = self.gnn_model.features.weight.shape[0]
-        total_nodes = torch.LongTensor(np.arange(total_node_nums)).to(device)
-        seed = self.gnn_model.features.weight[:, 0]
-        seed_idx = torch.LongTensor(np.argwhere(seed.detach().cpu().numpy() == 1)).to(device)
-        seed = torch.unsqueeze(seed, 1)
-        predictions = self.gnn_model(total_nodes)  # predict all, for prediction propagation
-        predictions = (predictions + seed) / 2
-
-        predictions = self.propagate(predictions, seed_idx, idx)  # then select
-
-        return predictions.flatten()
-
-    def backward(self, prediction: torch.LongTensor):
-        """
-        Backward pass for i_DeepIS module.
-
-        Args:
-
-        - prediction (torch.LongTensor): Predictions.
-
-        Returns:
-
-        - torch.Tensor: Resulting propagated predictions after backward pass.
-        """
-        device = next(self.gnn_model.parameters()).device
-        total_node_nums = self.gnn_model.features.weight.shape[0]
-        total_nodes = torch.LongTensor(np.arange(total_node_nums)).to(device)
-        res = self.propagate.backward(prediction)
-        self.gnn_model.features.weight[:, 0] = res
-        for i in range(10):
-            temp = self.gnn_model(total_nodes).squeeze()
-            res = 2 * prediction - temp
-            self.gnn_model.features.weight[:, 0] = res.float()
-        return res
-
-    def loss(self, predictions, labels, λ, γ):
-        """
-        Computes the loss function for i_DeepIS module.
-
-        Args:
-
-        - predictions (torch.Tensor): Predicted values.
-
-        - labels (torch.Tensor): Ground truth labels.
-
-        - λ (float): Influence spread coefficient.
-
-        - γ (float): Regularization coefficient.
-
-        Returns:
-
-        - Loss (torch.Tensor): Computed loss value.
-        """
-        L1 = torch.sum(torch.abs(predictions - labels)) / len(labels)  # node-level error
-        L2 = torch.abs(torch.sum(predictions) - torch.sum(labels)) / (
-                torch.sum(labels) + 1e-5)  # influence spread error
-        Reg = sum(torch.sum(param ** 2) for param in self.reg_params)
-        Loss = L1 + λ * L2 + γ * Reg
-        return Loss
+import torch
+import torch.nn as nn
+import numpy as np
+import scipy.sparse as sp
+
+
+class Identity(nn.Module):
+    """
+    Identity module to select specific elements from input tensor.
+    """
+
+    def __init__(self):
+        super(Identity, self).__init__()
+
+    def forward(self, preds, idx):
+        """
+        Forward pass to select specific elements from input tensor.
+
+        Args:
+
+        - preds (torch.Tensor): Input tensor.
+
+        - idx (torch.Tensor): Indices of elements to select.
+
+        Returns:
+
+        - torch.Tensor: Selected elements from input tensor.
+        """
+        return preds[idx]
+
+
+class DiffusionPropagate(nn.Module):
+    """
+    Module for diffusion propagation.
+    """
+
+    def __init__(self, prob_matrix, niter):
+        """
+        Initializes the DiffusionPropagate module.
+
+        Args:
+
+        - prob_matrix (torch.Tensor): Probability matrix for diffusion.
+
+        - niter (int): Number of iterations for diffusion propagation.
+        """
+        super(DiffusionPropagate, self).__init__()
+        self.niter = niter
+        if sp.isspmatrix(prob_matrix):
+            prob_matrix = prob_matrix.toarray()
+        self.register_buffer('prob_matrix', torch.FloatTensor(prob_matrix))
+
+    def forward(self, preds, seed_idx, idx):
+        """
+        Performs forward pass for diffusion propagation.
+
+        Args:
+
+        - preds (torch.Tensor): Input tensor of predictions.
+
+        - seed_idx (torch.Tensor): Indices of seed nodes.
+
+        - idx (torch.Tensor): Indices of nodes to propagate to.
+
+        Returns:
+
+        - torch.Tensor: Resulting propagated predictions.
+        """
+        temp = preds
+        temp = temp.flatten()
+        device = preds.device
+        for i in range(self.niter):
+            P2 = self.prob_matrix.T * preds.view((1, -1)).expand(self.prob_matrix.shape)
+            P3 = torch.ones(self.prob_matrix.shape).to(device) - P2
+            preds = torch.ones((self.prob_matrix.shape[0],)).to(device) - torch.prod(P3, dim=1)
+            #preds[seed_idx] = 1
+        preds = (preds + temp) / 2
+        return preds[idx]
+
+    def backward(self, preds):
+        """
+        Perform backward pass for diffusion propagation.
+
+        Args:
+
+        - preds (torch.Tensor):  Prediction of diffusion.
+
+        Returns:
+
+        - res (torch.Tensor): Prediction of seeds.
+        """
+        device = preds.device
+        res = preds
+        temp = preds
+        for j in range(10):
+            for i in range(self.niter):
+                P2 = self.prob_matrix.T * res.view((1, -1)).expand(self.prob_matrix.shape)
+                P3 = torch.ones(self.prob_matrix.shape).to(device) - P2
+                temp = torch.ones((self.prob_matrix.shape[0],)).to(device) - torch.prod(P3, dim=1)
+                #temp[preds == 1] = 1
+            res = 2 * preds - temp
+            res = torch.maximum(torch.minimum(res, torch.tensor(1)), torch.tensor(0))
+        return res
+
+
+class i_DeepIS(nn.Module):
+    """
+    Invertible Deep Influence Spread (i_DeepIS) module for graph source localization.
+    """
+
+    def __init__(self, gnn_model: nn.Module, propagate: nn.Module):
+        """
+        Initializes the i_DeepIS module.
+
+        Args:
+
+        - gnn_model (nn.Module): Graph neural network model.
+
+        - propagate (nn.Module): Propagation module for diffusion.
+        """
+        super(i_DeepIS, self).__init__()
+        self.gnn_model = gnn_model
+        self.propagate = propagate
+
+        self.reg_params = list(filter(lambda x: x.requires_grad, self.gnn_model.parameters()))
+
+    def forward(self, idx: torch.LongTensor):
+        """
+        Forward pass for i_DeepIS module.
+
+        Args:
+
+        - idx (torch.LongTensor): Indices of nodes to fetch predictions for.
+
+        Returns:
+
+        - torch.Tensor: Predictions for selected nodes.
+        """
+        device = next(self.gnn_model.parameters()).device
+        total_node_nums = self.gnn_model.features.weight.shape[0]
+        total_nodes = torch.LongTensor(np.arange(total_node_nums)).to(device)
+        seed = self.gnn_model.features.weight[:, 0]
+        seed_idx = torch.LongTensor(np.argwhere(seed.detach().cpu().numpy() == 1)).to(device)
+        seed = torch.unsqueeze(seed, 1)
+        predictions = self.gnn_model(total_nodes)  # predict all, for prediction propagation
+        predictions = (predictions + seed) / 2
+
+        predictions = self.propagate(predictions, seed_idx, idx)  # then select
+
+        return predictions.flatten()
+
+    def backward(self, prediction: torch.LongTensor):
+        """
+        Backward pass for i_DeepIS module.
+
+        Args:
+
+        - prediction (torch.LongTensor): Predictions.
+
+        Returns:
+
+        - torch.Tensor: Resulting propagated predictions after backward pass.
+        """
+        device = next(self.gnn_model.parameters()).device
+        total_node_nums = self.gnn_model.features.weight.shape[0]
+        total_nodes = torch.LongTensor(np.arange(total_node_nums)).to(device)
+        res = self.propagate.backward(prediction)
+        self.gnn_model.features.weight[:, 0] = res
+        for i in range(10):
+            temp = self.gnn_model(total_nodes).squeeze()
+            res = 2 * prediction - temp
+            self.gnn_model.features.weight[:, 0] = res.float()
+        return res
+
+    def loss(self, predictions, labels, λ, γ):
+        """
+        Computes the loss function for i_DeepIS module.
+
+        Args:
+
+        - predictions (torch.Tensor): Predicted values.
+
+        - labels (torch.Tensor): Ground truth labels.
+
+        - λ (float): Influence spread coefficient.
+
+        - γ (float): Regularization coefficient.
+
+        Returns:
+
+        - Loss (torch.Tensor): Computed loss value.
+        """
+        L1 = torch.sum(torch.abs(predictions - labels)) / len(labels)  # node-level error
+        L2 = torch.abs(torch.sum(predictions) - torch.sum(labels)) / (
+                torch.sum(labels) + 1e-5)  # influence spread error
+        Reg = sum(torch.sum(param ** 2) for param in self.reg_params)
+        Loss = L1 + λ * L2 + γ * Reg
+        return Loss
```

### Comparing `GraphSL-0.8/GraphSL/GNN/IVGD/main.py` & `GraphSL-0.9/GraphSL/GNN/SLVAE/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,447 +1,454 @@
-import torch.nn.functional as F
-import numpy as np
-import torch
-import torch.nn as nn
-from GraphSL.GNN.IVGD.correction import correction
-from GraphSL.GNN.IVGD.i_deepis import i_DeepIS, DiffusionPropagate
-from GraphSL.GNN.IVGD.training import FeatureCons, get_idx_new_seeds
-from GraphSL.GNN.IVGD.model.MLP import MLPTransform
-from GraphSL.GNN.IVGD.training import train_model
-from sklearn.metrics import roc_auc_score,f1_score,accuracy_score,precision_score,recall_score
-from GraphSL.Evaluation import Metric
-import torch.optim as optim
-import warnings
-warnings.filterwarnings("ignore")
-
-
-
-class IVGD_model(torch.nn.Module):
-    """
-     Invertible Validity-aware Graph Diffusion (IVGD) Model.
-    """
-
-    def __init__(self, alpha, tau, rho):
-        """
-        Initializes the IVGD_model.
-
-        Args:
-
-        - alpha (float): Value of alpha parameter.
-
-        - tau (float): Value of tau parameter.
-
-        - rho (float): Value of rho parameter.
-        """
-        super(IVGD_model, self).__init__()
-        self.number_layer = 5
-        self.alpha1 = alpha
-        self.alpha2 = alpha
-        self.alpha3 = alpha
-        self.alpha4 = alpha
-        self.alpha5 = alpha
-
-        self.tau1 = tau
-        self.tau2 = tau
-        self.tau3 = tau
-        self.tau4 = tau
-        self.tau5 = tau
-
-        self.net1 = correction()
-        self.net2 = correction()
-        self.net3 = correction()
-        self.net4 = correction()
-        self.net5 = correction()
-
-        self.rho1 = rho
-        self.rho2 = rho
-        self.rho3 = rho
-        self.rho4 = rho
-        self.rho5 = rho
-
-    def forward(self, x, label, lamda):
-        """
-        Perform the forward pass of IVGD_model.
-
-        Args:
-
-        - x (torch.Tensor): Input tensor.
-
-        - label (torch.Tensor): Label tensor.
-
-        - lamda (float): Value of lambda parameter.
-
-        Returns:
-
-        - x (torch.Tensor): Output tensor after forward pass.
-        """
-        sum = torch.sum(label)
-        label = torch.cat((1 - label, label), dim=1)
-        x = torch.cat((1 - x, x), dim=1)
-        prob = x[:, 1].unsqueeze(-1)
-        x = (self.tau1 * self.net1(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho1 * (torch.sum(x) - sum) + self.alpha1 * x) / (
-                    self.tau1 + self.alpha1)
-        prob = x[:, 1].unsqueeze(-1)
-        lamda = lamda + self.rho1 * (torch.sum(prob) - sum)
-        x = (self.tau2 * self.net2(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho2 * (torch.sum(x) - sum) + self.alpha2 * x) / (
-                    self.tau2 + self.alpha2)
-        prob = x[:, 1].unsqueeze(-1)
-        lamda = lamda + self.rho2 * (torch.sum(prob) - sum)
-        x = (self.tau3 * self.net3(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho3 * (torch.sum(x) - sum) + self.alpha3 * x) / (
-                    self.tau3 + self.alpha3)
-        prob = x[:, 1].unsqueeze(-1)
-        lamda = lamda + self.rho3 * (torch.sum(prob) - sum)
-        x = (self.tau4 * self.net4(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho4 * (torch.sum(x) - sum) + self.alpha4 * x) / (
-                    self.tau4 + self.alpha4)
-        prob = x[:, 1].unsqueeze(-1)
-        lamda = lamda + self.rho4 * (torch.sum(prob) - sum)
-        x = (self.tau5 * self.net5(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho5 * (torch.sum(x) - sum) + self.alpha5 * x) / (
-                    self.tau5 + self.alpha5)
-        return x
-
-    def correction(self, pred):
-        """
-        Corrects predictions based on input.
-
-        Args:
-
-        - pred (torch.Tensor): Input tensor of predictions.
-
-        Returns:
-
-        - torch.Tensor: Corrected predictions.
-        """
-        temp = pred[:, 0].unsqueeze(-1)
-        return (self.net1(temp) + self.net2(temp) + self.net3(temp) + self.net4(temp) + self.net5(
-            temp)) / self.number_layer
-
-
-class IVGD:
-    """
-    Implement the Invertible Validity-aware Graph Diffusion (IVGD) model.
-
-    Wang, Junxiang, Junji Jiang, and Liang Zhao. "An invertible graph diffusion neural network for source localization." Proceedings of the ACM Web Conference 2022. 2022.
-    """
-
-    def __init__(self):
-        """
-        Initializes the IVGD model.
-        """
-
-    def train_diffusion(self, adj, train_dataset):
-        """
-        Train the diffusion model.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): Adjacency matrix of the graph.
-
-        - train_dataset (torch.utils.data.dataset.Subset): the training dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
-
-        Returns:
-
-        - diffusion_model (torch.nn.Module): Trained diffusion model.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.GNN.IVGD.main import IVGD
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        ivgd = IVGD()
-
-        diffusion_model = ivgd.train_diffusion(adj, train_dataset)
-
-        """
-        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-        num_node = adj.shape[0]
-        adj_coo = adj.tocoo()
-        values = adj_coo.data
-        indices = np.vstack((adj_coo.row, adj_coo.col))
-
-        i = torch.LongTensor(indices)
-        v = torch.FloatTensor(values)
-        shape = adj.shape
-
-        prob_matrix = torch.sparse.FloatTensor(i, v, torch.Size(shape)).to_dense()
-        prob_matrix = prob_matrix + torch.eye(n=prob_matrix.shape[0])
-        prob_matrix = prob_matrix/prob_matrix.sum(dim = 1,keepdims=True)
-        ndim = 5
-        niter = 2
-        propagate_model = DiffusionPropagate(prob_matrix, niter=niter)
-        fea_constructor = FeatureCons(ndim=ndim)
-        fea_constructor.prob_matrix = prob_matrix
-        args_dict = {
-            'learning_rate': 1e-8,
-            'λ': 0,
-            'γ': 0,
-            'idx_split_args': {'ntraining': int(num_node / 2), 'nstopping': int(num_node / 6),
-                               'nval': int(num_node / 3)},
-            'test': False,
-            'device': device,
-            'print_interval': 10
-        }
-        gnn_model = MLPTransform(input_dim=ndim, hiddenunits=[ndim, ndim], num_classes=1, device=device)
-        diffusion_model = i_DeepIS(gnn_model=gnn_model, propagate=propagate_model)
-        diffusion_model, result = train_model(diffusion_model, fea_constructor, prob_matrix, train_dataset, **args_dict)
-        print(f"train mean error:{result['train']['mean error']:.3f}")
-        print(f"early_stopping mean error:{result['early_stopping']['mean error']:.3f}")
-        print(f"validation mean error:{result['valtest']['mean error']:.3f}")
-        print(f"run time:{result['runtime']:.3f} seconds")
-        print(f"run time per epoch:{result['runtime_perepoch']:.3f} seconds")
-        return diffusion_model
-
-    def train(self, adj, train_dataset, diffusion_model, thres_list=[0.1, 0.3, 0.5, 0.7, 0.9],lr =1e-3, weight_decay = 1e-4, num_epoch = 10):
-        """
-        Train the IVGD model.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
-
-        - train_dataset (torch.utils.data.dataset.Subset): the training dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
-
-        - diffusion_model (torch.nn.Module): Trained diffusion model.
-
-        - thres_list (list): List of threshold values.
-
-        - lr (float): Learning rate.
-
-        - weight_decay (float): Weight decay.
-
-        - num_epoch (int): Number of epochs for training.
-
-        Returns:
-
-        - ivgd (torch.nn.Module): Trained IVGD model.
-
-        - opt_thres (float): Optimal threshold value.
-
-        - train_auc (float): Training AUC.
-
-        - opt_f1 (float): Optimal F1 score.
-
-        - pred (numpy.ndarray): Predicted seed vector of the training set, every column is the prediction of every simulation. It is used to adjust thres_list.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.GNN.IVGD.main import IVGD
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        ivgd = IVGD()
-
-        diffusion_model = ivgd.train_diffusion(adj, train_dataset)
-
-        ivgd_model, thres, auc, f1, pred =ivgd.train(adj, train_dataset, diffusion_model)
-
-        print("IVGD:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-
-        """
-        criterion = nn.CrossEntropyLoss()
-        #train_num = len(train_dataset)
-        num_node = adj.shape[0]
-        alpha = 1
-        tau = 1
-        rho = 1e-3
-        lamda = 0
-        ivgd = IVGD_model(alpha=alpha, tau=tau, rho=rho)
-        optimizer = optim.Adam(ivgd.parameters(), lr = lr, weight_decay = weight_decay)
-        ivgd.train()
-        train_num = len(train_dataset)
-        for i,influ_mat in enumerate(train_dataset):
-            seed_vec = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-            seed_preds = get_idx_new_seeds(diffusion_model, influ_vec)
-            seed_preds = seed_preds.unsqueeze(-1).float()
-            seed_vec = seed_vec.unsqueeze(-1).float()
-            for epoch in range(num_epoch):
-                optimizer.zero_grad()
-                seed_correction = ivgd(seed_preds, seed_vec, lamda)
-                loss = criterion(seed_correction, seed_vec.squeeze(-1).long())
-                loss.backward(retain_graph=True)
-                optimizer.step()
-            print(f"optimize simulation {i+1}: loss = {loss:.3f}")
-        
-        ivgd.eval()
-        train_auc = 0
-        for influ_mat in train_dataset:
-            seed_vec = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-            seed_preds = get_idx_new_seeds(diffusion_model, influ_vec)
-            seed_preds = torch.tensor(seed_preds).unsqueeze(-1).float()
-            seed_vec = seed_vec.unsqueeze(-1).float()
-            seed_correction = ivgd(seed_preds, seed_preds, lamda)
-            seed_correction = F.softmax(seed_correction, dim=1)
-            seed_correction = seed_correction[:, 1].unsqueeze(-1)
-            seed_correction = self.normalize(seed_correction)
-            seed_correction = seed_correction.squeeze(-1).detach().numpy()
-            seed_vec = seed_vec.detach().numpy()
-            train_auc += roc_auc_score(seed_vec, seed_correction)
-        train_auc = train_auc / train_num
-
-        pred = np.zeros((num_node,train_num))
-        seed_all = np.zeros((num_node,train_num))
-        for i,influ_mat in enumerate(train_dataset):
-            seed_all[:,i] = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-            seed_preds = get_idx_new_seeds(diffusion_model, influ_vec)
-            seed_preds = torch.tensor(seed_preds).unsqueeze(-1).float()
-            seed_correction = ivgd(seed_preds, seed_preds, lamda)
-            seed_correction = F.softmax(seed_correction, dim=1)
-            seed_correction = seed_correction[:, 1].unsqueeze(-1)
-            seed_correction = self.normalize(seed_correction)
-            seed_correction = seed_correction.squeeze(-1).detach().numpy()
-            pred[:,i] = seed_correction
-
-        opt_f1 = 0
-        opt_thres = 0
-        # Find optimal threshold and F1 score
-        for thres in thres_list:
-            train_f1 = 0
-            for i in range(train_num):
-                train_f1 += f1_score(seed_all[:,i], pred[:,i] >= thres)
-            train_f1 = train_f1 / train_num
-            print(f"thres = {thres:.3f}, train_f1 = {train_f1:.3f}")
-            if train_f1 > opt_f1:
-                opt_f1 = train_f1
-                opt_thres = thres
-
-
-        return ivgd, opt_thres, train_auc, opt_f1, pred
-
-    def test(self, test_dataset, diffusion_model, IVGD_model, thres):
-        """
-        Test the IVGD model on the given test dataset.
-
-        Args:
-
-        - test_dataset (torch.utils.data.dataset.Subset): the test dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
-
-        - diffusion_model (torch.nn.Module): Trained diffusion model.
-
-        - IVGD_model (torch.nn.Module): Trained IVGD model.
-
-        - thres (float): Threshold value.
-
-        Returns:
-
-        - metric (Metric): Object containing test metrics.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.GNN.IVGD.main import IVGD
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        ivgd = IVGD()
-
-        diffusion_model = ivgd.train_diffusion(adj, train_dataset)
-
-        ivgd_model, thres, auc, f1, pred =ivgd.train(adj, train_dataset, diffusion_model)
-
-        print("IVGD:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-
-        metric = ivgd.test(test_dataset, diffusion_model, ivgd_model, thres)
-
-        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-        """
-        test_num = len(test_dataset)
-        test_acc = 0
-        test_pr = 0
-        test_re = 0
-        test_f1 = 0
-        test_auc = 0
-
-        lamda = 0
-        # Loop through each test dataset
-        for influ_mat in test_dataset:
-            seed_vec = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-
-            # Get seed predictions from the diffusion model
-            seed_preds = get_idx_new_seeds(diffusion_model, influ_vec)
-            seed_preds = torch.tensor(seed_preds).unsqueeze(-1).float()
-            seed_vec = seed_vec.unsqueeze(-1).float()
-
-            # Obtain seed correction predictions from the IVGD model
-            seed_correction = IVGD_model(seed_preds, seed_preds, lamda)
-            seed_correction = F.softmax(seed_correction, dim=1)
-            seed_correction = seed_correction[:, 1].unsqueeze(-1)
-            seed_correction = self.normalize(seed_correction)
-            seed_correction = seed_correction.squeeze(-1).detach().numpy()
-            seed_vec = seed_vec.squeeze(-1).detach().numpy()
-
-            # Compute metrics
-            test_acc += accuracy_score(seed_vec, seed_correction >= thres)
-            test_pr += precision_score(seed_vec, seed_correction >= thres, zero_division = 1)
-            test_re += recall_score(seed_vec, seed_correction >= thres, zero_division = 1)
-            test_f1 += f1_score(seed_vec, seed_correction >= thres, zero_division = 1)
-            test_auc += roc_auc_score(seed_vec, seed_correction)
-
-        # Compute average metrics
-        test_acc = test_acc / test_num
-        test_pr = test_pr / test_num
-        test_re = test_re / test_num
-        test_f1 = test_f1 / test_num
-        test_auc = test_auc / test_num
-
-        # Create Metric object containing test metrics
-        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
-        return metric
-
-    def normalize(self, x):
-        """
-        The input tensor x is normalized to between 0 and 1.
-
-        Args:
-
-        - x (torch.Tensor): Input tensor to be normalized.
-
-        Returns:
-
-        - x (torch.Tensor): Normalized tensor.
-        """
-        # Compute minimum and maximum values along each dimension
-        min_vals, _ = torch.min(x, dim=0)
-        max_vals, _ = torch.max(x, dim=0)
-
-        # Compute the range and handle cases where the range is too small
-        rang = max_vals - min_vals
-        rang[torch.lt(rang, 1e-6)] = 1e-6
-
-        # Perform normalization
-        x = (x - min_vals) / rang
-        return x
+import torch.nn as nn
+import torch
+import torch.nn.functional as F
+import numpy as np
+from GraphSL.GNN.SLVAE.model import VAE,GNN,DiffusionPropagate
+from torch.optim import Adam
+from sklearn.metrics import roc_auc_score,f1_score,accuracy_score,precision_score,recall_score
+from GraphSL.Evaluation import Metric
+class SLVAE_model(nn.Module):
+    """
+    Source Localization Variational Autoencoder (SLVAE) model combining VAE, GNN, and propagation modules.
+
+    Attributes:
+    - vae (nn.Module): Variational Autoencoder module.
+
+    - gnn (nn.Module): Graph Neural Network module.
+
+    - propagate (nn.Module): Propagation module.
+
+    - reg_params (list): List of parameters requiring gradients.
+    """
+
+    def __init__(self, vae: nn.Module, gnn: nn.Module, propagate: nn.Module):
+        """
+        Initialize the SLVAE_model.
+
+        Args:
+        - vae (nn.Module): Variational Autoencoder module.
+
+        - gnn (nn.Module): Graph Neural Network module.
+
+        - propagate (nn.Module): Propagation module.
+        """
+        super(SLVAE_model, self).__init__()
+        self.vae = vae
+        self.gnn = gnn
+        self.propagate = propagate
+        self.reg_params = list(filter(lambda x: x.requires_grad, self.gnn.parameters()))
+
+    def forward(self, seed_vec, train_mode):
+        """
+        Forward pass method of the SLVAE model.
+
+        Args:
+
+        - seed_vec (torch.Tensor): Seed vector.
+
+        - train_mode (bool): Flag indicating whether in training mode.
+
+        Returns:
+
+        - seed_hat (torch.Tensor): reconstructed seed vector.
+
+        - mean (torch.Tensor): Mean of the VAE.
+
+        - log_var (torch.Tensor): Log variance of the VAE.
+
+        - predictions (torch.Tensor): Predictions made by the SLVAE model.
+        """
+        # Pass seed_vec through VAE to obtain reconstructed seed vector, mean, and log variance
+        seed_hat, mean, log_var = self.vae(seed_vec)
+
+        if train_mode:
+            # Ensure values of seed_hat are within range [0, 1]
+            seed_hat.clamp(0, 1)
+            # Pass seed_hat through GNN and perform propagation
+            predictions = self.gnn(seed_hat)
+            predictions = self.propagate(predictions)
+        else:
+            # Ensure values of seed_vec are within range [0, 1]
+            seed_vec.clamp(0, 1)
+            # Pass seed_vec through GNN and perform propagation
+            predictions = self.gnn(seed_vec)
+            predictions = self.propagate(predictions)
+
+        predictions = torch.transpose(predictions, 0, 1)
+
+        # Return reconstructed seed vector, mean, log variance, and predictions
+        return seed_hat, mean, log_var, predictions
+
+    def train_loss(self, x, x_hat, mean, log_var, y, y_hat):
+        """
+        Compute training loss.
+
+        Args:
+
+        - x (torch.Tensor): Seed vector.
+
+        - x_hat (torch.Tensor): Reconstructed seed tensor.
+
+        - mean (torch.Tensor): Mean of the VAE.
+
+        - log_var (torch.Tensor): Log variance of the VAE.
+
+        - y (torch.Tensor): Diffusion vector.
+
+        - y_hat (torch.Tensor): Predicted Diffusion vector.
+
+        Returns:
+
+        - total_loss (torch.Tensor): Total loss is the sum of prediction loss, reconstruction loss and KL divergence.
+        """
+        forward_loss = F.mse_loss(y_hat, y)
+        reproduction_loss = F.binary_cross_entropy(x_hat, x, reduction='mean')
+        KLD = -0.5 * torch.sum(1 + log_var - mean.pow(2) - log_var.exp())
+        total_loss = forward_loss + reproduction_loss + KLD
+        return total_loss
+
+    def infer_loss(self, y_true, y_hat, x_hat, train_pred):
+        """
+        Compute inference loss.
+
+        Args:
+
+        - y_true (torch.Tensor): True label tensor.
+
+        - y_hat (torch.Tensor): Predicted label tensor.
+
+        - x_hat (torch.Tensor): Reconstructed input tensor.
+
+        - train_pred (torch.Tensor): Predicted tensor during training.
+
+        Returns:
+
+        - total_loss (torch.Tensor): Total loss tensor.
+        """
+        device = y_true.device
+        BN = nn.BatchNorm1d(1, affine=False).to(device)
+        forward_loss = F.mse_loss(y_hat, y_true)
+        log_pmf = []
+        for pred in train_pred:
+            log_lh = torch.zeros(1).to(device)
+            for i, x_i in enumerate(x_hat[0]):
+                temp = x_i * torch.log(pred[i]) + (1 - x_i) * torch.log(1 - pred[i]).to(torch.double)
+                log_lh += temp
+            log_pmf.append(log_lh)
+
+        log_pmf = torch.stack(log_pmf)
+        log_pmf = BN(log_pmf.float())
+
+        pmf_max = torch.max(log_pmf)
+
+        pdf_sum = pmf_max + torch.logsumexp(log_pmf - pmf_max, dim=0)
+
+        total_loss = forward_loss - pdf_sum
+
+        return total_loss
+
+class SLVAE:
+    """
+    Implement the Source Localization Variational Autoencoder (SLVAE) model.
+
+    Ling C, Jiang J, Wang J, et al. Source localization of graph diffusion via variational autoencoders for graph inverse problems[C]//Proceedings of the 28th ACM SIGKDD conference on knowledge discovery and data mining. 2022: 1010-1020.
+    """
+
+    def __init__(self):
+        """
+        Initialize the SLVAE model.
+        """
+
+    def train(self, adj, train_dataset, thres_list=[0.1, 0.3, 0.5, 0.7, 0.9], lr = 1e-3, weight_decay = 1e-4, num_epoch = 50,print_epoch =10):
+        """
+        Train the SLVAE model.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
+
+        - train_dataset (torch.utils.data.dataset.Subset): the training dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
+
+        - thres_list (list): List of threshold values to try.
+
+        - lr (float): Learning rate.
+
+        - weight_decay (float): Weight decay.
+
+        - num_epoch (int): Number of training epochs.
+
+        - print_epoch (int): Number of epochs every time to print loss.
+
+        Returns:
+
+        - slvae_model (SLVAE_model): Trained SLVAE model.
+
+        - seed_vae_train (torch.Tensor): The latent representations of training seed vector from VAE, which is used to initialize seed vector in the test set.
+
+        - opt_thres (float): Optimal threshold.
+
+        - train_auc (float): Train AUC.
+
+        - opt_f1 (float): Optimal F1 score.
+
+        - pred (numpy.ndarray): Predicted seed vector of the training set, every column is the prediction of every simulation. It is used to adjust thres_list.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.GNN.SLVAE.main import SLVAE
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        slave = SLVAE()
+
+        slvae_model, seed_vae_train, thres, auc, f1, pred = slave.train(adj, train_dataset)
+
+        print("SLVAE:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+        """
+        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+        num_node = adj.shape[0]
+        adj_coo = adj.tocoo()
+        values = adj_coo.data
+        indices = np.vstack((adj_coo.row, adj_coo.col))
+
+        i = torch.LongTensor(indices)
+        v = torch.FloatTensor(values)
+        shape = adj.shape
+
+        adj_matrix = torch.sparse_coo_tensor(i, v, torch.Size(shape)).to_dense()
+        train_num = len(train_dataset)
+        vae = VAE().to(device)
+        gnn = GNN(adj_matrix=adj_matrix)
+        propagate = DiffusionPropagate(adj_matrix, niter=2)
+
+        slvae_model = SLVAE_model(vae, gnn, propagate).to(device)
+
+        optimizer = Adam(slvae_model.parameters(), lr=lr)
+
+        # Train SLVAE
+        print("train SLVAE:")
+        slvae_model.train()
+        for epoch in range(num_epoch):
+            overall_loss = 0
+            for influ_mat in train_dataset:
+                seed_vec = influ_mat[:, 0]
+                influ_vec = influ_mat[:, -1]
+                influ_vec = influ_vec.unsqueeze(-1).float()
+                seed_vec = seed_vec.unsqueeze(-1).float()
+                optimizer.zero_grad()
+                seed_vec_hat, mean, log_var, influ_vec_hat = slvae_model(seed_vec, True)
+                loss = slvae_model.train_loss(seed_vec, seed_vec_hat, mean, log_var, influ_vec, influ_vec_hat)
+
+                overall_loss += loss.item()
+
+                loss.backward()
+                optimizer.step()
+            average_loss = overall_loss/train_num
+            if epoch % print_epoch == 0:
+                print(f"epoch = {epoch}, loss = {average_loss:.3f}")
+
+        # Evaluation
+        print("infer seed from training set:")
+
+        slvae_model.eval()
+        for param in slvae_model.parameters():
+            param.requires_grad = False
+
+        seed_vae_train = torch.zeros(size=(train_num, num_node))
+        for i, influ_mat in enumerate(train_dataset):
+            seed_vec = influ_mat[:, 0].unsqueeze(-1).float()
+            seed_vae_train[i, :] = slvae_model.vae(seed_vec)[0].squeeze(-1)
+        seed_infer = []
+        seed_vae_mean = torch.mean(seed_vae_train, 0).unsqueeze(-1).to(device)
+        for i in range(train_num):
+            seed_vec_hat, _, _, influ_vec_hat = slvae_model(seed_vae_mean, False)
+            seed_infer.append(seed_vec_hat)
+
+        for seed in seed_infer:
+            seed.requires_grad = True
+
+        optimizer = Adam(seed_infer, lr = lr, weight_decay = weight_decay)
+
+        for epoch in range(num_epoch):
+            overall_loss = 0
+            for i, influ_mat in enumerate(train_dataset):
+                influ_vec = influ_mat[:, -1]
+                influ_vec = influ_vec.unsqueeze(-1).float()
+                optimizer.zero_grad()
+                seed_vec_hat, _, _, influ_vec_hat = slvae_model(seed_infer[i], False)
+                loss = slvae_model.infer_loss(influ_vec, influ_vec_hat, seed_vec_hat, seed_vae_train)
+
+                overall_loss += loss.item()
+
+                loss.backward()
+                optimizer.step()
+            
+            average_loss = overall_loss/train_num
+
+
+            if epoch % print_epoch ==0:
+                print(f"epoch = {epoch}, obj = {average_loss:.4f}")
+
+        train_auc = 0
+        for i, influ_mat in enumerate(train_dataset):
+            seed_vec = influ_mat[:, 0]
+            seed_vec = seed_vec.squeeze(-1).detach().numpy()
+            seed_pred = seed_infer[i].detach().numpy()
+            train_auc += roc_auc_score(seed_vec, seed_pred)
+        train_auc = train_auc / train_num
+
+        opt_f1 = 0
+        opt_thres = 0
+        for thres in thres_list:
+            train_f1 = 0
+            for i, influ_mat in enumerate(train_dataset):
+                seed_vec = influ_mat[:, 0]
+                seed_vec = seed_vec.squeeze(-1).detach().numpy()
+                seed_pred = seed_infer[i].detach().numpy()
+                train_f1 += f1_score(seed_vec, seed_pred >= thres, zero_division = 1)
+            train_f1 = train_f1 / train_num
+            print(f"thres = {thres:.3f}, train_f1 = {train_f1:.3f}")
+            if train_f1 > opt_f1:
+                opt_f1 = train_f1
+                opt_thres = thres
+        
+        pred = np.zeros((num_node,train_num))
+
+        for i in range(train_num):
+            pred[:,i] = seed_infer[i].squeeze(-1).detach().numpy()
+
+
+        return slvae_model, seed_vae_train, opt_thres, train_auc, opt_f1, pred
+
+    def infer(self, test_dataset, slvae_model, seed_vae_train, thres, lr=0.001,num_epoch = 50, print_epoch = 10):
+        """
+        Infer using the SLVAE model.
+
+        Args:
+
+        - test_dataset (torch.utils.data.dataset.Subset): the test dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
+
+        - slvae_model (SLVAE_model): Trained SLVAE model.
+
+        - seed_vae_train (torch.Tensor): The latent representations of training seed vector from VAE, which is used to initialize
+          seed vector in the test set.
+
+        - thres (float): Threshold value.
+
+        - lr (float): Learning rate.
+
+        - num_epoch (int): Number of epochs.
+
+        - print_epoch (int): Number of epochs every time to print loss.
+
+
+        Returns:
+
+        - Metric: Evaluation metric containing accuracy, precision, recall, F1 score, and AUC.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.GNN.SLVAE.main import SLVAE
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        slave = SLVAE()
+
+        slvae_model, seed_vae_train, thres, auc, f1, pred = slave.train(adj, train_dataset)
+
+        print("SLVAE:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+
+        metric = slave.infer(test_dataset, slvae_model, seed_vae_train, thres)
+
+        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+        """
+        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+        test_num = len(test_dataset)
+        slvae_model.eval()
+        for param in slvae_model.parameters():
+            param.requires_grad = False
+
+        seed_infer = []
+        seed_mean = torch.mean(seed_vae_train, 0).unsqueeze(-1).to(device)
+        for i in range(test_num):
+            seed_vec_hat, _, _, influ_vec_hat = slvae_model(seed_mean, False)
+            seed_infer.append(seed_vec_hat)
+
+        for seed in seed_infer:
+            seed.requires_grad = True
+
+        optimizer = Adam(seed_infer, lr=lr)
+
+        print("infer seed from test set:")
+        for epoch in range(num_epoch):
+            overall_loss = 0
+            for i, influ_mat in enumerate(test_dataset):
+                influ_vec = influ_mat[:, -1]
+                influ_vec = influ_vec.unsqueeze(-1).float()
+                optimizer.zero_grad()
+                seed_vec_hat, _, _, influ_vec_hat = slvae_model(seed_infer[i], False)
+                loss = slvae_model.infer_loss(influ_vec, influ_vec_hat, seed_vec_hat, seed_vae_train)
+
+                overall_loss += loss.item()
+
+                average_loss = overall_loss / test_num
+
+                loss.backward()
+                optimizer.step()
+
+            
+            if epoch % print_epoch == 0:
+                print(f"epoch = {epoch}, obj = {average_loss:.4f}")
+
+        test_acc = 0
+        test_pr = 0
+        test_re = 0
+        test_f1 = 0
+        test_auc = 0
+
+        for i, influ_mat in enumerate(test_dataset):
+            seed_vec = influ_mat[:, 0]
+            seed_vec = seed_vec.squeeze(-1).detach().numpy()
+            seed_pred = seed_infer[i].detach().numpy()
+            test_acc += accuracy_score(seed_vec, seed_pred >= thres)
+            test_pr += precision_score(seed_vec, seed_pred >= thres, zero_division = 1)
+            test_re += recall_score(seed_vec, seed_pred >= thres, zero_division = 1)
+            test_f1 += f1_score(seed_vec, seed_pred >= thres, zero_division = 1)
+            test_auc += roc_auc_score(seed_vec, seed_pred)
+
+        test_acc = test_acc / test_num
+        test_pr = test_pr / test_num
+        test_re = test_re / test_num
+        test_f1 = test_f1 / test_num
+        test_auc = test_auc / test_num
+
+        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
+        return metric
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `GraphSL-0.8/GraphSL/GNN/IVGD/model/MLP.py` & `GraphSL-0.9/GraphSL/GNN/IVGD/model/MLP.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import torch
-import torch.nn as nn
-from typing import List
-from torch.nn.functional import normalize
-
-class MLPTransform(nn.Module):
-    def __init__(self, 
-                input_dim,
-                hiddenunits: List[int],
-                num_classes,
-                bias=True,
-                drop_prob=0.5,n_power_iterations=10,eps=1e-12,coeff=0.9,device='cuda'):
-        super(MLPTransform, self).__init__()
-        # Here features is just a placeholder, each time before forward, we will substutute the embedding layer with desired node feature matrix
-        # and when saving model params, we will first pop self.features.weight
-        self.features = None
-
-        fcs = [nn.Linear(input_dim, hiddenunits[0], bias=bias)]
-        for i in range(1, len(hiddenunits)):
-            fcs.append(nn.Linear(hiddenunits[i-1], hiddenunits[i]))
-        fcs.append(nn.Linear(hiddenunits[-1], num_classes))
-
-        self.fcs = nn.ModuleList(fcs)
-
-        if drop_prob is 0:
-            self.dropout = lambda x: x
-        else:
-            self.dropout = nn.Dropout(drop_prob)
-        self.act_fn = nn.ReLU()
-        self.n_power_iterations =n_power_iterations
-        self.eps = eps
-        self.coeff = coeff
-        self.device=device
-
-    def forward(self, nodes: torch.LongTensor):
-        # ipdb.set_trace()
-        layer_inner = self.act_fn(self.fcs[0](self.dropout(self.features(nodes))))
-        for fc in self.fcs[1:-1]:
-            weight =self.compute_weight(fc)
-            fc.weight.data.copy_(weight)
-            layer_inner = self.act_fn(fc(layer_inner))
-
-        res = torch.sigmoid( self.fcs[-1](self.dropout(layer_inner)) )
-        return res
-    def compute_weight(self, module):
-        # NB: If `do_power_iteration` is set, the `u` and `v` vectors are
-        #     updated in power iteration **in-place**. This is very important
-        #     because in `DataParallel` forward, the vectors (being buffers) are
-        #     broadcast from the parallelized module to each module replica,
-        #     which is a new module object created on the fly. And each replica
-        #     runs its own spectral norm power iteration. So simply assigning
-        #     the updated vectors to the module this function runs on will cause
-        #     the update to be lost forever. And the next time the parallelized
-        #     module is replicated, the same randomly initialized vectors are
-        #     broadcast and used!
-        #
-        #     Therefore, to make the change propagate back, we rely on two
-        #     important bahaviors (also enforced via tests):
-        #       1. `DataParallel` doesn't clone storage if the broadcast tensor
-        #          is alreay on correct device; and it makes sure that the
-        #          parallelized module is already on `device[0]`.
-        #       2. If the out tensor in `out=` kwarg has correct shape, it will
-        #          just fill in the values.
-        #     Therefore, since the same power iteration is performed on all
-        #     devices, simply updating the tensors in-place will make sure that
-        #     the module replica on `device[0]` will update the _u vector on the
-        #     parallized module (by shared storage).
-        #
-        #    However, after we update `u` and `v` in-place, we need to **clone**
-        #    them before using them to normalize the weight. This is to support
-        #    backproping through two forward passes, e.g., the common pattern in
-        #    GAN training: loss = D(real) - D(fake). Otherwise, engine will
-        #    complain that variables needed to do backward for the first forward
-        #    (i.e., the `u` and `v` vectors) are changed in the second forward.
-        weight = module.weight.clone()
-        u = torch.rand(weight.shape[0],device=self.device)
-        v = torch.rand(weight.shape[0],device=self.device)
-        with torch.no_grad():
-            for _ in range(self.n_power_iterations):
-                # Spectral norm of weight equals to `u^T W v`, where `u` and `v`
-                # are the first left and right singular vectors.
-                # This power iteration produces approximations of `u` and `v`.
-                v = normalize(torch.mv(weight.t(), u), dim=0, eps=self.eps, out=v)
-                u = normalize(torch.mv(weight, v), dim=0, eps=self.eps, out=u)
-            if self.n_power_iterations > 0:
-                # See above on why we need to clone
-                u = u.clone()
-                v = v.clone()
-
-        sigma = torch.dot(u, torch.mv(weight, v))
-        # soft normalization: only when sigma larger than coeff
-        factor = torch.max(torch.ones(1).to(weight.device), sigma / self.coeff)
-        weight = weight / factor
-
-        return weight
-
-
+import torch
+import torch.nn as nn
+from typing import List
+from torch.nn.functional import normalize
+
+class MLPTransform(nn.Module):
+    def __init__(self, 
+                input_dim,
+                hiddenunits: List[int],
+                num_classes,
+                bias=True,
+                drop_prob=0.5,n_power_iterations=10,eps=1e-12,coeff=0.9,device='cuda'):
+        super(MLPTransform, self).__init__()
+        # Here features is just a placeholder, each time before forward, we will substutute the embedding layer with desired node feature matrix
+        # and when saving model params, we will first pop self.features.weight
+        self.features = None
+
+        fcs = [nn.Linear(input_dim, hiddenunits[0], bias=bias)]
+        for i in range(1, len(hiddenunits)):
+            fcs.append(nn.Linear(hiddenunits[i-1], hiddenunits[i]))
+        fcs.append(nn.Linear(hiddenunits[-1], num_classes))
+
+        self.fcs = nn.ModuleList(fcs)
+
+        if drop_prob is 0:
+            self.dropout = lambda x: x
+        else:
+            self.dropout = nn.Dropout(drop_prob)
+        self.act_fn = nn.ReLU()
+        self.n_power_iterations =n_power_iterations
+        self.eps = eps
+        self.coeff = coeff
+        self.device=device
+
+    def forward(self, nodes: torch.LongTensor):
+        # ipdb.set_trace()
+        layer_inner = self.act_fn(self.fcs[0](self.dropout(self.features(nodes))))
+        for fc in self.fcs[1:-1]:
+            weight =self.compute_weight(fc)
+            fc.weight.data.copy_(weight)
+            layer_inner = self.act_fn(fc(layer_inner))
+
+        res = torch.sigmoid( self.fcs[-1](self.dropout(layer_inner)) )
+        return res
+    def compute_weight(self, module):
+        # NB: If `do_power_iteration` is set, the `u` and `v` vectors are
+        #     updated in power iteration **in-place**. This is very important
+        #     because in `DataParallel` forward, the vectors (being buffers) are
+        #     broadcast from the parallelized module to each module replica,
+        #     which is a new module object created on the fly. And each replica
+        #     runs its own spectral norm power iteration. So simply assigning
+        #     the updated vectors to the module this function runs on will cause
+        #     the update to be lost forever. And the next time the parallelized
+        #     module is replicated, the same randomly initialized vectors are
+        #     broadcast and used!
+        #
+        #     Therefore, to make the change propagate back, we rely on two
+        #     important bahaviors (also enforced via tests):
+        #       1. `DataParallel` doesn't clone storage if the broadcast tensor
+        #          is alreay on correct device; and it makes sure that the
+        #          parallelized module is already on `device[0]`.
+        #       2. If the out tensor in `out=` kwarg has correct shape, it will
+        #          just fill in the values.
+        #     Therefore, since the same power iteration is performed on all
+        #     devices, simply updating the tensors in-place will make sure that
+        #     the module replica on `device[0]` will update the _u vector on the
+        #     parallized module (by shared storage).
+        #
+        #    However, after we update `u` and `v` in-place, we need to **clone**
+        #    them before using them to normalize the weight. This is to support
+        #    backproping through two forward passes, e.g., the common pattern in
+        #    GAN training: loss = D(real) - D(fake). Otherwise, engine will
+        #    complain that variables needed to do backward for the first forward
+        #    (i.e., the `u` and `v` vectors) are changed in the second forward.
+        weight = module.weight.clone()
+        u = torch.rand(weight.shape[0],device=self.device)
+        v = torch.rand(weight.shape[0],device=self.device)
+        with torch.no_grad():
+            for _ in range(self.n_power_iterations):
+                # Spectral norm of weight equals to `u^T W v`, where `u` and `v`
+                # are the first left and right singular vectors.
+                # This power iteration produces approximations of `u` and `v`.
+                v = normalize(torch.mv(weight.t(), u), dim=0, eps=self.eps, out=v)
+                u = normalize(torch.mv(weight, v), dim=0, eps=self.eps, out=u)
+            if self.n_power_iterations > 0:
+                # See above on why we need to clone
+                u = u.clone()
+                v = v.clone()
+
+        sigma = torch.dot(u, torch.mv(weight, v))
+        # soft normalization: only when sigma larger than coeff
+        factor = torch.max(torch.ones(1).to(weight.device), sigma / self.coeff)
+        weight = weight / factor
+
+        return weight
+
+
```

### Comparing `GraphSL-0.8/GraphSL/GNN/IVGD/preprocessing.py` & `GraphSL-0.9/GraphSL/GNN/IVGD/preprocessing.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from typing import List
-import numpy as np
-import scipy.sparse as sp
-import scipy.sparse.linalg as spla
-
-
-def gen_seeds(size: int = None) -> np.ndarray:
-    """
-    Generate an array of random seeds.
-
-    Args:
-
-    - size (int, optional): Size of the array to generate. If None, a single random seed is returned.
-
-    Returns:
-
-    - np.ndarray: Array of random seeds.
-    """
-    max_uint32 = np.iinfo(np.uint32).max
-    return np.random.randint(max_uint32 + 1, size=size, dtype=np.uint32)
-
-
-def exclude_idx(idx: np.ndarray, idx_exclude_list: List[np.ndarray]) -> np.ndarray:
-    """
-    Exclude indices from a given array based on a list of arrays containing indices to exclude.
-
-    Args:
-
-    - idx (np.ndarray): Array of indices.
-
-    - idx_exclude_list (List[np.ndarray]): List of arrays containing indices to exclude.
-
-    Returns:
-
-    - np.ndarray: Array of indices after exclusion.
-    """
-    idx_exclude = np.concatenate(idx_exclude_list)
-    return np.array([i for i in idx if i not in idx_exclude])
-
-
-def gen_splits_(array, train_size, stopping_size, val_size):
-    """
-    Generate train, stopping, and validation indices splits from a given array.
-
-    Args:
-
-    - array: Array of indices.
-
-    - train_size (int): Size of the training split.
-
-    - stopping_size (int): Size of the stopping split.
-
-    - val_size (int): Size of the validation split.
-
-    Returns:
-
-    - train_idx (numpy.ndarray): Train indices splits.
-
-    - stopping_idx (numpy.ndarray): Stopping indices splits.
-
-    - val_idx (numpy.ndarray): Validation indices splits.
-
-    """
-    assert train_size + stopping_size + val_size <= len(array), 'length error'
-    from sklearn.model_selection import train_test_split
-    train_idx, tmp = train_test_split(array, train_size=train_size, test_size=stopping_size + val_size)
-    stopping_idx, val_idx = train_test_split(tmp, train_size=stopping_size, test_size=val_size)
-
-    return train_idx, stopping_idx, val_idx
-
-
-def normalize_attributes(attr_matrix):
-    """
-    Normalize attributes in a matrix.
-
-    Args:
-
-    - attr_matrix: Matrix containing attributes to normalize.
-
-    Returns:
-
-    - attr_mat_norm (np.ndarray): Normalized attribute matrix.
-    """
-    epsilon = 1e-12
-    if isinstance(attr_matrix, sp.csr_matrix):
-        attr_norms = spla.norm(attr_matrix, ord=1, axis=1)
-        attr_invnorms = 1 / np.maximum(attr_norms, epsilon)
-        attr_mat_norm = attr_matrix.multiply(attr_invnorms[:, np.newaxis])
-    else:
-        attr_norms = np.linalg.norm(attr_matrix, ord=1, axis=1)
-        attr_invnorms = 1 / np.maximum(attr_norms, epsilon)
-        attr_mat_norm = attr_matrix * attr_invnorms[:, np.newaxis]
-    return attr_mat_norm
-
+from typing import List
+import numpy as np
+import scipy.sparse as sp
+import scipy.sparse.linalg as spla
+
+
+def gen_seeds(size: int = None) -> np.ndarray:
+    """
+    Generate an array of random seeds.
+
+    Args:
+
+    - size (int, optional): Size of the array to generate. If None, a single random seed is returned.
+
+    Returns:
+
+    - np.ndarray: Array of random seeds.
+    """
+    max_uint32 = np.iinfo(np.uint32).max
+    return np.random.randint(max_uint32 + 1, size=size, dtype=np.uint32)
+
+
+def exclude_idx(idx: np.ndarray, idx_exclude_list: List[np.ndarray]) -> np.ndarray:
+    """
+    Exclude indices from a given array based on a list of arrays containing indices to exclude.
+
+    Args:
+
+    - idx (np.ndarray): Array of indices.
+
+    - idx_exclude_list (List[np.ndarray]): List of arrays containing indices to exclude.
+
+    Returns:
+
+    - np.ndarray: Array of indices after exclusion.
+    """
+    idx_exclude = np.concatenate(idx_exclude_list)
+    return np.array([i for i in idx if i not in idx_exclude])
+
+
+def gen_splits_(array, train_size, stopping_size, val_size):
+    """
+    Generate train, stopping, and validation indices splits from a given array.
+
+    Args:
+
+    - array: Array of indices.
+
+    - train_size (int): Size of the training split.
+
+    - stopping_size (int): Size of the stopping split.
+
+    - val_size (int): Size of the validation split.
+
+    Returns:
+
+    - train_idx (numpy.ndarray): Train indices splits.
+
+    - stopping_idx (numpy.ndarray): Stopping indices splits.
+
+    - val_idx (numpy.ndarray): Validation indices splits.
+
+    """
+    assert train_size + stopping_size + val_size <= len(array), 'length error'
+    from sklearn.model_selection import train_test_split
+    train_idx, tmp = train_test_split(array, train_size=train_size, test_size=stopping_size + val_size)
+    stopping_idx, val_idx = train_test_split(tmp, train_size=stopping_size, test_size=val_size)
+
+    return train_idx, stopping_idx, val_idx
+
+
+def normalize_attributes(attr_matrix):
+    """
+    Normalize attributes in a matrix.
+
+    Args:
+
+    - attr_matrix: Matrix containing attributes to normalize.
+
+    Returns:
+
+    - attr_mat_norm (np.ndarray): Normalized attribute matrix.
+    """
+    epsilon = 1e-12
+    if isinstance(attr_matrix, sp.csr_matrix):
+        attr_norms = spla.norm(attr_matrix, ord=1, axis=1)
+        attr_invnorms = 1 / np.maximum(attr_norms, epsilon)
+        attr_mat_norm = attr_matrix.multiply(attr_invnorms[:, np.newaxis])
+    else:
+        attr_norms = np.linalg.norm(attr_matrix, ord=1, axis=1)
+        attr_invnorms = 1 / np.maximum(attr_norms, epsilon)
+        attr_mat_norm = attr_matrix * attr_invnorms[:, np.newaxis]
+    return attr_mat_norm
+
```

### Comparing `GraphSL-0.8/GraphSL/GNN/IVGD/training.py` & `GraphSL-0.9/GraphSL/GNN/IVGD/training.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,483 +1,483 @@
-from typing import  Tuple
-import time
-import numpy as np
-import torch
-import torch.nn as nn
-from torch.utils.data import TensorDataset, DataLoader
-import scipy.sparse as sp
-import sys
-sys.path.append('../../')
-from .preprocessing import gen_seeds, gen_splits_
-from .earlystopping import EarlyStopping, stopping_args
-
-class FeatureCons:
-    """
-    Initial feature constructor for different models.
-    """
-
-    def __init__(self, ndim=None):
-        """
-        Initialize FeatureCons object.
-
-        Args:
-
-        - ndim (int): Number of dimensions.
-        """
-        self.prob_matrix = None
-        self.ndim = ndim
-
-    def __deepis_fea(self, seed_vec):
-        """
-        Deeply compute features based on the given seed vector.
-
-        Args:
-
-        - seed_vec (torch.Tensor): Seed vector.
-
-        Returns:
-
-        - attr_mat(numpy.ndarray): Feature matrix.
-        """
-        seed_vec = seed_vec.reshape((-1, 1))
-        import scipy.sparse as sp
-        if sp.isspmatrix(self.prob_matrix):
-            self.prob_matrix = self.prob_matrix.toarray()
-        assert seed_vec.shape[0] == self.prob_matrix.shape[0], 'Seed vector is illegal'
-        attr_mat = [seed_vec]
-        for i in range(self.ndim - 1):
-            attr_mat.append(self.prob_matrix.T @ attr_mat[(-1)])
-
-        attr_mat = np.concatenate(attr_mat, axis=(-1))
-        return attr_mat
-
-    def __call__(self, seed_vec):
-        """
-        Call method to compute features based on the given seed vector.
-
-        Args:
-
-        - seed_vec (torch.Tensor): Seed vector.
-
-        Returns:
-
-        - numpy.ndarray: Feature matrix.
-        """
-        return self.__deepis_fea(seed_vec)
-
-
-def get_dataloaders(idx, labels_np, batch_size=None):
-    """
-    Get data loaders for training, validation, and testing.
-
-    Args:
-
-    - idx (dict): Dictionary containing indices for different phases, training, early stopping, and validation/test.
-
-    - labels_np (numpy.ndarray): Labels as numpy array.
-
-    - batch_size (int): Batch size.
-
-    Returns:
-
-    - dataloaders (dict): Dictionary containing data loaders for different phases.
-    """
-    labels = torch.FloatTensor(labels_np)
-    if batch_size is None:
-        batch_size = max((val.numel() for val in idx.values()))
-    datasets = {phase: TensorDataset(torch.LongTensor(ind), labels[ind]) for phase, ind in idx.items()}
-    dataloaders = {phase: DataLoader(dataset=dataset, batch_size=batch_size, shuffle=True) for phase, dataset in
-                   datasets.items()}
-    return dataloaders
-
-
-def construct_attr_mat(prob_matrix, seed_vec, order=5):
-    """
-    Construct attribute matrix based on the given probability matrix and seed vector.
-
-    Args:
-
-    - prob_matrix (scipy.sparse.csr_matrix): Probability matrix.
-
-    - seed_vec (numpy.ndarray): Seed vector.
-
-    - order (int): Order of attribute matrix construction.
-
-    Returns:
-
-    - attr_mat (numpy.ndarray): Attribute matrix.
-    """
-    lanczos_flag = False
-    if lanczos_flag:
-        return lanczos_algo(prob_matrix, seed_vec, order)
-    seed_vec = seed_vec.reshape((-1, 1))
-    assert seed_vec.shape[0] == prob_matrix.shape[0]
-    attr_mat = [seed_vec]
-    if sp.isspmatrix(prob_matrix):
-        prob_matrix = prob_matrix.toarray()
-    for i in range(1, order + 1):
-        attr_mat.append(prob_matrix.T @ attr_mat[(-1)])
-
-    attr_mat = np.concatenate(attr_mat, axis=(-1))
-    return attr_mat
-
-
-def lanczos_algo(prob_matrix, seed_vec, order=5, epsilon=0.001):
-    """
-    Lanczos algorithm for computing attribute matrix.
-
-    Args:
-
-    - prob_matrix (numpy.ndarray or scipy.sparse.csr_matrix): Probability matrix.
-
-    - seed_vec (numpy.ndarray): Seed vector.
-
-    - order (int): Order of attribute matrix construction.
-
-    - epsilon (float): Threshold for stopping the iteration.
-
-    Returns:
-
-    - numpy.ndarray: Attribute matrix.
-    """
-    S = prob_matrix.T
-    seed_vec = seed_vec.flatten()
-    beta = np.zeros((order + 1,))
-    gamma = np.zeros((order + 1,))
-    q = [np.zeros((len(seed_vec),)), seed_vec / np.linalg.norm(seed_vec, ord=2)]
-    for j in range(1, order + 1):
-        z = S @ q[j]
-        gamma[j] = q[j].reshape((1, -1)) @ z
-        z = z - gamma[j] * q[j] - beta[(j - 1)] * q[(j - 1)]
-        beta[j] = np.linalg.norm(z, ord=2)
-        if beta[j] < epsilon:
-            break
-        q.append(z / beta[j])
-
-    q = q[1:]
-    q = np.array(q).T
-    return q
-
-
-def update_embedding(model, feature_mat):
-    """
-    Update the embedding layer of the model with the new feature matrix.
-
-    Args:
-
-    - model (torch.nn.Module): Model.
-
-    - feature_mat (numpy.ndarray): Feature matrix.
-
-    Returns:
-
-    - torch.nn.Module: Updated model.
-    """
-    assert getattr(model, 'gnn_model', None) is not None, 'Object model should have a submodule `gnn_model` '
-    device = next(model.parameters()).device
-    if model.gnn_model.features is None:
-        new_embedding_layer = nn.Embedding(feature_mat.shape[0], feature_mat.shape[1])
-        new_embedding_layer.weight = nn.Parameter(torch.FloatTensor(feature_mat), requires_grad=False)
-        model.gnn_model.features = new_embedding_layer
-    else:
-        assert feature_mat.shape[1] == model.gnn_model.features.weight.shape[1], \
-            'New dimension of new embedding weights is not consistent with the old dimension'
-        model.gnn_model.features.weight = nn.Parameter(torch.FloatTensor(feature_mat), requires_grad=False)
-        model.gnn_model.features.num_embeddings = feature_mat.shape[0]
-        model.gnn_model.features.embedding_dim = feature_mat.shape[1]
-    model = model.to(device)
-    return model
-
-
-def PIteration(prob_matrix, predictions, seed_idx, substitute=True, piter=10):
-    """
-    Perform final prediction iteration to fit the ideal equation system.
-
-    Args:
-
-    - prob_matrix (numpy.ndarray): Probability matrix.
-
-    - predictions (numpy.ndarray): Predictions.
-
-    - seed_idx (numpy.ndarray): Seed indices.
-
-    - substitute (bool): Whether to substitute seed indices.
-
-    - piter (int): Number of iterations.
-
-    Returns:
-
-    - final_preds (numpy.ndarray): Final predictions.
-    """
-
-    def one_iter(prob_matrix, predictions):
-        P2 = np.multiply(prob_matrix.T, np.broadcast_to(predictions.reshape((1, -1)), prob_matrix.shape))
-        P3 = np.ones(prob_matrix.shape) - P2
-        one_iter_preds = np.ones((prob_matrix.shape[0],)) - np.prod(P3, axis=1).flatten()
-        return one_iter_preds
-
-    # predictions = predictions.flatten()
-    assert prob_matrix.shape[0] == prob_matrix.shape[1]
-    assert predictions.shape[0] == prob_matrix.shape[0]
-    import scipy.sparse as sp
-    if sp.isspmatrix(prob_matrix):
-        prob_matrix = prob_matrix.toarray()
-
-    final_preds = predictions
-    for i in range(piter):
-        final_preds = one_iter(prob_matrix, final_preds)
-        if substitute:
-            final_preds[seed_idx] = 1
-
-    return final_preds
-
-
-def train_model(model, fea_constructor, prob_matrix, diff_mat, learning_rate: float, λ, γ,
-                idx_split_args: dict = {'ntraining': 200, 'nstopping': 400, 'nval': 10},
-                stopping_args: dict = stopping_args, test: bool = False, device: str = 'cuda', torch_seed: int = None,
-                print_interval: int = 10, batch_size=None) -> Tuple[(nn.Module, dict)]:
-    """
-    Train the model using the specified parameters.
-
-    Args:
-
-    - model (nn.Module): Model to be trained.
-
-    - fea_constructor (nn.Module): Feature constructor object.
-
-    - prob_matrix (torch.Tensor): Probability matrix.
-
-    - diff_mat (torch.utils.data.dataset.Subset): The diffusion matrix (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
-
-    - learning_rate (float): Learning rate for optimizer.
-
-    - λ: Lambda value.
-
-    - γ: Gamma value.
-
-    - idx_split_args (dict): Split of the dataset, ntraining is the number of training set, nstopping is the number of samples to determine the early stopping, and nval is the number of validation set.
-
-    - stopping_args (dict): Stopping arguments.
-
-    - test (bool): Whether to perform testing.
-
-    - device (str): Device for training, cpu or cuda.
-
-    - torch_seed (int): Seed for torch.
-
-    - print_interval (int): Print interval.
-
-    - batch_size (int): Batch size.
-
-    Returns:
-
-    - model (nn.Module): Trained model.
-
-    - result (dict): Results of diffusion model,including predictions, train mean error, early_stopping mean error, val/test mean error, runtime, and runtime per epoch.
-    """
-    if torch_seed is None:
-        torch_seed = gen_seeds()
-    torch.manual_seed(seed=torch_seed)
-    #logging.log(22, f"PyTorch seed: {torch_seed}")
-    γ = torch.tensor(γ, device=device)
-    optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
-    early_stopping = EarlyStopping(model, **stopping_args)
-    epoch_stats = {'train': {}, 'stopping': {}}
-    start_time = time.time()
-    start_time_str = time.strftime('%Y-%m-%d_%H-%M-%S', time.localtime())
-    last_time = start_time
-    temp_attr_mat_dict = {}
-
-    # Loop through epochs
-    for epoch in range(early_stopping.max_epochs):
-        idx_np = {}
-        idx_np['train'], idx_np['stopping'], idx_np['valtest'] = gen_splits_(np.arange(prob_matrix.shape[0]),
-                                                                             train_size=idx_split_args['ntraining'],
-                                                                             stopping_size=idx_split_args['nstopping'],
-                                                                             val_size=idx_split_args['nval'])
-        idx_all = {key: torch.LongTensor(val) for key, val in idx_np.items()}
-
-        # Initialize epoch statistics
-        for phase in epoch_stats.keys():
-            epoch_stats[phase]['loss'] = []
-            epoch_stats[phase]['error'] = []
-
-        # Loop through different matrices
-        for i, influ_mat in enumerate(diff_mat):
-            try:
-                attr_mat = temp_attr_mat_dict[i]
-            except KeyError:
-                seed_vec = influ_mat[:, 0]
-                attr_mat = fea_constructor(seed_vec)
-                temp_attr_mat_dict[i] = attr_mat
-
-            model = update_embedding(model, attr_mat)
-            model = model.to(device)
-            influ_vec = influ_mat[:, -1]
-            labels_all = influ_vec.numpy()
-            dataloaders = get_dataloaders(idx_all, labels_all, batch_size=batch_size)
-
-            # Iterate through training and validation/test phases
-            for phase in epoch_stats.keys():
-                if phase == 'train':
-                    model.train()
-                else:
-                    model.eval()
-
-                # Iterate through batches
-                for idx, labels in dataloaders[phase]:
-                    idx = idx.to(device)
-                    labels = labels.to(device)
-                    optimizer.zero_grad()
-                    with torch.set_grad_enabled(phase == 'train'):
-                        preds = model(idx)
-                        loss = model.loss(preds, labels, λ, γ)
-                        error = np.mean(np.abs(preds.cpu().detach().numpy() - labels.cpu().detach().numpy()))
-                        if phase == 'train':
-                            loss.backward()
-                            optimizer.step()
-                        epoch_stats[phase]['loss'].append(loss.item())
-                        epoch_stats[phase]['error'].append(error)
-
-        # Calculate epoch statistics
-        for phase in epoch_stats.keys():
-            epoch_stats[phase]['loss'] = np.mean(epoch_stats[phase]['loss'])
-            epoch_stats[phase]['error'] = np.mean(epoch_stats[phase]['error'])
-
-        # Log information
-        if epoch % print_interval == 0:
-            duration = time.time() - last_time
-            last_time = time.time()
-            #logging.info(
-            print(f"Epoch {epoch}: Train loss = {epoch_stats['train']['loss']:.4f}, Train error = {epoch_stats['train']['error']:.4f}, early stopping loss = {epoch_stats['stopping']['loss']:.4f}, early stopping error = {epoch_stats['stopping']['error']:.4f}, ({duration:.3f} sec)")
-
-        # Check early stopping
-        if len(early_stopping.stop_vars) > 0:
-            stop_vars = [epoch_stats['stopping'][key] for key in early_stopping.stop_vars]
-            if early_stopping.check(stop_vars, epoch):
-                break
-
-    # Calculate runtime statistics
-    runtime = time.time() - start_time
-    runtime_perepoch = runtime / (epoch + 1)
-    #logging.log(22, f"Last epoch: {epoch}, best epoch: {early_stopping.best_epoch} ({runtime:.3f} sec)")
-
-    # Load best model state
-    model.load_state_dict(early_stopping.best_state)
-
-    # Calculate errors
-    train_preds = get_predictions(model, idx_all['train'])
-    train_error = np.abs(train_preds - labels_all[idx_all['train']]).mean()
-    stopping_preds = get_predictions(model, idx_all['stopping'])
-    stopping_error = np.abs(stopping_preds - labels_all[idx_all['stopping']]).mean()
-    #logging.log(21, f"Early stopping error: {stopping_error}")
-    valtest_preds = get_predictions(model, idx_all['valtest'])
-    valtest_error = np.abs(valtest_preds - labels_all[idx_all['valtest']]).mean()
-    valtest_name = 'Test' if test else 'Validation'
-    #logging.log(22, f"{valtest_name} mean error: {valtest_error}")
-
-    # Prepare results
-    result = {}
-    result['predictions'] = get_predictions(model, torch.arange(len(labels_all)))
-    result['train'] = {'mean error': train_error}
-    result['early_stopping'] = {'mean error': stopping_error}
-    result['valtest'] = {'mean error': valtest_error}
-    result['runtime'] = runtime
-    result['runtime_perepoch'] = runtime_perepoch
-
-    return model, result
-
-
-def get_predictions(model, idx, batch_size=None):
-    """
-    Get predictions from the model.
-
-    Args:
-
-    - model (nn.Module): Diffusion model.
-
-    - idx (Tensor): Indices.
-
-    - batch_size (int): Batch size.
-
-    Returns:
-
-    - numpy.ndarray: Predictions.
-    """
-    if batch_size is None:
-        batch_size = idx.numel()
-    dataset = TensorDataset(idx)
-    dataloader = DataLoader(dataset=dataset, batch_size=batch_size, shuffle=False)
-    preds = []
-    for idx, in dataloader:
-        with torch.set_grad_enabled(False):
-            pred = model(idx)
-            preds.append(pred)
-
-    return torch.cat(preds, dim=0).cpu().numpy()
-
-
-class GetPrediction:
-    """
-    Callable class for getting predictions.
-    """
-
-    def __init__(self, model, fea_constructor):
-        """
-        Initialize GetPrediction object.
-
-        Args:
-        - model (nn.Module): Model for prediction.
-        - fea_constructor: Feature constructor object.
-        """
-        self.model = model
-        self.fea_constructor = fea_constructor
-
-    def __call__(self, seed_vec, prob_matrix, piter=2):
-        """
-        Call method to get predictions.
-
-        Args:
-        - seed_vec (array-like): Seed vector.
-        - prob_matrix (numpy.ndarray): Probability matrix.
-        - piter (int): Iteration number.
-
-        Returns:
-        - numpy.ndarray: Predictions.
-        """
-        assert len(seed_vec) == prob_matrix.shape[0], 'Illegal seed vector or prob_matrix'
-        if sp.isspmatrix(prob_matrix):
-            prob_matrix = prob_matrix.toarray()
-
-        self.fea_constructor.prob_matrix = prob_matrix
-
-        idx = np.arange(prob_matrix.shape[0])
-        attr_mat = self.fea_constructor(seed_vec)
-        self.model = update_embedding(self.model, attr_mat)
-        preds = self.model(idx).detach().cpu().numpy()
-
-        seed_idx = np.argwhere(seed_vec == 1)
-        preds = PIteration(prob_matrix, preds, seed_idx=seed_idx, piter=iter)
-        return preds
-
-
-
-def get_idx_new_seeds(model, prediction):
-    """
-    Get indices for new seeds.
-
-    Given each node's probability, predict the seed vector on the same graph.
-
-    Args:
-
-    - model (nn.module): Model for prediction.
-
-    - prediction (torch.Tensor): Prediction of diffusion.
-
-    Returns:
-
-    - result (torch.Tensor): Prediction of seeds.
-    """
-    device = next(model.parameters()).device
-    prediction = torch.tensor(prediction).to(device)
-    result = model.backward(prediction)
-    return result
+from typing import  Tuple
+import time
+import numpy as np
+import torch
+import torch.nn as nn
+from torch.utils.data import TensorDataset, DataLoader
+import scipy.sparse as sp
+import sys
+sys.path.append('../../')
+from .preprocessing import gen_seeds, gen_splits_
+from .earlystopping import EarlyStopping, stopping_args
+
+class FeatureCons:
+    """
+    Initial feature constructor for different models.
+    """
+
+    def __init__(self, ndim=None):
+        """
+        Initialize FeatureCons object.
+
+        Args:
+
+        - ndim (int): Number of dimensions.
+        """
+        self.prob_matrix = None
+        self.ndim = ndim
+
+    def __deepis_fea(self, seed_vec):
+        """
+        Deeply compute features based on the given seed vector.
+
+        Args:
+
+        - seed_vec (torch.Tensor): Seed vector.
+
+        Returns:
+
+        - attr_mat(numpy.ndarray): Feature matrix.
+        """
+        seed_vec = seed_vec.reshape((-1, 1))
+        import scipy.sparse as sp
+        if sp.isspmatrix(self.prob_matrix):
+            self.prob_matrix = self.prob_matrix.toarray()
+        assert seed_vec.shape[0] == self.prob_matrix.shape[0], 'Seed vector is illegal'
+        attr_mat = [seed_vec]
+        for i in range(self.ndim - 1):
+            attr_mat.append(self.prob_matrix.T @ attr_mat[(-1)])
+
+        attr_mat = np.concatenate(attr_mat, axis=(-1))
+        return attr_mat
+
+    def __call__(self, seed_vec):
+        """
+        Call method to compute features based on the given seed vector.
+
+        Args:
+
+        - seed_vec (torch.Tensor): Seed vector.
+
+        Returns:
+
+        - numpy.ndarray: Feature matrix.
+        """
+        return self.__deepis_fea(seed_vec)
+
+
+def get_dataloaders(idx, labels_np, batch_size=None):
+    """
+    Get data loaders for training, validation, and testing.
+
+    Args:
+
+    - idx (dict): Dictionary containing indices for different phases, training, early stopping, and validation/test.
+
+    - labels_np (numpy.ndarray): Labels as numpy array.
+
+    - batch_size (int): Batch size.
+
+    Returns:
+
+    - dataloaders (dict): Dictionary containing data loaders for different phases.
+    """
+    labels = torch.FloatTensor(labels_np)
+    if batch_size is None:
+        batch_size = max((val.numel() for val in idx.values()))
+    datasets = {phase: TensorDataset(torch.LongTensor(ind), labels[ind]) for phase, ind in idx.items()}
+    dataloaders = {phase: DataLoader(dataset=dataset, batch_size=batch_size, shuffle=True) for phase, dataset in
+                   datasets.items()}
+    return dataloaders
+
+
+def construct_attr_mat(prob_matrix, seed_vec, order=5):
+    """
+    Construct attribute matrix based on the given probability matrix and seed vector.
+
+    Args:
+
+    - prob_matrix (scipy.sparse.csr_matrix): Probability matrix.
+
+    - seed_vec (numpy.ndarray): Seed vector.
+
+    - order (int): Order of attribute matrix construction.
+
+    Returns:
+
+    - attr_mat (numpy.ndarray): Attribute matrix.
+    """
+    lanczos_flag = False
+    if lanczos_flag:
+        return lanczos_algo(prob_matrix, seed_vec, order)
+    seed_vec = seed_vec.reshape((-1, 1))
+    assert seed_vec.shape[0] == prob_matrix.shape[0]
+    attr_mat = [seed_vec]
+    if sp.isspmatrix(prob_matrix):
+        prob_matrix = prob_matrix.toarray()
+    for i in range(1, order + 1):
+        attr_mat.append(prob_matrix.T @ attr_mat[(-1)])
+
+    attr_mat = np.concatenate(attr_mat, axis=(-1))
+    return attr_mat
+
+
+def lanczos_algo(prob_matrix, seed_vec, order=5, epsilon=0.001):
+    """
+    Lanczos algorithm for computing attribute matrix.
+
+    Args:
+
+    - prob_matrix (numpy.ndarray or scipy.sparse.csr_matrix): Probability matrix.
+
+    - seed_vec (numpy.ndarray): Seed vector.
+
+    - order (int): Order of attribute matrix construction.
+
+    - epsilon (float): Threshold for stopping the iteration.
+
+    Returns:
+
+    - numpy.ndarray: Attribute matrix.
+    """
+    S = prob_matrix.T
+    seed_vec = seed_vec.flatten()
+    beta = np.zeros((order + 1,))
+    gamma = np.zeros((order + 1,))
+    q = [np.zeros((len(seed_vec),)), seed_vec / np.linalg.norm(seed_vec, ord=2)]
+    for j in range(1, order + 1):
+        z = S @ q[j]
+        gamma[j] = q[j].reshape((1, -1)) @ z
+        z = z - gamma[j] * q[j] - beta[(j - 1)] * q[(j - 1)]
+        beta[j] = np.linalg.norm(z, ord=2)
+        if beta[j] < epsilon:
+            break
+        q.append(z / beta[j])
+
+    q = q[1:]
+    q = np.array(q).T
+    return q
+
+
+def update_embedding(model, feature_mat):
+    """
+    Update the embedding layer of the model with the new feature matrix.
+
+    Args:
+
+    - model (torch.nn.Module): Model.
+
+    - feature_mat (numpy.ndarray): Feature matrix.
+
+    Returns:
+
+    - torch.nn.Module: Updated model.
+    """
+    assert getattr(model, 'gnn_model', None) is not None, 'Object model should have a submodule `gnn_model` '
+    device = next(model.parameters()).device
+    if model.gnn_model.features is None:
+        new_embedding_layer = nn.Embedding(feature_mat.shape[0], feature_mat.shape[1])
+        new_embedding_layer.weight = nn.Parameter(torch.FloatTensor(feature_mat), requires_grad=False)
+        model.gnn_model.features = new_embedding_layer
+    else:
+        assert feature_mat.shape[1] == model.gnn_model.features.weight.shape[1], \
+            'New dimension of new embedding weights is not consistent with the old dimension'
+        model.gnn_model.features.weight = nn.Parameter(torch.FloatTensor(feature_mat), requires_grad=False)
+        model.gnn_model.features.num_embeddings = feature_mat.shape[0]
+        model.gnn_model.features.embedding_dim = feature_mat.shape[1]
+    model = model.to(device)
+    return model
+
+
+def PIteration(prob_matrix, predictions, seed_idx, substitute=True, piter=10):
+    """
+    Perform final prediction iteration to fit the ideal equation system.
+
+    Args:
+
+    - prob_matrix (numpy.ndarray): Probability matrix.
+
+    - predictions (numpy.ndarray): Predictions.
+
+    - seed_idx (numpy.ndarray): Seed indices.
+
+    - substitute (bool): Whether to substitute seed indices.
+
+    - piter (int): Number of iterations.
+
+    Returns:
+
+    - final_preds (numpy.ndarray): Final predictions.
+    """
+
+    def one_iter(prob_matrix, predictions):
+        P2 = np.multiply(prob_matrix.T, np.broadcast_to(predictions.reshape((1, -1)), prob_matrix.shape))
+        P3 = np.ones(prob_matrix.shape) - P2
+        one_iter_preds = np.ones((prob_matrix.shape[0],)) - np.prod(P3, axis=1).flatten()
+        return one_iter_preds
+
+    # predictions = predictions.flatten()
+    assert prob_matrix.shape[0] == prob_matrix.shape[1]
+    assert predictions.shape[0] == prob_matrix.shape[0]
+    import scipy.sparse as sp
+    if sp.isspmatrix(prob_matrix):
+        prob_matrix = prob_matrix.toarray()
+
+    final_preds = predictions
+    for i in range(piter):
+        final_preds = one_iter(prob_matrix, final_preds)
+        if substitute:
+            final_preds[seed_idx] = 1
+
+    return final_preds
+
+
+def train_model(model, fea_constructor, prob_matrix, diff_mat, learning_rate: float, λ, γ,
+                idx_split_args: dict = {'ntraining': 200, 'nstopping': 400, 'nval': 10},
+                stopping_args: dict = stopping_args, test: bool = False, device: str = 'cuda', torch_seed: int = None,
+                print_interval: int = 10, batch_size=None) -> Tuple[(nn.Module, dict)]:
+    """
+    Train the model using the specified parameters.
+
+    Args:
+
+    - model (nn.Module): Model to be trained.
+
+    - fea_constructor (nn.Module): Feature constructor object.
+
+    - prob_matrix (torch.Tensor): Probability matrix.
+
+    - diff_mat (torch.utils.data.dataset.Subset): The diffusion matrix (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
+
+    - learning_rate (float): Learning rate for optimizer.
+
+    - λ: Lambda value.
+
+    - γ: Gamma value.
+
+    - idx_split_args (dict): Split of the dataset, ntraining is the number of training set, nstopping is the number of samples to determine the early stopping, and nval is the number of validation set.
+
+    - stopping_args (dict): Stopping arguments.
+
+    - test (bool): Whether to perform testing.
+
+    - device (str): Device for training, cpu or cuda.
+
+    - torch_seed (int): Seed for torch.
+
+    - print_interval (int): Print interval.
+
+    - batch_size (int): Batch size.
+
+    Returns:
+
+    - model (nn.Module): Trained model.
+
+    - result (dict): Results of diffusion model,including predictions, train mean error, early_stopping mean error, val/test mean error, runtime, and runtime per epoch.
+    """
+    if torch_seed is None:
+        torch_seed = gen_seeds()
+    torch.manual_seed(seed=torch_seed)
+    #logging.log(22, f"PyTorch seed: {torch_seed}")
+    γ = torch.tensor(γ, device=device)
+    optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
+    early_stopping = EarlyStopping(model, **stopping_args)
+    epoch_stats = {'train': {}, 'stopping': {}}
+    start_time = time.time()
+    start_time_str = time.strftime('%Y-%m-%d_%H-%M-%S', time.localtime())
+    last_time = start_time
+    temp_attr_mat_dict = {}
+
+    # Loop through epochs
+    for epoch in range(early_stopping.max_epochs):
+        idx_np = {}
+        idx_np['train'], idx_np['stopping'], idx_np['valtest'] = gen_splits_(np.arange(prob_matrix.shape[0]),
+                                                                             train_size=idx_split_args['ntraining'],
+                                                                             stopping_size=idx_split_args['nstopping'],
+                                                                             val_size=idx_split_args['nval'])
+        idx_all = {key: torch.LongTensor(val) for key, val in idx_np.items()}
+
+        # Initialize epoch statistics
+        for phase in epoch_stats.keys():
+            epoch_stats[phase]['loss'] = []
+            epoch_stats[phase]['error'] = []
+
+        # Loop through different matrices
+        for i, influ_mat in enumerate(diff_mat):
+            try:
+                attr_mat = temp_attr_mat_dict[i]
+            except KeyError:
+                seed_vec = influ_mat[:, 0]
+                attr_mat = fea_constructor(seed_vec)
+                temp_attr_mat_dict[i] = attr_mat
+
+            model = update_embedding(model, attr_mat)
+            model = model.to(device)
+            influ_vec = influ_mat[:, -1]
+            labels_all = influ_vec.numpy()
+            dataloaders = get_dataloaders(idx_all, labels_all, batch_size=batch_size)
+
+            # Iterate through training and validation/test phases
+            for phase in epoch_stats.keys():
+                if phase == 'train':
+                    model.train()
+                else:
+                    model.eval()
+
+                # Iterate through batches
+                for idx, labels in dataloaders[phase]:
+                    idx = idx.to(device)
+                    labels = labels.to(device)
+                    optimizer.zero_grad()
+                    with torch.set_grad_enabled(phase == 'train'):
+                        preds = model(idx)
+                        loss = model.loss(preds, labels, λ, γ)
+                        error = np.mean(np.abs(preds.cpu().detach().numpy() - labels.cpu().detach().numpy()))
+                        if phase == 'train':
+                            loss.backward()
+                            optimizer.step()
+                        epoch_stats[phase]['loss'].append(loss.item())
+                        epoch_stats[phase]['error'].append(error)
+
+        # Calculate epoch statistics
+        for phase in epoch_stats.keys():
+            epoch_stats[phase]['loss'] = np.mean(epoch_stats[phase]['loss'])
+            epoch_stats[phase]['error'] = np.mean(epoch_stats[phase]['error'])
+
+        # Log information
+        if epoch % print_interval == 0:
+            duration = time.time() - last_time
+            last_time = time.time()
+            #logging.info(
+            print(f"Epoch {epoch}: Train loss = {epoch_stats['train']['loss']:.4f}, Train error = {epoch_stats['train']['error']:.4f}, early stopping loss = {epoch_stats['stopping']['loss']:.4f}, early stopping error = {epoch_stats['stopping']['error']:.4f}, ({duration:.3f} sec)")
+
+        # Check early stopping
+        if len(early_stopping.stop_vars) > 0:
+            stop_vars = [epoch_stats['stopping'][key] for key in early_stopping.stop_vars]
+            if early_stopping.check(stop_vars, epoch):
+                break
+
+    # Calculate runtime statistics
+    runtime = time.time() - start_time
+    runtime_perepoch = runtime / (epoch + 1)
+    #logging.log(22, f"Last epoch: {epoch}, best epoch: {early_stopping.best_epoch} ({runtime:.3f} sec)")
+
+    # Load best model state
+    model.load_state_dict(early_stopping.best_state)
+
+    # Calculate errors
+    train_preds = get_predictions(model, idx_all['train'])
+    train_error = np.abs(train_preds - labels_all[idx_all['train']]).mean()
+    stopping_preds = get_predictions(model, idx_all['stopping'])
+    stopping_error = np.abs(stopping_preds - labels_all[idx_all['stopping']]).mean()
+    #logging.log(21, f"Early stopping error: {stopping_error}")
+    valtest_preds = get_predictions(model, idx_all['valtest'])
+    valtest_error = np.abs(valtest_preds - labels_all[idx_all['valtest']]).mean()
+    valtest_name = 'Test' if test else 'Validation'
+    #logging.log(22, f"{valtest_name} mean error: {valtest_error}")
+
+    # Prepare results
+    result = {}
+    result['predictions'] = get_predictions(model, torch.arange(len(labels_all)))
+    result['train'] = {'mean error': train_error}
+    result['early_stopping'] = {'mean error': stopping_error}
+    result['valtest'] = {'mean error': valtest_error}
+    result['runtime'] = runtime
+    result['runtime_perepoch'] = runtime_perepoch
+
+    return model, result
+
+
+def get_predictions(model, idx, batch_size=None):
+    """
+    Get predictions from the model.
+
+    Args:
+
+    - model (nn.Module): Diffusion model.
+
+    - idx (Tensor): Indices.
+
+    - batch_size (int): Batch size.
+
+    Returns:
+
+    - numpy.ndarray: Predictions.
+    """
+    if batch_size is None:
+        batch_size = idx.numel()
+    dataset = TensorDataset(idx)
+    dataloader = DataLoader(dataset=dataset, batch_size=batch_size, shuffle=False)
+    preds = []
+    for idx, in dataloader:
+        with torch.set_grad_enabled(False):
+            pred = model(idx)
+            preds.append(pred)
+
+    return torch.cat(preds, dim=0).cpu().numpy()
+
+
+class GetPrediction:
+    """
+    Callable class for getting predictions.
+    """
+
+    def __init__(self, model, fea_constructor):
+        """
+        Initialize GetPrediction object.
+
+        Args:
+        - model (nn.Module): Model for prediction.
+        - fea_constructor: Feature constructor object.
+        """
+        self.model = model
+        self.fea_constructor = fea_constructor
+
+    def __call__(self, seed_vec, prob_matrix, piter=2):
+        """
+        Call method to get predictions.
+
+        Args:
+        - seed_vec (array-like): Seed vector.
+        - prob_matrix (numpy.ndarray): Probability matrix.
+        - piter (int): Iteration number.
+
+        Returns:
+        - numpy.ndarray: Predictions.
+        """
+        assert len(seed_vec) == prob_matrix.shape[0], 'Illegal seed vector or prob_matrix'
+        if sp.isspmatrix(prob_matrix):
+            prob_matrix = prob_matrix.toarray()
+
+        self.fea_constructor.prob_matrix = prob_matrix
+
+        idx = np.arange(prob_matrix.shape[0])
+        attr_mat = self.fea_constructor(seed_vec)
+        self.model = update_embedding(self.model, attr_mat)
+        preds = self.model(idx).detach().cpu().numpy()
+
+        seed_idx = np.argwhere(seed_vec == 1)
+        preds = PIteration(prob_matrix, preds, seed_idx=seed_idx, piter=iter)
+        return preds
+
+
+
+def get_idx_new_seeds(model, prediction):
+    """
+    Get indices for new seeds.
+
+    Given each node's probability, predict the seed vector on the same graph.
+
+    Args:
+
+    - model (nn.module): Model for prediction.
+
+    - prediction (torch.Tensor): Prediction of diffusion.
+
+    Returns:
+
+    - result (torch.Tensor): Prediction of seeds.
+    """
+    device = next(model.parameters()).device
+    prediction = torch.tensor(prediction).to(device)
+    result = model.backward(prediction)
+    return result
```

### Comparing `GraphSL-0.8/GraphSL/GNN/IVGD/validity_net.py` & `GraphSL-0.9/GraphSL/GNN/IVGD/validity_net.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-import torch
-from GraphSL.GNN.IVGD.correction import correction
-
-
-class validity_net(torch.nn.Module):
-    """
-    Validity-aware layers.
-
-    Attributes:
-        
-    - number_layer (int): Number of layers.
-    
-    - alpha1, alpha2, alpha3, alpha4, alpha5 (float): Alpha values for each layer.
-    
-    - tau1, tau2, tau3, tau4, tau5 (float): Tau values for each layer.
-    
-    - net1, net2, net3, net4, net5 (correction): Correction layer.
-    
-    - rho1, rho2, rho3, rho4, rho5 (float): Rho values for each layer.
-    """
-
-    def __init__(self, alpha, tau, rho):
-        """
-        Initialize the validity_net model.
-
-        Args:
-            
-        - alpha (float): Alpha value.
-        
-        - tau (float): Tau value.
-        
-        - rho (float): Rho value.
-        """
-        super(validity_net, self).__init__()
-        self.number_layer = 5
-        self.alpha1 = alpha
-        self.alpha2 = alpha
-        self.alpha3 = alpha
-        self.alpha4 = alpha
-        self.alpha5 = alpha
-
-        self.tau1 = tau
-        self.tau2 = tau
-        self.tau3 = tau
-        self.tau4 = tau
-        self.tau5 = tau
-
-        self.net1 = correction()
-        self.net2 = correction()
-        self.net3 = correction()
-        self.net4 = correction()
-        self.net5 = correction()
-
-        self.rho1 = rho
-        self.rho2 = rho
-        self.rho3 = rho
-        self.rho4 = rho
-        self.rho5 = rho
-
-    def forward(self, x, label, lamda):
-        """
-        Forward pass of the validity-ware layer.
-
-        Args:
-
-        - x (torch.Tensor): corrected prediction of seed vector.
-
-        - label (torch.Tensor): Source Label.
-
-        - lamda (torch.Tensor): Lambda tensor.
-
-        Returns:
-
-        - Tensor: prediction subject to the validity constraint.
-
-        """
-        sum = torch.sum(label)
-        label = torch.cat((1 - label, label), dim=1)
-        x = torch.cat((1 - x, x), dim=1)
-        prob = x[:, 1].unsqueeze(-1)
-        x = (self.tau1 * self.net1(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho1 * (torch.sum(x) - sum) + self.alpha1 * x) / (
-                    self.tau1 + self.alpha1)
-        prob = x[:, 1].unsqueeze(-1)
-        lamda = lamda + self.rho1 * (torch.sum(prob) - sum)
-        x = (self.tau2 * self.net2(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho2 * (torch.sum(x) - sum) + self.alpha2 * x) / (
-                    self.tau2 + self.alpha2)
-        prob = x[:, 1].unsqueeze(-1)
-        lamda = lamda + self.rho2 * (torch.sum(prob) - sum)
-        x = (self.tau3 * self.net3(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho3 * (torch.sum(x) - sum) + self.alpha3 * x) / (
-                    self.tau3 + self.alpha3)
-        prob = x[:, 1].unsqueeze(-1)
-        lamda = lamda + self.rho3 * (torch.sum(prob) - sum)
-        x = (self.tau4 * self.net4(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho4 * (torch.sum(x) - sum) + self.alpha4 * x) / (
-                    self.tau4 + self.alpha4)
-        prob = x[:, 1].unsqueeze(-1)
-        lamda = lamda + self.rho4 * (torch.sum(prob) - sum)
-        x = (self.tau5 * self.net5(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
-             - self.rho5 * (torch.sum(x) - sum) + self.alpha5 * x) / (
-                    self.tau5 + self.alpha5)
-        return x
-
-    def correction(self, pred):
-        """
-        Impose validity constraint on predictions.
-
-        Args:
-
-        - pred (torch.Tensor): Predictions tensor.
-
-        Returns:
-
-        - Tensor: predictions tensor after passing validity-ware layers.
-        """
-        temp = pred[:, 0].unsqueeze(-1)
-        return (self.net1(temp) + self.net2(temp) + self.net3(temp) + self.net4(temp) + self.net5(temp)) / self.number_layer
+import torch
+from GraphSL.GNN.IVGD.correction import correction
+
+
+class validity_net(torch.nn.Module):
+    """
+    Validity-aware layers.
+
+    Attributes:
+        
+    - number_layer (int): Number of layers.
+    
+    - alpha1, alpha2, alpha3, alpha4, alpha5 (float): Alpha values for each layer.
+    
+    - tau1, tau2, tau3, tau4, tau5 (float): Tau values for each layer.
+    
+    - net1, net2, net3, net4, net5 (correction): Correction layer.
+    
+    - rho1, rho2, rho3, rho4, rho5 (float): Rho values for each layer.
+    """
+
+    def __init__(self, alpha, tau, rho):
+        """
+        Initialize the validity_net model.
+
+        Args:
+            
+        - alpha (float): Alpha value.
+        
+        - tau (float): Tau value.
+        
+        - rho (float): Rho value.
+        """
+        super(validity_net, self).__init__()
+        self.number_layer = 5
+        self.alpha1 = alpha
+        self.alpha2 = alpha
+        self.alpha3 = alpha
+        self.alpha4 = alpha
+        self.alpha5 = alpha
+
+        self.tau1 = tau
+        self.tau2 = tau
+        self.tau3 = tau
+        self.tau4 = tau
+        self.tau5 = tau
+
+        self.net1 = correction()
+        self.net2 = correction()
+        self.net3 = correction()
+        self.net4 = correction()
+        self.net5 = correction()
+
+        self.rho1 = rho
+        self.rho2 = rho
+        self.rho3 = rho
+        self.rho4 = rho
+        self.rho5 = rho
+
+    def forward(self, x, label, lamda):
+        """
+        Forward pass of the validity-ware layer.
+
+        Args:
+
+        - x (torch.Tensor): corrected prediction of seed vector.
+
+        - label (torch.Tensor): Source Label.
+
+        - lamda (torch.Tensor): Lambda tensor.
+
+        Returns:
+
+        - Tensor: prediction subject to the validity constraint.
+
+        """
+        sum = torch.sum(label)
+        label = torch.cat((1 - label, label), dim=1)
+        x = torch.cat((1 - x, x), dim=1)
+        prob = x[:, 1].unsqueeze(-1)
+        x = (self.tau1 * self.net1(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
+             - self.rho1 * (torch.sum(x) - sum) + self.alpha1 * x) / (
+                    self.tau1 + self.alpha1)
+        prob = x[:, 1].unsqueeze(-1)
+        lamda = lamda + self.rho1 * (torch.sum(prob) - sum)
+        x = (self.tau2 * self.net2(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
+             - self.rho2 * (torch.sum(x) - sum) + self.alpha2 * x) / (
+                    self.tau2 + self.alpha2)
+        prob = x[:, 1].unsqueeze(-1)
+        lamda = lamda + self.rho2 * (torch.sum(prob) - sum)
+        x = (self.tau3 * self.net3(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
+             - self.rho3 * (torch.sum(x) - sum) + self.alpha3 * x) / (
+                    self.tau3 + self.alpha3)
+        prob = x[:, 1].unsqueeze(-1)
+        lamda = lamda + self.rho3 * (torch.sum(prob) - sum)
+        x = (self.tau4 * self.net4(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
+             - self.rho4 * (torch.sum(x) - sum) + self.alpha4 * x) / (
+                    self.tau4 + self.alpha4)
+        prob = x[:, 1].unsqueeze(-1)
+        lamda = lamda + self.rho4 * (torch.sum(prob) - sum)
+        x = (self.tau5 * self.net5(prob) - label * torch.softmax(x, dim=1) / label.shape[0] - lamda
+             - self.rho5 * (torch.sum(x) - sum) + self.alpha5 * x) / (
+                    self.tau5 + self.alpha5)
+        return x
+
+    def correction(self, pred):
+        """
+        Impose validity constraint on predictions.
+
+        Args:
+
+        - pred (torch.Tensor): Predictions tensor.
+
+        Returns:
+
+        - Tensor: predictions tensor after passing validity-ware layers.
+        """
+        temp = pred[:, 0].unsqueeze(-1)
+        return (self.net1(temp) + self.net2(temp) + self.net3(temp) + self.net4(temp) + self.net5(temp)) / self.number_layer
```

### Comparing `GraphSL-0.8/GraphSL/GNN/SLVAE/model.py` & `GraphSL-0.9/GraphSL/GNN/SLVAE/model.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,466 +1,466 @@
-import torch.nn as nn
-import torch
-import torch.nn.functional as F
-import scipy.sparse as sp
-class Encoder(nn.Module):
-    """
-    Encoder module for a variational autoencoder (VAE).
-
-    Attributes:
-
-    - input_dim (int): Dimension of the input.
-
-    - hidden_dim (int): Dimension of the hidden layer.
-
-    - latent_dim (int): Dimension of the latent space.
-    """
-
-    def __init__(self, input_dim=784, hidden_dim=512, latent_dim=256):
-        """
-        Initialize the Encoder.
-
-        Args:
-
-        - input_dim (int): Dimension of the input.
-
-        - hidden_dim (int): Dimension of the hidden layer.
-
-        - latent_dim (int): Dimension of the latent space.
-        """
-        super(Encoder, self).__init__()
-
-        self.linear1 = nn.Linear(input_dim, hidden_dim)
-        self.linear2 = nn.Linear(hidden_dim, hidden_dim)
-        self.mean = nn.Linear(hidden_dim, latent_dim)
-        self.var = nn.Linear(hidden_dim, latent_dim)
-        self.LeakyReLU = nn.LeakyReLU(0.2)
-
-    def forward(self, x):
-        """
-        Forward pass of the Encoder.
-
-        Args:
-        - x (torch.Tensor): Input tensor.
-
-        Returns:
-
-        - mean (torch.Tensor): The mean of the latent space.
-
-        - log_var (torch.Tensor): The log variance of the latent space.
-
-        """
-        x = self.LeakyReLU(self.linear1(x))
-        x = self.LeakyReLU(self.linear2(x))
-
-        mean = self.mean(x)
-        log_var = self.var(x)
-        return mean, log_var
-
-
-class Decoder(nn.Module):
-    """
-    Decoder module for a variational autoencoder (VAE).
-
-    Attributes:
-
-    - output_dim (int): Dimension of the output.
-
-    - hidden_dim (int): Dimension of the hidden layer.
-
-    - latent_dim (int): Dimension of the latent space.
-    """
-
-    def __init__(self, output_dim=784, hidden_dim=512, latent_dim=256):
-        """
-        Initialize the Decoder.
-
-        Args:
-
-        - output_dim (int): Dimension of the output.
-
-
-        - hidden_dim (int): Dimension of the hidden layer.
-
-        - latent_dim (int): Dimension of the latent space.
-        """
-        super(Decoder, self).__init__()
-
-        self.linear2 = nn.Linear(latent_dim, hidden_dim)
-        self.linear1 = nn.Linear(hidden_dim, hidden_dim)
-        self.output = nn.Linear(hidden_dim, output_dim)
-        self.LeakyReLU = nn.LeakyReLU(0.2)
-
-    def forward(self, x):
-        """
-        Forward pass of the Decoder.
-
-        Args:
-
-        - x (torch.Tensor): Input tensor.
-
-        Returns:
-
-        - x_hat (torch.Tensor): Decoded output tensor.
-        """
-        x = self.LeakyReLU(self.linear2(x))
-        x = self.LeakyReLU(self.linear1(x))
-
-        x_hat = torch.sigmoid(self.output(x))
-        return x_hat
-
-
-
-class VAE(nn.Module):
-    """
-    Variational Autoencoder (VAE) model.
-
-    Attributes:
-
-    - input_dim (int): Dimension of the input.
-
-    - hidden_dim (int): Dimension of the hidden layer.
-
-    - latent_dim (int): Dimension of the latent space.
-    """
-
-    def __init__(self, input_dim=1, hidden_dim=512, latent_dim=256):
-        """
-        Initialize the VAE model.
-
-        Args:
-
-        - input_dim (int): Dimension of the input.
-
-        - hidden_dim (int): Dimension of the hidden layer.
-
-        - latent_dim (int): Dimension of the latent space.
-        """
-        super(VAE, self).__init__()
-
-        # Encoder
-        self.encoder = nn.Sequential(
-            nn.Linear(input_dim, hidden_dim),
-            nn.LeakyReLU(0.2),
-            nn.Linear(hidden_dim, latent_dim),
-            nn.LeakyReLU(0.2)
-        )
-
-        # Latent mean and variance
-        self.mean_layer = nn.Linear(latent_dim, 2)
-        self.logvar_layer = nn.Linear(latent_dim, 2)
-
-        # Decoder
-        self.decoder = nn.Sequential(
-            nn.Linear(2, latent_dim),
-            nn.LeakyReLU(0.2),
-            nn.Linear(latent_dim, hidden_dim),
-            nn.LeakyReLU(0.2),
-            nn.Linear(hidden_dim, input_dim),
-            nn.Sigmoid()
-        )
-
-    def encode(self, x):
-        """
-        Encode input data into latent space.
-
-        Args:
-
-        - x (torch.Tensor): Input tensor.
-
-        Returns:
-
-        - mean (torch.Tensor):  The mean of latent space
-
-        - logvar (torch.Tensor):   Log variance of latent space.
-        """
-        x = self.encoder(x)
-        mean, logvar = self.mean_layer(x), self.logvar_layer(x)
-        return mean, logvar
-
-    def reparameterization(self, mean, var, device):
-        """
-        Reparameterization trick to sample from the latent space.
-
-        Args:
-
-        - mean (torch.Tensor): Mean of the latent space.
-
-        - var (torch.Tensor): Variance of the latent space.
-
-        - device (torch.device): Device to be used for computation, cpu or cuda.
-
-        Returns:
-
-        - z (torch.Tensor): Sampled latent vector.
-        """
-        epsilon = torch.randn_like(var).to(device)
-        z = mean + var * epsilon
-        return z
-
-    def decode(self, x):
-        """
-        Decode latent vector into output space.
-
-        Args:
-
-        - x (torch.Tensor): Latent vector.
-
-        Returns:
-
-        - torch.Tensor: Decoded output tensor.
-        """
-        return self.decoder(x)
-
-    def forward(self, x):
-        """
-        Forward pass of the VAE.
-
-        Args:
-
-        - x (torch.Tensor): Input tensor.
-
-        Returns:
-
-        - x_hat (tensor.Tensor): The reconstructed input.
-
-        - mean (tensor.Tensor): The mean of the latent space.
-
-        - log_var (tensor.Tensor): The log variance of the latent space.
-
-        """
-        device = x.device
-        mean, log_var = self.encode(x)
-        z = self.reparameterization(mean, log_var, device)
-        x_hat = self.decode(z)
-        return x_hat, mean, log_var
-
-
-class GNN(nn.Module):
-    """
-    Graph Neural Network (GNN) model.
-
-    Attributes:
-
-    - input_dim (int): Dimension of the input.
-
-    - adj_matrix (torch.Tensor): adjacency matrix representing graph connectivity.
-
-    - hiddenunits (List[int]): List of hidden units for each layer.
-
-    - num_classes (int): Number of output classes.
-
-    - bias (bool): Whether to include bias in linear layers.
-
-    - drop_prob (float): Dropout probability.
-    """
-
-    def __init__(self, adj_matrix, input_dim=5, hiddenunits=[64, 64], num_classes=1, bias=True, drop_prob=0.5):
-        """
-        Initialize the GNN model.
-
-        Args:
-
-        - adj_matrix (torch.Tensor): adjacency matrix representing graph connectivity.
-
-        - input_dim (int): Dimension of the input.
-
-        - hiddenunits (List[int]): List of hidden units for each layer.
-
-        - num_classes (int): Number of output classes.
-
-        - bias (bool): Whether to include bias in linear layers.
-
-        - drop_prob (float): Dropout probability.
-        """
-        super(GNN, self).__init__()
-
-        self.input_dim = input_dim
-
-        # Convert sparse matrix to dense if needed
-        if sp.isspmatrix(adj_matrix):
-            adj_matrix = adj_matrix.toarray()
-
-        self.adj_matrix = nn.Parameter(torch.FloatTensor(adj_matrix), requires_grad=False)
-
-        # Define fully connected layers
-        fcs = [nn.Linear(input_dim, hiddenunits[0], bias=bias)]
-        for i in range(1, len(hiddenunits)):
-            fcs.append(nn.Linear(hiddenunits[i - 1], hiddenunits[i]))
-        fcs.append(nn.Linear(hiddenunits[-1], num_classes))
-
-        self.fcs = nn.ModuleList(fcs)
-
-        # Define dropout layer
-        if drop_prob == 0:
-            self.dropout = lambda x: x
-        else:
-            self.dropout = nn.Dropout(drop_prob)
-
-        # Activation function
-        self.act_fn = nn.ReLU()
-
-    def forward(self, seed_vec):
-        """
-        Forward pass of the GNN.
-
-        Args:
-
-        - seed_vec (torch.Tensor): Input seed vector.
-
-        Returns:
-
-        - res (torch.Tensor): Predicted output.
-        """
-        for i in range(self.input_dim - 1):
-            if i == 0:
-                mat = self.adj_matrix.T @ seed_vec
-                attr_mat = torch.cat((seed_vec.unsqueeze(0), mat.unsqueeze(0)), 0)
-            else:
-                mat = self.adj_matrix.T @ attr_mat[-1]
-                attr_mat = torch.cat((attr_mat, mat.unsqueeze(0)), 0)
-
-        layer_inner = self.act_fn(self.fcs[0](self.dropout(attr_mat.permute(*torch.arange(attr_mat.ndim - 1, -1, -1)))))
-        for fc in self.fcs[1:-1]:
-            layer_inner = self.act_fn(fc(layer_inner))
-        res = torch.sigmoid(self.fcs[-1](self.dropout(layer_inner)))
-        return res
-
-    def loss(self, y, y_hat):
-        """
-        Calculate loss.
-
-        Args:
-
-        - y (torch.Tensor): Ground truth.
-
-        - y_hat (torch.Tensor): Predicted output.
-
-        Returns:
-
-        - forward_loss (torch.Tensor): Forward loss.
-        """
-        forward_loss = F.mse_loss(y_hat, y)
-        return forward_loss
-
-
-class DiffusionPropagate(nn.Module):
-    """
-    Diffusion Propagation module for graph data.
-
-    Attributes:
-
-    - adj_matrix (torch.Tensor): adjacency matrix representing graph connectivity.
-
-    - niter (int): Number of diffusion iterations.
-    """
-
-    def __init__(self, adj_matrix, niter):
-        """
-        Initialize the DiffusionPropagate module.
-
-        Args:
-
-        - adj_matrix (torch.Tensor): adjacency matrix representing graph connectivity.
-
-        - niter (int): Number of diffusion iterations.
-        """
-        super(DiffusionPropagate, self).__init__()
-
-        self.niter = niter
-
-        # Convert sparse matrix to dense if needed
-        if sp.isspmatrix(adj_matrix):
-            adj_matrix = adj_matrix.toarray()
-
-        self.register_buffer('adj_matrix', torch.FloatTensor(adj_matrix))
-
-    def forward(self, preds):
-        """
-        Forward pass of the DiffusionPropagate module.
-
-        Args:
-
-        - preds (torch.Tensor): Predictions.
-
-        Returns:
-
-        - prop_preds (torch.Tensor): Propagated predictions.
-        """
-        device = preds.device
-
-        for i in range(preds.shape[0]):
-            prop_pred = preds[i]
-            for j in range(self.niter):
-                P2 = self.adj_matrix.T * prop_pred.view((1, -1)).expand(self.adj_matrix.shape)
-                P3 = torch.ones(self.adj_matrix.shape).to(device) - P2
-                prop_pred = torch.ones((self.adj_matrix.shape[0],)).to(device) - torch.prod(P3, dim=1)
-                prop_pred = prop_pred.unsqueeze(0)
-            if i == 0:
-                prop_preds = prop_pred
-            else:
-                prop_preds = torch.cat((prop_preds, prop_pred), 0)
-
-        return prop_preds
-
-
-
-class ForwardModel(nn.Module):
-    def __init__(self, gnn_model: nn.Module, propagate: nn.Module):
-        """
-        Constructor for ForwardModel class.
-
-        Args:
-            
-            gnn_model (nn.Module): Graph Neural Network model used as feature extractor.
-            
-            propagate (nn.Module): Module to perform additional computation on GNN outputs.
-        """
-        super(ForwardModel, self).__init__()
-        self.gnn_model = gnn_model  # Assigning the GNN model
-        self.propagate = propagate  # Assigning the propagation module
-        self.relu = nn.ReLU(inplace=True)  # ReLU activation function
-
-        # Extracting parameters requiring gradients from gnn_model for optimization
-        self.reg_params = list(filter(lambda x: x.requires_grad, self.gnn_model.parameters()))
-
-    def forward(self, seed_vec):
-        """
-        Forward pass of the ForwardModel.
-
-        Args:
-            
-            seed_vec (torch.Tensor): Input tensor for the forward pass.
-
-        Returns:
-            
-           predictions (torch.Tensor): Predictions after the forward pass.
-        """
-        # Extracting indices where seed_vec equals 1
-        seed_idx = (seed_vec == 1).nonzero(as_tuple=False)
-
-        # Forward pass through the GNN model
-        predictions = self.gnn_model(seed_vec)
-
-        # Additional computation using propagate module, possibly considering seed indices
-        predictions = self.propagate(predictions, seed_idx)
-
-        # Applying ReLU activation function
-        predictions = self.relu(predictions)
-
-        return predictions
-
-    def loss(self, y, y_hat):
-        """
-        Compute the loss between predicted and actual values.
-
-        Args:
-            y (torch.Tensor): Actual values.
-            
-            y_hat (torch.Tensor): Predicted values.
-
-        Returns:
-            forward_loss (torch.Tensor): Forward loss computed using Mean Squared Error.
-        """
-        # Computing Mean Squared Error loss
-        forward_loss = F.mse_loss(y_hat, y)
-        return forward_loss
+import torch.nn as nn
+import torch
+import torch.nn.functional as F
+import scipy.sparse as sp
+class Encoder(nn.Module):
+    """
+    Encoder module for a variational autoencoder (VAE).
+
+    Attributes:
+
+    - input_dim (int): Dimension of the input.
+
+    - hidden_dim (int): Dimension of the hidden layer.
+
+    - latent_dim (int): Dimension of the latent space.
+    """
+
+    def __init__(self, input_dim=784, hidden_dim=512, latent_dim=256):
+        """
+        Initialize the Encoder.
+
+        Args:
+
+        - input_dim (int): Dimension of the input.
+
+        - hidden_dim (int): Dimension of the hidden layer.
+
+        - latent_dim (int): Dimension of the latent space.
+        """
+        super(Encoder, self).__init__()
+
+        self.linear1 = nn.Linear(input_dim, hidden_dim)
+        self.linear2 = nn.Linear(hidden_dim, hidden_dim)
+        self.mean = nn.Linear(hidden_dim, latent_dim)
+        self.var = nn.Linear(hidden_dim, latent_dim)
+        self.LeakyReLU = nn.LeakyReLU(0.2)
+
+    def forward(self, x):
+        """
+        Forward pass of the Encoder.
+
+        Args:
+        - x (torch.Tensor): Input tensor.
+
+        Returns:
+
+        - mean (torch.Tensor): The mean of the latent space.
+
+        - log_var (torch.Tensor): The log variance of the latent space.
+
+        """
+        x = self.LeakyReLU(self.linear1(x))
+        x = self.LeakyReLU(self.linear2(x))
+
+        mean = self.mean(x)
+        log_var = self.var(x)
+        return mean, log_var
+
+
+class Decoder(nn.Module):
+    """
+    Decoder module for a variational autoencoder (VAE).
+
+    Attributes:
+
+    - output_dim (int): Dimension of the output.
+
+    - hidden_dim (int): Dimension of the hidden layer.
+
+    - latent_dim (int): Dimension of the latent space.
+    """
+
+    def __init__(self, output_dim=784, hidden_dim=512, latent_dim=256):
+        """
+        Initialize the Decoder.
+
+        Args:
+
+        - output_dim (int): Dimension of the output.
+
+
+        - hidden_dim (int): Dimension of the hidden layer.
+
+        - latent_dim (int): Dimension of the latent space.
+        """
+        super(Decoder, self).__init__()
+
+        self.linear2 = nn.Linear(latent_dim, hidden_dim)
+        self.linear1 = nn.Linear(hidden_dim, hidden_dim)
+        self.output = nn.Linear(hidden_dim, output_dim)
+        self.LeakyReLU = nn.LeakyReLU(0.2)
+
+    def forward(self, x):
+        """
+        Forward pass of the Decoder.
+
+        Args:
+
+        - x (torch.Tensor): Input tensor.
+
+        Returns:
+
+        - x_hat (torch.Tensor): Decoded output tensor.
+        """
+        x = self.LeakyReLU(self.linear2(x))
+        x = self.LeakyReLU(self.linear1(x))
+
+        x_hat = torch.sigmoid(self.output(x))
+        return x_hat
+
+
+
+class VAE(nn.Module):
+    """
+    Variational Autoencoder (VAE) model.
+
+    Attributes:
+
+    - input_dim (int): Dimension of the input.
+
+    - hidden_dim (int): Dimension of the hidden layer.
+
+    - latent_dim (int): Dimension of the latent space.
+    """
+
+    def __init__(self, input_dim=1, hidden_dim=512, latent_dim=256):
+        """
+        Initialize the VAE model.
+
+        Args:
+
+        - input_dim (int): Dimension of the input.
+
+        - hidden_dim (int): Dimension of the hidden layer.
+
+        - latent_dim (int): Dimension of the latent space.
+        """
+        super(VAE, self).__init__()
+
+        # Encoder
+        self.encoder = nn.Sequential(
+            nn.Linear(input_dim, hidden_dim),
+            nn.LeakyReLU(0.2),
+            nn.Linear(hidden_dim, latent_dim),
+            nn.LeakyReLU(0.2)
+        )
+
+        # Latent mean and variance
+        self.mean_layer = nn.Linear(latent_dim, 2)
+        self.logvar_layer = nn.Linear(latent_dim, 2)
+
+        # Decoder
+        self.decoder = nn.Sequential(
+            nn.Linear(2, latent_dim),
+            nn.LeakyReLU(0.2),
+            nn.Linear(latent_dim, hidden_dim),
+            nn.LeakyReLU(0.2),
+            nn.Linear(hidden_dim, input_dim),
+            nn.Sigmoid()
+        )
+
+    def encode(self, x):
+        """
+        Encode input data into latent space.
+
+        Args:
+
+        - x (torch.Tensor): Input tensor.
+
+        Returns:
+
+        - mean (torch.Tensor):  The mean of latent space
+
+        - logvar (torch.Tensor):   Log variance of latent space.
+        """
+        x = self.encoder(x)
+        mean, logvar = self.mean_layer(x), self.logvar_layer(x)
+        return mean, logvar
+
+    def reparameterization(self, mean, var, device):
+        """
+        Reparameterization trick to sample from the latent space.
+
+        Args:
+
+        - mean (torch.Tensor): Mean of the latent space.
+
+        - var (torch.Tensor): Variance of the latent space.
+
+        - device (torch.device): Device to be used for computation, cpu or cuda.
+
+        Returns:
+
+        - z (torch.Tensor): Sampled latent vector.
+        """
+        epsilon = torch.randn_like(var).to(device)
+        z = mean + var * epsilon
+        return z
+
+    def decode(self, x):
+        """
+        Decode latent vector into output space.
+
+        Args:
+
+        - x (torch.Tensor): Latent vector.
+
+        Returns:
+
+        - torch.Tensor: Decoded output tensor.
+        """
+        return self.decoder(x)
+
+    def forward(self, x):
+        """
+        Forward pass of the VAE.
+
+        Args:
+
+        - x (torch.Tensor): Input tensor.
+
+        Returns:
+
+        - x_hat (tensor.Tensor): The reconstructed input.
+
+        - mean (tensor.Tensor): The mean of the latent space.
+
+        - log_var (tensor.Tensor): The log variance of the latent space.
+
+        """
+        device = x.device
+        mean, log_var = self.encode(x)
+        z = self.reparameterization(mean, log_var, device)
+        x_hat = self.decode(z)
+        return x_hat, mean, log_var
+
+
+class GNN(nn.Module):
+    """
+    Graph Neural Network (GNN) model.
+
+    Attributes:
+
+    - input_dim (int): Dimension of the input.
+
+    - adj_matrix (torch.Tensor): adjacency matrix representing graph connectivity.
+
+    - hiddenunits (List[int]): List of hidden units for each layer.
+
+    - num_classes (int): Number of output classes.
+
+    - bias (bool): Whether to include bias in linear layers.
+
+    - drop_prob (float): Dropout probability.
+    """
+
+    def __init__(self, adj_matrix, input_dim=5, hiddenunits=[64, 64], num_classes=1, bias=True, drop_prob=0.5):
+        """
+        Initialize the GNN model.
+
+        Args:
+
+        - adj_matrix (torch.Tensor): adjacency matrix representing graph connectivity.
+
+        - input_dim (int): Dimension of the input.
+
+        - hiddenunits (List[int]): List of hidden units for each layer.
+
+        - num_classes (int): Number of output classes.
+
+        - bias (bool): Whether to include bias in linear layers.
+
+        - drop_prob (float): Dropout probability.
+        """
+        super(GNN, self).__init__()
+
+        self.input_dim = input_dim
+
+        # Convert sparse matrix to dense if needed
+        if sp.isspmatrix(adj_matrix):
+            adj_matrix = adj_matrix.toarray()
+
+        self.adj_matrix = nn.Parameter(torch.FloatTensor(adj_matrix), requires_grad=False)
+
+        # Define fully connected layers
+        fcs = [nn.Linear(input_dim, hiddenunits[0], bias=bias)]
+        for i in range(1, len(hiddenunits)):
+            fcs.append(nn.Linear(hiddenunits[i - 1], hiddenunits[i]))
+        fcs.append(nn.Linear(hiddenunits[-1], num_classes))
+
+        self.fcs = nn.ModuleList(fcs)
+
+        # Define dropout layer
+        if drop_prob == 0:
+            self.dropout = lambda x: x
+        else:
+            self.dropout = nn.Dropout(drop_prob)
+
+        # Activation function
+        self.act_fn = nn.ReLU()
+
+    def forward(self, seed_vec):
+        """
+        Forward pass of the GNN.
+
+        Args:
+
+        - seed_vec (torch.Tensor): Input seed vector.
+
+        Returns:
+
+        - res (torch.Tensor): Predicted output.
+        """
+        for i in range(self.input_dim - 1):
+            if i == 0:
+                mat = self.adj_matrix.T @ seed_vec
+                attr_mat = torch.cat((seed_vec.unsqueeze(0), mat.unsqueeze(0)), 0)
+            else:
+                mat = self.adj_matrix.T @ attr_mat[-1]
+                attr_mat = torch.cat((attr_mat, mat.unsqueeze(0)), 0)
+
+        layer_inner = self.act_fn(self.fcs[0](self.dropout(attr_mat.permute(*torch.arange(attr_mat.ndim - 1, -1, -1)))))
+        for fc in self.fcs[1:-1]:
+            layer_inner = self.act_fn(fc(layer_inner))
+        res = torch.sigmoid(self.fcs[-1](self.dropout(layer_inner)))
+        return res
+
+    def loss(self, y, y_hat):
+        """
+        Calculate loss.
+
+        Args:
+
+        - y (torch.Tensor): Ground truth.
+
+        - y_hat (torch.Tensor): Predicted output.
+
+        Returns:
+
+        - forward_loss (torch.Tensor): Forward loss.
+        """
+        forward_loss = F.mse_loss(y_hat, y)
+        return forward_loss
+
+
+class DiffusionPropagate(nn.Module):
+    """
+    Diffusion Propagation module for graph data.
+
+    Attributes:
+
+    - adj_matrix (torch.Tensor): adjacency matrix representing graph connectivity.
+
+    - niter (int): Number of diffusion iterations.
+    """
+
+    def __init__(self, adj_matrix, niter):
+        """
+        Initialize the DiffusionPropagate module.
+
+        Args:
+
+        - adj_matrix (torch.Tensor): adjacency matrix representing graph connectivity.
+
+        - niter (int): Number of diffusion iterations.
+        """
+        super(DiffusionPropagate, self).__init__()
+
+        self.niter = niter
+
+        # Convert sparse matrix to dense if needed
+        if sp.isspmatrix(adj_matrix):
+            adj_matrix = adj_matrix.toarray()
+
+        self.register_buffer('adj_matrix', torch.FloatTensor(adj_matrix))
+
+    def forward(self, preds):
+        """
+        Forward pass of the DiffusionPropagate module.
+
+        Args:
+
+        - preds (torch.Tensor): Predictions.
+
+        Returns:
+
+        - prop_preds (torch.Tensor): Propagated predictions.
+        """
+        device = preds.device
+
+        for i in range(preds.shape[0]):
+            prop_pred = preds[i]
+            for j in range(self.niter):
+                P2 = self.adj_matrix.T * prop_pred.view((1, -1)).expand(self.adj_matrix.shape)
+                P3 = torch.ones(self.adj_matrix.shape).to(device) - P2
+                prop_pred = torch.ones((self.adj_matrix.shape[0],)).to(device) - torch.prod(P3, dim=1)
+                prop_pred = prop_pred.unsqueeze(0)
+            if i == 0:
+                prop_preds = prop_pred
+            else:
+                prop_preds = torch.cat((prop_preds, prop_pred), 0)
+
+        return prop_preds
+
+
+
+class ForwardModel(nn.Module):
+    def __init__(self, gnn_model: nn.Module, propagate: nn.Module):
+        """
+        Constructor for ForwardModel class.
+
+        Args:
+            
+            gnn_model (nn.Module): Graph Neural Network model used as feature extractor.
+            
+            propagate (nn.Module): Module to perform additional computation on GNN outputs.
+        """
+        super(ForwardModel, self).__init__()
+        self.gnn_model = gnn_model  # Assigning the GNN model
+        self.propagate = propagate  # Assigning the propagation module
+        self.relu = nn.ReLU(inplace=True)  # ReLU activation function
+
+        # Extracting parameters requiring gradients from gnn_model for optimization
+        self.reg_params = list(filter(lambda x: x.requires_grad, self.gnn_model.parameters()))
+
+    def forward(self, seed_vec):
+        """
+        Forward pass of the ForwardModel.
+
+        Args:
+            
+            seed_vec (torch.Tensor): Input tensor for the forward pass.
+
+        Returns:
+            
+           predictions (torch.Tensor): Predictions after the forward pass.
+        """
+        # Extracting indices where seed_vec equals 1
+        seed_idx = (seed_vec == 1).nonzero(as_tuple=False)
+
+        # Forward pass through the GNN model
+        predictions = self.gnn_model(seed_vec)
+
+        # Additional computation using propagate module, possibly considering seed indices
+        predictions = self.propagate(predictions, seed_idx)
+
+        # Applying ReLU activation function
+        predictions = self.relu(predictions)
+
+        return predictions
+
+    def loss(self, y, y_hat):
+        """
+        Compute the loss between predicted and actual values.
+
+        Args:
+            y (torch.Tensor): Actual values.
+            
+            y_hat (torch.Tensor): Predicted values.
+
+        Returns:
+            forward_loss (torch.Tensor): Forward loss computed using Mean Squared Error.
+        """
+        # Computing Mean Squared Error loss
+        forward_loss = F.mse_loss(y_hat, y)
+        return forward_loss
```

### Comparing `GraphSL-0.8/GraphSL/Prescribed.py` & `GraphSL-0.9/GraphSL/Prescribed.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,656 +1,680 @@
-import numpy as np
-import networkx as nx
-import copy
-import torch
-from sklearn.metrics import roc_auc_score,f1_score,accuracy_score,precision_score,recall_score
-from scipy.sparse import csgraph,coo_matrix
-from GraphSL.Evaluation import Metric
-
-class LPSI:
-    """
-    Implement the Label Propagation based Source Identification (LPSI) algorithm.
-
-    Wang, Zheng, et al. "Multiple source detection without knowing the underlying propagation model." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 31. No. 1. 2017.
-    """
-
-    def __init__(self):
-        """
-        Initialize the LPSI module.
-        """
-
-    def predict(self, laplacian, num_node, alpha, diff_vec):
-        """
-        Prediction of the LPSI algorithm.
-
-        Args:
-
-        - laplacian (numpy.ndarray): The Laplacian matrix of the graph.
-
-        - num_node (int): Number of nodes in the graph.
-
-        - alpha (float): the fraction of label information that a node gets from its neighbors (between 0 and 1).
-
-        - diff_vec (numpy.ndarray): The diffusion vector.
-
-        Returns:
-
-        - x (numpy.ndarray): Prediction of source nodes.
-        """
-        x = (1 - alpha) * np.matmul(np.linalg.pinv(np.eye(N=num_node) - alpha * laplacian,hermitian=True), diff_vec)
-        return x
-
-    def train(self, adj, train_dataset, alpha_list=[0.001, 0.01, 0.1], thres_list=[0.1, 0.3, 0.5, 0.7, 0.9]):
-        """
-         Train the LPSI algorithm.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
-
-        - train_dataset (torch.utils.data.dataset.Subset): the training dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
-
-        - alpha_list (list): List of the fraction of label information that a node gets from its neighbors (between 0 and 1) to try.
-
-        - thres_list (list): List of threshold values to try.
-
-        Returns:
-
-        - opt_alpha (float): Optimal fraction of label information that a node gets from its neighbors, between 0 and 1.
-
-        - opt_thres (float): Optimal threshold value.
-
-        - opt_auc (float): Optimal Area Under the Curve (AUC) value.
-
-        - opt_f1 (float): Optimal F1 score value.
-
-        - opt_pred (numpy.ndarray): Prediction of training seed vector given opt_alpha, every column is the prediction of every simulation. It is used to adjust thres_list.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.Prescribed import LPSI
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        lpsi = LPSI()
-
-        alpha, thres, auc, f1, pred =lpsi.train(adj, train_dataset)
-
-        print("LPSI:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-        """
-        laplacian = csgraph.laplacian(adj, normed=True)
-        laplacian = np.array(coo_matrix.todense(laplacian))
-        num_node = adj.shape[0]
-        train_num = len(train_dataset)
-        opt_auc = 0
-        opt_alpha = 0
-        for alpha in alpha_list:
-            train_auc = 0
-            for influ_mat in train_dataset:
-                seed_vec = influ_mat[:, 0]
-                influ_vec = influ_mat[:, -1]
-                x = self.predict(laplacian, num_node, alpha, influ_vec)
-                train_auc += roc_auc_score(seed_vec, x)
-            train_auc = train_auc / train_num
-            print(f"alpha = {alpha}, train_auc = {train_auc:.3f}")
-            if train_auc > opt_auc:
-                opt_auc = train_auc
-                opt_alpha = alpha
-        
-        opt_pred =np.zeros((num_node,train_num))
-        seed_all = np.zeros((num_node,train_num))
-        for i,influ_mat in enumerate(train_dataset):
-                seed_all[:,i] = influ_mat[:, 0]
-                influ_vec = influ_mat[:, -1]
-                opt_pred[:,i] = self.predict(laplacian, num_node, opt_alpha, influ_vec)
-
-        opt_f1 = 0
-        opt_thres = 0
-        for thres in thres_list:
-            print(f"thres = {thres:.3f}")
-            train_f1 = 0
-            for i in range(train_num):
-                train_f1 += f1_score(seed_all[:,i], opt_pred[:,i] >= thres, zero_division = 1)
-            train_f1 = train_f1 / train_num
-            print(f"thres = {thres:.3f}, train_f1 = {train_f1:.3f}")
-            if train_f1 > opt_f1:
-                opt_f1 = train_f1
-                opt_thres = thres
-        return opt_alpha, opt_thres, opt_auc, opt_f1, opt_pred
-
-    def test(self, adj, test_dataset, alpha, thres):
-        """
-        Test the LPSI algorithm.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
-
-        - test_dataset (torch.utils.data.dataset.Subset): The test dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
-
-        - alpha (float): The fraction of label information that a node gets from its neighbors (between 0 and 1).
-
-        - thres (float): Threshold value.
-
-        Returns:
-
-        - metric (Metric): Evaluation metric containing accuracy, precision, recall, F1 score, and AUC.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.Prescribed import LPSI
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset = split_dataset(dataset)
-
-        lpsi = LPSI()
-
-        alpha, thres, auc, f1, pred = lpsi.train(adj, train_dataset)
-
-        print("LPSI:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-
-        metric=lpsi.test(adj, test_dataset, alpha, thres)
-
-        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-        """
-        laplacian = csgraph.laplacian(adj, normed=True)
-        laplacian = np.array(coo_matrix.todense(laplacian))
-        num_node = adj.shape[0]
-        test_num = len(test_dataset)
-        test_acc = 0
-        test_pr = 0
-        test_re = 0
-        test_f1 = 0
-        test_auc = 0
-        for influ_mat in test_dataset:
-            seed_vec = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-            x = self.predict(laplacian, num_node, alpha, influ_vec)
-            test_acc += accuracy_score(seed_vec, x >= thres)
-            test_pr += precision_score(seed_vec, x >= thres, zero_division = 1)
-            test_re += recall_score(seed_vec, x >= thres, zero_division = 1)
-            test_f1 += f1_score(seed_vec, x >= thres, zero_division = 1)
-            test_auc += roc_auc_score(seed_vec, x)
-
-        test_acc = test_acc / test_num
-        test_pr = test_pr / test_num
-        test_re = test_re / test_num
-        test_f1 = test_f1 / test_num
-        test_auc = test_auc / test_num
-        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
-        return metric
-
-class NetSleuth:
-    """
-    Implement the NetSleuth algorithm.
-
-    Prakash, B. Aditya, Jilles Vreeken, and Christos Faloutsos. "Spotting culprits in epidemics: How many and which ones?." 2012 IEEE 12th international conference on data mining. IEEE, 2012.
-    """
-
-    def __init__(self):
-
-        """
-        Initialize the NetSleuth.
-        """
-
-    def predict(self, G, k, diff_vec):
-        """
-        Prediction of the NetSleuth algorithm.
-
-        Args:
-
-        - G (networkx.Graph): The input graph.
-
-        - k (int): Number of source nodes to identify.
-
-        - diff_vec (torch.Tensor): The diffusion vector.
-
-        Returns:
-
-        - seed_vec (torch.Tensor): A binary tensor representing identified source nodes.
-
-        """
-        g = copy.deepcopy(G)  # Creating a deep copy of the input graph
-        g.remove_nodes_from([n for n in g if n not in np.where(diff_vec == 1)[0]])  # Removing non-relevant nodes
-        lap = nx.laplacian_matrix(g).toarray()  # Computing the Laplacian matrix of the modified graph
-
-        seed = []
-        while len(seed) < k:
-            value, vector = np.linalg.eig(lap)
-            index = np.argmax(vector[np.argmin(value)])
-            seed_index = list(g.nodes)[index]
-            seed.append(seed_index)
-            g.remove_node(seed_index)
-            if len(g.nodes) == 0:
-                break
-            lap = nx.laplacian_matrix(g).toarray()
-
-        seed_vec = torch.zeros(diff_vec.shape)
-        seed_vec[seed] = 1
-        return seed_vec
-
-    def train(self, adj, train_dataset, k_list=[5, 10, 50]):
-        """
-        Train the NetSleuth algorithm.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
-
-        - train_dataset (torch.utils.data.dataset.Subset): The training dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
-
-        - k_list (list): List of the numbers of source nodes to try.
-
-        Returns:
-
-        - opt_k (int): Optimal number of source nodes.
-
-        - opt_auc (float): Optimal Area Under the Curve (AUC) value.
-
-        - train_f1 (float): Training F1 score value.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.Prescribed import NetSleuth
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        netSleuth = NetSleuth()
-
-        k, auc, f1=netSleuth.train(adj, train_dataset)
-
-        print("NetSleuth:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-        """
-        # Y should be no more than number of nodes
-        num_node = adj.shape[0]
-        condition = lambda k: k <= num_node
-        k_list = list(filter(condition, k_list))
-
-        G = nx.from_numpy_array(adj)
-        opt_auc = 0
-        opt_k = 0
-        train_num = len(train_dataset)
-        for k in k_list:
-            train_auc = 0
-            for influ_mat in train_dataset:
-                seed_vec = influ_mat[:, 0]
-                influ_vec = influ_mat[:, -1]
-                x = self.predict(G, k, influ_vec)
-                train_auc += roc_auc_score(seed_vec, x)
-            train_auc = train_auc / train_num
-            print(f"k = {k}, train_auc = {train_auc:.3f}")
-
-            if train_auc > opt_auc:
-                opt_auc = train_auc
-                opt_k = k
-
-        train_f1 = 0
-        for influ_mat in train_dataset:
-            seed_vec = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-            x = self.predict(G, opt_k, influ_vec)
-            train_f1 += f1_score(seed_vec, x, zero_division = 1)
-        train_f1 = train_f1 / train_num
-
-        return opt_k, opt_auc, train_f1
-
-    def test(self, adj, test_dataset, k):
-        """
-        Test the NetSleuth algorithm.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
-
-        - test_dataset (torch.utils.data.dataset.Subset): The test dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
-
-        - k (int): Number of source nodes.
-
-
-        Returns:
-
-        - metric (Metric): Evaluation metric containing accuracy, precision, recall, F1 score, and AUC.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.Prescribed import NetSleuth
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        netSleuth = NetSleuth()
-
-        k, auc, f1=netSleuth.train(adj, train_dataset)
-
-        print("NetSleuth:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-
-        metric = netSleuth.test(adj, test_dataset, k)
-
-        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-        """
-        G = nx.from_numpy_array(adj)
-        test_num = len(test_dataset)
-        test_acc = 0
-        test_pr = 0
-        test_re = 0
-        test_f1 = 0
-        test_auc = 0
-        for influ_mat in test_dataset:
-            seed_vec = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-            x = self.predict(G, k, influ_vec)
-            test_acc += accuracy_score(seed_vec, x)
-            test_pr += precision_score(seed_vec, x, zero_division = 1)
-            test_re += recall_score(seed_vec, x, zero_division = 1)
-            test_f1 += f1_score(seed_vec, x, zero_division = 1)
-            test_auc += roc_auc_score(seed_vec, x)
-
-        test_acc = test_acc / test_num
-        test_pr = test_pr / test_num
-        test_re = test_re / test_num
-        test_f1 = test_f1 / test_num
-        test_auc = test_auc / test_num
-        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
-        return metric
-
-
-
-class OJC:
-    """
-    Implement the Optimal-Jordan-Cover (OJC) algorithm.
-
-    Zhu, Kai, Zhen Chen, and Lei Ying. "Catch’em all: Locating multiple diffusion sources in networks with partial observations." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 31. No. 1. 2017.
-    """
-
-    def __init__(self):
-        """
-        Initialize the OJC module.
-        """
-
-    def get_K_list(self, G, Y, I, target):
-        """
-         Get the list of potential source nodes.
-
-        Args:
-
-        - G (networkx.Graph): The input graph.
-
-        - Y (int): Number of desired source nodes.
-
-        - I (list): list of diffused nodes.
-
-        - target (numpy.ndarray): Target vector.
-
-        Returns:
-
-        - K (list): List of potential source nodes.
-        """
-        K = list()
-        for n1 in G.nodes():
-            count = 0
-            for n2 in G[n1]:
-                if target[n2] == 1:
-                    count += 1
-                if count == Y:
-                    K.append(n1)
-                    break
-        K = list(set(K + I))
-        return K
-
-    def Candidate(self, G, Y, I, target):
-        """
-        Identify potential source nodes based on the given criteria.
-
-        Args:
-
-        - G (networkx.Graph): The input graph.
-
-        - Y (int): Number of desired source nodes.
-
-        - I (list): List of diffused nodes.
-
-        - target (torch.Tensor): Target vector.
-
-        Returns:
-
-        - K (list): List of potential source nodes.
-
-        - G_bar (networkx.Graph): Subgraph containing potential source nodes.
-        """
-        K = self.get_K_list(G, Y, I, target)
-        G_prime = G.subgraph(K)
-        G_prime = nx.Graph(G_prime)
-        if nx.is_connected(G_prime):
-            G_bar = G_prime
-        else:
-            component = nx.connected_components(G_prime)
-            R = [list(c)[0] for c in component]
-            for n in R[1:]:
-                if nx.has_path(G, n, R[0]):
-                    path = nx.shortest_path(G, R[0], n)
-                    nx.add_path(G_prime, path)
-            G_bar = G_prime
-        return K, G_bar
-
-    def predict(self, G, Y, I, target, num_source):
-        """
-        Prediction of the OJC algorithm.
-
-        Args:
-
-        - G (networkx.Graph): The input graph.
-
-        - Y (int): Number of source nodes.
-
-        - I (list): List of diffused nodes.
-
-        - target (numpy.ndarray): Target vector.
-
-        - num_source (int): Maximal number of source nodes.
-
-        Returns:
-
-        - x (numpy.ndarray): A binary vector representing identified potential source nodes.
-        """
-        K, G_bar = self.Candidate(G, Y, I, target)
-        ecc = []
-        for n in K:
-            long_path = 0
-            for i in I:
-                if nx.has_path(G_bar, n, i):
-                    path = nx.shortest_path_length(G_bar, n, i)
-                else:
-                    path = 0
-                if path > long_path:
-                    long_path = path
-            ecc.append(long_path)
-        ecc_arr = np.array(ecc)
-        index = np.argsort(ecc_arr).tolist()
-        index = index[:num_source]
-        x = np.zeros(target.shape)
-        x[index] = 1
-        return x
-
-    def train(self, adj, train_dataset, Y_list=[5, 10, 50]):
-        """
-        Train the OJC algorithm.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
-
-        - train_dataset (torch.utils.data.dataset.Subset): The train dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
-
-        - Y_list (list): List of numbers of source nodes to try.
-
-
-        Returns:
-
-        - opt_Y (int): Optimal number of source nodes.
-
-        - opt_auc (float): Optimal Area Under the Curve (AUC) value.
-
-        - train_f1 (float): Training F1 score value.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.Prescribed import OJC
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        ojc = OJC()
-
-        Y, auc, f1 =ojc.train(adj, train_dataset)
-
-        print("OJC:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-        """
-        # Y should be no more than number of nodes
-        num_node = adj.shape[0]
-        condition = lambda k: k <= num_node
-        Y_list = list(filter(condition, Y_list))
-        G = nx.from_scipy_sparse_array(adj)
-        train_num = len(train_dataset)
-        opt_auc = 0
-        opt_Y = 0
-        for Y in Y_list:
-            train_auc = 0
-            for influ_mat in train_dataset:
-                seed_vec = influ_mat[:, 0]
-                influ_vec = influ_mat[:, -1]
-                num_source = len(influ_vec[influ_vec == 1])
-                I = (influ_vec == 1).nonzero().squeeze(-1).tolist()
-                x = self.predict(G, Y, I, influ_vec, num_source)
-                train_auc += roc_auc_score(seed_vec, x)
-            train_auc = train_auc / train_num
-            print(f"Y = {Y}, train_auc = {train_auc:.3f}")
-            if train_auc > opt_auc:
-                opt_auc = train_auc
-                opt_Y = Y
-
-        train_f1 = 0
-        for influ_mat in train_dataset:
-            seed_vec = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-            num_source = len(influ_vec[influ_vec == 1])
-            I = (influ_vec == 1).nonzero()[0].tolist()
-            x = self.predict(G, opt_Y, I, influ_vec, num_source)
-            train_f1 += f1_score(seed_vec, x, zero_division = 1)
-        train_f1 = train_f1 / train_num
-
-        return opt_Y, opt_auc, train_f1
-
-    def test(self, adj, test_dataset, Y):
-        """
-        Test the OJC algorithm.
-
-        Args:
-
-        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
-
-        - test_dataset (torch.utils.data.dataset.Subset): The test dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
-
-        - Y (int): Number of source nodes.
-
-        Returns:
-
-        - metric (Metric): Evaluation metric containing accuracy, precision, recall, F1 score, and AUC.
-
-        Example:
-
-        from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-
-        from GraphSL.Prescribed import OJC
-
-        data_name = 'karate'
-
-        graph = load_dataset(data_name)
-
-        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-        adj, train_dataset, test_dataset =split_dataset(dataset)
-
-        ojc = OJC()
-
-        Y, auc, f1 =ojc.train(adj, train_dataset)
-
-        print("OJC:")
-
-        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-
-        metric=ojc.test(adj, test_dataset, Y)
-
-        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-        """
-        G = nx.from_scipy_sparse_array(adj)
-        test_num = len(test_dataset)
-        test_acc = 0
-        test_pr = 0
-        test_re = 0
-        test_f1 = 0
-        test_auc = 0
-        for influ_mat in test_dataset:
-            seed_vec = influ_mat[:, 0]
-            influ_vec = influ_mat[:, -1]
-            num_source = len(influ_vec[influ_vec == 1])
-            I = (influ_vec == 1).nonzero()[0].tolist()
-            x = self.predict(G, Y, I, influ_vec, num_source)
-            test_acc += accuracy_score(seed_vec, x)
-            test_pr += precision_score(seed_vec, x, zero_division = 1)
-            test_re += recall_score(seed_vec, x, zero_division = 1)
-            test_f1 += f1_score(seed_vec, x, zero_division = 1)
-            test_auc += roc_auc_score(seed_vec, x)
-
-        test_acc = test_acc / test_num
-        test_pr = test_pr / test_num
-        test_re = test_re / test_num
-        test_f1 = test_f1 / test_num
-        test_auc = test_auc / test_num
-        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
-        return metric
+import numpy as np
+import networkx as nx
+import copy
+import torch
+from sklearn.metrics import roc_auc_score,f1_score,accuracy_score,precision_score,recall_score
+from scipy.sparse import csgraph,coo_matrix
+from GraphSL.Evaluation import Metric
+
+class LPSI:
+    """
+    Implement the Label Propagation based Source Identification (LPSI) algorithm.
+
+    Wang, Zheng, et al. "Multiple source detection without knowing the underlying propagation model." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 31. No. 1. 2017.
+    """
+
+    def __init__(self):
+        """
+        Initialize the LPSI module.
+        """
+
+    def predict(self, laplacian, num_node, alpha, diff_vec):
+        """
+        Prediction of the LPSI algorithm.
+
+        Args:
+
+        - laplacian (numpy.ndarray): The Laplacian matrix of the graph.
+
+        - num_node (int): Number of nodes in the graph.
+
+        - alpha (float): the fraction of label information that a node gets from its neighbors (between 0 and 1).
+
+        - diff_vec (numpy.ndarray): The diffusion vector.
+
+        Returns:
+
+        - x (numpy.ndarray): Prediction of source nodes.
+        """
+        x = (1 - alpha) * np.matmul(np.linalg.pinv(np.eye(N=num_node) - alpha * laplacian,hermitian=True), diff_vec)
+        return x
+
+    def train(self, adj, train_dataset, alpha_list=[0.001, 0.01, 0.1], thres_list=[0.1, 0.3, 0.5, 0.7, 0.9]):
+        """
+         Train the LPSI algorithm.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
+
+        - train_dataset (torch.utils.data.dataset.Subset): the training dataset (number of simulations * number of graph nodes * 2 (the first column is seed vector and the second column is diffusion vector)).
+
+        - alpha_list (list): List of the fraction of label information that a node gets from its neighbors (between 0 and 1) to try.
+
+        - thres_list (list): List of threshold values to try.
+
+        Returns:
+
+        - opt_alpha (float): Optimal fraction of label information that a node gets from its neighbors, between 0 and 1.
+
+        - opt_thres (float): Optimal threshold value.
+
+        - opt_auc (float): Optimal Area Under the Curve (AUC) value.
+
+        - opt_f1 (float): Optimal F1 score value.
+
+        - opt_pred (numpy.ndarray): Prediction of training seed vector given opt_alpha, every column is the prediction of every simulation. It is used to adjust thres_list.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.Prescribed import LPSI
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name,data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        lpsi = LPSI()
+
+        alpha, thres, auc, f1, pred =lpsi.train(adj, train_dataset)
+
+        print("LPSI:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+        """
+        laplacian = csgraph.laplacian(adj, normed=True)
+        laplacian = np.array(coo_matrix.todense(laplacian))
+        num_node = adj.shape[0]
+        train_num = len(train_dataset)
+        opt_auc = 0
+        opt_alpha = 0
+        for alpha in alpha_list:
+            train_auc = 0
+            for influ_mat in train_dataset:
+                seed_vec = influ_mat[:, 0]
+                influ_vec = influ_mat[:, -1]
+                x = self.predict(laplacian, num_node, alpha, influ_vec)
+                train_auc += roc_auc_score(seed_vec, x)
+            train_auc = train_auc / train_num
+            print(f"alpha = {alpha}, train_auc = {train_auc:.3f}")
+            if train_auc > opt_auc:
+                opt_auc = train_auc
+                opt_alpha = alpha
+        
+        opt_pred =np.zeros((num_node,train_num))
+        seed_all = np.zeros((num_node,train_num))
+        for i,influ_mat in enumerate(train_dataset):
+                seed_all[:,i] = influ_mat[:, 0]
+                influ_vec = influ_mat[:, -1]
+                opt_pred[:,i] = self.predict(laplacian, num_node, opt_alpha, influ_vec)
+
+        opt_f1 = 0
+        opt_thres = 0
+        for thres in thres_list:
+            print(f"thres = {thres:.3f}")
+            train_f1 = 0
+            for i in range(train_num):
+                train_f1 += f1_score(seed_all[:,i], opt_pred[:,i] >= thres, zero_division = 1)
+            train_f1 = train_f1 / train_num
+            print(f"thres = {thres:.3f}, train_f1 = {train_f1:.3f}")
+            if train_f1 > opt_f1:
+                opt_f1 = train_f1
+                opt_thres = thres
+        return opt_alpha, opt_thres, opt_auc, opt_f1, opt_pred
+
+    def test(self, adj, test_dataset, alpha, thres):
+        """
+        Test the LPSI algorithm.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
+
+        - test_dataset (torch.utils.data.dataset.Subset): The test dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
+
+        - alpha (float): The fraction of label information that a node gets from its neighbors (between 0 and 1).
+
+        - thres (float): Threshold value.
+
+        Returns:
+
+        - metric (Metric): Evaluation metric containing accuracy, precision, recall, F1 score, and AUC.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.Prescribed import LPSI
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset = split_dataset(dataset)
+
+        lpsi = LPSI()
+
+        alpha, thres, auc, f1, pred = lpsi.train(adj, train_dataset)
+
+        print("LPSI:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+
+        metric=lpsi.test(adj, test_dataset, alpha, thres)
+
+        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+        """
+        laplacian = csgraph.laplacian(adj, normed=True)
+        laplacian = np.array(coo_matrix.todense(laplacian))
+        num_node = adj.shape[0]
+        test_num = len(test_dataset)
+        test_acc = 0
+        test_pr = 0
+        test_re = 0
+        test_f1 = 0
+        test_auc = 0
+        for influ_mat in test_dataset:
+            seed_vec = influ_mat[:, 0]
+            influ_vec = influ_mat[:, -1]
+            x = self.predict(laplacian, num_node, alpha, influ_vec)
+            test_acc += accuracy_score(seed_vec, x >= thres)
+            test_pr += precision_score(seed_vec, x >= thres, zero_division = 1)
+            test_re += recall_score(seed_vec, x >= thres, zero_division = 1)
+            test_f1 += f1_score(seed_vec, x >= thres, zero_division = 1)
+            test_auc += roc_auc_score(seed_vec, x)
+
+        test_acc = test_acc / test_num
+        test_pr = test_pr / test_num
+        test_re = test_re / test_num
+        test_f1 = test_f1 / test_num
+        test_auc = test_auc / test_num
+        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
+        return metric
+
+class NetSleuth:
+    """
+    Implement the NetSleuth algorithm.
+
+    Prakash, B. Aditya, Jilles Vreeken, and Christos Faloutsos. "Spotting culprits in epidemics: How many and which ones?." 2012 IEEE 12th international conference on data mining. IEEE, 2012.
+    """
+
+    def __init__(self):
+
+        """
+        Initialize the NetSleuth.
+        """
+
+    def predict(self, G, k, diff_vec):
+        """
+        Prediction of the NetSleuth algorithm.
+
+        Args:
+
+        - G (networkx.Graph): The input graph.
+
+        - k (int): Number of source nodes to identify.
+
+        - diff_vec (torch.Tensor): The diffusion vector.
+
+        Returns:
+
+        - seed_vec (torch.Tensor): A binary tensor representing identified source nodes.
+
+        """
+        g = copy.deepcopy(G)  # Creating a deep copy of the input graph
+        g.remove_nodes_from([n for n in g if n not in np.where(diff_vec == 1)[0]])  # Removing non-relevant nodes
+        lap = nx.laplacian_matrix(g).toarray()  # Computing the Laplacian matrix of the modified graph
+
+        seed = []
+        while len(seed) < k:
+            value, vector = np.linalg.eig(lap)
+            index = np.argmax(vector[np.argmin(value)])
+            seed_index = list(g.nodes)[index]
+            seed.append(seed_index)
+            g.remove_node(seed_index)
+            if len(g.nodes) == 0:
+                break
+            lap = nx.laplacian_matrix(g).toarray()
+
+        seed_vec = torch.zeros(diff_vec.shape)
+        seed_vec[seed] = 1
+        return seed_vec
+
+    def train(self, adj, train_dataset, k_list=[5, 10, 50]):
+        """
+        Train the NetSleuth algorithm.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
+
+        - train_dataset (torch.utils.data.dataset.Subset): The training dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
+
+        - k_list (list): List of the numbers of source nodes to try.
+
+        Returns:
+
+        - opt_k (int): Optimal number of source nodes.
+
+        - opt_auc (float): Optimal Area Under the Curve (AUC) value.
+
+        - train_f1 (float): Training F1 score value.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.Prescribed import NetSleuth
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        netSleuth = NetSleuth()
+
+        k, auc, f1=netSleuth.train(adj, train_dataset)
+
+        print("NetSleuth:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+        """
+        # Y should be no more than number of nodes
+        num_node = adj.shape[0]
+        condition = lambda k: k <= num_node
+        k_list = list(filter(condition, k_list))
+
+        G = nx.from_numpy_array(adj)
+        opt_auc = 0
+        opt_k = 0
+        train_num = len(train_dataset)
+        for k in k_list:
+            train_auc = 0
+            for influ_mat in train_dataset:
+                seed_vec = influ_mat[:, 0]
+                influ_vec = influ_mat[:, -1]
+                x = self.predict(G, k, influ_vec)
+                train_auc += roc_auc_score(seed_vec, x)
+            train_auc = train_auc / train_num
+            print(f"k = {k}, train_auc = {train_auc:.3f}")
+
+            if train_auc > opt_auc:
+                opt_auc = train_auc
+                opt_k = k
+
+        train_f1 = 0
+        for influ_mat in train_dataset:
+            seed_vec = influ_mat[:, 0]
+            influ_vec = influ_mat[:, -1]
+            x = self.predict(G, opt_k, influ_vec)
+            train_f1 += f1_score(seed_vec, x, zero_division = 1)
+        train_f1 = train_f1 / train_num
+
+        return opt_k, opt_auc, train_f1
+
+    def test(self, adj, test_dataset, k):
+        """
+        Test the NetSleuth algorithm.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
+
+        - test_dataset (torch.utils.data.dataset.Subset): The test dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
+
+        - k (int): Number of source nodes.
+
+
+        Returns:
+
+        - metric (Metric): Evaluation metric containing accuracy, precision, recall, F1 score, and AUC.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.Prescribed import NetSleuth
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        netSleuth = NetSleuth()
+
+        k, auc, f1=netSleuth.train(adj, train_dataset)
+
+        print("NetSleuth:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+
+        metric = netSleuth.test(adj, test_dataset, k)
+
+        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+        """
+        G = nx.from_numpy_array(adj)
+        test_num = len(test_dataset)
+        test_acc = 0
+        test_pr = 0
+        test_re = 0
+        test_f1 = 0
+        test_auc = 0
+        for influ_mat in test_dataset:
+            seed_vec = influ_mat[:, 0]
+            influ_vec = influ_mat[:, -1]
+            x = self.predict(G, k, influ_vec)
+            test_acc += accuracy_score(seed_vec, x)
+            test_pr += precision_score(seed_vec, x, zero_division = 1)
+            test_re += recall_score(seed_vec, x, zero_division = 1)
+            test_f1 += f1_score(seed_vec, x, zero_division = 1)
+            test_auc += roc_auc_score(seed_vec, x)
+
+        test_acc = test_acc / test_num
+        test_pr = test_pr / test_num
+        test_re = test_re / test_num
+        test_f1 = test_f1 / test_num
+        test_auc = test_auc / test_num
+        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
+        return metric
+
+
+
+class OJC:
+    """
+    Implement the Optimal-Jordan-Cover (OJC) algorithm.
+
+    Zhu, Kai, Zhen Chen, and Lei Ying. "Catch’em all: Locating multiple diffusion sources in networks with partial observations." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 31. No. 1. 2017.
+    """
+
+    def __init__(self):
+        """
+        Initialize the OJC module.
+        """
+
+    def get_K_list(self, G, Y, I, target):
+        """
+         Get the list of potential source nodes.
+
+        Args:
+
+        - G (networkx.Graph): The input graph.
+
+        - Y (int): Number of desired source nodes.
+
+        - I (list): list of diffused nodes.
+
+        - target (numpy.ndarray): Target vector.
+
+        Returns:
+
+        - K (list): List of potential source nodes.
+        """
+        K = list()
+        for n1 in G.nodes():
+            count = 0
+            for n2 in G[n1]:
+                if target[n2] == 1:
+                    count += 1
+                if count == Y:
+                    K.append(n1)
+                    break
+        K = list(set(K + I))
+        return K
+
+    def Candidate(self, G, Y, I, target):
+        """
+        Identify potential source nodes based on the given criteria.
+
+        Args:
+
+        - G (networkx.Graph): The input graph.
+
+        - Y (int): Number of desired source nodes.
+
+        - I (list): List of diffused nodes.
+
+        - target (torch.Tensor): Target vector.
+
+        Returns:
+
+        - K (list): List of potential source nodes.
+
+        - G_bar (networkx.Graph): Subgraph containing potential source nodes.
+        """
+        K = self.get_K_list(G, Y, I, target)
+        G_prime = G.subgraph(K)
+        G_prime = nx.Graph(G_prime)
+        if nx.is_connected(G_prime):
+            G_bar = G_prime
+        else:
+            component = nx.connected_components(G_prime)
+            R = [list(c)[0] for c in component]
+            for n in R[1:]:
+                if nx.has_path(G, n, R[0]):
+                    path = nx.shortest_path(G, R[0], n)
+                    nx.add_path(G_prime, path)
+            G_bar = G_prime
+        return K, G_bar
+
+    def predict(self, G, Y, I, target, num_source):
+        """
+        Prediction of the OJC algorithm.
+
+        Args:
+
+        - G (networkx.Graph): The input graph.
+
+        - Y (int): Number of source nodes.
+
+        - I (list): List of diffused nodes.
+
+        - target (numpy.ndarray): Target vector.
+
+        - num_source (int): Maximal number of source nodes.
+
+        Returns:
+
+        - x (numpy.ndarray): A binary vector representing identified potential source nodes.
+        """
+        K, G_bar = self.Candidate(G, Y, I, target)
+        ecc = []
+        for n in K:
+            long_path = 0
+            for i in I:
+                if nx.has_path(G_bar, n, i):
+                    path = nx.shortest_path_length(G_bar, n, i)
+                else:
+                    path = 0
+                if path > long_path:
+                    long_path = path
+            ecc.append(long_path)
+        ecc_arr = np.array(ecc)
+        index = np.argsort(ecc_arr).tolist()
+        index = index[:num_source]
+        x = np.zeros(target.shape)
+        x[index] = 1
+        return x
+
+    def train(self, adj, train_dataset, Y_list=[5, 10, 50]):
+        """
+        Train the OJC algorithm.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
+
+        - train_dataset (torch.utils.data.dataset.Subset): The train dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
+
+        - Y_list (list): List of numbers of source nodes to try.
+
+
+        Returns:
+
+        - opt_Y (int): Optimal number of source nodes.
+
+        - opt_auc (float): Optimal Area Under the Curve (AUC) value.
+
+        - train_f1 (float): Training F1 score value.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.Prescribed import OJC
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        ojc = OJC()
+
+        Y, auc, f1 =ojc.train(adj, train_dataset)
+
+        print("OJC:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+        """
+        # Y should be no more than number of nodes
+        num_node = adj.shape[0]
+        condition = lambda k: k <= num_node
+        Y_list = list(filter(condition, Y_list))
+        G = nx.from_scipy_sparse_array(adj)
+        train_num = len(train_dataset)
+        opt_auc = 0
+        opt_Y = 0
+        for Y in Y_list:
+            train_auc = 0
+            for influ_mat in train_dataset:
+                seed_vec = influ_mat[:, 0]
+                influ_vec = influ_mat[:, -1]
+                num_source = len(influ_vec[influ_vec == 1])
+                I = (influ_vec == 1).nonzero().squeeze(-1).tolist()
+                x = self.predict(G, Y, I, influ_vec, num_source)
+                train_auc += roc_auc_score(seed_vec, x)
+            train_auc = train_auc / train_num
+            print(f"Y = {Y}, train_auc = {train_auc:.3f}")
+            if train_auc > opt_auc:
+                opt_auc = train_auc
+                opt_Y = Y
+
+        train_f1 = 0
+        for influ_mat in train_dataset:
+            seed_vec = influ_mat[:, 0]
+            influ_vec = influ_mat[:, -1]
+            num_source = len(influ_vec[influ_vec == 1])
+            I = (influ_vec == 1).nonzero()[0].tolist()
+            x = self.predict(G, opt_Y, I, influ_vec, num_source)
+            train_f1 += f1_score(seed_vec, x, zero_division = 1)
+        train_f1 = train_f1 / train_num
+
+        return opt_Y, opt_auc, train_f1
+
+    def test(self, adj, test_dataset, Y):
+        """
+        Test the OJC algorithm.
+
+        Args:
+
+        - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
+
+        - test_dataset (torch.utils.data.dataset.Subset): The test dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
+
+        - Y (int): Number of source nodes.
+
+        Returns:
+
+        - metric (Metric): Evaluation metric containing accuracy, precision, recall, F1 score, and AUC.
+
+        Example:
+
+        import os
+
+        curr_dir = os.getcwd()
+
+        from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+
+        from GraphSL.Prescribed import OJC
+
+        data_name = 'karate'
+
+        graph = load_dataset(data_name, data_dir=curr_dir)
+
+        dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+        adj, train_dataset, test_dataset =split_dataset(dataset)
+
+        ojc = OJC()
+
+        Y, auc, f1 =ojc.train(adj, train_dataset)
+
+        print("OJC:")
+
+        print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+
+        metric=ojc.test(adj, test_dataset, Y)
+
+        print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+        """
+        G = nx.from_scipy_sparse_array(adj)
+        test_num = len(test_dataset)
+        test_acc = 0
+        test_pr = 0
+        test_re = 0
+        test_f1 = 0
+        test_auc = 0
+        for influ_mat in test_dataset:
+            seed_vec = influ_mat[:, 0]
+            influ_vec = influ_mat[:, -1]
+            num_source = len(influ_vec[influ_vec == 1])
+            I = (influ_vec == 1).nonzero()[0].tolist()
+            x = self.predict(G, Y, I, influ_vec, num_source)
+            test_acc += accuracy_score(seed_vec, x)
+            test_pr += precision_score(seed_vec, x, zero_division = 1)
+            test_re += recall_score(seed_vec, x, zero_division = 1)
+            test_f1 += f1_score(seed_vec, x, zero_division = 1)
+            test_auc += roc_auc_score(seed_vec, x)
+
+        test_acc = test_acc / test_num
+        test_pr = test_pr / test_num
+        test_re = test_re / test_num
+        test_f1 = test_f1 / test_num
+        test_auc = test_auc / test_num
+        metric = Metric(test_acc, test_pr, test_re, test_f1, test_auc)
+        return metric
```

### Comparing `GraphSL-0.8/GraphSL/data/utils.py` & `GraphSL-0.9/GraphSL/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,209 +1,204 @@
-import numpy as np
-import networkx as nx
-import random
-import ndlib.models.ModelConfig as mc
-import ndlib.models.epidemics as ep
-import torch
-import copy
-
-
-def load_dataset(dataset, data_dir='GraphSL\data'):
-    """
-    Load a dataset from a pickle file.
-
-    Args:
-        
-    - dataset (str): The name of the dataset file, 'karate', 'dolphins', 'jazz', 'netscience', 'cora_ml', 'power_grid','meme8000', 'digg16000'.
-        
-    - data_dir (str): The directory where the dataset files are stored. Default is 'data'.
-
-    Returns:
-        
-    - graph (dict): A dictionary containing the dataset.
-
-    Example:
-
-    from data.utils import load_dataset
-
-    data_name = 'karate'
-
-    graph = load_dataset(data_name)
-    """
-    from pathlib import Path
-    import pickle
-    import sys
-
-    sys.path.append(data_dir)  # for pickle.load
-
-    data_dir = Path(data_dir)
-    graph_name = dataset
-    path_to_file = data_dir / graph_name
-    with open(path_to_file, 'rb') as f:
-        graph = pickle.load(f)
-    return graph
-
-
-def generate_seed_vector(top_nodes, seed_num, G):
-    """
-    Generate a seed vector for diffusion simulation.
-
-    Args:
-
-    - top_nodes (list): List of top nodes based on node degree.
-
-    - seed_num (int): Number of seed nodes.
-
-    - G (networkx.Graph): The graph object.
-
-    Returns:
-
-        seed_vector (list): Seed vector for diffusion simulation.
-    """
-    seed_nodes = random.sample(top_nodes, seed_num)
-    seed_vector = [1 if node in seed_nodes else 0 for node in G.nodes()]
-    return seed_vector
-
-
-def diffusion_generation(graph, sim_num=10, diff_type='IC', time_step=10, repeat_step=10, seed_ratio=0.1,
-                         infect_prob=0.1, recover_prob=0.005, threshold=0.5):
-    """
-    Generate diffusion matrices for a graph.
-
-    Args:
-
-    - graph (dict): Dictionary containing the graph information.
-
-    - sim_num (int): Number of simulations.
-
-    - diff_type (str): Type of diffusion model (IC, LT, SI, SIS, SIR). IC stands for Independent Cascade, LT stands for Linear Threshold, SI stands for Susceptible or Infective, SIS stands for Susceptible or Infective or Susceptible, SIR stands for Susceptible or Infective or Recovered.
-
-    - time_step (int): Number of time steps in the simulation.
-
-    - repeat_step (int): Number of repetitions for each simulation.
-
-    - seed_ratio (float): Ratio of seed nodes.
-
-    - infect_prob (float): Infection probability,  used in SIS, SIR or SI.
-
-    - recover_prob (float): Recovery probability, used in SIS or SIR.
-
-    - threshold (float): Threshold parameter for diffusion models, used in IC or LT.
-
-    Returns:
-
-    - dataset (dict): Dictionary containing ('adj_mat') adjacency matrix and ('diff_mat') diffusion matrices.
-
-    Example:
-
-    from data.utils import load_dataset, diffusion_generation
-
-    data_name = 'karate'
-
-    graph = load_dataset(data_name)
-
-    dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-    """
-    adj_mat = graph['adj_mat']
-    G = nx.from_scipy_sparse_array(adj_mat)
-    node_num = len(G.nodes())
-    seed_num = int(seed_ratio * node_num)
-    simulation = []
-
-    degree_list = list(G.degree())
-    degree_list.sort(key=lambda x: x[1], reverse=True)
-    top_nodes = [x[0] for x in degree_list[:int(len(degree_list) * 0.3)]]
-
-    for i in range(sim_num):
-        seed_vector = generate_seed_vector(top_nodes, seed_num, G)
-        inf_vec_all = torch.zeros(node_num)
-        config = mc.Configuration()
-        for k in range(repeat_step):
-            if diff_type == 'LT':
-                model = ep.ThresholdModel(G)
-                for n in G.nodes():
-                    config.add_node_configuration("threshold", n, threshold)
-            elif diff_type == 'IC':
-                model = ep.IndependentCascadesModel(G)
-                for e in G.edges():
-                    config.add_edge_configuration("threshold", e, threshold)
-            elif diff_type == 'SIS':
-                model = ep.SISModel(G)
-                config.add_model_parameter('beta', infect_prob)
-                config.add_model_parameter('lambda', recover_prob)
-            elif diff_type == 'SIR':
-                model = ep.SIRModel(G)
-                config.add_model_parameter('beta', infect_prob)
-                config.add_model_parameter('gamma', recover_prob)
-            elif diff_type == 'SI':
-                model = ep.SIModel(G)
-                config.add_model_parameter('beta', infect_prob)
-            else:
-                raise ValueError('Only IC, LT, SI, SIR and SIS are supported.')
-
-            config.add_model_initial_configuration("Infected", seed_vector)
-
-            model.set_initial_status(config)
-
-            iterations = model.iteration_bunch(time_step)
-
-            node_status = iterations[0]['status']
-
-            for j in range(1, len(iterations)):
-                node_status.update(iterations[j]['status'])
-
-            inf_vec = np.array(list(node_status.values()))
-            inf_vec[inf_vec == 2] = 1
-
-            inf_vec_all += inf_vec
-
-        inf_vec_all = inf_vec_all / repeat_step
-
-        simulation.append([seed_vector, inf_vec_all])
-
-    simulation = torch.Tensor(simulation).permute(0, 2, 1)
-
-    dataset = {'adj_mat': adj_mat, 'diff_mat': simulation}
-    return dataset
-
-
-def split_dataset(dataset, train_ratio: float = 0.6, seed: int = 0):
-    """
-    Split the dataset into training and testing sets.
-
-    Args:
-
-    - dataset (dict): Dictionary containing the dataset.
-
-    - train_ratio (float): Ratio of training data. Default is 0.6.
-
-    - seed (int): Random seed for reproducibility. Default is 0.
-
-    Returns:
-
-    - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
-
-    - train_dataset (torch.utils.data.dataset.Subset): The train dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
-
-    - test_dataset (torch.utils.data.dataset.Subset): The test dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
-
-    Example:
-
-    from data.utils import load_dataset, diffusion_generation, split_dataset
-
-    data_name = 'karate'
-
-    graph = load_dataset(data_name)
-
-    dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
-
-    adj, train_dataset, test_dataset =split_dataset(dataset)
-    """
-    adj = dataset['adj_mat']
-    diff_mat = copy.deepcopy(dataset['diff_mat'])
-    all_num = len(diff_mat)
-    train_num = int(all_num * train_ratio)
-    test_num = all_num - train_num
-    train_diff_mat, test_diff_mat = torch.utils.data.random_split(diff_mat, [train_num, test_num],
-                                                                  generator=torch.Generator().manual_seed(seed))
-
-    return adj, train_diff_mat, test_diff_mat
+import numpy as np
+import networkx as nx
+import random
+import ndlib.models.ModelConfig as mc
+import ndlib.models.epidemics as ep
+import torch
+import copy
+
+
+def load_dataset(dataset, data_dir):
+    """
+    Load a dataset from a pickle file.
+
+    Args:
+        
+    - dataset (str): The name of the dataset file, 'karate', 'dolphins', 'jazz', 'netscience', 'cora_ml', 'power_grid','meme8000', 'digg16000'.
+        
+    - data_dir (str): The directory where the dataset files are stored.
+
+    Returns:
+        
+    - graph (dict): A dictionary containing the dataset.
+
+    """
+    import pickle
+
+    data_dir = data_dir+"\\data\\"+dataset
+    with open(data_dir, 'rb') as f:
+        graph = pickle.load(f)
+    return graph
+
+
+def generate_seed_vector(top_nodes, seed_num, G):
+    """
+    Generate a seed vector for diffusion simulation.
+
+    Args:
+
+    - top_nodes (list): List of top nodes based on node degree.
+
+    - seed_num (int): Number of seed nodes.
+
+    - G (networkx.Graph): The graph object.
+
+    Returns:
+
+        seed_vector (list): Seed vector for diffusion simulation.
+    """
+    seed_nodes = random.sample(top_nodes, seed_num)
+    seed_vector = [1 if node in seed_nodes else 0 for node in G.nodes()]
+    return seed_vector
+
+
+def diffusion_generation(graph, sim_num=10, diff_type='IC', time_step=10, repeat_step=10, seed_ratio=0.1,
+                         infect_prob=0.1, recover_prob=0.005, threshold=0.5):
+    """
+    Generate diffusion matrices for a graph.
+
+    Args:
+
+    - graph (dict): Dictionary containing the graph information.
+
+    - sim_num (int): Number of simulations.
+
+    - diff_type (str): Type of diffusion model (IC, LT, SI, SIS, SIR). IC stands for Independent Cascade, LT stands for Linear Threshold, SI stands for Susceptible or Infective, SIS stands for Susceptible or Infective or Susceptible, SIR stands for Susceptible or Infective or Recovered.
+
+    - time_step (int): Number of time steps in the simulation.
+
+    - repeat_step (int): Number of repetitions for each simulation.
+
+    - seed_ratio (float): Ratio of seed nodes.
+
+    - infect_prob (float): Infection probability,  used in SIS, SIR or SI.
+
+    - recover_prob (float): Recovery probability, used in SIS or SIR.
+
+    - threshold (float): Threshold parameter for diffusion models, used in IC or LT.
+
+    Returns:
+
+    - dataset (dict): Dictionary containing ('adj_mat') adjacency matrix and ('diff_mat') diffusion matrices.
+
+    Example:
+
+    import os
+
+    curr_dir = os.getcwd()
+
+    from data.utils import load_dataset, diffusion_generation
+
+    data_name = 'karate'
+
+    graph = load_dataset(data_name, data_dir=curr_dir)
+
+    dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+    """
+    adj_mat = graph['adj_mat']
+    G = nx.from_scipy_sparse_array(adj_mat)
+    node_num = len(G.nodes())
+    seed_num = int(seed_ratio * node_num)
+    simulation = []
+
+    degree_list = list(G.degree())
+    degree_list.sort(key=lambda x: x[1], reverse=True)
+    top_nodes = [x[0] for x in degree_list[:int(len(degree_list) * 0.3)]]
+
+    for i in range(sim_num):
+        seed_vector = generate_seed_vector(top_nodes, seed_num, G)
+        inf_vec_all = torch.zeros(node_num)
+        config = mc.Configuration()
+        for k in range(repeat_step):
+            if diff_type == 'LT':
+                model = ep.ThresholdModel(G)
+                for n in G.nodes():
+                    config.add_node_configuration("threshold", n, threshold)
+            elif diff_type == 'IC':
+                model = ep.IndependentCascadesModel(G)
+                for e in G.edges():
+                    config.add_edge_configuration("threshold", e, threshold)
+            elif diff_type == 'SIS':
+                model = ep.SISModel(G)
+                config.add_model_parameter('beta', infect_prob)
+                config.add_model_parameter('lambda', recover_prob)
+            elif diff_type == 'SIR':
+                model = ep.SIRModel(G)
+                config.add_model_parameter('beta', infect_prob)
+                config.add_model_parameter('gamma', recover_prob)
+            elif diff_type == 'SI':
+                model = ep.SIModel(G)
+                config.add_model_parameter('beta', infect_prob)
+            else:
+                raise ValueError('Only IC, LT, SI, SIR and SIS are supported.')
+
+            config.add_model_initial_configuration("Infected", seed_vector)
+
+            model.set_initial_status(config)
+
+            iterations = model.iteration_bunch(time_step)
+
+            node_status = iterations[0]['status']
+
+            for j in range(1, len(iterations)):
+                node_status.update(iterations[j]['status'])
+
+            inf_vec = np.array(list(node_status.values()))
+            inf_vec[inf_vec == 2] = 1
+
+            inf_vec_all += inf_vec
+
+        inf_vec_all = inf_vec_all / repeat_step
+
+        simulation.append([seed_vector, inf_vec_all])
+
+    simulation = torch.Tensor(simulation).permute(0, 2, 1)
+
+    dataset = {'adj_mat': adj_mat, 'diff_mat': simulation}
+    return dataset
+
+
+def split_dataset(dataset, train_ratio: float = 0.6, seed: int = 0):
+    """
+    Split the dataset into training and testing sets.
+
+    Args:
+
+    - dataset (dict): Dictionary containing the dataset.
+
+    - train_ratio (float): Ratio of training data. Default is 0.6.
+
+    - seed (int): Random seed for reproducibility. Default is 0.
+
+    Returns:
+
+    - adj (scipy.sparse.csr_matrix): The adjacency matrix of the graph.
+
+    - train_dataset (torch.utils.data.dataset.Subset): The train dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
+
+    - test_dataset (torch.utils.data.dataset.Subset): The test dataset (number of simulations * number of graph nodes * 2(the first column is seed vector and the second column is diffusion vector)).
+
+    Example:
+
+    import os
+
+    curr_dir = os.getcwd()
+
+    from data.utils import load_dataset, diffusion_generation, split_dataset
+
+    data_name = 'karate'
+
+    graph = load_dataset(data_name, data_dir = curr_dir)
+
+    dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.1)
+
+    adj, train_dataset, test_dataset =split_dataset(dataset)
+    """
+    adj = dataset['adj_mat']
+    diff_mat = copy.deepcopy(dataset['diff_mat'])
+    all_num = len(diff_mat)
+    train_num = int(all_num * train_ratio)
+    test_num = all_num - train_num
+    train_diff_mat, test_diff_mat = torch.utils.data.random_split(diff_mat, [train_num, test_num],
+                                                                  generator=torch.Generator().manual_seed(seed))
+
+    return adj, train_diff_mat, test_diff_mat
```

### Comparing `GraphSL-0.8/GraphSL.egg-info/SOURCES.txt` & `GraphSL-0.9/GraphSL.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 GraphSL/Evaluation.py
 GraphSL/Prescribed.py
 GraphSL/__init__.py
+GraphSL/utils.py
 GraphSL.egg-info/PKG-INFO
 GraphSL.egg-info/SOURCES.txt
 GraphSL.egg-info/dependency_links.txt
 GraphSL.egg-info/requires.txt
 GraphSL.egg-info/top_level.txt
 GraphSL/GNN/__init__.py
 GraphSL/GNN/GCNSI/__init__.py
@@ -22,10 +23,8 @@
 GraphSL/GNN/IVGD/preprocessing.py
 GraphSL/GNN/IVGD/training.py
 GraphSL/GNN/IVGD/validity_net.py
 GraphSL/GNN/IVGD/model/MLP.py
 GraphSL/GNN/IVGD/model/__init__.py
 GraphSL/GNN/SLVAE/__init__.py
 GraphSL/GNN/SLVAE/main.py
-GraphSL/GNN/SLVAE/model.py
-GraphSL/data/__init__.py
-GraphSL/data/utils.py
+GraphSL/GNN/SLVAE/model.py
```

### Comparing `GraphSL-0.8/LICENSE` & `GraphSL-0.9/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Junxiang Wang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Junxiang Wang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `GraphSL-0.8/README.md` & `GraphSL-0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,138 +1,152 @@
-[![Documentation Status](https://readthedocs.org/projects/graphsl/badge/?version=latest)](https://graphsl.readthedocs.io/en/latest/?badge=latest)
-[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
-
-# GraphSL: Graph Source Localization Library
-
-This is the source code of the GraphSL (Graph Source Localization) library to support the research and development of the graph learning community.
-
-# Introduction
-
-## Problem Definition
-
-![image](SL_example.png)
-
-Graph diffusion is a fundamental task in graph learning, which aims to predict future graph cascade patterns given source nodes. Conversely, its inverse problem, graph source localization, though rarely explored, stands as an extremely important topic: it focuses on the detection of source nodes given their future graph cascade patterns. As illustrated in the above figure, graph diffusion seeks to predict the cascade pattern $\lbrace b,c,d,e \rbrace$ from a source node $b$, whereas graph source localization aims to identify source nodes $b$ from the cascade pattern $\lbrace b,c,d,e \rbrace$. 
-
-Graph source localization spans a broad spectrum of promising research and real-world applications. For instance, online social media platforms like Twitter and Facebook have been instrumental in disseminating rumors and misinformation with significant repercussions. Additionally, the rapid propagation of computer viruses across the Internet, infecting millions of computers, underscores the critical need for tracking their sources. Moreover, in smart grids, where isolated failures can trigger rolling blackouts leading to substantial financial losses, graph source localization plays a pivotal role. Hence, the graph source localization problem demands attention and extensive investigations from machine learning researchers.
-
-The GraphSL library includes six state-of-the-art approaches and eight benchmark datasets.
-
-
-## Approaches
-
-![image](overview.png)
-
- Existing graph source localization methods can be categorized into two groups: Prescribed methods and Graph Neural Networks (GNN)-based methods.
-
-Prescribed methods rely on hand-crafted rules and heuristics. For instance, LPSI propagates infection in networks and labels local peaks as source nodes. NetSleuth employed the Minimum Description Length principle to identify the optimal set of source nodes and virus propagation ripple. OJC identified a set of nodes (Jordan cover) that cover all observed infected nodes with the minimum radius.
-
-GNN-based methods learn rules from graph data in an end-to-end manner by capturing graph topology and neighboring information. For example, GCNSI utilized LPSI to enhance input and then applied Graph Convolutional Networks (GCN) for source identification; IVGD introduced a graph residual scenario to make existing graph diffusion models invertible, and it devises a new set of validity-aware layers to project inferred sources to feasible regions. SLVAE used forward diffusion estimation and deep generative models to approximate source distribution, leveraging prior knowledge for generalization under arbitrary diffusion patterns.
-
-## Benchmark Datasets
-
-|       Dataset      |  #Node |  #Edge | Average Degree | Seed-Diffusion Pairs |
-|:------------------:|:------:|:------:|:--------------:|:--------------------------:|
-|       Karate       |   34   |   78   |      4.588     |             No             |
-|      Dolphins      |   62   |   159  |      5.129     |             No             |
-|         Jazz       |   198  |  2,742 |     27.697     |             No             |
-| Network   Science  |  1,589 |  2,742 |      3.451     |             No             |
-|       Cora-ML      |  2,810 |  7,981 |      5.68      |             No             |
-|    Power   Grid    |  4,941 |  6,594 |      2.669     |             No             |
-|     Memetracker    |  7,884 | 47,911 |     12.154     |            Yes             |
-|        Digg        | 15,912 | 78,649 |      9.885     |            Yes             |
-
-
-Aside from methods, we also provide eight benchmark datasets to facilitate the research of the graph source localization problem. Memetracker and Digg provide Seed-Diffusion vector pairs. While others do not have such pairs, they can be generated by information diffusion simulations. All datasets are introduced as follows:
-
-1. Karate: Karate depicts the social ties among members of a university karate club.
-
-2. Dolphins: Dolphins represents a social network of bottlenose dolphins, with edges indicating frequent associations between dolphins.
-
-3. Jazz: Jazz illustrates a collaboration network among Jazz musicians, where edges signify instances of playing together in a band.
-
-4. Network Science: Network Science portrays a coauthorship network of scientists engaged in network theory and experimentation, with each edge representing co-authorship of a paper.
-
-5. Cora-ML: Cora-ML is a portal network of computer science research papers obtained through machine learning techniques.
-
-6. Power Grid: Power Grid delineates the topology network of the Western States Power Grid in the United States.
-
-7. Memetracker: Memetracker tracks frequently used phrases on news social media, and a small subset of the whole Memetracker network was retrieved here.
-
-8. Digg: Digg showcases a reply network within social news, and a small subset of the whole Digg network was retrieved here.
-
-# Installation
-
-#### Installation via PyPI
-```bash
-pip install GraphSL
-```
-
-#### Installation via GitHub
-Clone the repo from [here](https://github.com/xianggebenben/GraphSL) (this repo).
-
-Install requirements:
-```bash
-pip install -r requirements.txt
-```
-
-# Quickstart
-``` python
-
-   from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-   from GraphSL.Prescribed import LPSI, NetSleuth, OJC
-   from GraphSL.GNN.GCNSI.main import GCNSI
-   from GraphSL.GNN.IVGD.main import IVGD
-   from GraphSL.GNN.SLVAE.main import SLVAE
-   data_name = 'karate'  # 'karate', 'dolphins', 'jazz', 'netscience', 'cora_ml', 'power_grid', , 'meme8000', 'digg16000'
-   graph = load_dataset(data_name)
-   if data_name not in ['meme8000', 'digg16000']:
-       dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.3)
-   else:
-       dataset = graph
-   adj, train_dataset, test_dataset =split_dataset(dataset)
-   lpsi = LPSI()
-   alpha, thres, auc, f1, pred =lpsi.train(adj, train_dataset)
-   print("LPSI:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric=lpsi.test(adj, test_dataset, alpha, thres)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   netSleuth = NetSleuth()
-   k, auc, f1=netSleuth.train(adj, train_dataset)
-   print("NetSleuth:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric = netSleuth.test(adj, test_dataset, k)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   ojc = OJC()
-   Y, auc, f1 =ojc.train(adj, train_dataset)
-   print("OJC:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric=ojc.test(adj, test_dataset, Y)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   gcnsi = GCNSI()
-   gcnsi_model, thres, auc, f1, pred =gcnsi.train(adj, train_dataset)
-   print("GCNSI:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric = gcnsi.test(adj, test_dataset, gcnsi_model, thres)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   ivgd = IVGD()
-   diffusion_model = ivgd.train_diffusion(adj, train_dataset)
-   ivgd_model, thres, auc, f1, pred =ivgd.train(adj, train_dataset, diffusion_model)
-   print("IVGD:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric = ivgd.test(test_dataset, diffusion_model, ivgd_model, thres)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   slave = SLVAE()
-   slvae_model, seed_vae_train, thres, auc, f1, pred = slave.train(adj, train_dataset)
-   print("SLVAE:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric = slave.infer(test_dataset, slvae_model, seed_vae_train, thres)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-```
-
-# Documentation
-
-Official documentation, including a detailed [API reference](https://graphsl.readthedocs.io/en/latest/modules.html), is available on [Read the Docs](https://graphsl.readthedocs.io/en/latest/#).
-
-# Contact
-
-Feel free to Email Junxiang Wang (junxiang.wang@alumni.emory.edu) if you have any questions.
+[![Documentation Status](https://readthedocs.org/projects/graphsl/badge/?version=latest)](https://graphsl.readthedocs.io/en/latest/?badge=latest)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![PyPI version](https://badge.fury.io/py/graphsl.svg)](https://badge.fury.io/py/graphsl)
+[![Downloads](https://pepy.tech/badge/graphsl)](https://pepy.tech/project/graphsl)
+
+
+# GraphSL: Graph Source Localization Library
+
+This is the source code of the GraphSL (Graph Source Localization) library, in order to support the research and development of the graph learning community.
+
+# Introduction
+
+## Problem Definition
+
+![image](SL_example.png)
+
+Graph diffusion is a fundamental task in graph learning, which aims to predict future graph cascade patterns given source nodes. Conversely, its inverse problem, graph source localization, though rarely explored, stands as an extremely important topic: it focuses on the detection of source nodes given their future graph cascade patterns. As illustrated in the above figure, graph diffusion seeks to predict the cascade pattern $\lbrace b,c,d,e \rbrace$ from a source node $b$, whereas graph source localization aims to identify source nodes $b$ from the cascade pattern $\lbrace b,c,d,e \rbrace$. 
+
+Graph source localization spans a broad spectrum of promising research and real-world applications. For instance, online social media platforms like Twitter and Facebook have been instrumental in disseminating rumors and misinformation with significant repercussions. Additionally, the rapid propagation of computer viruses across the Internet, infecting millions of computers, underscores the critical need for tracking their sources. Moreover, in smart grids, where isolated failures can trigger rolling blackouts leading to substantial financial losses, graph source localization plays a pivotal role. Hence, the graph source localization problem demands attention and extensive investigations from machine learning researchers.
+
+The GraphSL library includes six state-of-the-art approaches and eight benchmark datasets.
+
+
+## Approaches
+
+![image](overview.png)
+
+ Existing graph source localization methods can be categorized into two groups: Prescribed methods and Graph Neural Networks (GNN)-based methods.
+
+Prescribed methods rely on hand-crafted rules and heuristics. For instance, LPSI propagates infection in networks and labels local peaks as source nodes. NetSleuth employed the Minimum Description Length principle to identify the optimal set of source nodes and virus propagation ripple. OJC identified a set of nodes (Jordan cover) that cover all observed infected nodes with the minimum radius.
+
+GNN-based methods learn rules from graph data in an end-to-end manner by capturing graph topology and neighboring information. For example, GCNSI utilized LPSI to enhance input and then applied Graph Convolutional Networks (GCN) for source identification; IVGD introduced a graph residual scenario to make existing graph diffusion models invertible, and it devises a new set of validity-aware layers to project inferred sources to feasible regions. SLVAE used forward diffusion estimation and deep generative models to approximate source distribution, leveraging prior knowledge for generalization under arbitrary diffusion patterns.
+
+## Benchmark Datasets
+
+|       Dataset      |  #Node |  #Edge | Average Degree | Seed-Diffusion Pairs |
+|:------------------:|:------:|:------:|:--------------:|:--------------------------:|
+|       Karate       |   34   |   78   |      4.588     |             No             |
+|      Dolphins      |   62   |   159  |      5.129     |             No             |
+|         Jazz       |   198  |  2,742 |     27.697     |             No             |
+| Network   Science  |  1,589 |  2,742 |      3.451     |             No             |
+|       Cora-ML      |  2,810 |  7,981 |      5.68      |             No             |
+|    Power   Grid    |  4,941 |  6,594 |      2.669     |             No             |
+|     Memetracker    |  7,884 | 47,911 |     12.154     |            Yes             |
+|        Digg        | 15,912 | 78,649 |      9.885     |            Yes             |
+
+
+Aside from methods, we also provide eight benchmark datasets to facilitate the research of the graph source localization problem. Memetracker and Digg provide Seed-Diffusion vector pairs. While others do not have such pairs, they can be generated by information diffusion simulations. All datasets are introduced as follows:
+
+1. Karate: Karate depicts the social ties among members of a university karate club.
+
+2. Dolphins: Dolphins represents a social network of bottlenose dolphins, with edges indicating frequent associations between dolphins.
+
+3. Jazz: Jazz illustrates a collaboration network among Jazz musicians, where edges signify instances of playing together in a band.
+
+4. Network Science: Network Science portrays a coauthorship network of scientists engaged in network theory and experimentation, with each edge representing co-authorship of a paper.
+
+5. Cora-ML: Cora-ML is a portal network of computer science research papers obtained through machine learning techniques.
+
+6. Power Grid: Power Grid delineates the topology network of the Western States Power Grid in the United States.
+
+7. Memetracker: Memetracker tracks frequently used phrases on news social media, and a small subset of the whole Memetracker network was retrieved here.
+
+8. Digg: Digg showcases a reply network within social news, and a small subset of the whole Digg network was retrieved here.
+
+# Installation
+
+First, install GraphSL using pip:
+
+
+    pip install GraphSL
+
+Or, clone the repo from https://github.com/xianggebenben/GraphSL and install requirements:
+
+    pip install -r requirements.txt
+
+Second, download the data folder of the repo from https://github.com/xianggebenben/GraphSL, which contains eight datasets.
+
+
+# Quickstart
+
+Now, you can import and use GraphSL in your Python code. Please make sure your Python code and the data folder are in the same directory:
+
+``` python
+from GraphSL.utils import load_dataset, diffusion_generation, split_dataset
+from GraphSL.Prescribed import LPSI, NetSleuth, OJC
+from GraphSL.GNN.GCNSI.main import GCNSI
+from GraphSL.GNN.IVGD.main import IVGD
+from GraphSL.GNN.SLVAE.main import SLVAE
+data_name = 'karate'  # 'karate', 'dolphins', 'jazz', 'netscience', 'cora_ml', 'power_grid', , 'meme8000', 'digg16000'
+graph = load_dataset(data_name)
+if data_name not in ['meme8000', 'digg16000']:
+ dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.3)
+else:
+ dataset = graph
+adj, train_dataset, test_dataset =split_dataset(dataset)
+lpsi = LPSI()
+alpha, thres, auc, f1, pred =lpsi.train(adj, train_dataset)
+print("LPSI:")
+print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+metric=lpsi.test(adj, test_dataset, alpha, thres)
+print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+netSleuth = NetSleuth()
+k, auc, f1=netSleuth.train(adj, train_dataset)
+print("NetSleuth:")
+print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+metric = netSleuth.test(adj, test_dataset, k)
+print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+ojc = OJC()
+Y, auc, f1 =ojc.train(adj, train_dataset)
+print("OJC:")
+print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+metric=ojc.test(adj, test_dataset, Y)
+print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+gcnsi = GCNSI()
+gcnsi_model, thres, auc, f1, pred =gcnsi.train(adj, train_dataset)
+print("GCNSI:")
+print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+metric = gcnsi.test(adj, test_dataset, gcnsi_model, thres)
+print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+ivgd = IVGD()
+diffusion_model = ivgd.train_diffusion(adj, train_dataset)
+ivgd_model, thres, auc, f1, pred =ivgd.train(adj, train_dataset, diffusion_model)
+print("IVGD:")
+print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+metric = ivgd.test(test_dataset, diffusion_model, ivgd_model, thres)
+print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+slave = SLVAE()
+slvae_model, seed_vae_train, thres, auc, f1, pred = slave.train(adj, train_dataset)
+print("SLVAE:")
+print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+metric = slave.infer(test_dataset, slvae_model, seed_vae_train, thres)
+print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+```
+
+# Documentation
+
+Official documentation, including a detailed [API reference](https://graphsl.readthedocs.io/en/latest/modules.html), is available on [Read the Docs](https://graphsl.readthedocs.io/en/latest/#).
+
+# Citation
+If you use this package in your research, please consider citing our work as follows:
+```bibtex
+@article{wang2024joss,
+  year = {2024},
+  author = {Wang Junxiang, Zhao Liang},
+  title = {GraphSL: A Open-Source Library for Graph Source Localization Approaches and Benchmark Datasets},
+  journal = {preprint}
+}
+```
+# Contact
+
+Feel free to Email Junxiang Wang (junxiang.wang@alumni.emory.edu) if you have any questions.
```

