# Comparing `tmp/activetigger-0.0.9.tar.gz` & `tmp/activetigger-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activetigger-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "activetigger-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `activetigger-0.0.9.tar` & `activetigger-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      202 2024-03-20 20:46:47.257197 activetigger-0.0.9/.gitignore
--rw-r--r--   0        0        0     1119 2024-03-20 07:40:20.123595 activetigger-0.0.9/LICENSE
--rw-r--r--   0        0        0     1256 2024-03-20 07:40:20.123595 activetigger-0.0.9/README.md
--rw-r--r--   0        0        0       52 2024-03-20 20:47:28.385533 activetigger-0.0.9/activetigger/__init__.py
--rw-r--r--   0        0        0      140 2024-03-20 17:03:01.443605 activetigger-0.0.9/activetigger/__main__.py
--rw-r--r--   0        0        0    27852 2024-03-20 09:11:24.671302 activetigger-0.0.9/activetigger/api.py
--rw-r--r--   0        0        0     2388 2024-03-20 07:40:20.123595 activetigger-0.0.9/activetigger/datamodels.py
--rw-r--r--   0        0        0     4578 2024-03-20 07:40:20.123595 activetigger-0.0.9/activetigger/functions.py
--rw-r--r--   0        0        0    32818 2024-03-20 18:11:21.230087 activetigger-0.0.9/activetigger/models.py
--rw-r--r--   0        0        0    41813 2024-03-20 20:44:25.356028 activetigger-0.0.9/activetigger/server.py
--rw-r--r--   0        0        0    56953 2024-03-20 07:40:20.127595 activetigger-0.0.9/activetigger/widget.py
--rw-r--r--   0        0        0      430 2024-03-20 09:12:27.407943 activetigger-0.0.9/html/welcome.html
--rw-r--r--   0        0        0   541841 2024-03-20 07:40:20.131595 activetigger-0.0.9/img/active_tigger.png
--rw-r--r--   0        0        0      819 2024-03-20 17:34:40.961794 activetigger-0.0.9/pyproject.toml
--rw-r--r--   0        0        0       35 2024-02-15 16:22:17.128105 activetigger-0.0.9/pytest.ini
--rw-r--r--   0        0        0      554 2024-03-20 17:34:30.865686 activetigger-0.0.9/requirements.txt
--rw-r--r--   0        0        0      867 2024-03-20 20:47:43.497657 activetigger-0.0.9/setup.py
--rw-r--r--   0        0        0       89 2024-02-15 16:22:17.128105 activetigger-0.0.9/tests/test_api.py
--rw-r--r--   0        0        0     2098 2024-03-20 07:40:20.135595 activetigger-0.0.9/tests/test_project.py
--rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 activetigger-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      225 2024-04-29 11:59:08.825555 activetigger-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1119 2024-02-26 10:50:38.000000 activetigger-0.1.0/LICENSE
+-rw-r--r--   0        0        0       47 2024-03-20 21:05:20.000000 activetigger-0.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     1532 2024-04-29 12:01:45.858393 activetigger-0.1.0/README.md
+-rw-r--r--   0        0        0       52 2024-04-29 12:00:56.767568 activetigger-0.1.0/activetigger/__init__.py
+-rw-r--r--   0        0        0      140 2024-03-20 17:03:01.000000 activetigger-0.1.0/activetigger/__main__.py
+-rw-r--r--   0        0        0    36036 2024-04-29 09:39:06.960074 activetigger-0.1.0/activetigger/api.py
+-rw-r--r--   0        0        0     3458 2024-04-28 14:01:42.211751 activetigger-0.1.0/activetigger/datamodels.py
+-rw-r--r--   0        0        0     7081 2024-04-28 14:03:22.302180 activetigger-0.1.0/activetigger/functions.py
+-rw-r--r--   0        0        0      430 2024-03-20 09:12:27.000000 activetigger-0.1.0/activetigger/html/welcome.html
+-rw-r--r--   0        0        0  1167848 2024-04-19 14:23:17.022833 activetigger-0.1.0/activetigger/img/active_tigger.png
+-rw-r--r--   0        0        0    33304 2024-04-28 14:07:36.731438 activetigger-0.1.0/activetigger/models.py
+-rw-r--r--   0        0        0    45002 2024-04-29 09:50:29.740629 activetigger-0.1.0/activetigger/server.py
+-rw-r--r--   0        0        0    61193 2024-04-29 10:16:28.176488 activetigger-0.1.0/activetigger/widget.py
+-rw-r--r--   0        0        0      196 2024-04-29 09:50:11.156824 activetigger-0.1.0/config.yaml
+-rw-r--r--   0        0        0      838 2024-03-27 17:01:50.295115 activetigger-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-02-09 19:50:15.000000 activetigger-0.1.0/pytest.ini
+-rw-r--r--   0        0        0      575 2024-04-29 10:19:50.297560 activetigger-0.1.0/requirements.txt
+-rw-r--r--   0        0        0       89 2024-02-09 14:40:46.000000 activetigger-0.1.0/tests/test_api.py
+-rw-r--r--   0        0        0     2098 2024-02-18 21:23:56.000000 activetigger-0.1.0/tests/test_project.py
+-rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 activetigger-0.1.0/PKG-INFO
```

### Comparing `activetigger-0.0.9/LICENSE` & `activetigger-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `activetigger-0.0.9/activetigger/models.py` & `activetigger-0.1.0/activetigger/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import pandas as pd
-from pandas import DataFrame, Series
+from pandas import DataFrame
 import logging
 import json
 import os
 from pathlib import Path
 import torch
 import numpy as np
 import shutil
 from transformers import AutoModelForSequenceClassification, AutoTokenizer
 from transformers import Trainer, TrainingArguments, TrainerCallback
 import datasets
 from sklearn.preprocessing import StandardScaler
 from sklearn.linear_model import LogisticRegression
-from sklearn.naive_bayes import MultinomialNB, BernoulliNB
+from sklearn.naive_bayes import MultinomialNB
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.metrics import precision_score, f1_score, accuracy_score, recall_score
-from sklearn.model_selection import cross_val_score, KFold, cross_val_predict
+from sklearn.model_selection import KFold, cross_val_predict
 from multiprocessing import Process
 from datetime import datetime
 import pickle
+from pydantic import ValidationError
+import activetigger.functions as functions
+from activetigger.datamodels import LiblinearParams, KnnParams, RandomforestParams, LassoParams, Multi_naivebayesParams, BertParams
+
 
 logging.basicConfig(filename = "log",
                             format='%(asctime)s %(message)s',
                             encoding='utf-8', level=logging.DEBUG)
 
 
 class BertModel():
@@ -109,15 +113,15 @@
             Y_pred = df["prediction"]
             Y = df["labels"]
             f = df.apply(lambda x : x["prediction"] != x["labels"], axis=1)
             r["f1_micro"] = f1_score(Y, Y_pred, average = "micro"),
             r["f1_macro"] = f1_score(Y, Y_pred, average = "macro"),
             r["f1_weighted"] = f1_score(Y, Y_pred, average = "weighted"),
             r["f1"] = list(f1_score(Y, Y_pred, average = None)),
-            r["precision"] = list(precision_score(list(Y), list(Y_pred), average="micro")),
+            r["precision"] = precision_score(list(Y), list(Y_pred), average="micro"),
             r["recall"] = list(recall_score(list(Y), list(Y_pred), average=None)),
             r["accuracy"] = accuracy_score(Y, Y_pred),
             r["false_prediction"] = df[f][["text","labels","prediction"]].to_dict()
 
             with open(self.path / "statistics.json","w") as f:
                 json.dump(r,f)
         
@@ -143,14 +147,15 @@
         if gpu:
             self.model.cuda()
 
         # Start prediction with batches
         predictions = []
         logging.info(f"Start prediction with {len(df)} entries")
         for chunk in [df[col_text][i:i+batch] for i in range(0,df.shape[0],batch)]:
+            print("Next chunck prediction")
             chunk = self.tokenizer(list(chunk), 
                             padding=True, 
                             truncation=True, 
                             max_length=512, 
                             return_tensors="pt")
             if gpu:
                 chunk = chunk.to("cuda")
@@ -171,15 +176,15 @@
         # Calculate entropy
         entropy = -1 * (pred * np.log(pred)).sum(axis=1)
         pred["entropy"] = entropy
 
         # Calculate label
         pred["prediction"] = pred.drop(columns="entropy").idxmax(axis=1)
 
-        # Write the file
+        # Write the file in parquet
         pred.to_parquet(self.path / "predict.parquet")
 
         return pred
 
 class BertModels():
     """
     Managing bertmodel training
@@ -232,37 +237,36 @@
         + if prediction available
         + compression if available / launch it
         """
         r:dict = {}
         if self.path.exists(): #if bert models have been trained
             all_files = os.listdir(self.path)
             trained = [i for i in all_files if os.path.isdir(self.path / i) and (self.path / i / "finished").exists()]
-            #trained = [i for i in trained if i[0]!="_"] #skip temporary training
             for i in trained:
                 predict = False
                 compressed = False
                 # test if prediction available
                 if (self.path / i / "predict.parquet").exists(): 
                     predict = True
                 # test if compression available
                 if (self.path / f"{i}.tar.gz").exists():
                     compressed = True
                 else :
                     self.start_compression(i)
                 scheme = i.split("__")[-1] #scheme after __
                 if not scheme in r: 
                     r[scheme] = {}
-                r[scheme][i] = [predict, compressed]
+                r[scheme][i] = {"predicted":predict, 
+                                "compressed":compressed}
         return r
     
     def training(self) -> dict:
         """
         Currently under training
         """
-        #return {u:self.processes[u][0].status for u in self.processes}
         return {u:self.processes[u][0].name for u in self.processes if self.processes[u][0].status == "training"}
 
     def delete(self, bert_name:str) -> dict:
         """
         Delete bert model
         """
         if not (self.path / bert_name).exists():
@@ -290,26 +294,31 @@
         """
 
         # Check if there is no other competing processes
         # For the moment : 1 active process by user
         if user in self.processes:
             return {"error":"processes already launched, cancel it before"}
 
-        # Set default parameters if needed
+        # set default parameters if needed
         if base_model is None:
             base_model = "almanach/camembert-base"
         if params is None:
             params = self.params_default
         if test_size is None:
             test_size = 0.2
+        # test json parameters
+        try:
+            e = BertParams(**params)
+        except ValidationError as e:
+            return {"error":e.json()}
 
         # name integrating the scheme
         name = f"{name}__{scheme}"
 
-        # Launch as a independant process
+        # launch as a independant process
         args = {
                 "path":self.path,
                 "name":name,
                 "df":df,
                 "col_label":col_label,
                 "col_text":col_text,
                 "base_model":base_model,
@@ -351,16 +360,17 @@
         self.processes[user] = [b,process]
         return {"success":"bert model predicting"}
 
     def start_compression(self, name):
         """
         Compress bertmodel as a separate process
         """
+        print(self.path / name, 'gztar', self.path)
         process = Process(target=shutil.make_archive, 
-                          args = (self.path / name, 'gztar', self.path))
+                          args = (self.path / name, 'gztar', self.path / name))
         process.start()
         print("starting compression")
 
     def train_bert(self,
                path:Path,
                name:str,
                df:DataFrame,
@@ -502,22 +512,26 @@
 
         # save log history of the training for statistics
         with open(current_path  / "log_history.txt", "w") as f:
             json.dump(trainer.state.log_history, f)
 
         return True
     
-    def stop_user_training(self,user:str):
+    def stop_user_process(self,user:str):
         """
         Stop the process of an user
         """
         if not user in self.processes:
             return {"error":"no current processes"}
         self.processes[user][1].terminate() # end process
-        shutil.rmtree(self.processes[user][0].path) #delete files
+
+        # delete files in case of training
+        b = self.processes[user][0]
+        if b.status == "training":
+            shutil.rmtree(self.processes[user][0].path)
         del self.processes[user] # delete process
         return {"success":"process terminated"}
     
     def rename(self, former_name:str, new_name:str):
         """
         Rename a model (copy it)
         """
@@ -529,16 +543,14 @@
             return {"error":"model not trained completly"}
 
         # keep the scheme information
         if not "__" in new_name:
             new_name = new_name + "__" + former_name.split("__")[-1]
 
         os.rename(self.path / former_name, self.path / new_name)
-
-        #shutil.copytree(self.path / former_name, self.path / new_name)
         return {"success":"model renamed"}
             
     def get(self, name:str, lazy = False)-> BertModel|None:
         """
         Get a model
         """
         if not (self.path / name).exists():
@@ -561,67 +573,101 @@
             p = self.processes[u][1]
             # test if process completed (training)
             if (b.status == "training") and (not p.is_alive()):
                 to_del.append(b.name)
             # test if process completed (predicting)
             if (b.status == "predicting") and (not p.is_alive()):
                 to_del.append(b.name)
-            print(to_del)
         # Update the current active processes
         self.processes = {u:self.processes[u] for u in self.processes if self.processes[u][0].name not in to_del}
-        #self.processes = [b for b in self.processes if b[0].name not in to_del]
         return True
     
     def export_prediction(self, name:str, format:str|None = None):
         """
         Export predict file if exists
         """
-        file_name = f"predict.csv"
-        if not (self.path / name / file_name).exists():
+        file_name = f"predict.parquet"
+        path = self.path / name / file_name
+
+        # change format if needed
+        if format == "csv":
+            df = pd.read_parquet(path)
+            print(df)
+            file_name = f"predict.csv"
+            path = self.path / name / file_name
+            df.to_csv(path)
+
+        print(path)
+        if not path.exists():
             return {"error":"file does not exist"}
-        return file_name, self.path / name / file_name
+        
+        r =  {"name":file_name, 
+              "path":path}
+        return r
 
     def export_bert(self, name:str):
         """
         Export bert archive if exists
         """
         file_name = f"{name}.tar.gz"
         if not (self.path / file_name).exists():
             return {"error":"file does not exist"}
-        return file_name, self.path / file_name
+        r =  {"name":file_name, 
+              "path":self.path / file_name}
+        return r
         
- 
 class SimpleModels():
     """
     Managing simplemodels
     - define available models
     - save a simplemodel/user
     - train simplemodels
     """
+    # Models and default parameters
     available_models = {
         "liblinear": {
                 "cost":1
             },
         "knn" : {
                 "n_neighbors":3
             },
         "randomforest": {
                 "n_estimators":500,
                 "max_features":None
                 },
         "lasso": {
                 "C":32
+                },
+        "multi_naivebayes":
+                {
+                    "alpha":1,
+                    "fit_prior":True,
+                    "class_prior":None
                 }
             }
-    
-    def __init__(self, path:Path):
-        self.existing:dict = {}
-        self.save_file:str = "simplemodels.pickle"
-        self.path:Path = path
-        self.loads()
+
+    # To validate JSON
+    validation = {
+        "liblinear": LiblinearParams,
+        "knn": KnnParams,
+        "randomforest": RandomforestParams,
+        "lasso": LassoParams,
+        "multi_naivebayes":Multi_naivebayesParams
+    }
+    
+    def __init__(self, path:Path, executor):
+        """
+        Init Simplemodels class
+        """
+        self.existing:dict = {} # computed simplemodels
+        self.computing:dict = {} # curently under computation
+        self.path:Path = path # path to operate
+        self.executor = executor # access to executor for multiprocessing
+        self.save_file:str = "simplemodels.pickle" # file to save current state
+        self.loads() # load existing simplemodels
 
     def __repr__(self) -> str:
         return str(self.available())
 
     def available(self):
         """
         Available simplemodels
@@ -633,15 +679,24 @@
                 sm = self.existing[u][s]
                 r[u][s] = {"name":sm.name, 
                            "params":sm.model_params,
                            "features":sm.features,
                            "statistics":sm.statistics
                            }
         return r
-        
+
+    def training(self):
+        """
+        Training simplemodels
+        """
+        r = {}
+        for u in self.computing:
+            r[u] = list(self.computing[u].keys())
+        return r   
+
     def exists(self, user:str, scheme:str):
         """
         Test if a simplemodel exists for a user/scheme
         """
         if user in self.existing:
             if scheme in self.existing[user]:
                 return True
@@ -680,24 +735,38 @@
     
         # data for training
         Y = df[col_label]
         X = df[col_predictors]
         labels = Y.unique()
         
         return X, Y, labels
-    
-    def fit_model(self, name, X, Y, model_params = None):
+
+    def standardize(self,df):
         """
-        Fit model
-        TODO: add naive bayes
+        Apply standardization
         """
-        # only keep tagged Y
-        f = Y.notnull()
-        X = X[f]
-        Y = Y[f]
+        scaler = StandardScaler()
+        df_stand = scaler.fit_transform(df)
+        return pd.DataFrame(df_stand,columns=df.columns,index=df.index)
+
+    def add_simplemodel(self, 
+                        user, 
+                        scheme,
+                        features,
+                        name, 
+                        df, 
+                        col_labels,
+                        col_features,
+                        standardize,
+                        model_params:dict|None = None):
+        """
+        A a new simplemodel for a user and a scheme
+        """
+        X, Y, labels = self.load_data(df, col_labels, col_features, standardize)
+
         # default parameters
         if model_params is None:
             model_params = self.available_models[name]
 
         # Select model
         if name == "knn":
             model = KNeighborsClassifier(n_neighbors=model_params["n_neighbors"])
@@ -718,46 +787,28 @@
             #Number of variables randomly sampled as candidates at each split: 
             # it is “mtry” in R and it is “max_features” Python
             #  The sample.fraction parameter specifies the fraction of observations to be used in each tree
             model = RandomForestClassifier(n_estimators=model_params["n_estimators"], 
                                                 random_state=42,
                                                 max_features=model_params["max_features"])
 
-        # Fit modelmax_features
-        model.fit(X, Y)
-        return model, model_params
-
-    def standardize(self,df):
-        """
-        Apply standardization
-        """
-        scaler = StandardScaler()
-        df_stand = scaler.fit_transform(df)
-        return pd.DataFrame(df_stand,columns=df.columns,index=df.index)
-
-    def add_simplemodel(self, 
-                        user, 
-                        scheme,
-                        features,
-                        name, 
-                        df, 
-                        col_labels,
-                        col_features,
-                        standardize,
-                        model_params:dict|None = None):
-        """
-        A a new simplemodel for a user and a scheme
-        """
-        X, Y, labels = self.load_data(df, col_labels, col_features, standardize)
-        model, model_params = self.fit_model(name, X, Y, model_params)
-        sm = SimpleModel(name, X, Y, labels, model, features, standardize, model_params)
-        if not user in self.existing:
-            self.existing[user] = {}
-        self.existing[user][scheme] = sm
-        self.dumps() #save pickle
+        if name == "multi_naivebayes":
+            # Only with dtf or tfidf for features
+            # TODO: calculate class prior for docfreq & termfreq
+            model = MultinomialNB(alpha=model_params["alpha"],
+                                    fit_prior=model_params["fit_prior"],
+                                    class_prior=model_params["class_prior"])
+
+        # launch the compuation (model + statistics) as a future process
+        # TODO: refactore the SimpleModel class / move to API the executor call ?
+        future_result = self.executor.submit(functions.fit_model, model=model, X=X, Y=Y, labels=labels)
+        sm = SimpleModel(name, user, X, Y, labels, "computing", features, standardize, model_params)
+        if not user in self.computing:
+            self.computing[user] = {}
+        self.computing[user][scheme] = {"future":future_result, "sm":sm}
 
     def dumps(self):
         """
         Dumps all simplemodels to a pickle
         """
         with open(self.path / self.save_file, 'wb') as file:
             pickle.dump(self.existing, file)
@@ -771,45 +822,60 @@
         with open(self.path / self.save_file, 'rb') as file:
             self.existing = pickle.load(file)
         return True
 
 class SimpleModel():
     def __init__(self,
                  name: str,
+                 user: str,
                  X: DataFrame,
                  Y: DataFrame,
                  labels: list,
                  model,
                  features:list,
                  standardize: bool,
                  model_params: dict|None
                  ) -> None:
+        """
+        Define a specific Simplemodel with parameters
+        TODO : add timestamp ?
+        TODO : not sure that statistics function are still usefull since it is calculated during the fit
+        """
         self.name = name
+        self.user = user
         self.features = features
         self.X = X
         self.Y = Y
         self.labels = labels
-        self.model = model
         self.model_params = model_params
-        self.proba = self.compute_proba(model, X)
         self.standardize = standardize
-        self.statistics = self.compute_statistics(model, X, Y, labels)
-        self.cv10 = self.compute_10cv(model, X, Y)
-        print(self.statistics)
+        self.model = model
+        self.proba = None
+        self.statistics = None
+        self.cv10 = None
+        if not type(model) is str: #TODO : tester si c'est un modèle
+            self.proba = self.compute_proba(model, X)
+            self.statistics = self.compute_statistics(model, X, Y, labels)
+            self.cv10 = self.compute_10cv(model, X, Y)
 
     def json(self):
         """
         Return json representation
         """
         return {
             "name":str(self.name),
             "features":list(self.features),
             "labels":list(self.labels),
             "params":dict(self.model_params)
         }
+    
+    def compute_stats(self):
+        self.proba = self.compute_proba(self.model, self.X)
+        self.statistics = self.compute_statistics(self.model, self.X, self.Y, self.labels)
+        self.cv10 = self.compute_10cv(self.model, self.X, self.Y)
 
     def compute_proba(self, model, X):
         """
         Compute proba + entropy
         """
         proba = model.predict_proba(X)
         proba = pd.DataFrame(proba, 
@@ -875,49 +941,8 @@
         Y_pred = cross_val_predict(model, X, Y, cv=kf)
         weighted_f1 = f1_score(Y, Y_pred,average = "weighted")
         accuracy = accuracy_score(Y, Y_pred)
         macro_f1 = f1_score(Y, Y_pred,average = "macro")
         r = {"weighted_f1":round(weighted_f1,3), 
              "macro_f1":round(macro_f1,3),
              "accuracy":round(accuracy,3)}
-        return r
-
-#         self.available_models = {
-#                 #"simplebayes": {
-#                 #        "distribution":"multinomial",
-#                 #        "smooth":1,
-#                 #        "prior":"uniform"
-#                 #    },            C = self.model_params["C"])
-#         if self.name == "naivebayes":
-#             if not "distribution" in self.model_params:
-#                 raise TypeError("Missing distribution parameter for naivebayes")
-            
-#         # only dfm as predictor
-#             alpha = 1
-#             if "smooth" in self.model_params:
-#                 alpha = self.model_params["smooth"]
-#             fit_prior = True
-#             class_prior = None
-#             if "prior" in self.model_params:
-#                 if self.model_params["prior"] == "uniform":
-#                     fit_prior = True
-#                     class_prior = None
-#                 if self.model_params["prior"] == "docfreq":
-#                     fit_prior = False
-#                     class_prior = None #TODO
-#                 if self.model_params["prior"] == "termfreq":
-#                     fit_prior = False
-#                     class_prior = None #TODO
- 
-#             if self.model_params["distribution"] == "multinomial":
-#                 self.model = MultinomialNB(alpha=alpha,
-#                                            fit_prior=fit_prior,
-#                                            class_prior=class_prior)
-#             elif self.model_params["distribution"] == "bernouilli":
-#                 self.model = BernoulliNB(alpha=alpha,
-#                                            fit_prior=fit_prior,
-#                                            class_prior=class_prior)
-#             self.model_params = {
-#                                     "distribution":self.model_params["distribution"],
-#                                     "smooth":alpha,
-#                                     "prior":"uniform"
-#                                 }
+        return r
```

### Comparing `activetigger-0.0.9/activetigger/server.py` & `activetigger-0.1.0/activetigger/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import yaml
+import yaml # type: ignore
 from datetime import datetime
 import concurrent.futures
 from pathlib import Path
 import sqlite3
 import re
 import json
 import shutil
@@ -12,53 +12,78 @@
 from pandas import DataFrame, Series
 from fastapi import UploadFile # type: ignore
 from fastapi.encoders import jsonable_encoder # type: ignore
 from datetime import datetime, timedelta, timezone
 from jose import jwt # type: ignore
 import activetigger.functions as functions
 from activetigger.models import BertModels, SimpleModels
-from activetigger.datamodels import ProjectModel, SchemesModel, SchemeModel, SimpleModelModel, UserInDB
+from activetigger.datamodels import ProjectModel, SchemeModel, SimpleModelModel, UserInDB
+from pydantic import ValidationError
 
 class Server():
     """
-    Server to manage projects
+    Server to manage backend
     """
+    # files name
     db_name:str =  "activetigger.db"
     features_file:str = "features.parquet"
     labels_file:str = "labels.parquet"
     data_file:str = "data.parquet"
     test_file:str = "test.parquet"
     default_user:str = "root"
     ALGORITHM = "HS256"
+    n_workers = 2
 
     def __init__(self) -> None:
         """
         Start the server
         """
         self.time_start:datetime = datetime.now()
 
         # YAML configuration file
         with open('config.yaml') as f:
             config = yaml.safe_load(f)
         self.path = Path(config["path"])
+        self.path_fastext = Path(config["path_fasttext"])
         self.SECRET_KEY = config["secret_key"] #generate it automatically ?
-        
+
+        # create the database
         self.db = self.path / self.db_name
+        if not self.db.exists():
+            self.create_db()
 
-        # Activity of the server
+        # activity of the server
         self.projects: dict = {}
         self.processes:list = []
-        self.executor = concurrent.futures.ProcessPoolExecutor(max_workers=2)
+        self.executor = concurrent.futures.ProcessPoolExecutor(max_workers=self.n_workers)
 
-        # Create the database in the first launch
-        if not self.db.exists():
-            self.create_db()
+        # update users from YAML config file
+        existing = self.existing_users()
+        current = config["users"]
+        for u in current:
+            if not u in existing:
+                self.add_user(u, current[u])
+        for u in existing:
+            if (not u in current) and u != self.default_user:
+                self.delete_user(u)
+                
+    def recreate_executor(self):
+        """
+        Recreate future executor
+        """
+        del self.executor
+        self.executor = concurrent.futures.ProcessPoolExecutor(max_workers=self.n_workers)
 
     def __del__(self): 
-        print("Closing the server")
+        """
+        Close the server
+        """
+        print("Ending the server")
+        self.executor.shutdown()
+        print("Server off")
             
     def create_db(self) -> None:
         """
         Initialize the database
         """
 
         # create the repertory if needed
@@ -142,34 +167,31 @@
                 connect TEXT
                 )
         '''
         cursor.execute(create_table_sql)
         conn.commit()
         conn.close()
 
-        # create generic user
+        # create root user
         self.add_user(self.default_user,self.default_user)
 
-        return None
-
     def log_action(self, 
                    user:str, 
                    action:str, 
                    project:str = "general",
-                   connect = "not implemented"):
+                   connect = "not implemented") -> None:
         """
         Log action in the database
         """
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
         query = "INSERT INTO logs (user, project, action, connect) VALUES (?, ?, ?, ?)"
         cursor.execute(query, (user, project, action, connect))
         conn.commit()
         conn.close()
-        return None
 
     def db_get_project(self, project_name:str) -> ProjectModel|None:
         """
         Get project from database
         """
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
@@ -183,15 +205,15 @@
             p = ProjectModel(**json.loads(existing_project[2]))
             return p
         else:
             return None
 
     def exists(self, project_name) -> bool:
         """
-        Test if a project exists
+        Test if a project exists in the database
         """
         existing = self.existing_projects()
         v = (project_name in existing)
         return v
     
     def existing_projects(self) -> list:
         """
@@ -213,15 +235,17 @@
         cursor = conn.cursor()
         query = "SELECT user FROM users"
         cursor.execute(query)
         existing_users = cursor.fetchall()
         conn.close()
         return [i[0] for i in existing_users]
     
-    def add_user(self, name:str, password:str, projects = "all"):
+    def add_user(self, name:str, 
+                 password:str, 
+                 projects = "all") -> bool:
         """
         Add user to database
         """
         # test if the user doesn't exist
         if name in self.existing_users():
             return {"error":"Username already exists"}
         hash_pwd = functions.get_hash(password)
@@ -230,60 +254,82 @@
         cursor = conn.cursor()
         insert_query = "INSERT INTO users (user, key, projects) VALUES (?, ?, ?)"
         cursor.execute(insert_query, (name, hash_pwd, projects))
         conn.commit()
         conn.close()
         return {"success":"User added to the database"}
     
-    def get_user(self, name):
+    def delete_user(self, 
+                    name:str) -> dict:
+        """
+        Deleting user
+        """
+        if not name in self.existing_users():
+            return {"error":"Username does not exist"}
+        conn = sqlite3.connect(self.db)
+        cursor = conn.cursor()
+        query = "DELETE FROM users WHERE user = ?"
+        cursor.execute(query, (name,))
+        conn.close()
+        return {"success":"User deleted"}    
+    
+    def get_user(self, name) -> UserInDB|dict:
         """
-        Authentificate user
+        Get user from database
         """
         if not name in self.existing_users():
             return {"error":"Username doesn't exist"}
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
         query = "SELECT * FROM users WHERE user = ?"
         cursor.execute(query, (name,))
         user = cursor.fetchone()
-        print(user)
         u = UserInDB(username = name, hashed_password = user[3])
         conn.close()
         return u
 
     def authenticate_user(self, username: str, password: str):
+        """
+        User authentification
+        """
         user = self.get_user(username)
         if "error" in user:
             return user
         if not functions.compare_to_hash(password, user.hashed_password):
             return {"error":"Wrong password"}
         return user
     
     def create_access_token(self, data: dict, expires_min: int  = 60):
+        """
+        Create access token
+        """
         to_encode = data.copy()
         expire = datetime.now(timezone.utc) + timedelta(minutes=expires_min)
         to_encode.update({"exp": expire})
         encoded_jwt = jwt.encode(to_encode, 
                                  self.SECRET_KEY, 
                                  algorithm=self.ALGORITHM)
         return encoded_jwt
     
     def decode_access_token(self, token:str):
+        """
+        Decode access token
+        """
         payload = jwt.decode(token, self.SECRET_KEY, algorithms=[self.ALGORITHM])
         return payload
 
-    def start_project(self, project_name:str) -> bool:
+    def start_project(self, project_name:str) -> dict:
         """
-        Load project in memory
+        Load project in server
         """        
         if not self.exists(project_name):
-            raise ValueError("Project don't exist")
+            return {"error":"Project does not exist"}
 
-        self.projects[project_name] = Project(project_name, self.db)
-        return True
+        self.projects[project_name] = Project(project_name, self.db, self.executor)
+        return {"success":"Project loaded"}
 
     def set_project_parameters(self, project: ProjectModel) -> dict:
         """
         Update project parameters in the DB
         """
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
@@ -301,35 +347,42 @@
             cursor.execute(insert_query, (project.project_name, json.dumps(jsonable_encoder(project))))
         conn.commit()
         conn.close()
         return {"success":"project updated"}
 
     def create_project(self, 
                        params:ProjectModel, 
-                       file:UploadFile) -> ProjectModel:
+                       file:UploadFile) -> ProjectModel|dict:
         """
         Set up a new project
         - load data and save
         - initialize parameters in the db
         - initialize files
         - add preliminary tags
         """
         # create directory for the project
+        if self.exists(params.project_name):
+            return {"error":"Project name already exist"}
         params.dir = self.path / params.project_name
         if params.dir.exists():
-            return {"error":"This name is already used as a file"}
+            return {"error":"This name is already used"}
         os.makedirs(params.dir)
 
-        # write total dataset
+        # copy total dataset
         with open(params.dir / "data_raw.csv","wb") as f:
             f.write(file.file.read())
 
-        # random sample of the needed data, index as str
+        # TODO : maximise the aleardy tagged in the annotate dataset, and None in the test
+        # if possible, annotated data in the annotation dataset
+        # if possible, test data without annotation
+
+        # random sample of the needed data
         n_rows = params.n_train + params.n_test
-        content = pd.read_csv(params.dir / "data_raw.csv").sample(n_rows)
+        content = pd.read_csv(params.dir / "data_raw.csv")
+        content = content.sample(n_rows)
         content = content.set_index(params.col_id)
         content.index = [str(i) for i in list(content.index)] #type: ignore
     
         # create the empty annotated file / features file
         # Put the id column as index for the rest of the treatment
         content[0:params.n_train].to_parquet(params.dir / self.data_file, index=True)
         content[params.n_train:].to_parquet(params.dir / self.test_file, index=True)
@@ -381,67 +434,62 @@
     
 
     def delete_project(self, project_name:str) -> dict:
         """
         Delete a project
         """
 
-        if self.exists(project_name):
-            params = self.db_get_project(project_name)
-            self.remove_project_parameters(project_name)
-            shutil.rmtree(params.dir)
-            return {"success":"project deleted"}
-        else:
-            return {"error":"project doesn't exist"}
+        if not self.exists(project_name):
+            return {"error":"Project doesn't exist"}
 
-    def remove_project_parameters(self, project_name:str) -> bool:
-        """
-        Delete database entry
-        To add: save dump of a project when deleted ?
-        """
+        # remove files
+        params = self.db_get_project(project_name)
+        shutil.rmtree(params.dir)
+
+        # clean database
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
         cursor.execute(f"DELETE FROM projects WHERE project_name = ?", (project_name,))
         cursor.execute(f"DELETE FROM schemes WHERE project = ?", (project_name,))
         cursor.execute(f"DELETE FROM annotations WHERE project = ?", (project_name,))
         conn.commit()
         conn.close()
-        return True
+
+        return {"success":"Project deleted"}
     
 
 class Project(Server):
     """
     Project object
     """
 
     def __init__(self, 
                  project_name:str,
-                 path_db:Path) -> None:
+                 path_db:Path, 
+                 executor) -> None:
         """
         Load existing project
         """
         self.name: str = project_name
         self.db = path_db
+        self.executor = executor # where to send processes
         self.params: ProjectModel = self.load_params(project_name)
+        if self.params.dir is None:
+            raise ValueError("No directory exists for this project")
         self.content: DataFrame = pd.read_parquet(self.params.dir / self.data_file) #type: ignore
         self.schemes: Schemes = Schemes(project_name, 
-                                        self.params.dir / self.labels_file,
+                                        self.params.dir / self.labels_file, 
+                                        self.params.dir / self.test_file, 
                                         self.db) #type: ignore
-        self.features: Features = Features(project_name,
-                                           self.params.dir / self.features_file,
-                                           self.db) #type: ignore
+        self.features: Features = Features(project_name, self.params.dir / self.features_file, self.db) #type: ignore
         self.bertmodels: BertModels = BertModels(self.params.dir)
-        self.simplemodels: SimpleModels = SimpleModels(self.params.dir)
-        self.lock:list = [] # prevent competition
+        self.simplemodels: SimpleModels = SimpleModels(self.params.dir, executor)
 
-        # Compute features if requested
-        if ("sbert" in self.params.embeddings) & (not "sbert" in self.features.map):
-            self.compute_embeddings(emb="sbert")
-        if ("fasttext" in self.params.embeddings) & (not "fasttext" in self.features.map):
-            self.compute_embeddings(emb="fasttext")
+    def __del__(self):
+        pass
 
     def load_params(self, project_name:str) -> ProjectModel:
         """
         Load params from database
         """
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
@@ -451,310 +499,327 @@
         conn.commit()
         conn.close()
 
         if existing_project:
             return ProjectModel(**json.loads(existing_project[2]))
         else:
             raise NameError(f"{project_name} does not exist.")
-
-    async def compute_embeddings(self,
-                           emb:str) -> dict:
-        """
-        Compute embeddings
-        """
-        print("start compute embeddings ",emb, self.content.shape)
-        if emb == "fasttext":
-            f = functions.to_fasttext
-        if emb == "sbert":
-            f = functions.to_sbert
-        calc_emb = f(self.content[self.params.col_text])
-        self.features.add(emb, calc_emb)
-        return {"success":f"{emb} embeddings computed"}
-    
-    def fit_simplemodel(self,
-                        model:str,
-                        features:list|str,
-                        scheme:str,
-                        user:str = "user",
-                        model_params: None|dict = None
-                        ) -> bool:
-        """
-        Create and fit a simple model with project data
-        """
-
-        # build the dataset with label + predictors
-        df_features = self.features.get(features)
-        df_scheme = self.schemes.get_scheme_data(scheme)
-        col_features = list(df_features.columns)
-        data = pd.concat([df_scheme,
-                          df_features],
-                          axis=1)
-        self.simplemodels.add_simplemodel(user = user, 
-                                          scheme = scheme, 
-                                          features=features, 
-                                          name = model, 
-                                          df = data, 
-                                          col_labels = "labels", 
-                                          col_features = col_features,
-                                          model_params = model_params,
-                                          standardize = True
-                                          ) 
-        return True
     
     def update_simplemodel(self, simplemodel: SimpleModelModel) -> dict:
+        """
+        Update simplemodel on the base of an already existing
+        simplemodel object
+        """
         if simplemodel.features is None or len(simplemodel.features)==0:
             return {"error":"Empty features"}
         if not simplemodel.model in list(self.simplemodels.available_models.keys()):
             return {"error":"Model doesn't exist"}
         if not simplemodel.scheme in self.schemes.available():
             return {"error":"Scheme doesn't exist"}
         if len(self.schemes.available()[simplemodel.scheme]) < 2:
             return {"error":"2 different labels needed"}
-        self.fit_simplemodel(
-                            model=simplemodel.model,
-                            features=simplemodel.features,
-                            scheme=simplemodel.scheme,
-                            user =simplemodel.user,
-                            model_params=simplemodel.params
-                            )
-        return {"success":"new simplemodel"}
-     
+        # force dfm for multi_naivebayes
+        if simplemodel.model == "multi_naivebayes":
+            simplemodel.features = ["dfm"]
+            simplemodel.standardize = False
+        
+        # test if the parameters have the correct format
+        try:
+            validation = self.simplemodels.validation[simplemodel.model]
+            r = validation(**simplemodel.params)
+        except ValidationError as e:
+            return {"error":e.json()}
+        
+        df_features = self.features.get(simplemodel.features)
+        df_scheme = self.schemes.get_scheme_data(scheme=simplemodel.scheme)
+        col_features = list(df_features.columns)
+        data = pd.concat([df_scheme,
+                          df_features],
+                          axis=1)
+        self.simplemodels.add_simplemodel(user = simplemodel.user, 
+                                          scheme = simplemodel.scheme, 
+                                          features=simplemodel.features, 
+                                          name = simplemodel.model, 
+                                          df = data, 
+                                          col_labels = "labels", 
+                                          col_features = col_features,
+                                          model_params = simplemodel.params,
+                                          standardize = simplemodel.standardize
+                                          ) 
+        
+        return {"success":"Simplemodel updated"}
+
     def get_next(self,
                  scheme:str,
                  selection:str = "deterministic",
                  sample:str = "untagged",
                  user:str = "user",
                  tag:None|str = None,
                  frame:None|list = None) -> dict:
         """
-        Get next item
-        Related to a specific scheme
-        TODO : add lock feature
+        Get next item for a specific scheme with a specific method
+        - deterministic
+        - random
+        - active
+        - maxprob
+        - test
         """
 
+        # specific case of test, random element
+        if selection == "test": 
+            df = self.schemes.get_scheme_data(scheme, complete=True, kind="test")
+            f = df["labels"].isnull()
+            element_id = df[f].sample(random_state=42).index[0]
+            element =  {
+            "element_id":element_id,
+            "text":df.loc[element_id, "text"],
+            "selection":"test",
+            "context":{},
+            "info":"",
+            "predict":{
+                    "label":None,
+                    "proba":None
+                    },
+            "frame":[],
+            }
+            return element
+
         # select the current state of annotation
         df = self.schemes.get_scheme_data(scheme, complete=True)
 
         # build filters regarding the selection mode
         f = df["labels"].apply(lambda x : True)
         if sample == "untagged":
             f = df["labels"].isnull()
         if sample == "tagged":
             f = df["labels"].notnull()
 
         # manage frame selection (if projection, only in the box)
-        if user in self.features.available_projections:
-            if "data" in self.features.available_projections[user]:
-                projection = self.features.available_projections[user]["data"]
-                f_frame = (projection[0] > frame[0]) & (projection[0] < frame[2]) & (projection[1] > frame[1]) & (projection[1] < frame[3])
-                f = f & f_frame
-        
-        val = ""
+        try:
+            if user in self.features.available_projections:
+                if "data" in self.features.available_projections[user]:
+                    projection = self.features.available_projections[user]["data"]
+                    f_frame = (projection[0] > frame[0]) & (projection[0] < frame[2]) & (projection[1] > frame[1]) & (projection[1] < frame[3])
+                    f = f & f_frame
+        except:
+            print("Problem on frame")
 
         # test if there is at least one element available
         if sum(f) == 0:
             return {"error":"No element available"}
 
         # select type of selection
         if selection == "deterministic": # next row
             element_id = df[f].index[0]
+            indicator = None
         if selection == "random": # random row
             element_id = df[f].sample(random_state=42).index[0]
-        if selection == "maxprob": # higher prob 
-            # only possible if the model has been trained
+            indicator = None
+        if selection == "maxprob": # higher prob, only possible if the model has been trained
             if not self.simplemodels.exists(user,scheme):
                 return {"error":"Simplemodel doesn't exist"}
             if tag is None: # default label to first
-                tag = self.schemes.available()[scheme][0]
+                return {"error":"Select a tag"}
             sm = self.simplemodels.get_model(user, scheme) # get model
-            element_id = sm.proba[f][tag].sort_values(ascending=False).index[0] # get max proba id
-            val = f"probability: {round(sm.proba[f][tag].sort_values(ascending=False)[0],2)}"
-        if selection == "active": #higher entropy
-            # only possible if the model has been trained
+            proba = sm.proba.reindex(f.index)
+            element_id = proba[f][tag].sort_values(ascending=False).index[0] # get max proba id
+            indicator = f"probability: {round(proba.loc[element_id,tag],2)}"
+        if selection == "active": #higher entropy, only possible if the model has been trained
             if not self.simplemodels.exists(user,scheme):
-                return {"error":"Simplemodel doesn't exist"}
+                return  {"error":"Simplemodel doesn't exist"}
             sm = self.simplemodels.get_model(user, scheme) # get model
-            element_id = sm.proba[f]["entropy"].sort_values(ascending=False).index[0] # get max entropy id
-            val = round(sm.proba[f]['entropy'].sort_values(ascending=False)[0],2)
-            val = f"entropy: {val}"
-
-        # get prediction if it exists
+            proba = sm.proba.reindex(f.index)
+            element_id = proba[f]["entropy"].sort_values(ascending=False).index[0] # get max entropy id
+            indicator = round(proba.loc[element_id,'entropy'],2)
+            indicator = f"entropy: {indicator}"
+        
+        # get prediction of the id if it exists
         predict = {"label":None,
                    "proba":None}
+
         if self.simplemodels.exists(user,scheme):
             sm = self.simplemodels.get_model(user, scheme)
             predicted_label = sm.proba.loc[element_id,"prediction"]
             predicted_proba = round(sm.proba.loc[element_id,predicted_label],2)
             predict = {"label":predicted_label, 
                        "proba":predicted_proba}
 
         element =  {
             "element_id":element_id,
             "text":self.content.fillna("NA").loc[element_id,self.params.col_text],
             "context":dict(self.content.fillna("NA").loc[element_id, self.params.cols_context]),
             "selection":selection,
-            "info":str(val),
+            "info":indicator,
             "predict":predict,
-            "frame":frame
+            "frame":frame,
                 }
-        
+        print(element)        
         return element
     
-    def get_element(self,element_id):
+    def get_element(self, 
+                    element_id:str,
+                    scheme:str|None = None,
+                    user:str|None = None):
         """
         Get an element of the database
-        TO REMOVE
+        TODO: better homogeneise with get_next ?
+        TODO:; test if element exists
         """
-        columns = ["text"]
-        return {"element_id":element_id,
-                "text":self.content.loc[element_id,"text"]
-                }
+        # get prediction if it exists
+        predict = {"label":None, "proba":None}
+        if (user is not None) & (scheme is not None):
+            if self.simplemodels.exists(user,scheme):
+                sm = self.simplemodels.get_model(user, scheme)
+                predicted_label = sm.proba.loc[element_id,"prediction"]
+                predicted_proba = round(sm.proba.loc[element_id,predicted_label],2)
+                predict = {"label":predicted_label, 
+                        "proba":predicted_proba}
+        r = { 
+            "element_id":element_id,
+            "text":self.content.loc[element_id,self.params.col_text],
+            "context":dict(self.content.fillna("NA").loc[element_id, self.params.cols_context]),
+            "selection":"request",
+            "predict":predict
+            }
+        return r
 
     def get_params(self) -> ProjectModel:
         """
         Send parameters
         """
         return self.params
     
-    def get_stats_annotations(self, scheme:str, user:str):
-
-        df = self.schemes.get_scheme_data(scheme)
-        df["labels"].value_counts()
-
-        stats = {
-                    "dataset total":len(self.content),
-                    "annotated elements":len(df),
-                    "different users":list(self.schemes.get_distinct_users(scheme)),
-                    "annotations distribution":json.loads(df["labels"].value_counts().to_json()),
-                    "last annotation":"TO DO",
-                }
-        return stats
-    
     def get_description(self, scheme:str|None, user:str|None):
         """
-        Generate a description of a project/scheme
+        Generate a description of a current project/scheme/user
+        Return:
+            JSON
         """
         r = {
             "N dataset":len(self.content)
             }
         
         if scheme is None:
-            return None
+            return {"error":"Scheme not defined"}
         
-        df = self.schemes.get_scheme_data(scheme)
+        # part train
+        df = self.schemes.get_scheme_data(scheme, kind="add")
         r["N annotated"] = len(df)
         r["Users"] = list(self.schemes.get_distinct_users(scheme))
         r["Annotations"] = json.loads(df["labels"].value_counts().to_json())
 
+        # part test
+        df = self.schemes.get_scheme_data(scheme, kind="test")
+        r["N test annotated"] = len(df)
+
         if self.simplemodels.exists(user, scheme):
             sm = self.simplemodels.get_model(user, scheme) # get model
             r["Simplemodel 10-CV"] = sm.cv10
 
         return r
 
     def get_state(self):
         """
         Send state of the project
         """
         # update if needed
         self.bertmodels.update()
 
-        options = {
-                    "params":self.params,
-                    "next":{
-                        "methods":["deterministic","random","maxprob","active"],
-                        "sample":["untagged","all","tagged"],
-                        },
-                    "schemes":{
-                                "available":self.schemes.available()
-                                },
-                    "features":{
-                            "available":list(self.features.map.keys()),
-                            "training":self.features.training,
-                            "options":["sbert","fasttext"]
-                            },
-                    "simplemodel":{ #change names existing/available to available/options
-                                    "existing":self.simplemodels.available(),
-                                    "available":self.simplemodels.available_models
-                                },
-                    "bertmodels":{
-                                "options":self.bertmodels.base_models,
-                                "available":self.bertmodels.trained(),
-                                "training":self.bertmodels.training(),
-#                                "predictions":self.bertmodels.predictions(),
-#        
-                                "base_parameters":self.bertmodels.params_default
-                                },
-                    "projections":{
-                                "available":self.features.possible_projections
-                                }
-                   }
-        # TODO : change available label to default ... 
-        return  options
+        r = {
+            "params":self.params,
+            "next":{
+                    "methods_min":["deterministic","random","test"],
+                    "methods":["deterministic","random","maxprob","active","test"],
+                    "sample":["untagged","all","tagged"],
+                    },
+            "schemes":{
+                    "available":self.schemes.available()
+                    },
+            "features":{
+                    "options":self.features.options,
+                    "available":list(self.features.map.keys()),
+                    "training":self.features.training,
+                    },
+            "simplemodel":{
+                    "options":self.simplemodels.available_models,
+                    "available":self.simplemodels.available(),
+                    "training":self.simplemodels.training(),
+                    },
+            "bertmodels":{
+                    "options":self.bertmodels.base_models,
+                    "available":self.bertmodels.trained(),
+                    "training":self.bertmodels.training(),
+                    "base_parameters":self.bertmodels.params_default
+                    },
+            "projections":{
+                    "available":self.features.possible_projections
+                    }
+            }
+        return  r
     
     def add_regex(self, name: str, value: str) -> dict:
         """
         Add regex to features
         """
         if name in self.features.map:
             return {"error":"a feature already has this name"}
 
         pattern = re.compile(value)
         f = self.content[self.params.col_text].apply(lambda x: bool(pattern.search(x)))
-        print("compile feature", f.shape)
         self.features.add(name,f)
         return {"success":"regex added"}
     
-    def export_features(self, features:list, format:str|None = None):
+    def export_features(self, features:list, format:str = "parquet"):
         """
         Export features data in different formats
         """
-        if format is None:
-            format = "csv"
+        if len(features)==0:
+            return {"error":"No features selected"}
 
-        path = self.path / self.name # path of the data
+        path = self.params.dir # path of the data
         if not path.exists():
             raise ValueError("Problem of filesystem for project")
 
         data = self.features.get(features)
 
         file_name = f"extract_schemes_{self.name}.{format}"
 
+        # create files
         if format == "csv":
             data.to_csv(path / file_name)
-
         if format == "parquet":
             data.to_parquet(path / file_name)
 
-        return file_name, path / file_name
+        r = { "name":file_name,
+              "path":path / file_name}
+
+        return r
 
 
-    def export_data(self, scheme:str, format:str|None = None):
+    def export_data(self, scheme:str, format:str = "parquet"):
         """
         Export annotation data in different formats
         """
-        if format is None:
-            format = "csv"
-
-        path = self.path / self.name # path of the data
+        path = self.params.dir# path of the data
         if not path.exists():
             raise ValueError("Problem of filesystem for project")
 
         data = self.schemes.get_scheme_data(scheme=scheme,
-                                     complete=True)
+                                            complete=True)
         
         file_name = f"data_{self.name}_{scheme}.{format}"
 
+        # Create files
         if format == "csv":
             data.to_csv(path / file_name)
-
         if format == "parquet":
             data.to_parquet(path / file_name)
 
-        return file_name, path / file_name
+        r = {"name":file_name,"path":path / file_name}
+        return r
 
 class Features():
     """
     Manage project features
     Comment : 
     - as a file
     - use "__" as separator
@@ -778,14 +843,27 @@
         # managing projections
         self.possible_projections:dict = {
                             "umap":{"n_neighbors":15, "min_dist":0.1, "n_components":2, "metric":'euclidean'},
                             "tsne":{"n_components":2,  "learning_rate":'auto', "init":'random', "perplexity":3}
                             }
         self.available_projections:dict = {}
 
+        # options
+        self.options:dict = {"sbert":{},
+                        "fasttext":{},
+                        "dfm":{ 
+                                    "tfidf":False,
+                                    "ngrams":1,
+                                    "min_term_freq":5,
+                                    "max_term_freq":100,
+                                    "norm":None,
+                                    "log":None
+                                    }
+                        }
+
 
     def __repr__(self) -> str:
         return f"Available features : {self.map}"
     
     def load(self):
         """
         Load file and agregate columns
@@ -815,109 +893,124 @@
         # change type
         if type(content)==Series:
             content = pd.DataFrame(content)
 
         # add to the table & dictionnary
         content.columns = [f"{name}__{i}" for i in content.columns]
         self.map[name] = list(content.columns)
-        self.content = pd.concat([self.content,content],
+
+        self.content = pd.concat([self.content,
+                                  content],
                                      axis=1)
         # save
+
         self.content.to_parquet(self.path)
         return {"success":"feature added"}
 
     def delete(self, name:str):
         """
         Delete feature
         """
         if not name in self.map:
             return {"error":"feature doesn't exist"}
 
         col = self.get([name])
         del self.map[name]
-        self.content.drop(columns=col)
+        self.content = self.content.drop(columns=col)
         self.content.to_parquet(self.path)
         return {"success":"feature deleted"}
             
     def get(self, features:list|str = "all"):
         """
         Get content for specific features
-        TODO : test if the feature exists
         """
         if features == "all":
             features = list(self.map.keys())
         if type(features) is str:
             features = [features]
 
         cols = []
+        missing = []
         for i in features:
             if i in self.map:
                 cols += self.map[i]
+            else:
+                missing.append(i)
 
+        if len(i)>0:
+            print("Missing features:", missing)
         return self.content[cols]
         
 
 class Schemes():
     """
     Manage project schemes & tags
 
     Tables :
     - schemes
     - annotations
     """
     def __init__(self,
                  project_name: str,
-                 path:Path, 
+                 path_content:Path, # training data
+                 path_test:Path, # test data
                  db_path:Path) -> None:
         """
         Init empty
         """
         self.project_name = project_name
-        self.path = path
         self.db = db_path
-        self.content = pd.read_parquet(self.path) #text + context
+        self.content = pd.read_parquet(path_content) #text + context   
+        self.test = pd.read_parquet(path_test)
         available = self.available()
 
-        # create a default scheme
+        # create a default scheme if not available
         if len(available) == 0:
             self.add_scheme(SchemeModel(project_name = project_name, 
                                  name = "default",
-                                 tags = [],
-                                 user = "server")
+                                 tags = [])
                                  )
 
     def __repr__(self) -> str:
         return f"Coding schemes available {self.available()}"
 
-    def get_scheme_data(self, scheme:str, complete = False) -> DataFrame:
+    def get_scheme_data(self, scheme:str, 
+                        complete = False, 
+                        kind = "add") -> DataFrame:
         """
         Get data from a scheme : id, text, context, labels
         """
         if not scheme in self.available():
             raise ValueError("Scheme doesn't exist")
         
         # get all elements from the db
         # - last element for each id
         # - for a specific scheme
 
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
         query = '''
-            SELECT element_id, tag, MAX(time) AS last_timestamp
+            SELECT element_id, tag, user, MAX(time)
             FROM annotations
             WHERE scheme = ? AND project = ? AND action = ?
-            GROUP BY element_id;
+            GROUP BY element_id
+            ORDER BY time DESC;
         '''
-        cursor.execute(query, (scheme, self.project_name, "add"))
+        cursor.execute(query, (scheme, self.project_name, kind))
         results = cursor.fetchall()
         conn.close()
-        df = pd.DataFrame(results, columns =["id","labels","timestamp"]).set_index("id")
+        df = pd.DataFrame(results, columns =["id","labels","user","timestamp"]).set_index("id")
         df.index = [str(i) for i in df.index]
+
         if complete: # all the elements
-            return self.content.join(df)
+            if kind == "add":
+                return self.content.join(df)
+            if kind == "test":
+                return self.test.join(df)
+        
         return df
     
     def get_table(self, scheme:str,
                         min:int,
                         max:int, 
                         mode:str,
                         user:str = "all"):
@@ -1059,21 +1152,23 @@
         query = "SELECT name, params FROM schemes WHERE project = ?"
         cursor.execute(query, (self.project_name,))
         results = cursor.fetchall()
         conn.commit()
         conn.close()
         return {i[0]:json.loads(i[1]) for i in results}
    
-    def get(self) -> SchemesModel:
+    def get(self) -> dict:
         """
         state of the schemes
         """
-        return SchemesModel(project_name=self.project_name,
-                            availables=self.available()
-                            )
+        r = {
+            "project_name":self.project_name,
+            "availables":self.available()
+        }
+        return r #SchemesModel(project_name=self.project_name,availables=self.available())
 
     def delete_tag(self, 
                    element_id:str,
                    scheme:str,
                    user:str = "server") -> bool:
         """
         Delete a recorded tag
@@ -1093,61 +1188,70 @@
         conn.close()
         return True
 
     def push_tag(self,
                  element_id:str, 
                  tag:str|None,
                  scheme:str,
-                 user:str = "server"):
+                 user:str = "server",
+                 selection:str = "training"):
         """
         Record a tag
         """
+
         # test if the action is possible
         a = self.available()
         if not scheme in a:
             return {"error":"scheme unavailable"}
         if (not tag is None) and (not tag in a[scheme]):
             return {"error":"this tag doesn't belong to this scheme"}
-        if not element_id in self.content.index:
-            return {"error":"element doesn't exist"}
-    
+
+        # TODO : add a test also for testing
+        #if (not element_id in self.content.index):
+        #    return {"error":"element doesn't exist"}
+
+        # type of tag regarding the selection mode
+        action = "add"
+        if selection == "test":
+            action = "test"
+
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
         query = '''
             INSERT INTO annotations (action, user, project, element_id, scheme, tag)
             VALUES (?,?,?,?,?,?);
         '''
-        cursor.execute(query, ("add", user, self.project_name, element_id, scheme, tag))
+        cursor.execute(query, (action, user, self.project_name, element_id, scheme, tag))
         conn.commit()
         conn.close()
         return {"success":"tag added"}
     
-    def push_table(self, table, user:str):
+    def push_table(self, table, user:str) -> bool:
         """
         Push table index/tags to update
         Comments:
         - only update modified labels
         """        
         data = {i:j for i,j in zip(table.list_ids,table.list_labels)}
         for i in data:
             r = self.push_tag(i, 
                             data[i],
                             table.scheme,
                             user)
-        return {"success":"labels modified"}
+        return True
 
     def get_recent_tags(self,
                     user:str,
                     scheme:str,
                     n:int) -> list:
         """
         Get the id of the n last tags added/updated
         by a user for a scheme of a project
         """
-        print("get recent tags for ",user)
+        print("get recent tags for ", user)
         # add case for all users
 
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
         if user == "all": # all users
             query = """
                     SELECT DISTINCT element_id 
@@ -1182,8 +1286,8 @@
                 FROM annotations
                 WHERE project = ? AND scheme = ? AND action = ?
                 """
         cursor.execute(query, (self.project_name,scheme, "add"))
         results = cursor.fetchall()
         conn.commit()
         conn.close()
-        return results
+        return results
```

### Comparing `activetigger-0.0.9/activetigger/widget.py` & `activetigger-0.1.0/activetigger/widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import ipywidgets as widgets
 from ipywidgets import Layout
 from IPython.display import display, clear_output
 import plotly.graph_objects as go
 import json
 import requests as rq
-from pathlib import Path
 import pandas as pd
 import time
 import asyncio
-import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
 from IPython.display import display, clear_output
-import distinctipy
+import importlib
+import numpy as np
+from io import BytesIO
+import textwrap
+
 
 
 class Widget():
     """
     Widget
 
     Comment
@@ -58,15 +60,15 @@
                     params = params,
                     json = json_data,
                     data = data,
                     files=files,
                     headers=self.headers)
         
         if r.status_code == 422:
-            return {"error":"Not authorized"}
+            return {"status":"error", "message":"Not authorized"}
 
         return json.loads(r.content)
     
     def _get(self,
              route:str, 
              params:dict|None = None, 
              data:dict|None = None,
@@ -75,16 +77,17 @@
         Get from API
         """
         url = self.URL_SERVER + route
         r = rq.get(url, 
                     params = params,
                     data = data,
                     headers=self.headers)
+        
         if r.status_code == 422:
-            return {"error":"Not authorized"}
+            return {"status":"error", "message":"Not authorized"}
 
         if is_json:
             return json.loads(r.content)
         return r.content
     
     def _connect_user(self, user:str, password:str):
         """
@@ -98,60 +101,74 @@
             return None
 
         # Update widget configuration
         self.headers = {"Authorization": f"Bearer {r['access_token']}",
            "username":user}
         self.user = user
 
+        # Display
+        self.current_user.value = f"Connected as <b>{self.user}</b>"
+
         # Disable connecting options
         self.existing_users.disabled = True
         self.password.disabled = True
         self.connect_user.disabled = True
         return None
 
     def start(self) -> None:
         """
         Start project
         """
         # Get existing projects
-        existing = self._get("/server")
+        try:
+            r = self._get("/server")
+            existing = r["data"]
+        except:
+            print(f"Failed to connect to the server. Please check if the server is available at {self.URL_SERVER}")
+            return None
 
         # Stop potential async
         Widget.async_update = False
 
         # Image
+        data_path = importlib.resources.files("activetigger")
         image_path = "img/active_tigger.png"
-        img = open(image_path, 'rb').read()
-        img_at = widgets.Image(value=img, format='png', width=50, height=50)
+        img = open(data_path / image_path, 'rb').read()
+        img_at = widgets.Image(value=img, format='png', width=100, height=100)
 
         # Users
         self.existing_users = widgets.Dropdown(description = "User:", 
                                           options = existing["users"],
                                           layout={'width': '200px'})
         self.password = widgets.Text(description = "Password:", layout={'width': '200px'})
         self.connect_user = widgets.Button(description="Connect")
         self.connect_user.style.button_color = 'lightgreen'
         self.connect_user.on_click(lambda x : self._connect_user(user = self.existing_users.value,
                                                  password = self.password.value))
-
+        self.current_user = widgets.HTML(value="Not connected")
+        if self.user is not None:
+            self.current_user.value = f"Connected as <b>{self.user}</b>"
         # Existing projects
         existing_projects = widgets.Dropdown(
             options=existing["projects"],
             description='Available :',
             layout={'width': '300px'},
             disabled=False)
 
         # Start existing project
         start = widgets.Button(description="Launch")
         start.style.button_color = 'lightgreen'
         def start_project(b):
             self.project_name = existing_projects.value
+            if existing_projects.value is None:
+                print("No project selected")
+                return None
             self.state = self.get_state()
-            if "error" in self.state:
-                print("Not connected")
+            if len(self.state) == 0:
+                self.current_user.value = "<div  style='background-color: #ffcc00;'>Please identify yourself. Not connected</div>"
                 return None
             self.interface()
         start.on_click(start_project)
 
         # Create a new project
         create = widgets.Button(description="New project")
         create.on_click(lambda x: self._create_new_project())
@@ -159,26 +176,29 @@
         # Delete a project
         delete = widgets.Button(description="Delete project", button_style='danger')
         delete.on_click(lambda x: self._delete_project(existing_projects.value))
 
         # Display
         clear_output()
         self.output = widgets.VBox([widgets.HBox([img_at, self.existing_users, self.password, self.connect_user]),
+                                    self.current_user,
                                     widgets.HBox([existing_projects, start, delete, create]) 
                                     ])
         #display(self.output)
         self.global_output.children = [self.output]
         display(self.global_output)
 
     def get_state(self) -> dict:
         """
         Get state variable
         """
         state = self._get(route = f"/state/{self.project_name}")
-        return state
+        if state["status"]=="error":
+            return {}
+        return state["data"]
 
     def _delete_project(self, project_name:str) -> dict:
         """
         Delete existing project
         """
         params = {
                 "project_name": project_name,
@@ -199,18 +219,24 @@
         #------------------------
 
         project_name = widgets.Text(disabled=False,
                                     description="Name:",
                                     layout={'width': '200px'})
 
         # load file
-        file = widgets.Text(disabled=False,
-                            description="Path:",
-                            layout={'width': '300px'},
-                            value = "path to a csv")
+#        file = widgets.Text(disabled=False,
+#                            description="Path:",
+#                            layout={'width': '300px'},
+#                            value = "path to a csv")
+        file = widgets.FileUpload(
+            description= 'Select file',
+            accept='.csv',
+            multiple=False,
+        )
+        box_file = widgets.HBox([file])
         layout=widgets.Layout(width='100px', margin='0px 0px 0px 50px')
         load = widgets.Button(description="Load",
                               layout=layout)
         load.style.button_color = 'lightgreen'
 
         # WARNING : BUG dans VS Code sur l'upload donc utiliser un
         # chemin
@@ -278,33 +304,35 @@
                     "col_text": column_text.value,
                     "col_id":column_id.value,
                     "col_label":column_label.value,
                     "cols_context": list(columns_context.value),
                     "n_train":n_train.value,
                     "n_test":n_test.value
                     }
-            files = {'file': (file.value,
-                              open(file.value, 'rb'))}
+            files = {'file': (file.value[0]["name"],
+                              BytesIO(file.value[0]["content"]))}
             r = self._post(route="/projects/new", 
                        files=files,
                        data=data
                        )
             # if project exit
-            if "error" in r:
-                print("Project name alreay exists")
+            print(r)
+            if r["status"] == "error":
+                print(r["message"])
             else:
                 self.start()
         validate.on_click(create_project)
         validate.style.button_color = 'lightgreen'
 
         # manage 2-level menu display
-        self.output = widgets.VBox([widgets.HBox([project_name, file, load])])
+        self.output = widgets.VBox([widgets.HBox([project_name, box_file, load])])
         
         def load_file(b):
-            df = self._load_file(file.value)
+            #df = self._load_file(file.value)
+            df = self._load_file(file)
             column_text.options = df.columns
             column_id.options = df.columns
             column_label.options = df.columns
             columns_context.options = df.columns
             info.value = f"Size of the dataset: {len(df)}"
             if len(df.columns)>1:
                 column_text.value = column_text.options[1]
@@ -319,26 +347,26 @@
                                                                      n_train,
                                                                      n_test,
                                                                      validate]
         load.on_click(load_file)
         self.global_output.children = [self.output]
         display(self.global_output)
 
-    def _load_file(self,path) -> pd.DataFrame:
+    def _load_file(self, file):
         """
         Load file
         """
-        path = Path(path)
-        if not path.exists():
+        if len(file.value) == 0:
             print("File doesn't exist")
             return pd.DataFrame()
-        if not path.suffix == '.csv':
-            print("File not csv")
+        if file.value[0]["type"] != "text/csv":
+            print("Only CSV")
             return pd.DataFrame()
-        df = pd.read_csv(path)
+        content = file.value[0]["content"]
+        df = pd.read_csv(BytesIO(content))
         return df
     
     def _display_next(self) -> bool:
         """
         Get next element from the current widget options
         """
 
@@ -354,30 +382,30 @@
 
         params = {
                 "project_name":self.project_name,
                 "scheme":self.select_scheme.value,
                 "selection":self._mode_selection.value,
                 "sample":self._mode_sample.value,
                 "user":self.user,
-                "tag":None,
+                "tag":self._mode_label.value,
                 "frame":x1y1x2y2
                 }
         r = self._get(route = "/elements/next",
                       params = params)
         
         # Managing errors
-        if "error" in r:
-            print(r)
+        if r["status"] == "error":
+            print(r["message"])
             return False
 
         # Update interface
-        self.current_element = r
-        self._textarea.value = r["text"]
-        self.info_element.value = r["info"]
-        self.info_predict.value = f"Predict SimpleModel: <b>{r['predict']['label']}</b> (p = {r['predict']['proba']})"
+        self.current_element = r["data"]
+        self._textarea.value = self.current_element["text"]
+        self.info_element.value = str(self.current_element["info"])
+        self.info_predict.value = f"Predict SimpleModel: <b>{self.current_element['predict']['label']}</b> (p = {self.current_element['predict']['proba']})"
         return True
 
     def _display_buttons_labels(self) -> bool:
         """
         Dispaly labels to annotate (panel annotation)
         Managing tag posting
         """
@@ -387,31 +415,32 @@
         # function to post
         def send_tag(v):
             data = {
                     "project_name":self.project_name,
                     "scheme":self.select_scheme.value,
                     "element_id":self.current_element["element_id"],
                     "tag":v.description,
-                    "user":self.user
+                    "user":self.user,
+                    "selection":self.current_element["selection"] #mode of selection of the element
                     }
+            
             r = self._post(route = "/tags/add",
-                       params = {"project_name":self.project_name},
-                       json_data = data)
+                            params = {"project_name":self.project_name},
+                            json_data = data)
             
             # add in history
             if "error" in r:
                 print(r)
             else:
                 self.history.append(self.current_element["element_id"])
             self._display_next()
 
             # check if simplemodel need to be retrained
             if self.is_simplemodel() and (len(self.history) % self.simplemodel_autotrain.value == 0):
-                # retrain with the parameters of the state
-                sm = self.state["simplemodel"]["existing"][self.user][self.select_scheme.value]
+                sm = self.state["simplemodel"]["available"][self.user][self.select_scheme.value]
                 self.create_simplemodel(self.select_scheme.value,
                            model = sm["name"], 
                            parameters = sm["params"], 
                            features = sm["features"])
                 
         # create buttons
         buttons = []
@@ -422,21 +451,19 @@
             buttons.append(b)
         
         # add buttons
         self._labels.children = buttons
         return True
 
     def is_simplemodel(self)->bool:
-        if self.user in self.state["simplemodel"]["existing"]:
-            if self.select_scheme.value in self.state["simplemodel"]["existing"][self.user]:
+        if self.user in self.state["simplemodel"]["available"]:
+            if self.select_scheme.value in self.state["simplemodel"]["available"][self.user]:
                 return True
         return False
 
-
-
     def update_global(self):
         """
         Global update of the widget
         """
         self.state = self.get_state()
         self.update_tab_annotations(False)
         self.update_tab_schemes(False)
@@ -488,60 +515,61 @@
         """
         if state:
             self.state = self.get_state()
         self.available_features.options = self.state["features"]["available"]
         if len(self.state["features"]["available"])>0:
             self.available_features.value = self.state["features"]["available"][0]
 
-        self.add_features.options = self.state["features"]["options"]
+        self.add_features.options = self.state["features"]["options"].keys()
+        self.features_params.value = json.dumps(self.state["features"]["options"][self.add_features.value])
 
         c = self.state["features"]["training"]
         if len(c) == 0:
             c = "None"
-        self.info_features.value = f"Processes currently running: {c}"
+        self.info_features.value = f"<div style='background-color: #ffcc00; padding: 10px;'>Processes currently running: {c}</div>"
 
         return True
 
     def update_tab_description(self, state = True):
         """
         Update Description tab
         """
         if state:
             self.state = self.get_state()
         params = {"project_name":self.project_name,
                   "scheme":self.select_scheme.value,
                   "user":self.user}
         r = self._get("/description",params = params)
         text = ""
-        for k,v in r.items():
+        for k,v in r["data"].items():
             text += f"<br>- <b>{k}</b>: {v}"
         self.data_description.value = text
         return True
 
     def update_tab_annotations(self, state = True):
         """
         Update Annotations Tab
         """
         if state:
             self.state = self.get_state()
 
         self._display_next()
         self._display_buttons_labels()
 
-        self._mode_selection.options = ["deterministic","random"]
+        self._mode_selection.options = self.state["next"]["methods_min"]
         self._mode_sample.options = self.state["next"]["sample"]
         self._mode_label.disabled = True
         # to display context
         if self.add_context.value:
             self.display_context.value = json.dumps(self.current_element["context"])
         else:
             self.display_context.value = ""
         # case of a simplemodel is available for the user and the scheme
         if self.is_simplemodel():
-            self._mode_selection.options = self.state["next"]["methods"] #["deterministic","random","maxprob","active"]
+            self._mode_selection.options = self.state["next"]["methods"]
             self._mode_label.disabled = False
             self._mode_label.options = self.state["schemes"]["available"][self.select_scheme.value]
         # projection
         self.projection_method.options = list(self.state["projections"]["available"].keys())
         self.projection_params.value = json.dumps(self.state["projections"]["available"]["umap"], indent=2)
         self.projection_features.options = self.state["features"]["available"]
 
@@ -557,31 +585,37 @@
     def update_tab_simplemodel(self, state = True):
         """
         Update Simplemodel Tab
         """
         if state:
             self.state = self.get_state()
 
-        self.select_simplemodel.options = list(self.state["simplemodel"]["available"].keys())
+        self.select_simplemodel.options = list(self.state["simplemodel"]["options"].keys())
         self.select_features.options = self.state["features"]["available"]
 
+        name = "No model"
+        statistics = ""
+        self.simplemodel_params.value = ""
+        status = ""
+
         # if a model has already be trained for the user and the scheme
-        if (self.user in self.state["simplemodel"]["existing"]) and (self.select_scheme.value in self.state["simplemodel"]["existing"][self.user]):
-            current_model = self.state["simplemodel"]["existing"][self.user][self.select_scheme.value]
+        if (self.user in self.state["simplemodel"]["available"]) and (self.select_scheme.value in self.state["simplemodel"]["available"][self.user]):
+            current_model = self.state["simplemodel"]["available"][self.user][self.select_scheme.value]
             name = current_model['name']
             statistics = f"F1: {round(current_model['statistics']['weighted_f1'],2)} - accuracy: {round(current_model['statistics']['accuracy'],2)}"
             self.simplemodel_params.value = json.dumps(current_model["params"], indent=2)
             self.select_simplemodel.value = name
-        else:
-            name = "No model"
-            statistics = ""
-            self.simplemodel_params.value = ""
+
+        # if there is a model under training
+        if (self.user in self.state["simplemodel"]["training"]) and (self.select_scheme.value in self.state["simplemodel"]["training"][self.user]):
+            status = "Computing"
+            self.computing_simplemodel = True
 
         # display information
-        self.simplemodel_state.value = f"Current model: {name}"
+        self.simplemodel_state.value = f"<b>{status}</b> - Current model: {name}"
         self.simplemodel_statistics.value = statistics
 
     def update_tab_data(self, state = True):
         """
         Update Data tab
         """
         if state:
@@ -590,15 +624,15 @@
                    "project_name":self.project_name,
                    "scheme":self.select_scheme.value,
                    "min":self.sample_min.value,
                    "max":self.sample_max.value,
                    "mode":self.sample_type.value
                   }
         r = self._get("/elements/table", params = params)
-        df = pd.DataFrame(r)
+        df = pd.DataFrame(r["data"])
         buttons = []
         for i,j in df.iterrows():
             options = self.state["schemes"]["available"][self.select_scheme.value]
             if not j["labels"] in options:
                 options.append(j["labels"]) # case of a old label
             menu = widgets.Dropdown(options = options, 
                                  value = j["labels"],
@@ -615,20 +649,22 @@
     def update_tab_exports(self, state = True):
         if state:
             self.state = self.get_state()
         self.export_features_columns.options = self.state["features"]["available"]
 
         prediction = []
         if self.select_scheme.value in self.state["bertmodels"]["available"]:
-            prediction = [i[0] for i in self.state["bertmodels"]["available"][self.select_scheme.value] if i[1]] #if predict
+            temp = self.state["bertmodels"]["available"][self.select_scheme.value]
+            prediction = [i for i in temp if temp[i]["predicted"]]
         self.select_bert_model_predict.options = prediction
 
         bert = []
         if self.select_scheme.value in self.state["bertmodels"]["available"]:
-            bert = [i[0] for i in self.state["bertmodels"]["available"][self.select_scheme.value] if i[2]] #if compressed
+            temp = self.state["bertmodels"]["available"][self.select_scheme.value]
+            bert = [i for i in temp if temp[i]["compressed"]]
         self.select_bert_model.options  = bert
 
     def create_scheme(self, s):
         """
         Create new scheme
         """
         if s == "":
@@ -722,46 +758,60 @@
             return "Model missing"
         if parameters is None:
             return "Parameters missing"
         if (features is None) or (len(features)==0):
             return "Need at least one feature" 
         # TODO : test if parameters is valid
         params = {"project_name":self.project_name}
+        if type(parameters) is str:
+            try:
+                parameters = json.loads(parameters)
+            except:
+                print(parameters)
+                raise ValueError("Problem in the json parameters")
         data = {
                 "model":model,
                 "features":features,
                 "params":parameters,
                 "scheme":scheme,
                 "user":self.user
                 }
         
         r = self._post("/models/simplemodel", 
                        params = params, 
                        json_data = data)
+        if "error" in r:
+            # TODO : upgrade display on widget
+            print(r["message"])
+            return False
         self.update_tab_simplemodel()
         return True
     
     def create_bertmodel(self):
         """
         Create a bertmodel
         """
         self.compute_new_bert.disabled = True
         if self.new_bert_base.value is None:
             return "Model missing"
         if self.new_bert_params.value is None:
             return "Parameters missing"
+        try:
+            bert_params = json.loads(self.new_bert_params.value)
+        except:
+            raise ValueError("Problem in the json parameters")
         
         params = {"project_name":self.project_name}
         data = {
                 "project_name":self.project_name,
                 "scheme":self.select_scheme.value,
                 "user":self.user,
                 "name":f"_{self.user}", # générique
                 "base_model":self.new_bert_base.value,
-                "params":json.loads(self.new_bert_params.value),
+                "params":bert_params,
                 "test_size":0.2
                 }
         
         r = self._post("/models/bert/train", 
                        params = params, 
                        json_data = data)
         time.sleep(2)
@@ -802,46 +852,53 @@
         return True
 
     def _display_element(self, element_id):
         """
         Display specific element
         """
         r = self._get(route = f"/elements/{element_id}",
-                      params = {"project_name":self.project_name})
+                      params = {"project_name":self.project_name,
+                                "scheme":self.select_scheme.value})
         # Managing errors
-        if "error" in r:
+        if r["status"]=="error":
             print(r)
             return False
         # Update interface
-        self.current_element = r
-        self._textarea.value = r["text"]
+        self.current_element = r["data"]
+        self._textarea.value = self.current_element ["text"]
         return True
 
     def _get_previous_element(self) -> bool:
         """
         Load previous element in history
         """
         if len(self.history) == 0:
             print("No element in history")
             return False
         element_id = self.history.pop()
         r = self._display_element(element_id) 
         return r
     
-    def compute_feature(self, feature_name) -> bool:
+    def compute_feature(self, feature_name, feature_params) -> bool:
         """
         Compute feature
         """
-        if not feature_name in self.state["features"]["options"]:
+        if not feature_name in self.state["features"]["options"].keys():
             return "This feature doesn't exist"
+        try:
+            feature_params = json.loads(feature_params) #test if ok
+        except:
+            raise ValueError("Problem in the json parameters")
         r = self._post(f"/features/add/{feature_name}", 
                     params ={
                             "project_name":self.project_name,
                             "user":self.user
-                            })
+                            },
+                    json_data = {"params":feature_params}
+                    )
         self.update_tab_features()
         return True
     
     def delete_feature(self, feature_name) -> bool:
         """
         Delete existing feature
         """
@@ -877,14 +934,15 @@
         params = {"project_name":self.project_name,
                   "former_name":former_name,
                   "new_name":new_name,
                   "user":self.user
                   }
         r = self._post("/models/bert/rename",
             params = params)
+        self.update_tab_bertmodels()
         return r
         
     def export_data(self, format):
         """
         Get exported data
         """
         params = {"project_name":self.project_name,
@@ -922,15 +980,15 @@
         params = {"project_name":self.project_name,
                   "name":name,
                   "format":format
                   }
         r = self._get("/export/prediction",
             params = params,
             is_json= False)
-        with open(f"./prediction_export.{format}","wb") as f:
+        with open(f"./prediction_{name}_export.{format}","wb") as f:
             f.write(r)
         print(f"Prediction exported in './prediction_{name}_export.{format}'")
 
     def export_bert(self, name:str):
         """
         Get BERT Model
         """
@@ -938,90 +996,93 @@
             return None
         params = {"project_name":self.project_name,
                   "name":name
                   }
         r = self._get("/export/bert",
             params = params,
             is_json= False)
-        if "error" in r:
+        if type(r) is dict:
             print(r)
             return None
         with open(f"./{name}.tar.gz","wb") as f:
             f.write(r)
         print(f"Bert exported in './{name}.tar.gz'")
 
     def compute_projection(self):
         """
         Start computing projection
         """
         params = {
                 "project_name":self.project_name,
                 "user":self.user
                 }
+        
+        try:
+            proj_params = json.loads(self.projection_params.value)
+        except:
+            raise ValueError("Problem in the json parameters")
+
         data = {
             "method":self.projection_method.value, 
             "features":self.projection_features.value,
-            "params":json.loads(self.projection_params.value),
+            "params":proj_params,
             }
         r = self._post("/elements/projection/compute",
             params = params,
             json_data = data)
-        if "success" in r:
+        if r["status"] == "waiting":
             self.projection_data = "computing"
-            self.visualization.children = [widgets.HTML(value = self.projection_data)]
+            self.visualization.children = [widgets.HTML(value = "<div  style='background-color: #ffcc00; padding: 10px;'>Computing</div>")]
         else:
             print(r)
 
     def plot_visualisation(self):
         """
         Produce the visualisation for the projection
-        TODO : legend ; display text
         """
         df = self.projection_data
-        f = go.FigureWidget([go.Scatter(x=df["0"], 
-                                        y=df["1"], 
+        df["to_show"] = df.apply(lambda x : f"{x.name}<br>{'<br>'.join(textwrap.wrap(x['texts'][0:300],width=30))}...", axis=1)
+        f = go.FigureWidget([go.Scatter(x=df[df["labels"]==i]["0"], 
+                                        y=df[df["labels"]==i]["1"], 
                                         mode='markers', 
-                                        customdata = df.index,
-                                        showlegend = False)])
-        scatter = f.data[0]
-        labels = list(df["labels"].unique())
-        colors = distinctipy.get_colors(len(labels)) 
-        colors_map = {labels[i]:colors[i] for i in range(0, len(labels))}
-        scatter.marker.color = [f"rgba({colors_map[i][0]}, {colors_map[i][1]}, {colors_map[i][2]}, 0.5)" for i in list(df["labels"])]
-        scatter.marker.size = [5] * 100
+                                        name = i,
+                                        customdata = np.stack((df[df["labels"]==i]["to_show"],), axis=-1),
+                                        hovertemplate="%{customdata[0]}",
+                                        showlegend = True) for i in df["labels"].unique()])
         f.layout.hovermode = 'closest'
         def update_point(trace, points, selector):
             # select specific text
-            element_id = trace.customdata[points.point_inds][0]
-            print(element_id)
-            self._display_element(element_id)
-        scatter.on_click(update_point)
+            if len(points.point_inds)>0:
+                element_id = trace.customdata[points.point_inds][0][0].split("<br>")[0] #TODO améliorer
+                self._display_element(element_id)
+        for i in range(0,len(f.data)):
+            f.data[i].on_click(update_point)
         self.visualization.children = [f]
 
     def display_bert_informations(self, name):
         """
         Display statistics for a BERT Model
         """
         params = {"project_name":self.project_name,
                             "name":name}
         r = self._get("/models/bert", params = params)
-        if "error" in r:
+        print(r)
+        if r["status"] == "error":
             print(r)
             return 
-        loss = pd.DataFrame(r["loss"])
+        loss = pd.DataFrame(r["data"]["loss"])
         with self.bert_statistics:
             clear_output(wait=True)
-            print(json.dumps(r["parameters"],indent=2))
             fig, ax = plt.subplots(figsize=(3,2))
             fig = loss.plot(ax = ax)
             plt.show(fig)
-            if "f1" in r:
-                print("f1:",r["f1"])
-                print("precision:",r["precision"])
-                print("recall:",r["recall"])
+            if "f1" in r["data"]:
+                print("f1:",r["data"]["f1"])
+                print("precision:",r["data"]["precision"])
+                print("recall:",r["data"]["recall"])
             else:
                 print("Compute prediction for scores")
     
     def get_projection_data(self):
         """
         Get projection data
         """
@@ -1049,23 +1110,26 @@
                 continue
             # check bertmodel status
             if self.bert_training and (not self.user in self.state["bertmodels"]["training"]):
                 self.bert_training = False
                 self.update_tab_bertmodels(state=False)
             # check features status
             if self.state["features"]["available"] != self.available_features.options:
-                self.available_features.options = self.state["features"]["available"]
+                self.update_tab_features(state=False)
+                #self.available_features.options = self.state["features"]["available"]
             # check projection status
             if (type(self.projection_data) is str) and (self.projection_data == "computing"):
                 r = self.get_projection_data()
-                if "data" in r:
-                    self.projection_data = pd.DataFrame(r["data"])
+                if ("data" in r) and (type(r["data"]) is dict):
+                    self.projection_data = pd.DataFrame(r["data"],)
                     self.plot_visualisation()
-        print("End asyncio loop")
-
+            # check simplemodel status
+            if self.computing_simplemodel and (not self.user in self.state["simplemodel"]["training"]):
+                self.computing_simplemodel = False
+                self.update_tab_simplemodel(state=False)
 
     def interface(self):
         """
         General interface
         - divided by tab
         """
 
@@ -1110,23 +1174,63 @@
                             widgets.HBox([self.select_scheme, valid_delete_scheme]),
                             widgets.HBox([new_scheme, valid_new_scheme]),
                             widgets.HTML(value="<hr>"),
                             widgets.HBox([self.select_label, valid_delete_label]),
                             widgets.HBox([new_label, valid_new_label]),
                         ])
 
+        #-------------
+        # Tab Features
+        #-------------
+        self.info_features  = widgets.HTML(value = "No process currently running")
+        self.available_features =  widgets.Dropdown(description = "Available")
+        delete_feature = widgets.Button(description = "Delete", button_style="danger")
+        delete_feature.on_click(lambda x: self.delete_feature(self.available_features.value))
+        self.add_features = widgets.Dropdown(description="Add: ", value="", options=[""])
+        self.features_params = widgets.Textarea(layout=widgets.Layout(width='200px',height='100px'))
+        def if_change_feature(change):
+            if change['type'] == 'change' and change['name'] == 'value':
+                self.features_params.value = json.dumps(self.state["features"]["options"][self.add_features.value],
+                                                        indent = 2)
+        self.add_features.observe(if_change_feature)
+        valid_compute_features = widgets.Button(description = "⚙️Compute")
+        valid_compute_features.on_click(lambda x : self.compute_feature(self.add_features.value, 
+                                                                        self.features_params.value))
+        valid_compute_features.style.button_color = 'lightgreen'
+        add_regex_value = widgets.Text(description="Add regex:")
+        valid_regex = widgets.Button(description = "Add")
+        valid_regex.style.button_color = 'lightgreen'
+        valid_regex.on_click(lambda x: self.add_regex(add_regex_value.value))
+
+        # Populate
+        self.update_tab_features()
+
+        # Group in tab
+        tab_features = widgets.VBox([
+            widgets.HBox([self.available_features,delete_feature]),
+            widgets.HTML(value = "<hr>"),
+            widgets.HBox([self.add_features,self.features_params,valid_compute_features]),
+            widgets.HTML(value = "<hr>"),
+            widgets.HBox([add_regex_value,valid_regex]),
+            self.info_features,
+             ])
+
         #-----------
         # Tab codage
         #-----------
         self._textarea = widgets.Textarea(value="",
                                    layout=widgets.Layout(width='600px',height='150px'), 
                                    description='')
         self._back = widgets.Button(description = "◄ back",layout=widgets.Layout(width='100px'))
         self._back.on_click(lambda x : self._get_previous_element())
         self._mode_selection = widgets.Dropdown(layout=widgets.Layout(width='120px'))
+        def on_change_method(change): # if method change, change the current element
+            if change['type'] == 'change' and change['name'] == 'value':
+                self._display_next()
+        self._mode_selection.observe(on_change_method)
         self._mode_sample = widgets.Dropdown(layout=widgets.Layout(width='120px'))
         self._mode_label = widgets.Dropdown(layout=widgets.Layout(width='120px'),
                                             disabled=True)
         self._labels = widgets.HBox()
         self.info_element = widgets.HTML()
         self.info_predict = widgets.HTML()
         self.add_context = widgets.ToggleButton(description='Context', value=False, icon='valid')
@@ -1156,28 +1260,26 @@
         
         
 
         # Populate
         self.update_tab_annotations()
         self._mode_selection.value = self._mode_selection.options[0]
         self._mode_sample.value = self._mode_sample.options[0]
-        #self._display_next()
-        #self._display_buttons_labels()
 
         # Group in tab
         tab_annotate = widgets.VBox([
                             #self._schemes,
                              widgets.HBox([self._back,
                                     self._mode_selection,
                                     self._mode_sample,
                                     self._mode_label,
-                                    self.info_element,
                                     self.add_context]),
                               self._textarea,
                               self.info_predict,
+                              self.info_element,
                               self.display_context,
                               self._labels,
                               widgets.HTML("<hr>"),
                               self.projection
                             ])
 
         #---------
@@ -1241,27 +1343,28 @@
         #----------------
         self.simplemodel_state = widgets.HTML(value = "State")
         self.simplemodel_statistics= widgets.HTML(value = "Statistics")
 
         self.select_simplemodel =  widgets.Dropdown(description = "Models")
         def on_change_scheme(change):
             if change['type'] == 'change' and change['name'] == 'value':
-                self.simplemodel_params.value = json.dumps(self.state["simplemodel"]["available"][self.select_simplemodel.value],
+                self.simplemodel_params.value = json.dumps(self.state["simplemodel"]["options"][self.select_simplemodel.value],
                                                            indent=2)
         self.select_simplemodel.observe(on_change_scheme)
         self.select_features = widgets.SelectMultiple()
-        self.simplemodel_params = widgets.Textarea(value="",
+        self.simplemodel_params = widgets.Textarea(value=json.dumps({}),
                                                    layout=widgets.Layout(width='300px',height='200px'))
         valid_model = widgets.Button(description = "⚙️Train")
         valid_model.on_click(lambda b : self.create_simplemodel(scheme=self.select_scheme.value, #attention il faudra revoir le choix du scheme
                                                                model = self.select_simplemodel.value,
-                                                               parameters = json.loads(self.simplemodel_params.value),
+                                                               parameters = self.simplemodel_params.value,
                                                                features = self.select_features.value))
-        self.simplemodel_autotrain = widgets.IntSlider(min=1, max=50, 
+        self.simplemodel_autotrain = widgets.IntSlider(min=5, max=50, 
                                       description="")
+        self.computing_simplemodel = False
         # Populate
         self.update_tab_simplemodel()
 
         # Group in tab
         tab_simplemodel = widgets.VBox([
                             widgets.HBox([self.simplemodel_state,self.simplemodel_statistics]),
                             self.select_simplemodel,
@@ -1269,41 +1372,14 @@
                                           self.select_features,
                                           self.simplemodel_params
                                           ]),
                             valid_model,
                             widgets.HTML(value="Autotrain every:"),
                             self.simplemodel_autotrain
              ])
-        #-------------
-        # Tab Features
-        #-------------
-        self.info_features  = widgets.HTML(value = "No process currently running")
-        self.available_features =  widgets.Dropdown(description = "Available")
-        delete_feature = widgets.Button(description = "Delete", button_style="danger")
-        delete_feature.on_click(lambda x: self.delete_feature(self.available_features.value))
-        self.add_features = widgets.Dropdown(description="Add: ", value="", options=[""])
-        valid_compute_features = widgets.Button(description = "⚙️Compute")
-        valid_compute_features.on_click(lambda x : self.compute_feature(self.add_features.value))
-        valid_compute_features.style.button_color = 'lightgreen'
-        add_regex_value = widgets.Text(description="Add regex:")
-        #add_regex_name = widgets.Text(description="Name:")
-        valid_regex = widgets.Button(description = "Add")
-        valid_regex.style.button_color = 'lightgreen'
-        valid_regex.on_click(lambda x: self.add_regex(add_regex_value.value))
-
-        # Populate
-        self.update_tab_features()
-
-        # Group in tab
-        tab_features = widgets.VBox([
-            widgets.HBox([self.available_features,delete_feature]),
-            widgets.HBox([self.add_features,valid_compute_features]),
-            widgets.HBox([add_regex_value,valid_regex]),
-            self.info_features,
-             ])
 
         #--------------
         # Tab BertModel
         #--------------
 
         """
         Logic : train a bertmodel by user
@@ -1311,17 +1387,17 @@
         TODO : upgrade management of models
         """
 
         self.bert_status = widgets.Text(disabled=True)
         self.available_bert = widgets.Dropdown(description="Select:")
         self.bert_statistics = widgets.Output()
         def on_change_model(change): # if select one, display its options on_select
-            if change['type'] == 'change' and change['name'] == 'value':
+            if change['type'] == 'change' and change['name'] == 'value' and self.available_bert.value is not None:
                 # available predict button
-                if self.state["bertmodels"]["available"][self.select_scheme.value][self.available_bert.value][0]:
+                if self.state["bertmodels"]["available"][self.select_scheme.value][self.available_bert.value]["predicted"]:
                     self.compute_prediction.disabled = True
                 else:
                     self.compute_prediction.disabled = False
                 # get information about the model
                 self.display_bert_informations(self.available_bert.value)
         self.available_bert.observe(on_change_model)
         self.bert_summary = widgets.Accordion(children=[self.bert_statistics], 
@@ -1352,17 +1428,17 @@
                                 self.new_bert_params,
                                 self.compute_new_bert,
                                 widgets.HTML(value="<hr>Save current model<br>"),
                                 widgets.HBox([self.bert_name, self.record_bert]),
                         
                              ])
 
-        #--------------
-        # Tab BertModel
-        #--------------
+        #-----------
+        # Tab Export
+        #-----------
 
         layout_button=widgets.Layout(width='80px')
         layout_menu=widgets.Layout(width='150px')
 
 
         # data
         export_tagged_data_presentation = widgets.HTML(value="<hr>Export tagged data<br>")
@@ -1440,11 +1516,10 @@
         
         # Update everything on tab change
         def on_tab_selected(change):
             self.update_global()
         self.output.observe(on_tab_selected, names='selected_index')
 
         # Display
-        #clear_output()
-        #display(self.output)
-        self.global_output.children = [self.output]
+        general_info = widgets.HTML(value=f"<b>Current user: {self.user}</b>")
+        self.global_output.children = [general_info, self.output]
```

### Comparing `activetigger-0.0.9/pyproject.toml` & `activetigger-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 name = "activetigger"
 authors = [{name = "Émilien Schultz - Julien Boelaert - Étienne Ollion", email = "emilien.schultz@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = ["fastapi[all]",
+		"sentencepiece",
 		"requests",
 		"uvicorn",
 		"argparse",
 		"datasets",
 		"fasttext",
 		"ipywidgets",
 		"pyyaml",
```

### Comparing `activetigger-0.0.9/requirements.txt` & `activetigger-0.1.0/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 transformers[torch]
 sentence_transformers
 typing-inspect
 typing_extensions
 spacy
 pyyaml
 protobuf
-umap-learn
-distinctipy
 python-jose[cryptography]
 bcrypt
 plotly
 matplotlib
+sentencepiece
+umap-learn
+Jupyter
+sacremoses
 
 https://github.com/explosion/spacy-models/releases/download/fr_core_news_sm-3.7.0/fr_core_news_sm-3.7.0.tar.gz#egg=fr_core_news_sm
 https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.7.1/en_core_web_sm-3.7.1.tar.gz#egg=en_core_web_sm
```

### Comparing `activetigger-0.0.9/tests/test_project.py` & `activetigger-0.1.0/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `activetigger-0.0.9/PKG-INFO` & `activetigger-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: activetigger
-Version: 0.0.9
+Version: 0.1.0
 Summary: ActiveTigger in Python
 Author-email: Émilien Schultz - Julien Boelaert - Étienne Ollion <emilien.schultz@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi[all]
+Requires-Dist: sentencepiece
 Requires-Dist: requests
 Requires-Dist: uvicorn
 Requires-Dist: argparse
 Requires-Dist: datasets
 Requires-Dist: fasttext
 Requires-Dist: ipywidgets
 Requires-Dist: pyyaml
@@ -41,43 +42,42 @@
 [![Python Version](https://img.shields.io/badge/python-3.11-blue)](https://www.python.org/downloads/)
 [![PyPI Version](https://img.shields.io/pypi/v/activetigger)](https://pypi.org/project/activetigger/)
 
 Server/client BERT fine tunning app using active learning
 
 [Python refactoring of R Shiny ActiveTigger app (Julien Boelaert & Etienne Ollion)]( https://gitlab.univ-lille.fr/julien.boelaert/activetigger)
 
-
 ## Installation
 
 You can install `activetigger` via pip:
 
 ```bash
 pip install activetigger
 ```
 
-And install the requirements with 
-
+## Use
 
-```bash
-pip install -r requirements.txt
-```
+Create a config file `config.yaml` in the directory where you want to launch the server :
 
-## Use
+- `path` : path to store files (for instance `./data`)
+- `secret_key` : to secure tokens. To generate it `openssl rand -hex 32C`
+- `path_fasttext`:  absolute path to fasttext model
+- `users`: list of user:password
 
-To launch the server
+Then, to launch the server (on port 8000)
 
 ```python
 python -m activetigger
 ```
 
 To use the widget in the `widget` module, you can do the following:
 
 ```python
 from activetigger import widget
-at = widget.Widget()
+at = widget.Widget(URL_SERVER="http://0.0.0.0:8000")
 ```
 
 ## Technical specifications
 
 - REST-like client/server architecture
 - Mixed data storage : sqlite + files
 - Backend Python
```

