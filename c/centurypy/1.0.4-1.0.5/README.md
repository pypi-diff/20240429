# Comparing `tmp/centurypy-1.0.4.tar.gz` & `tmp/centurypy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centurypy-1.0.4.tar", last modified: Fri Apr 26 17:33:20 2024, max compression
+gzip compressed data, was "centurypy-1.0.5.tar", last modified: Mon Apr 29 01:11:40 2024, max compression
```

## Comparing `centurypy-1.0.4.tar` & `centurypy-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-26 17:33:19.997066 centurypy-1.0.4/
--rw-r--r--   0 gerardovivas   (501) staff       (20)     1070 2023-12-18 17:56:28.000000 centurypy-1.0.4/LICENSE
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-26 17:33:19.996581 centurypy-1.0.4/PKG-INFO
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2612 2023-12-29 04:38:18.000000 centurypy-1.0.4/README.md
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-26 17:33:19.992741 centurypy-1.0.4/centurypy/
--rw-r--r--   0 gerardovivas   (501) staff       (20)       27 2023-10-13 17:46:30.000000 centurypy-1.0.4/centurypy/__init__.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2582 2024-04-26 16:08:47.000000 centurypy-1.0.4/centurypy/century.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     4398 2024-04-26 14:55:07.000000 centurypy-1.0.4/centurypy/genetic.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     5003 2024-04-26 17:26:55.000000 centurypy-1.0.4/centurypy/main.py
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-26 17:33:19.995757 centurypy-1.0.4/centurypy.egg-info/
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-26 17:33:19.000000 centurypy-1.0.4/centurypy.egg-info/PKG-INFO
--rw-r--r--   0 gerardovivas   (501) staff       (20)      272 2024-04-26 17:33:19.000000 centurypy-1.0.4/centurypy.egg-info/SOURCES.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)        1 2024-04-26 17:33:19.000000 centurypy-1.0.4/centurypy.egg-info/dependency_links.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       19 2024-04-26 17:33:19.000000 centurypy-1.0.4/centurypy.egg-info/requires.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       10 2024-04-26 17:33:19.000000 centurypy-1.0.4/centurypy.egg-info/top_level.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       38 2024-04-26 17:33:19.997211 centurypy-1.0.4/setup.cfg
--rw-r--r--   0 gerardovivas   (501) staff       (20)      873 2024-04-26 17:32:51.000000 centurypy-1.0.4/setup.py
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-29 01:11:40.140742 centurypy-1.0.5/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     1070 2024-04-28 15:02:42.000000 centurypy-1.0.5/LICENSE
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-29 01:11:40.140614 centurypy-1.0.5/PKG-INFO
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2612 2024-04-28 15:02:42.000000 centurypy-1.0.5/README.md
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-29 01:11:40.139729 centurypy-1.0.5/centurypy/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       27 2024-04-28 15:02:42.000000 centurypy-1.0.5/centurypy/__init__.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2253 2024-04-28 17:01:46.000000 centurypy-1.0.5/centurypy/century.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     4395 2024-04-28 21:02:22.000000 centurypy-1.0.5/centurypy/genetic.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     5814 2024-04-29 00:56:30.000000 centurypy-1.0.5/centurypy/main.py
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-29 01:11:40.140428 centurypy-1.0.5/centurypy.egg-info/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-29 01:11:40.000000 centurypy-1.0.5/centurypy.egg-info/PKG-INFO
+-rw-r--r--   0 gerardovivas   (501) staff       (20)      272 2024-04-29 01:11:40.000000 centurypy-1.0.5/centurypy.egg-info/SOURCES.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)        1 2024-04-29 01:11:40.000000 centurypy-1.0.5/centurypy.egg-info/dependency_links.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       19 2024-04-29 01:11:40.000000 centurypy-1.0.5/centurypy.egg-info/requires.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       10 2024-04-29 01:11:40.000000 centurypy-1.0.5/centurypy.egg-info/top_level.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       38 2024-04-29 01:11:40.140779 centurypy-1.0.5/setup.cfg
+-rw-r--r--   0 gerardovivas   (501) staff       (20)      872 2024-04-29 01:07:19.000000 centurypy-1.0.5/setup.py
```

### Comparing `centurypy-1.0.4/LICENSE` & `centurypy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `centurypy-1.0.4/PKG-INFO` & `centurypy-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centurypy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to train and run the CENTURY (Soil Organic Matter) model
 Home-page: https://github.com/vivas24/centurypy
 Author: Gerardo Vivas
 Author-email: vivas.fermin24@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `centurypy-1.0.4/README.md` & `centurypy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `centurypy-1.0.4/centurypy/century.py` & `centurypy-1.0.5/centurypy/century.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,75 +3,53 @@
 
 class Century:
 
     ACTIVE_CONTAINER_INDEX = 3
     RESPIRATION_CONTAINER_INDEX = 5
 
 
-    def __init__(self, Necromasa , LN , FraLA ,LENo ,PASo , ACTo , RESPo):
+    def __init__(self, initial_values ):
+        Necromasa , LN , FraLA ,LENo ,PASo , ACTo , RESPo = initial_values
         self.Necromasa = Necromasa
         self.LN = LN
         self.FraLA = FraLA
         self.fs = 0.85 - (0.018 * self.LN)
         self.Ftex = 0.85 - (0.68 * self.FraLA)
         self.ESTo = self.Necromasa * (1 - self.fs)
         self.METo = self.Necromasa * self.fs
         self.LENo = LENo
         self.PASo = PASo
         self.ACTo = ACTo
         self.RESPo = RESPo
 
 
     def resolve(self, time, params):
-        Kmet = params[0] 
-        Kest = params[1]
-        Kminl = params[2]
-        Khumac = params[3]
-        Kminp = params[4]
-        ResEL = params[5]
-        ResEA = params[6]
-        ResMet = params[7]
-        ResLA = params[8]
-        ResPA = params[9]
-        PartEst = params[10]
-        PartLen = params[11]
-        PartAct = params[12]
-
-        y0 = self.ESTo, self.METo, self.LENo, self.ACTo, self.PASo, self.RESPo
-        
-        args = (self.Ftex, Kmet, Kest, Kminl, Khumac, Kminp, ResEL, ResEA, ResMet, ResLA, ResPA, PartEst, PartLen, PartAct)
-        
+        y0 = (self.ESTo, self.METo, self.LENo, self.ACTo, self.PASo, self.RESPo)
+        args = (self.Ftex, params[0], params[1], params[2], params[3], params[4], params[5], 
+                params[6], params[7], params[8], params[9], params[10], params[11], params[12] )
         y = odeint(Century.ode, y0, time, args)
-        
         return ([row[Century.ACTIVE_CONTAINER_INDEX] for row in y ], [row[Century.RESPIRATION_CONTAINER_INDEX] for row in y ])
     
 
     @staticmethod
     def ode(y, time, Ftex, Kmet, Kest, Kminl, Khumac, Kminp, ResEL, ResEA, ResMet, ResLA, ResPA, PartEst, PartLen, PartAct):
         ESTo, METo, LENTo, ACTo, PASo, RESPo = y
-        
         dESTdt = -ESTo * Kest 
-        
         dMETdt = -METo * Kmet 
-        
         dLENTdt = ((1 - ResEL) * PartEst * ESTo * Kest)  \
                 + ((1 - Ftex - PartAct) * ACTo * Khumac) \
                 - (LENTo * Kminl)
-        
         dACTdt =  ((1 - ResEA) * (1 -PartEst) * ESTo * Kest) \
                 + ((1 - ResMet) * METo * Kmet) \
                 + ((1 - ResLA - PartLen) * LENTo * Kminl) \
                 + ((1 - ResPA) * PASo * Kminp) \
                 - (ACTo * Khumac)
-        
         dPASdt =  (PartAct * ACTo * Khumac) \
                 + (PartLen * LENTo * Kminl) \
                 - (PASo * Kminp) 
-        
         dRESPdt = (ResEL * PartEst * ESTo * Kest) \
                 + (ResEA * (1 - PartEst) * ESTo * Kest) \
                 + (Ftex * ACTo * Khumac) \
                 + (ResMet * METo * Kmet) \
                 + (ResLA * LENTo * Kminl) \
                 + (ResPA * PASo * Kminp)
-        
         return (dESTdt, dMETdt, dLENTdt, dACTdt, dPASdt, dRESPdt)
```

### Comparing `centurypy-1.0.4/centurypy/genetic.py` & `centurypy-1.0.5/centurypy/genetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,35 @@
         self.error = sys.maxsize
         self.start_time = time.time()
         self.population = []
         self.milestones = []
         self.fitness = []
         self.generate_population()
 
+    def generate_population(self):
+        for i in range(self.population_size):
+            child = list(np.random.rand(self.n_params))
+            self.population.append(child)
+
+    def evolve(self, generations):
+        for _ in range(generations):
+            self.evaluate_population()
+            self.update_error()
+            self.population = self.select_offspring()
+            self.mutate()
+            self.print_status()
+            self.generation += 1
+        self.print_status(True)
+
+    def evaluate_population(self):
+        fitness_tmp = []
+        for child in self.population:
+            y = self.mse(child)
+            fitness_tmp += [y]
+        self.fitness = np.array(fitness_tmp)
 
     def mse(self, parameters):
         model_data = self.century_model.resolve(self.time_data, parameters)
         max_value = 0
         for i in [0,1]:
             values_model = model_data[i]
             values_training = self.training_data[i]
@@ -34,86 +55,62 @@
             for j in range(len(values_model)):
                 sum += (values_model[j] - values_training[j]) ** 2
             avg = (sum / len(values_model))
             if(avg > max_value):
                 max_value = avg
         return round(max_value)
 
-    def generate_population(self):
-        for i in range(self.population_size):
-            child = list(np.random.rand(self.n_params))
-            self.population.append(child)
-
-    def mutate(self):
-        for i in range(len(self.population)):
-            child = self.population[i]
-            if np.random.random() < self.mutation_rate:
-                gen = list(np.random.rand(self.gen_len))
-                index = np.random.randint(len(child) - self.gen_len + 1)
-                child = child[0:index] + gen + child[index + self.gen_len:]
-            self.population[i] = child
-
-    def evaluate_population(self):
-        fitness_tmp = []
-        for child in self.population:
-            y = self.mse(child)
-            fitness_tmp += [y]
-        self.fitness = np.array(fitness_tmp)
-
     def update_error(self):
         fitness_sorted = sorted(self.fitness)
         error = fitness_sorted[0]
         if(error < self.error and error >= 0):
             self.error = error
             self.milestones.append([self.generation, self.error])
 
-    def choose_parents(self):
-        fitness_tmp = []
-        population_tmp = []
-        for i in range(int(self.population_size * self.selection_rate)):
-            index = np.random.choice(self.population_size)
-            fitness_tmp.append(self.fitness[index])
-            population_tmp.append(self.population[index])
-        parents = [x for _,x in sorted(zip(fitness_tmp,population_tmp))]
-        return (parents[0],parents[1])
-
     def select_offspring(self):
         offspring = []
         for i in range(self.population_size//2):
             parents =  self.choose_parents()
             cross_point = np.random.randint(self.n_params)
             offspring += [ parents[0][:cross_point] + parents[1][cross_point:] ]
             offspring += [ parents[1][:cross_point] + parents[0][cross_point:] ]
         return offspring
 
+    def choose_parents(self):
+        fitness_tmp = []
+        population_tmp = []
+        for i in range(int(self.population_size * self.selection_rate)):
+            index = np.random.choice(self.population_size)
+            fitness_tmp.append(self.fitness[index])
+            population_tmp.append(self.population[index])
+        parents = [x for _,x in sorted(zip(fitness_tmp,population_tmp))]
+        return (parents[0],parents[1])
 
-    def evolve(self, generations):
-        for _ in range(generations):
-            self.evaluate_population()
-            self.update_error()
-            self.population = self.select_offspring()
-            self.mutate()
-            self.print_status()
-            self.generation += 1
-        self.print_status(True)
-
-    def format_time(self, seconds):
-        hh = int(seconds // 3600)
-        mm = int((seconds - (hh * 3600)) // 60)
-        ss = int((seconds - (hh * 3600) - (mm * 60)))
-        return f'{ "0" if hh < 10 else "" }{hh}:{"0" if mm < 10 else ""}{mm}:{"0" if ss < 10 else ""}{ss}'
+    def mutate(self):
+        for i in range(len(self.population)):
+            child = self.population[i]
+            if np.random.random() < self.mutation_rate:
+                gen = list(np.random.rand(self.gen_len))
+                index = np.random.randint(len(child) - self.gen_len + 1)
+                child = child[0:index] + gen + child[index + self.gen_len:]
+            self.population[i] = child
 
     def print_status(self,done = False):
         time_formatted = self.format_time(time.time() - self.start_time)
         error_str = '{}'.format(self.error).rjust(10," ")
         if done: 
             print(f'DONE! => time: {time_formatted}, generation: {self.generation}, error: {error_str}')     
         else:
             print(f'time: {time_formatted}, generation: {self.generation}, error: {error_str}', end='\r') 
 
+    def format_time(self, seconds):
+        hh = int(seconds // 3600)
+        mm = int((seconds - (hh * 3600)) // 60)
+        ss = int((seconds - (hh * 3600) - (mm * 60)))
+        return f'{ "0" if hh < 10 else "" }{hh}:{"0" if mm < 10 else ""}{mm}:{"0" if ss < 10 else ""}{ss}'
 
     def solution(self):
         index = -1
         min_value = sys.maxsize
         for i in range(len(self.population)):
             child = self.population[i]
             value = self.mse(child)
```

### Comparing `centurypy-1.0.4/centurypy/main.py` & `centurypy-1.0.5/centurypy/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,44 +48,52 @@
     def __load_input_file(self, input_file):
         df = pd.read_csv(input_file,header=None)
         array = df.to_numpy()
         self.training_data = (array[:,1][:],array[:,2][:])
         self.time_data = array[:,0][:]
 
     def __load_century_model(self,input_values):
-        self.century_model = Century(
-            Necromasa = input_values['necromasa'], 
-            ACTo=input_values['acto'], 
-            LENo=input_values['leno'], 
-            PASo=input_values['paso'], 
-            RESPo= input_values['respo'] , 
-            LN= input_values['ln'], 
-            FraLA= input_values['frala']
-        )
+        self.century_model = Century([
+            input_values['necromasa'],
+            input_values['ln'],
+            input_values['frala'],
+            input_values['leno'],
+            input_values['paso'],
+            input_values['acto'],
+            input_values['respo'],
+        ])
 
     def __load_genetic_model(self):
         self.genetic_model = Genetic(self.century_model,
                                      self.time_data,
                                      self.training_data)
 
+    def fit_model(self, generations = 500, chart = False):
+        self.genetic_model.evolve(generations)
+        self.fitted_params = self.genetic_model.solution()
+        self.__save_parameters()
+        self.__display_parameters()
+        if chart:
+            self.__display_fitted_chart()
+
     def __save_parameters(self):
         f = open("parameters.txt","w")
         for i in range(len(self.fitted_params)):
             f.write(f'{self.params_name[i]}: {self.fitted_params[i]}\n')
         f.close()
 
     def __display_parameters(self):
         print('+++++++++++++++++++++++++++++++++++++++++++++++')
         print('+++++++++++++++ PARAMETERS ++++++++++++++++++++')
         for i in range(len(self.fitted_params)):
             param_name = self.params_name[i]
             print(f'{param_name.rjust(10," ")}: {self.fitted_params[i]}')
         print('+++++++++++++++++++++++++++++++++++++++++++++++')
 
-    def __display_chart(self):
+    def __display_fitted_chart(self):
         generations, error = zip(*self.genetic_model.milestones)
         solution = self.century_model.resolve(self.time_data, self.fitted_params )
         fig, axes = plt.subplots(2,1)
         colors = ['b','r']
         names = ['Active','Respiration']
         for i in [0,1]:
             name = names[i]
@@ -100,36 +108,49 @@
                          label = f'{name} (Solution)')
         axes[0].set(xlabel='Time',ylabel='C(mg)')
         axes[0].legend()
         axes[1].plot(generations,error,'b.-')
         axes[1].set(xlabel='Generations',ylabel='Error (MSE)')
         plt.show()
 
-    def fit_model(self, generations = 500, chart = False):
-        self.genetic_model.evolve(generations)
-        self.fitted_params = self.genetic_model.solution()
-        self.__save_parameters()
-        self.__display_parameters()
-        if chart:
-            self.__display_chart()
-
     def predict_values(self, day, chart = True):
-        time_data = np.linspace(0,day)
-        solution = self.century_model.resolve(time_data, self.fitted_params)
+        if int(day) < 0:
+           raise Exception("Day must be a positive number")
+        time_data = np.linspace(0,day,dtype=int)
+        solution_data = self.century_model.resolve(time_data, self.fitted_params)      
         if(chart):
-            fig = plt.subplot()
-            colors = ['b','r']
-            names = ['Active','Respiration']
-            for i in [0,1]:
-                name = names[i]
-                color = colors[i]
-                fig.plot(time_data,
-                            solution[i],
-                            f'{color}.')
-                fig.plot(time_data,
-                            solution[i],
-                            f'{color}-' , 
-                            label = f'{name}')
-            fig.set(xlabel='Time',ylabel='C(mg)')
-            fig.legend()
-            plt.show()
+            self.__display_prediction_chart(time_data, solution_data)
+        else:
+            self.__display_prediction_values(time_data,solution_data)
+
+    def __display_prediction_chart(self,time,data):
+        fig = plt.subplot()
+        colors = ['b','r']
+        names = ['Active','Respiration']
+        for i in [0,1]:
+            name = names[i]
+            color = colors[i]
+            fig.plot(time,
+                        data[i],
+                        f'{color}.')
+            fig.plot(time,
+                        data[i],
+                        f'{color}-' , 
+                        label = f'{name}')
+        fig.set(xlabel='Time',ylabel='C(mg)')
+        fig.legend()
+        plt.show()
+
+    def __display_prediction_values(self,time,data):
+        print('+++++++++++++++++++++++++++++++++++++++++++++++')
+        print('++++++++++++++++ SOLUTION +++++++++++++++++++++')
+        rows = zip(time,data[0],data[1])
+        active_label = 'Active'
+        respiration_label = 'Respiration'
+        for row in rows:
+            print(f'Day {row[0]}:')
+            print(f'{active_label.rjust(15," ")}: {"{:.2f}".format(row[1])}')
+            print(f'{respiration_label.rjust(15," ")}: {"{:.2f}".format(row[2])}')
+            print()
+        print('+++++++++++++++++++++++++++++++++++++++++++++++')
 
+
```

### Comparing `centurypy-1.0.4/centurypy.egg-info/PKG-INFO` & `centurypy-1.0.5/centurypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centurypy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to train and run the CENTURY (Soil Organic Matter) model
 Home-page: https://github.com/vivas24/centurypy
 Author: Gerardo Vivas
 Author-email: vivas.fermin24@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `centurypy-1.0.4/setup.py` & `centurypy-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 PACKAGE_NAME = 'centurypy'
 AUTHOR = 'Gerardo Vivas'
 AUTHOR_EMAIL = 'vivas.fermin24@gmail.com'
 URL = 'https://github.com/vivas24/centurypy'
 LICENSE = 'MIT'
 DESCRIPTION = 'Library to train and run the CENTURY (Soil Organic Matter) model' 
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
 LONG_DESC_TYPE = 'text/markdown'
-
 INSTALL_REQUIRES = [
     'numpy',
     'pandas',
     'scipy',
 ]
 
 setup(
```

