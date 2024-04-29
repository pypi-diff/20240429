# Comparing `tmp/ipd_axelrod-1.0.0.tar.gz` & `tmp/ipd_axelrod-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipd_axelrod-1.0.0.tar", last modified: Sun Apr 28 10:07:54 2024, max compression
+gzip compressed data, was "ipd_axelrod-1.1.0.tar", last modified: Mon Apr 29 16:21:42 2024, max compression
```

## Comparing `ipd_axelrod-1.0.0.tar` & `ipd_axelrod-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 toby       (502) staff       (20)        0 2024-04-28 10:07:54.071025 ipd_axelrod-1.0.0/
--rw-r--r--   0 toby       (502) staff       (20)     1069 2024-04-28 06:31:04.000000 ipd_axelrod-1.0.0/LICENSE
--rw-r--r--   0 toby       (502) staff       (20)      634 2024-04-28 10:07:54.070059 ipd_axelrod-1.0.0/PKG-INFO
--rw-r--r--   0 toby       (502) staff       (20)     4862 2024-04-27 07:13:37.000000 ipd_axelrod-1.0.0/README.md
--rw-r--r--   0 toby       (502) staff       (20)      511 2024-04-28 10:07:40.000000 ipd_axelrod-1.0.0/pyproject.toml
--rw-r--r--   0 toby       (502) staff       (20)      207 2024-04-28 09:57:31.000000 ipd_axelrod-1.0.0/readme-pypi.md
--rw-r--r--   0 toby       (502) staff       (20)       38 2024-04-28 10:07:54.071186 ipd_axelrod-1.0.0/setup.cfg
-drwxr-xr-x   0 toby       (502) staff       (20)        0 2024-04-28 10:07:54.036931 ipd_axelrod-1.0.0/src/
-drwxr-xr-x   0 toby       (502) staff       (20)        0 2024-04-28 10:07:54.055391 ipd_axelrod-1.0.0/src/IPD/
--rw-r--r--   0 toby       (502) staff       (20)        0 2024-04-28 06:25:56.000000 ipd_axelrod-1.0.0/src/IPD/__init__.py
--rw-r--r--   0 toby       (502) staff       (20)      194 2024-04-28 07:56:45.000000 ipd_axelrod-1.0.0/src/IPD/__main__.py
--rw-r--r--   0 toby       (502) staff       (20)     3152 2024-04-28 09:03:45.000000 ipd_axelrod-1.0.0/src/IPD/data.py
--rw-r--r--   0 toby       (502) staff       (20)     8889 2024-04-28 08:02:20.000000 ipd_axelrod-1.0.0/src/IPD/gui.py
--rw-r--r--   0 toby       (502) staff       (20)     2241 2024-04-28 09:46:16.000000 ipd_axelrod-1.0.0/src/IPD/main.py
--rw-r--r--   0 toby       (502) staff       (20)     1185 2024-04-28 09:05:46.000000 ipd_axelrod-1.0.0/src/IPD/play.py
--rw-r--r--   0 toby       (502) staff       (20)     1319 2024-04-28 08:02:58.000000 ipd_axelrod-1.0.0/src/IPD/profiles.py
--rw-r--r--   0 toby       (502) staff       (20)     6420 2024-04-28 09:41:20.000000 ipd_axelrod-1.0.0/src/IPD/strategies.py
-drwxr-xr-x   0 toby       (502) staff       (20)        0 2024-04-28 10:07:54.065769 ipd_axelrod-1.0.0/src/IPD_axelrod.egg-info/
--rw-r--r--   0 toby       (502) staff       (20)      634 2024-04-28 10:07:54.000000 ipd_axelrod-1.0.0/src/IPD_axelrod.egg-info/PKG-INFO
--rw-r--r--   0 toby       (502) staff       (20)      348 2024-04-28 10:07:54.000000 ipd_axelrod-1.0.0/src/IPD_axelrod.egg-info/SOURCES.txt
--rw-r--r--   0 toby       (502) staff       (20)        1 2024-04-28 10:07:54.000000 ipd_axelrod-1.0.0/src/IPD_axelrod.egg-info/dependency_links.txt
--rw-r--r--   0 toby       (502) staff       (20)        4 2024-04-28 10:07:54.000000 ipd_axelrod-1.0.0/src/IPD_axelrod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:21:42.782991 ipd_axelrod-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 16:21:42.782991 ipd_axelrod-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/readme-pypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:21:42.782991 ipd_axelrod-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:21:42.778991 ipd_axelrod-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:21:42.782991 ipd_axelrod-1.1.0/src/IPD/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/src/IPD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/src/IPD/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/src/IPD/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10184 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/src/IPD/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/src/IPD/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/src/IPD/play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/src/IPD/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-29 16:21:38.000000 ipd_axelrod-1.1.0/src/IPD/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:21:42.782991 ipd_axelrod-1.1.0/src/IPD_axelrod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 16:21:42.000000 ipd_axelrod-1.1.0/src/IPD_axelrod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-29 16:21:42.000000 ipd_axelrod-1.1.0/src/IPD_axelrod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:21:42.000000 ipd_axelrod-1.1.0/src/IPD_axelrod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 16:21:42.000000 ipd_axelrod-1.1.0/src/IPD_axelrod.egg-info/top_level.txt
```

### Comparing `ipd_axelrod-1.0.0/LICENSE` & `ipd_axelrod-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipd_axelrod-1.0.0/PKG-INFO` & `ipd_axelrod-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPD-axelrod
-Version: 1.0.0
+Version: 1.1.0
 Summary: A tool for the iterated prisoners dilemma
 Author: jumpingtj
 Project-URL: Homepage, https://github.com/jumpingtj/prisoners-dilemma
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ipd_axelrod-1.0.0/src/IPD/data.py` & `ipd_axelrod-1.1.0/src/IPD/data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,68 @@
 from copy import deepcopy
-from random import randint
+from random import Random, randint
 
 
-class Player(object):
+class Player:
+    first = None
+    name = "Unknown"
     def __init__(self, score=0):
-        self.name = None
         self.score = score
         self.last_action = None
         self.this_action = None
         self.opponent = None
 
+    def setup(self, random_instance=None, noise=0):
+        if random_instance:
+            self._random = random_instance
+        else:
+            self._random = Random()
+        self.noise = noise
+
     def _match_reset(self):
         self.history = []
         self.score = 0
         self.init_match()
 
     def init_match(self):
         """Runs before the start of a new match. Reset any variables here!
         """
         pass
 
     def reset_score(self):
         self.score = 0
 
-    def _action(self, opponent):
-        self.this_action = self.action(opponent)
+    def _action(self, opponent, first=False):
+        if first and self.first != None:
+            self.this_action = self.first
+        else:
+            self.this_action = self.action(opponent)
+        self.this_action = self.this_action ^ (self._random.random() < self.noise)
         return self.this_action
 
     def action(self, opponent):
         return True
 
     def update_history(self):
         self.history.append(self.this_action)
 
     def add_points(self, points):
         self.score += points
 
+    def random(self, prob):
+        return self._random.random() < prob
+
 
 # -------------------------------------------------- #
 
-class Population(object):
-    def __init__(self, members: list):
+class Population:
+    def __init__(self, members: list, noise=0):
         self.members = members
+        for m in self.members:
+            m.setup(noise=noise)
 
     def __repr__(self):
         return "{}".format(self.members)
 
     def __iter__(self):
         return iter(self.members)
 
@@ -110,8 +127,7 @@
             else:
                 dist[member.name] = 1
             total_num_players += 1
         for member in dist:
             prop = dist[member] / total_num_players * 100
             dist[member] = '%.2f' % prop
         return dist
-
```

### Comparing `ipd_axelrod-1.0.0/src/IPD/gui.py` & `ipd_axelrod-1.1.0/src/IPD/gui.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,112 +1,131 @@
-from tkinter import Tk, Frame, IntVar, Button, Label, Menu, Canvas, Entry, TclError, BOTH, TOP, E, S, messagebox
-import matplotlib
-matplotlib.use('TkAgg')
+from .main import run_simulation
+import matplotlib.pyplot as plt
+from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, \
     NavigationToolbar2Tk
-from matplotlib.figure import Figure
-import matplotlib.pyplot as plt
-from .main import run_simulation
+from tkinter import Tk, Frame, IntVar, Button, Label, Menu, Canvas, Entry, TclError, BOTH, TOP, E, S, messagebox, ttk, DoubleVar
+import matplotlib
+matplotlib.use('TkAgg')
 
 
 class SimulationGUI(Frame):
     def __init__(self, parent):
         super().__init__(parent)
         self.parent = parent
         self.pack(fill=BOTH)
         self.config(bg=bg['default'])
 
         self.header = Frame(self)
-        self.setting_frame = Frame(self)
         self.graph_frame = Frame(self)
         self.footer = Frame(self)
 
         self.header.grid(row=0, column=0, columnspan=2)
-        self.setting_frame.grid(row=1, column=0)
         self.graph_frame.grid(row=1, column=1)
         self.footer.grid(row=2, column=0, columnspan=2)
 
         self.curr_row = 0
 
-        self.init_strats()
-        self.init_params()
+        self.init_settings()
         self.init_graph()
         self.init_menu()
         self.init_decor()
 
+    def init_settings(self):
+        self.setting_frame_top = Frame(self)
+        self.setting_book = ttk.Notebook(self.setting_frame_top)
+        self.setting_book.grid()
+        self.setting_frame_mainsub = Frame(self)
+        self.setting_frame_pop = Frame(self)
+        self.setting_book.add(self.setting_frame_mainsub, text="Settings")
+        self.setting_book.add(self.setting_frame_pop, text="Population")
+        self.setting_frame_top.grid(row=1, column=0)
+        self.init_strats()
+        self.init_params()
+        # self.init_presets()
+        self.init_setting_buttons()
+
+    def init_setting_buttons(self):
+
+        self.setting_button_frame = Frame(self.setting_frame_top)
+        self.clear_button = Button(self.setting_button_frame, text='Clear',
+                                   font=fonts['sub_button'], height=2,
+                                   command=self.reset)
+        self.clear_button.grid(row=0, column=0)
+        self.execute_button = Button(self.setting_button_frame, text='Execute',
+                                     font=fonts['main_button'], height=2,
+                                     command=self.confirm, bg='blue')
+        self.execute_button.grid(row=0, column=1)
+        self.setting_button_frame.grid(row=self.curr_row, column=0)
+        self.curr_row += 1
+
     def init_strats(self):
         self.coop_strats = {
             'Kantian': IntVar(),
             'Tit for Tat': IntVar(),
             'Tit for 2 Tats': IntVar(),
             'Grudger': IntVar(),
         }
         self.self_strats = {
             'Defector': IntVar(),
+            'Wary Tit for Tat': IntVar(),
             'Mean Tit for Tat': IntVar(),
             'Conniver': IntVar(),
-            'Tester': IntVar()
+            'Tester': IntVar(),
+            'Grofman': IntVar()
         }
         self.neut_strats = {
-            'Wary Tit for Tat': IntVar(),
             'Random': IntVar(),
         }
         self.all_strats = {
             'Cooperative strategies': self.coop_strats,
-            'Selfish strategies': self.self_strats,
+            'Mean strategies': self.self_strats,
             'Neutral strategies': self.neut_strats
         }
-        Label(self.setting_frame, text="Initial Profile",
+        Label(self.setting_frame_pop, text="Initial Profile",
               font=fonts['header'], height=2).grid(row=self.curr_row, column=0)
         self.curr_row += 1
 
         for strategy_type in self.all_strats:
-            Label(self.setting_frame, text=strategy_type, font=fonts['sub_header'],
+            Label(self.setting_frame_pop, text=strategy_type, font=fonts['sub_header'],
                   padx=15, width=15).grid(row=self.curr_row)
             self.curr_row += 1
             for strategy in self.all_strats[strategy_type]:
-                Label(self.setting_frame, text=strategy + ' -', font=fonts['text'],
+                self.all_strats[strategy_type][strategy].set(10)
+                Label(self.setting_frame_pop, text=strategy + ' -', font=fonts['text'],
                       width=15, anchor=E).\
                     grid(row=self.curr_row, column=0)
-                Entry(self.setting_frame, width=entry_width, justify='right',
+                Entry(self.setting_frame_pop, width=entry_width, justify='right',
                       textvariable=self.all_strats[strategy_type][strategy]).\
                     grid(row=self.curr_row, column=1)
                 self.curr_row += 1
 
     def init_params(self):
         self.param = {
             'Rounds': IntVar(),
-            'Generations': IntVar()
+            'Generations': IntVar(), 
+            'Noise': DoubleVar()
         }
         self.param['Rounds'].set(10)
         self.param['Generations'].set(35)
+        self.param['Noise'].set(0.1)
 
-        Label(self.setting_frame, text="Simulation settings",
+        Label(self.setting_frame_mainsub, text="Simulation settings",
               font=fonts['sub_header'], height=2, width=15, anchor=S).\
             grid(row=self.curr_row, column=0)
         self.curr_row += 1
 
         for param in self.param:
-            Label(self.setting_frame, text=param + " -", width=12,
+            Label(self.setting_frame_mainsub, text=param + " -", width=12,
                   anchor=E).grid(row=self.curr_row, column=0)
-            Entry(self.setting_frame, width=entry_width, justify='right',
+            Entry(self.setting_frame_mainsub, width=entry_width, justify='right',
                   textvariable=self.param[param]).\
                 grid(row=self.curr_row, column=1)
             self.curr_row += 1
 
-        self.clear_button = Button(self.setting_frame, text='Clear',
-                                   font=fonts['sub_button'], height=2,
-                                   command=self.reset)
-        self.clear_button.grid(row=0, column=1)
-        self.execute_button = Button(self.setting_frame, text='Execute',
-                                     font=fonts['main_button'], height=2,
-                                     command=self.confirm, bg='blue')
-        self.execute_button.grid(row=self.curr_row, column=1)
-        self.curr_row += 1
-
     def init_presets(self):
         diverse = {
             # just make a function that changes all values to n.
         }
         defectors_among_kantians = {
             'Defector': 3,
             'Kantian': 97
@@ -115,50 +134,55 @@
             'Tit for Tat': 3,
             'Defector': 97
         }
         all_presets = {
             'Defectors among Kantians': [defectors_among_kantians, None],
             'TFT among Defectors': [tft_among_defectors, None]
         }
-        Label(self.setting_frame, text="~ Presets ~",
-              font=fonts['sub_header'], pady=10, width=20).\
+        self.presets_frame = Frame(self.setting_frame_mainsub)
+        Label(self.presets_frame, text="Presets",
+              font=fonts['sub_header']).\
             grid(row=self.curr_row, column=0)
         self.curr_row += 1
 
         for preset in all_presets:
-            all_presets[preset][1] = Button(self.setting_frame, text='select',
+            all_presets[preset][1] = Button(self.presets_frame, text='select',
                                             font=fonts['sub_button'],
                                             command=self.select_preset(preset))
             all_presets[preset][1].grid(row=self.curr_row, column=0)
-            Label(self.setting_frame, text=preset).\
+            Label(self.presets_frame, text=preset).\
                 grid(row=self.curr_row, column=1)
             self.curr_row += 1
+        self.presets_frame.grid()
 
     def init_graph(self):
         self.fig = Figure(figsize=(8, 5.25), dpi=100)
         self.canvas = FigureCanvasTkAgg(self.fig, self.graph_frame)
         self.plot_filler()
         self.canvas.get_tk_widget().pack(side=TOP, fill=BOTH, expand=True)
         toolbar = NavigationToolbar2Tk(self.canvas, self.graph_frame)
         toolbar.update()
         self.canvas._tkcanvas.pack()
 
     def init_menu(self):
         main_menu = Menu(self.parent)
         file_menu = Menu(main_menu, tearoff=0)
-        file_menu.add_command(label='Execute', accelerator='Cmd+E', command=self.execute_plot)
+        file_menu.add_command(
+            label='Execute', accelerator='Cmd+E', command=self.execute_plot)
         main_menu.add_cascade(label='File', menu=file_menu)
         self.parent.config(menu=main_menu)
 
     def init_decor(self):
         self.header.config(bg=bg['decor1'])
         self.footer.config(bg=bg['decor1'])
-        top_canvas = Canvas(self.header, bg=bg['decor1'], height=25, width=1100)
+        top_canvas = Canvas(
+            self.header, bg=bg['decor1'], height=25, width=1094)
         top_canvas.grid(row=0, column=0)
-        bot_canvas = Canvas(self.footer, bg=bg['decor1'], height=25, width=1100)
+        bot_canvas = Canvas(
+            self.footer, bg=bg['decor1'], height=25, width=1094)
         bot_canvas.grid(row=0, column=0)
 
     def set_graph_params(self):
         self.f.set_title("Population distibution with respect to time")
         self.f.set_xlabel("Generation")
         self.f.set_ylabel("Population density [%]")
         self.f.set_xbound(lower=0, upper=self.param['Generations'].get())
@@ -168,18 +192,22 @@
         self.fig.clear()
         self.f = self.fig.add_subplot(111)
         self.f.plot()
         self.set_graph_params()
         self.canvas.draw()
 
     def reset(self):
-        self.plot_filler()
-        for strat_list in self.all_strats:
-            for strat in self.all_strats[strat_list]:
-                self.all_strats[strat_list][strat].set(0)
+        response = messagebox.askquestion("Confirmation",
+                                          "Are you sure you would like to "
+                                          "reset simulation variables?")
+        if response == 'yes':
+            self.plot_filler()
+            for strat_list in self.all_strats:
+                for strat in self.all_strats[strat_list]:
+                    self.all_strats[strat_list][strat].set(0)
 
     def compile_profile(self):
         profile = {}
         for strategy_type in self.all_strats:
             for strategy in self.all_strats[strategy_type]:
                 try:
                     var = self.all_strats[strategy_type][strategy].get()
@@ -198,15 +226,16 @@
         if response == 'yes':
 
             self.execute_plot()
 
     def execute_plot(self):
         result = run_simulation(self.compile_profile(),
                                 self.param['Generations'].get(),
-                                self.param['Rounds'].get())
+                                self.param['Rounds'].get(), 
+                                self.param["Noise"].get())
         self.fig.clear()
         x_axis = result.pop('gens')
         self.f = self.fig.add_subplot(111)
         for strat in result:
             self.f.plot(x_axis, result[strat], label=strat)
         self.set_graph_params()
         self.f.legend()
@@ -218,15 +247,15 @@
     def select_preset(self, preset):
         pass
 
 
 def run_gui():
     root = Tk()
     root.title("IPD Simulation")
-    root.geometry("1107x631")
+    root.geometry("1100x631")
     root.resizable(False, False)
     ipd = SimulationGUI(root)
     root.mainloop()
 
 
 fonts = {
     'header': 'Calibri 19 bold',
```

### Comparing `ipd_axelrod-1.0.0/src/IPD/main.py` & `ipd_axelrod-1.1.0/src/IPD/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from .play import *
 
 NUM_GENS = 35
 NUM_ROUNDS = 100
 INITIAL_PROFILE = defectors_with_some_tft()
 
 
-def run_simulation(init_profile: dict, num_gens, num_rounds):
+def run_simulation(init_profile: dict, num_gens, num_rounds, noise):
     dist = {
         'gens': np.linspace(1, num_gens, num_gens)
     }
-    init_gen = populate(init_profile)
+    init_gen = populate(init_profile, noise)
     init_dist = init_gen.distribution()
     # print(init_dist)
     for strat in init_profile:
         dist[strat] = np.zeros(num_gens)
         dist[strat][0] = init_dist[strat]
     curr_gen = init_gen
     for gen in range(num_gens):
@@ -39,15 +39,15 @@
     plt.title('Changes to population distribution with respect to time')
     plt.xlabel('Generation')
     plt.ylabel('Population Distribution [%]')
     plt.legend()
     plt.show()
 
 
-def populate(input_dict):
+def populate(input_dict, noise=0):
     """ Example --
     >>> sample_dict = {
             'Kantian': 2,
             'Defector': 1
         }
     >>> sample_population = populate(sample_dict)
 
@@ -59,15 +59,15 @@
     profile = []
     for strategy in input_dict:
         if strategy not in all_strategies:
             raise Exception('Specified strategy does not exist.')
         else:
             for i in range(input_dict[strategy]):
                 profile.append(deepcopy(all_strategies[strategy]))
-    return Population(profile)
+    return Population(profile, noise)
 
 
 def update_gen_dist(curr_gen, num_rounds):
     round_robin(curr_gen, num_rounds)
     new_gen = curr_gen.create_next_gen()
     new_dist = new_gen.distribution()
     return new_gen, new_dist
```

### Comparing `ipd_axelrod-1.0.0/src/IPD/profiles.py` & `ipd_axelrod-1.1.0/src/IPD/profiles.py`

 * *Files identical despite different names*

### Comparing `ipd_axelrod-1.0.0/src/IPD/strategies.py` & `ipd_axelrod-1.1.0/src/IPD/strategies.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .data import Player, randint
+from .data import Player
+
 
 class Kantian(Player):
     """ Always cooperates. """
     def __init__(self, score=0):
         super().__init__()
         self.name = "Kantian"
 
@@ -17,93 +18,59 @@
     def action(self, opponent):
         return False
 
 
 class TitForTat(Player):
     """Starts by cooperating. After that, always cooperates unless
     opponent's last move was defect."""
-
-    def __init__(self, score=0):
-        super().__init__()
-        self.name = "Tit for Tat"
+    first = True
+    name = "Tit for Tat"
 
     def action(self, opponent):
-        # If there is no history, the first term evaluates to True. Therefore, python short-circuits and does not touch [-1], which would produce an error.
-        return not opponent.history or opponent.history[-1]
+        return opponent.history[-1]
 
 
 class TitFor2Tats(Player):
     """Starts by cooperating. After that, always cooperates unless
     opponent's last two moves were defect."""
-
-    def __init__(self, score=0):
-        super().__init__()
-        self.name = "Tit for 2 Tats"
-        self.opponent_last_actions = (True, True)
+    first = True
+    name = "Tit for 2 Tats"
 
     def action(self, opponent):
-        if not opponent.history:
-            self.opponent_last_actions = (self.opponent_last_actions[1], True)
-        else:
-            self.opponent_last_actions =\
-                (self.opponent_last_actions[1], opponent.history[-1])
-        return self.opponent_last_actions[0] or self.opponent_last_actions[1]
-
-    def init_match(self):
-        self.opponent_last_actions = (True, True)
+        return not (opponent.history[-3:-1] == [False, False])
 
 
 class MeanTitForTat(TitForTat):
     """ Tit for Tat, but occasionally defects. """
-
-    def __init__(self, score=0):
-        super().__init__()
-        self.name = "Mean Tit for Tat"
+    name = "Mean Tit for Tat"
 
     def action(self, opponent):
-        if not randint(0, 5):
-            return False
-        else:
-            return super().action(opponent)
+        return self.random(4/5) and super().action(opponent)
 
 
 class WaryTitForTat(TitForTat):
     """ Tit for Tat, but starts by defecting. """
-
-    def __init__(self, score=0):
-        super().__init__()
-        self.name = "Wary Tit for Tat"
-
-    def action(self, opponent):
-        if not opponent.history:
-            return False
-        else:
-            return super().action(opponent)
+    name = "Wary Tit for Tat"
+    first = False
 
 
 class Tester(TitForTat):
     """ Tit for 2 Tats exploiter. Tit for Tat, but occasionally defects
     then cooperates for a turn. If the opponent doesn't retaliate immediately,
     alternates between cooperating and defecting. """
-
-    def __init__(self, score=0):
-        super().__init__()
-        self.name = "Tester"
-        self.turn = 0
-        self.testing_turn = 0
-        self.opponent_retaliated = False
+    name = "Tester"
 
     def action(self, opponent):
         self.turn += 1
-        if self.testing_turn == 0 and not randint(0, 5):
+        if self.testing_turn == 0 and self.random(1/5):
             self.testing_turn += 1
             return False
         elif 0 < self.testing_turn <= 1:
             self.testing_turn += 1
-            if not opponent.history[-1]:
+            if opponent.history and not opponent.history[-1]:
                 self.opponent_retaliated = True
             return True
         elif self.testing_turn > 1 and not self.opponent_retaliated:
             return self.turn % 2
         else:
             return super().action(opponent)
 
@@ -113,50 +80,41 @@
         self.opponent_retaliated = False
 
 
 class Conniver(TitForTat):
     """ Kantian exploiter. Tit for Tat, but occasionally defects then cooperates
     for 2 turns. If opponent doesn't retaliate within 2 turns, defects until end. """
 
-    def __init__(self, score=0):
-        super().__init__()
-        self.name = "Conniver"
-        self.testing_turn = 0
-        self.opponent_retaliated = False
+    name = "Conniver"
 
     def action(self, opponent):
-        if self.testing_turn == 0 and not randint(0, 5):
+        if self.testing_turn == 0 and self.random(1/5):
             self.testing_turn += 1
             return False
         elif 0 < self.testing_turn <= 2:
             self.testing_turn += 1
-            if not opponent.history[-1]:
+            if opponent.history and not opponent.history[-1]:
                 self.opponent_retaliated = True
             return True
         elif self.testing_turn > 2 and not self.opponent_retaliated:
             return False
         else:
             return super().action(opponent)
 
     def init_match(self):
         self.testing_turn = 0
         self.opponent_retaliated = False
 
 
 class Grudger(Player):
     """ Cooperates until opponent defects. """
-
-    def __init__(self, score=0):
-        super().__init__()
-        self.name = "Grudger"
-        self.opponent_never_defected = True
+    first = True
+    name = "Grudger"
 
     def action(self, opponent):
-        if not opponent.history:
-            return True
         if not opponent.history[-1]:
             self.opponent_never_defected = False
         return self.opponent_never_defected
 
     def init_match(self):
         self.opponent_never_defected = True
 
@@ -198,29 +156,43 @@
     def __init__(self, score=0):
         super().__init__()
         self.name = "Clan Leader"
 
 
 class Random(Player):
     """ Cooperates or defects at 50/50. """
+
     def __init__(self, score=0):
         super().__init__()
         self.name = "Random"
 
     def action(self, opponent):
-        return randint(0, 1)
+        return self.random(1/2)
+
+
+class Grofman(Player):
+    """Cooperates on the first turn. Then"""
+
+    def __init__(self, score=0):
+        super().__init__()
+        self.name = "Grofman"
+
+    def action(self, opponent):
+        return len(self.history) == 0 or self.history[-1] == opponent.history[-1] or self.random(2 / 7)
+
 
 all_strategies = {
     'Kantian': Kantian(),
     'Defector': Defector(),
     'Tit for Tat': TitForTat(),
     'Tit for 2 Tats': TitFor2Tats(),
     'Mean Tit for Tat': MeanTitForTat(),
     'Wary Tit for Tat': WaryTitForTat(),
     'Tester': Tester(),
     'Conniver': Conniver(),
     'Grudger': Grudger(),
     'Pavlovian': Pavlovian(),
     'Clan Grunt': ClanGrunt(),
     'Clan Leader': ClanLeader(),
-    'Random': Random()
+    'Random': Random(),
+    'Grofman': Grofman()
 }
```

### Comparing `ipd_axelrod-1.0.0/src/IPD_axelrod.egg-info/PKG-INFO` & `ipd_axelrod-1.1.0/src/IPD_axelrod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPD-axelrod
-Version: 1.0.0
+Version: 1.1.0
 Summary: A tool for the iterated prisoners dilemma
 Author: jumpingtj
 Project-URL: Homepage, https://github.com/jumpingtj/prisoners-dilemma
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

