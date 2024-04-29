# Comparing `tmp/pyBrainGenixClient-2024.2.9.1.tar.gz` & `tmp/pybraingenixclient-2024.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBrainGenixClient-2024.2.9.1.tar", last modified: Fri Feb  9 19:59:52 2024, max compression
+gzip compressed data, was "pybraingenixclient-2024.4.29.tar", last modified: Mon Apr 29 17:10:02 2024, max compression
```

## Comparing `pyBrainGenixClient-2024.2.9.1.tar` & `pybraingenixclient-2024.4.29.tar`

### file list

```diff
@@ -1,106 +1,125 @@
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.778827 pyBrainGenixClient-2024.2.9.1/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.766826 pyBrainGenixClient-2024.2.9.1/BrainGenix/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.766826 pyBrainGenixClient-2024.2.9.1/BrainGenix/LibUtils/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     1804 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/LibUtils/ConfigCheck.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      232 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/LibUtils/GetID.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.766826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.766826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.766826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Authentication/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       48 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Authentication/Password.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       42 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Authentication/Token.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       55 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Authentication/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     4264 2024-02-09 19:59:37.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Client.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      380 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Configuration.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.766826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Modes/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       42 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Modes/Local.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       44 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Modes/Remote.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       51 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/Modes/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     3651 2024-02-09 19:59:37.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/RequestHandler.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      117 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.766826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Compartments/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Compartments/BS/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     2657 2024-02-07 03:16:18.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Compartments/BS/BS.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      410 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Compartments/BS/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       72 2024-02-07 03:13:44.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Compartments/BS/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       16 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Compartments/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Receptor/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      407 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Receptor/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     3178 2024-02-06 22:21:43.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Receptor/Receptor.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       84 2024-02-06 22:29:21.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Receptor/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Staple/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      228 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Staple/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     2218 2024-02-06 22:35:47.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Staple/Staple.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       80 2024-02-06 22:05:15.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Staple/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       43 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Neurons/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Neurons/BS/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     3538 2024-02-08 19:08:31.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Neurons/BS/BSNeuron.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      608 2024-02-08 19:08:31.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Neurons/BS/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       85 2024-02-06 22:29:16.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Neurons/BS/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       17 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Neurons/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       74 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Box/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     2814 2024-02-06 22:16:33.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Box/Box.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      267 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Box/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       74 2024-02-06 22:07:21.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Box/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.770826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Cylinder/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      317 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Cylinder/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     2774 2024-02-06 22:16:41.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Cylinder/Cylinder.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       84 2024-02-06 21:27:37.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Cylinder/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Sphere/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      218 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Sphere/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     2128 2024-02-06 22:16:37.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Sphere/Sphere.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       80 2024-02-06 21:27:43.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Sphere/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       61 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Simulation/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      143 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Simulation/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     5389 2024-02-09 19:59:37.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Simulation/Simulation.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       76 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Simulation/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampADC/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      227 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampADC/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     3219 2024-02-06 22:56:57.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampADC/PatchClampADC.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       94 2024-02-06 22:41:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampADC/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampDAC/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      232 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampDAC/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     2871 2024-02-06 22:51:50.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampDAC/PatchClampDAC.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       94 2024-02-06 22:36:44.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampDAC/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       55 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/Calcium/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     9323 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/Calcium/Calcium.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      518 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/Calcium/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       69 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/Calcium/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/EM/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      426 2024-02-08 20:10:41.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/EM/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)    10276 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/EM/EM.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       59 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/EM/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       39 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Visualizer/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      332 2024-02-08 20:15:59.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Visualizer/Configuration.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     4731 2024-02-09 00:35:29.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Visualizer/Visualizer.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       75 2024-02-07 20:51:18.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Visualizer/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      132 2024-02-07 20:47:27.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.774826 pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/StackStitcher/
--rwxrwxr-x   0 eliott    (1000) eliott    (1000)    10572 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/StackStitcher/StackStitcher.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       40 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/StackStitcher/__init__.py
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.778827 pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/Test/
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     2553 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/Test/Test.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       22 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/Test/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       51 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       37 2024-02-05 20:38:12.000000 pyBrainGenixClient-2024.2.9.1/BrainGenix/__init__.py
--rw-rw-r--   0 eliott    (1000) eliott    (1000)    34260 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/LICENSE.md
--rw-r--r--   0 eliott    (1000) eliott    (1000)      968 2024-02-09 19:59:52.778827 pyBrainGenixClient-2024.2.9.1/PKG-INFO
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      169 2024-01-08 21:14:13.000000 pyBrainGenixClient-2024.2.9.1/README.md
-drwxrwxr-x   0 eliott    (1000) eliott    (1000)        0 2024-02-09 19:59:52.778827 pyBrainGenixClient-2024.2.9.1/pyBrainGenixClient.egg-info/
--rw-r--r--   0 eliott    (1000) eliott    (1000)      968 2024-02-09 19:59:52.000000 pyBrainGenixClient-2024.2.9.1/pyBrainGenixClient.egg-info/PKG-INFO
--rw-rw-r--   0 eliott    (1000) eliott    (1000)     2981 2024-02-09 19:59:52.000000 pyBrainGenixClient-2024.2.9.1/pyBrainGenixClient.egg-info/SOURCES.txt
--rw-rw-r--   0 eliott    (1000) eliott    (1000)        1 2024-02-09 19:59:52.000000 pyBrainGenixClient-2024.2.9.1/pyBrainGenixClient.egg-info/dependency_links.txt
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       53 2024-02-09 19:59:52.000000 pyBrainGenixClient-2024.2.9.1/pyBrainGenixClient.egg-info/requires.txt
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       11 2024-02-09 19:59:52.000000 pyBrainGenixClient-2024.2.9.1/pyBrainGenixClient.egg-info/top_level.txt
--rw-rw-r--   0 eliott    (1000) eliott    (1000)      927 2024-02-09 19:59:44.000000 pyBrainGenixClient-2024.2.9.1/pyproject.toml
--rw-rw-r--   0 eliott    (1000) eliott    (1000)       38 2024-02-09 19:59:52.778827 pyBrainGenixClient-2024.2.9.1/setup.cfg
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.486566 pybraingenixclient-2024.4.29/BrainGenix/
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    38960 2024-04-28 19:18:38.000000 pybraingenixclient-2024.4.29/BrainGenix/BG_API.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.486566 pybraingenixclient-2024.4.29/BrainGenix/EVM/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.486566 pybraingenixclient-2024.4.29/BrainGenix/EVM/Debug/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      266 2024-04-11 00:00:32.000000 pybraingenixclient-2024.4.29/BrainGenix/EVM/Debug/DoubleEcho.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      254 2024-04-10 23:41:00.000000 pybraingenixclient-2024.4.29/BrainGenix/EVM/Debug/Echo.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       58 2024-04-11 00:00:42.000000 pybraingenixclient-2024.4.29/BrainGenix/EVM/Debug/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       19 2024-04-10 23:36:42.000000 pybraingenixclient-2024.4.29/BrainGenix/EVM/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.486566 pybraingenixclient-2024.4.29/BrainGenix/LibUtils/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1804 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/LibUtils/ConfigCheck.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      232 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/LibUtils/GetID.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.486566 pybraingenixclient-2024.4.29/BrainGenix/NES/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.486566 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.486566 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Authentication/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       48 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Authentication/Password.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       42 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Authentication/Token.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       55 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Authentication/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8430 2024-04-15 21:07:19.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Client.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      380 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Configuration.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Modes/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       42 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Modes/Local.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       44 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Modes/Remote.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       51 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/Modes/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3688 2024-04-15 21:06:55.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/RequestHandler.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      117 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Client/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/BS/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2707 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/BS/BS.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      410 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/BS/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       73 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/BS/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/SC/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      410 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/SC/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2707 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/SC/SC.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       73 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/SC/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       34 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Receptor/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      493 2024-04-28 19:13:26.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Receptor/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3427 2024-04-28 19:13:26.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Receptor/Receptor.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       84 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Receptor/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Staple/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      228 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Staple/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2242 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Staple/Staple.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Staple/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       43 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.490566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/BS/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3564 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/BS/BSNeuron.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      608 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/BS/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       85 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/BS/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/SC/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      661 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/SC/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3598 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/SC/SCNeuron.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       85 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/SC/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       33 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       74 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Models/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Box/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2856 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Box/Box.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      267 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Box/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       74 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Box/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Cylinder/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      317 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Cylinder/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2816 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Cylinder/Cylinder.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       84 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Cylinder/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Sphere/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      218 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Sphere/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2170 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Sphere/Sphere.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Sphere/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       61 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Simulation/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      168 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Simulation/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7304 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Simulation/Simulation.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       76 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Simulation/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampADC/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      227 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampADC/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3267 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampADC/PatchClampADC.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       94 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampADC/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampDAC/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      232 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampDAC/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2907 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampDAC/PatchClampDAC.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       94 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampDAC/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       55 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.494566 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/Calcium/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    11215 2024-04-11 02:40:05.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/Calcium/Calcium.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      744 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/Calcium/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       69 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/Calcium/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/EM/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      426 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/EM/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    13385 2024-04-15 21:08:12.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/EM/EM.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/EM/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       39 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/BrainGenix/NES/Visualizer/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      332 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Visualizer/Configuration.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     4789 2024-04-11 02:40:11.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Visualizer/Visualizer.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       75 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/Visualizer/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      167 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/NES/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/BrainGenix/Tools/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/BrainGenix/Tools/NeuroglancerConverter/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3728 2024-04-13 05:42:45.000000 pybraingenixclient-2024.4.29/BrainGenix/Tools/NeuroglancerConverter/NeuroglancerConverter.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       56 2024-04-13 02:47:28.000000 pybraingenixclient-2024.4.29/BrainGenix/Tools/NeuroglancerConverter/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/BrainGenix/Tools/StackStitcher/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    14378 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/Tools/StackStitcher/CaImagingStackStitcher.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    13141 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/Tools/StackStitcher/StackStitcher.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/Tools/StackStitcher/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/BrainGenix/Tools/Test/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2580 2024-04-11 02:41:57.000000 pybraingenixclient-2024.4.29/BrainGenix/Tools/Test/Test.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       22 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/Tools/Test/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       51 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/Tools/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       71 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/BrainGenix/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    34260 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/LICENSE.md
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1011 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      169 2024-04-10 23:35:49.000000 pybraingenixclient-2024.4.29/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/pyBrainGenixClient.egg-info/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1011 2024-04-29 17:10:02.000000 pybraingenixclient-2024.4.29/pyBrainGenixClient.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3587 2024-04-29 17:10:02.000000 pybraingenixclient-2024.4.29/pyBrainGenixClient.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-29 17:10:02.000000 pybraingenixclient-2024.4.29/pyBrainGenixClient.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       67 2024-04-29 17:10:02.000000 pybraingenixclient-2024.4.29/pyBrainGenixClient.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       11 2024-04-29 17:10:02.000000 pybraingenixclient-2024.4.29/pyBrainGenixClient.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      948 2024-04-29 17:09:47.000000 pybraingenixclient-2024.4.29/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2024-04-29 17:10:02.498566 pybraingenixclient-2024.4.29/setup.cfg
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/LibUtils/ConfigCheck.py` & `pybraingenixclient-2024.4.29/BrainGenix/LibUtils/ConfigCheck.py`

 * *Files identical despite different names*

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Client/RequestHandler.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Client/RequestHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import requests
 import time
 import requests_futures.sessions
 import json
 
 class RequestHandler:
 
-    def __init__(self, _URIBase:str, _Token:str):
+    def __init__(self, _URIBase:str, _Token:str, _Host:str):
         self.URIBase = _URIBase
         self.Token = _Token
+        self.Host = _Host
         self.RequestID:int = 0
         self.FuturesSession = requests_futures.sessions.FuturesSession()
 
         # Check that API is up
         try:
             Response = requests.get(f"{self.URIBase}/Hello")
         except:
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Compartments/BS/BS.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Compartments/BS/BS.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         # Run Configuration Check
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create On Server
         ShapeID = BrainGenix.LibUtils.GetID.GetID(_Configuration.Shape)
         QueryList:list = []
         QueryList.append({
-            "BSCreate": {
+            "Simulation/Compartments/BS/Create": {
                 "ShapeID": ShapeID,
                 "MembranePotential_mV": _Configuration.MembranePotential_mV,
                 "SpikeThreshold_mV": _Configuration.SpikeThreshold_mV,
                 "DecayTime_ms": _Configuration.DecayTime_ms,
                 "RestingPotential_mV": _Configuration.RestingPotential_mV,
                 "AfterHyperpolarizationAmplitude_mV": _Configuration.AfterHyperpolarizationAmplitude_mV,
                 "Name": _Configuration.Name,
@@ -48,15 +48,15 @@
 
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         ShapeID = BrainGenix.LibUtils.GetID.GetID(_Configuration.Shape)
         QueryList.append({
-            "BSCreate": {
+            "Simulation/Compartments/BS/Create": {
                 "ShapeID": ShapeID,
                 "MembranePotential_mV": _Configuration.MembranePotential_mV,
                 "SpikeThreshold_mV": _Configuration.SpikeThreshold_mV,
                 "DecayTime_ms": _Configuration.DecayTime_ms,
                 "RestingPotential_mV": _Configuration.RestingPotential_mV,
                 "AfterHyperpolarizationAmplitude_mV": _Configuration.AfterHyperpolarizationAmplitude_mV,
                 "Name": _Configuration.Name,
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Receptor/Receptor.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Receptor/Receptor.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 
         # Run Configuration Check
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create Box On Server
         SourceCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.SourceCompartment)
         DestinationCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.DestinationCompartment)
-        ReceptorLocation = json.dumps(_Configuration.ReceptorLocation_um)
+        # ReceptorLocation = json.dumps(_Configuration.ReceptorLocation_um)
         QueryList:list = []
         QueryList.append({
-            "ReceptorCreate": {
+            "Simulation/Receptor/Create": {
                 "SourceCompartmentID": SourceCompartmentID,
                 "DestinationCompartmentID": DestinationCompartmentID,
-                "ReceptorPosX_um": _Configuration.ReceptorLocation_um[0],
-                "ReceptorPosY_um": _Configuration.ReceptorLocation_um[1],
-                "ReceptorPosZ_um": _Configuration.ReceptorLocation_um[2],
+                "ReceptorMorphology": _Configuration.ReceptorMorphology,
+                # "ReceptorPosX_um": _Configuration.ReceptorLocation_um[0],
+                # "ReceptorPosY_um": _Configuration.ReceptorLocation_um[1],
+                # "ReceptorPosZ_um": _Configuration.ReceptorLocation_um[2],
+                "Neurotransmitter": _Configuration.Neurotransmitter,
                 "Conductance_nS": _Configuration.Conductance_nS,
                 "TimeConstantRise_ms": _Configuration.TimeConstantRise_ms,
                 "TimeConstantDecay_ms": _Configuration.TimeConstantDecay_ms,
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
         })
@@ -48,20 +50,21 @@
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         SourceCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.SourceCompartment)
         DestinationCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.DestinationCompartment)
         QueryList.append({
-            "ReceptorCreate": {
+            "Simulation/Receptor/Create": {
                 "SourceCompartmentID": SourceCompartmentID,
                 "DestinationCompartmentID": DestinationCompartmentID,
-                "ReceptorPosX_um": _Configuration.ReceptorLocation_um[0],
-                "ReceptorPosY_um": _Configuration.ReceptorLocation_um[1],
-                "ReceptorPosZ_um": _Configuration.ReceptorLocation_um[2],
+                # "ReceptorPosX_um": _Configuration.ReceptorLocation_um[0],
+                # "ReceptorPosY_um": _Configuration.ReceptorLocation_um[1],
+                # "ReceptorPosZ_um": _Configuration.ReceptorLocation_um[2],
+                "Neurotransmitter": _Configuration.Neurotransmitter,
                 "Conductance_nS": _Configuration.Conductance_nS,
                 "TimeConstantRise_ms": _Configuration.TimeConstantRise_ms,
                 "TimeConstantDecay_ms": _Configuration.TimeConstantDecay_ms,
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
         })
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Connections/Staple/Staple.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Connections/Staple/Staple.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create Staple On Server
         SourceCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.SourceCompartment)
         DestinationCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.DestinationCompartment)
         QueryList:list = []
         QueryList.append({
-            "StapleCreate": {
+            "Simulation/Staple/Create": {
                 "SourceCompartmentID": SourceCompartmentID,
                 "DestinationCompartmentID": DestinationCompartmentID,
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
         })
         Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
@@ -41,15 +41,15 @@
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         SourceCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.SourceCompartment)
         DestinationCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.DestinationCompartment)
         QueryList.append({
-            "StapleCreate": {
+            "Simulation/Staple/Create": {
                 "SourceCompartmentID": SourceCompartmentID,
                 "DestinationCompartmentID": DestinationCompartmentID,
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
         })
     Response = _RequestHandler.BuildPostQuery(QueryList, "/NES")
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Neurons/BS/BSNeuron.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/BS/BSNeuron.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create BSNeuron On Server
         self.SomaID = BrainGenix.LibUtils.GetID.GetID(_Configuration.Soma)
         self.AxonID = BrainGenix.LibUtils.GetID.GetID(_Configuration.Axon)
         QueryList:list = []
         QueryList.append({
-            "BSNeuronCreate": {
+            "Simulation/Neuron/BS/Create": {
                 "AxonID": self.AxonID,
                 "SomaID": self.SomaID,
                 "MembranePotential_mV": _Configuration.MembranePotential_mV,
                 "RestingPotential_mV": _Configuration.RestingPotential_mV,
                 "SpikeThreshold_mV": _Configuration.SpikeThreshold_mV,
                 "DecayTime_ms": _Configuration.DecayTime_ms,
                 "AfterHyperpolarizationAmplitude_mV": _Configuration.AfterHyperpolarizationAmplitude_mV,
@@ -48,15 +48,15 @@
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         SomaID = BrainGenix.LibUtils.GetID.GetID(_Configuration.Soma)
         AxonID = BrainGenix.LibUtils.GetID.GetID(_Configuration.Axon)
         QueryList.append({
-            "BSNeuronCreate": {
+            "Simulation/Neuron/BS/Create": {
                 "AxonID": AxonID,
                 "SomaID": SomaID,
                 "MembranePotential_mV": _Configuration.MembranePotential_mV,
                 "RestingPotential_mV": _Configuration.RestingPotential_mV,
                 "SpikeThreshold_mV": _Configuration.SpikeThreshold_mV,
                 "DecayTime_ms": _Configuration.DecayTime_ms,
                 "AfterHyperpolarizationAmplitude_mV": _Configuration.AfterHyperpolarizationAmplitude_mV,
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Models/Neurons/BS/Configuration.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Models/Neurons/BS/Configuration.py`

 * *Files identical despite different names*

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Box/Box.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Box/Box.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         # Run Configuration Check
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create Box On Server
         QueryList:list = []
         QueryList.append({
-                "BoxCreate": {
+                "Simulation/Geometry/Box/Create": {
                 "CenterPosX_um": _Configuration.CenterPosition_um[0],
                 "CenterPosY_um": _Configuration.CenterPosition_um[1],
                 "CenterPosZ_um": _Configuration.CenterPosition_um[2],
                 "ScaleX_um": _Configuration.Dimensions_um[0],
                 "ScaleY_um": _Configuration.Dimensions_um[1],
                 "ScaleZ_um": _Configuration.Dimensions_um[2],
                 "RotationX_rad": _Configuration.Rotation_rad[0],
@@ -49,15 +49,15 @@
 
 
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         QueryList.append({
-                "BoxCreate": {
+                "Simulation/Geometry/Box/Create": {
                 "CenterPosX_um": _Configuration.CenterPosition_um[0],
                 "CenterPosY_um": _Configuration.CenterPosition_um[1],
                 "CenterPosZ_um": _Configuration.CenterPosition_um[2],
                 "ScaleX_um": _Configuration.Dimensions_um[0],
                 "ScaleY_um": _Configuration.Dimensions_um[1],
                 "ScaleZ_um": _Configuration.Dimensions_um[2],
                 "RotationX_rad": _Configuration.Rotation_rad[0],
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Cylinder/Cylinder.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Cylinder/Cylinder.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         # Run Configuration Check
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create Cylinder On Server
         QueryList:list = []
         QueryList.append({
-                "CylinderCreate": {
+                "Simulation/Geometry/Cylinder/Create": {
                 "Point1Radius_um": _Configuration.Point1Radius_um,
                 "Point1PosX_um": _Configuration.Point1Position_um[0],
                 "Point1PosY_um": _Configuration.Point1Position_um[1],
                 "Point1PosZ_um": _Configuration.Point1Position_um[2],
                 "Point2Radius_um": _Configuration.Point2Radius_um,
                 "Point2PosX_um": _Configuration.Point2Position_um[0],
                 "Point2PosY_um": _Configuration.Point2Position_um[1],
@@ -49,15 +49,15 @@
 
 
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         QueryList.append({
-                "CylinderCreate": {
+                "Simulation/Geometry/Cylinder/Create": {
                 "Point1Radius_um": _Configuration.Point1Radius_um,
                 "Point1PosX_um": _Configuration.Point1Position_um[0],
                 "Point1PosY_um": _Configuration.Point1Position_um[1],
                 "Point1PosZ_um": _Configuration.Point1Position_um[2],
                 "Point2Radius_um": _Configuration.Point2Radius_um,
                 "Point2PosX_um": _Configuration.Point2Position_um[0],
                 "Point2PosY_um": _Configuration.Point2Position_um[1],
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Shapes/Sphere/Sphere.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Shapes/Sphere/Sphere.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         # Run Configuration Check
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create Sphere On Server
         QueryList:list = []
         QueryList.append({
-                "SphereCreate": {
+                "Simulation/Geometry/Sphere/Create": {
                 "Radius_um": _Configuration.Radius_um,
                 "CenterPosX_um": _Configuration.Center_um[0],
                 "CenterPosY_um": _Configuration.Center_um[1],
                 "CenterPosZ_um": _Configuration.Center_um[2],
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
@@ -43,15 +43,15 @@
 
 
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         QueryList.append({
-                "SphereCreate": {
+                "Simulation/Geometry/Sphere/Create": {
                 "Radius_um": _Configuration.Radius_um,
                 "CenterPosX_um": _Configuration.Center_um[0],
                 "CenterPosY_um": _Configuration.Center_um[1],
                 "CenterPosZ_um": _Configuration.Center_um[2],
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Simulation/Simulation.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Simulation/Simulation.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,46 +7,67 @@
 from BrainGenix.NES.Client import RequestHandler
 
 from BrainGenix.NES.Shapes import Sphere
 from BrainGenix.NES.Shapes import Box
 from BrainGenix.NES.Shapes import Cylinder
 
 from BrainGenix.NES.VSDA import EM
+from BrainGenix.NES.VSDA import Calcium
 from BrainGenix.NES.Models.Connections import Staple, Receptor
 from BrainGenix.NES.Visualizer import Visualizer
 from BrainGenix.NES import Tools
 
 import BrainGenix.LibUtils.ConfigCheck
 import BrainGenix.LibUtils.GetID
-import json
 import time
 
 import yaspin
 
 
 
 class Simulation():
 
     # create=False is used when this object is needed during loading (see BG_API.py)
-    def __init__(self, _Configuration:Configuration, _RequestHandler:RequestHandler, create=True):
+    def __init__(self, _Configuration:Configuration, _RequestHandler:RequestHandler, _Create:bool=True):
         # Create Attributes
-        self.Name = _Configuration.Name
         self.RequestHandler = _RequestHandler
 
-        if create:
+        if _Create:
+
+            self.Name = _Configuration.Name
+            
+
             # Run Configuration Check
             BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
             # Create Sim On Server
-            Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/Simulation/Create?SimulationName={_Configuration.Name}")
+            QueryList:list = []
+            QueryList.append({
+                "Simulation/Create": {
+                    "Name": _Configuration.Name,
+                }
+            })
+            Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
             assert(Response != None)
             self.ID = Response["SimulationID"]
+
+            # Send Seed
+            QueryList:list = []
+            QueryList.append({
+                "Simulation/SetRandomSeed": {
+                    "SimulationID": self.ID,
+                    "Seed": _Configuration.Seed,
+                }
+            })
+            Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
+            assert(Response != None)
         else:
             self.ID = 0 # Will be replaced after loading, but a valid number is provided for temporary use.
 
+
     ## Methods For Adding Objects
 
      # Tool Init Commands
     def AddPatchClampDAC(self, _PatchClampDACConfig:Tools.PatchClampDAC.Configuration):
         return Tools.PatchClampDAC.PatchClampDAC(_PatchClampDACConfig, self.RequestHandler, self.ID)
 
     def AddPatchClampADC(self, _PatchClampADCConfig:Tools.PatchClampADC.Configuration):
@@ -66,28 +87,44 @@
 
 
 
      # VSDA Init Commands
     def AddVSDAEM(self, _VSDAEMConfig:EM.Configuration):
         return EM.EM(_VSDAEMConfig, self.RequestHandler, self.ID)
 
+    def AddVSDACa(self, _VSDACAConfig:Calcium.Configuration):
+        return Calcium.Calcium(_VSDACAConfig, self.RequestHandler, self.ID)
+
+
 
      # Compartments Add Methods
     def AddBSCompartment(self, _BSCompartmentConfig:Models.Compartments.BS.Configuration):
         return Models.Compartments.BS.BS(_BSCompartmentConfig, self.RequestHandler, self.ID)
 
 
     def AddBSCompartments(self, _BSCompartmentConfigs:list):
         return Models.Compartments.BS.BatchCreate(_BSCompartmentConfigs, self.RequestHandler, self.ID)
 
+     # Compartments Add Methods
+    def AddSCCompartment(self, _SCCompartmentConfig:Models.Compartments.SC.Configuration):
+        return Models.Compartments.SC.SC(_SCCompartmentConfig, self.RequestHandler, self.ID)
+
+
+    def AddSCCompartments(self, _SCCompartmentConfigs:list):
+        return Models.Compartments.SC.BatchCreate(_SCCompartmentConfigs, self.RequestHandler, self.ID)
+
        
     # Neurons Add Methods
     def AddBSNeuron(self, _BSNeuronConfig:Models.Neurons.BS.Configuration):
         return Models.Neurons.BS.BSNeuron(_BSNeuronConfig, self.RequestHandler, self.ID)
 
+    # Neurons Add Methods
+    def AddSCNeuron(self, _SCNeuronConfig:Models.Neurons.SC.Configuration):
+        return Models.Neurons.SC.SCNeuron(_SCNeuronConfig, self.RequestHandler, self.ID)
+
     
      # Geometry Add Methods
     def AddSphere(self, _SphereConfig:Sphere.Configuration):
         return Sphere.Sphere(_SphereConfig, self.RequestHandler, self.ID)
 
     def AddSpheres(self, _SphereConfigs:list):
         return Sphere.BatchCreate(_SphereConfigs, self.RequestHandler, self.ID)
@@ -103,35 +140,67 @@
 
     def AddCylinders(self, _CylinderConfigs:list):
         return Cylinder.BatchCreate(_CylinderConfigs, self.RequestHandler, self.ID)
 
 
     ## Simulation Update Routes
     def Reset(self):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/Simulation/Reset?SimulationID={self.ID}")
+        QueryList:list = []
+        QueryList.append({
+            "Simulation/Reset": {
+                "SimulationID": self.ID
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response
 
     def RunFor(self, _SimulationDuration_ms:float):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/Simulation/RunFor?SimulationID={self.ID}&Runtime_ms={_SimulationDuration_ms}")
+        QueryList:list = []
+        QueryList.append({
+            "Simulation/RunFor": {
+                "SimulationID": self.ID,
+                "Runtime_ms": _SimulationDuration_ms
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response
 
     def RecordAll(self, _MaxRecordTime_ms:float):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/Simulation/RecordAll?SimulationID={self.ID}&MaxRecordTime_ms={_MaxRecordTime_ms}")
+        QueryList:list = []
+        QueryList.append({
+            "Simulation/RecordAll": {
+                "SimulationID": self.ID,
+                "MaxRecordTime_ms": _MaxRecordTime_ms
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response
 
     def GetRecording(self):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/Simulation/GetRecording?SimulationID={self.ID}")
+        QueryList:list = []
+        QueryList.append({
+            "Simulation/GetRecording": {
+                "SimulationID": self.ID,
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response
 
     def GetStatus(self):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/Simulation/GetStatus?SimulationID={self.ID}")
+        QueryList:list = []
+        QueryList.append({
+            "Simulation/GetStatus": {
+                "SimulationID": self.ID,
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response
 
 
     ## Wait Helpers
     def WaitUntilNotBusy(self, _Text:str="Waiting For Simulation Processing To Complete"):
         WaitSpinner = yaspin.yaspin(text=_Text, color="green", timer=True)
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampADC/PatchClampADC.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampADC/PatchClampADC.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         # Run Configuration Check
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create On Server
         SourceCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.SourceCompartment)
         QueryList:list = []
         QueryList.append({
-            "PatchClampADCCreate": {
+            "Simulation/PatchClampDAC/Create": {
                 "SourceCompartmentID": SourceCompartmentID,
                 "ClampPosX_um": _Configuration.ClampLocation_um[0],
                 "ClampPosY_um": _Configuration.ClampLocation_um[1],
                 "ClampPosZ_um": _Configuration.ClampLocation_um[2],
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
@@ -40,28 +40,28 @@
         self.ID = Response["PatchClampADCID"]
 
 
     ## Access Methods
     def SetSampleRate(self, _Timestep_ms:float):
         QueryList:list = []
         QueryList.append({
-            "PatchClampADCSetSampleRate": {
+            "Simulation/PatchClampDAC/SetSampleRate": {
                 "Timestep_ms": _Timestep_ms,
                 "PatchClampADCID": self.ID,
                 "SimulationID": self.SimulationID
             }
         })
         Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response["StatusCode"]
 
     def GetRecordedData(self):
         QueryList:list = []
         QueryList.append({
-            "PatchClampADCGetRecordedData": {
+            "Simulation/PatchClampDAC/GetRecordedData": {
                 "PatchClampADCID": self.ID,
                 "SimulationID": self.SimulationID
             }
         })
         Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response
@@ -70,15 +70,15 @@
 
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         SourceCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.SourceCompartment)
         QueryList.append({
-            "PatchClampADCCreate": {
+            "Simulation/PatchClampDAC/Create": {
                 "SourceCompartmentID": SourceCompartmentID,
                 "ClampPosX_um": _Configuration.ClampLocation_um[0],
                 "ClampPosY_um": _Configuration.ClampLocation_um[1],
                 "ClampPosZ_um": _Configuration.ClampLocation_um[2],
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Tools/PatchClampDAC/PatchClampDAC.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Tools/PatchClampDAC/PatchClampDAC.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         # Run Configuration Check
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create On Server
         DestinationCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.DestinationCompartment)
         QueryList:list = []
         QueryList.append({
-            "PatchClampDACCreate": {
+            "Simulation/PatchClampDAC/Create": {
                 "DestinationCompartmentID": DestinationCompartmentID,
                 "ClampPosX_um": _Configuration.ClampLocation_um[0],
                 "ClampPosY_um": _Configuration.ClampLocation_um[1],
                 "ClampPosZ_um": _Configuration.ClampLocation_um[2],
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
@@ -41,15 +41,15 @@
 
 
 
     ## Access Methods
     def SetOutputList(self, _ControlData:list):
         QueryList:list = []
         QueryList.append({
-            "PatchClampDACSetOutputList": {
+            "Simulation/PatchClampDAC/SetOutputList": {
                 "ControlData": _ControlData,
                 "PatchClampDACID": self.ID,
                 "SimulationID": self.SimulationID
             }
         })
         Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
@@ -59,15 +59,15 @@
 
 def BatchCreate(_Configs:list, _RequestHandler:object, _SimulationID:int):
 
     QueryList:list = []
     for _Configuration in _Configs:
         DestinationCompartmentID = BrainGenix.LibUtils.GetID.GetID(_Configuration.DestinationCompartment)
         QueryList.append({
-            "PatchClampDACCreate": {
+            "Simulation/PatchClampDAC/Create": {
                 "DestinationCompartmentID": DestinationCompartmentID,
                 "ClampPosX_um": _Configuration.ClampLocation_um[0],
                 "ClampPosY_um": _Configuration.ClampLocation_um[1],
                 "ClampPosZ_um": _Configuration.ClampLocation_um[2],
                 "Name": _Configuration.Name,
                 "SimulationID": _SimulationID
             }
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/VSDA/EM/EM.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/VSDA/Calcium/Calcium.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,89 +3,174 @@
 
 import json
 import base64
 import tqdm
 import yaspin
 import os
 import time
+import math
 
 from . import Configuration
 
 from BrainGenix.NES.Client import RequestHandler
 
 import BrainGenix.LibUtils.ConfigCheck
+import BrainGenix.LibUtils.GetID
 
 
 
-class EM:
+
+class Calcium:
 
     def __init__(self, _Configuration:Configuration, _RequestHandler:RequestHandler, _SimulationID:int):
         # Create Attributes
         self.RequestHandler = _RequestHandler
         self.SimulationID = _SimulationID
 
         # Run Configuration Check
         BrainGenix.LibUtils.ConfigCheck.ConfigCheck(_Configuration)
 
         # Create On Server
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/VSDA/EM/Initialize?SimulationID={_SimulationID}")
+        QueryList:list = []
+        QueryList.append({
+            "VSDA/Ca/Initialize": {
+                "SimulationID": _SimulationID
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
 
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/VSDA/EM/SetupMicroscope?SimulationID={_SimulationID}&PixelResolution_nm={_Configuration.PixelResolution_nm}&ImageWidth_px={_Configuration.ImageWidth_px}&ImageHeight_px={_Configuration.ImageHeight_px}&SliceThickness_nm={_Configuration.SliceThickness_nm}&ScanRegionOverlap_percent={_Configuration.ScanRegionOverlap_percent}&MicroscopeFOV_deg={_Configuration.MicroscopeFOV_deg}&NumPixelsPerVoxel_px={_Configuration.NumPixelsPerVoxel_px}")
+        QueryList:list = []
+        QueryList.append({
+            "VSDA/Ca/SetupMicroscope": {
+                "VoxelResolution_nm": _Configuration.VoxelResolution_nm,
+                "ImageWidth_px": _Configuration.ImageWidth_px,
+                "ImageHeight_px": _Configuration.ImageHeight_px,
+                "NumVoxelsPerSlice": _Configuration.NumVoxelsPerSlice,
+                "ScanRegionOverlap_percent": _Configuration.ScanRegionOverlap_percent,
+                "NumPixelsPerVoxel_px": _Configuration.NumPixelsPerVoxel_px,
+                "FlourescingNeuronIDs": _Configuration.FlourescingNeuronIDs,
+                "CalciumIndicator": _Configuration.CalciumIndicator,
+                "IndicatorRiseTime_ms": _Configuration.IndicatorRiseTime_ms,
+                "IndicatorDecayTime_ms": _Configuration.IndicatorDecayTime_ms,
+                "IndicatorInterval_ms": _Configuration.IndicatorInterval_ms,
+                "ImagingInterval_ms": _Configuration.ImagingInterval_ms,
+                "BrightnessAmplification": _Configuration.BrightnessAmplification,
+                "AttenuationPerUm": _Configuration.AttenuationPerUm,
+                "SimulationID": _SimulationID
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
 
 
 
     ## Access Methods
-    def DefineScanRegion(self, _Point1_um:list, _Point2_um:list):
-        Point1 = json.dumps(_Point1_um)
-        Point2 = json.dumps(_Point2_um)
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/VSDA/EM/DefineScanRegion?SimulationID={self.SimulationID}&Point1_um={Point1}&Point2_um={Point2}")
+    def DefineScanRegion(self, _Point1_um:list, _Point2_um:list, _Rotation_rad:list):
+        QueryList:list = []
+        QueryList.append({
+            "VSDA/Ca/DefineScanRegion": {
+                "Point1_um": _Point1_um,
+                "Point2_um": _Point2_um,
+                "SampleRotation_rad": _Rotation_rad,
+                "SimulationID": self.SimulationID
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         self.ScanRegionID = Response["ScanRegionID"]
 
 
     def QueueRenderOperation(self):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/VSDA/EM/QueueRenderOperation?SimulationID={self.SimulationID}&ScanRegionID={self.ScanRegionID}")
+        QueryList:list = []
+        QueryList.append({
+            "VSDA/Ca/QueueRenderOperation": {
+                "ScanRegionID": self.ScanRegionID,
+                "SimulationID": self.SimulationID
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response["StatusCode"]
 
 
     def GetRenderStatus(self):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/VSDA/EM/GetRenderStatus?SimulationID={self.SimulationID}")
+        QueryList:list = []
+        QueryList.append({
+            "VSDA/Ca/GetRenderStatus": {
+                "SimulationID": self.SimulationID
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response
     
 
     def GetImageStack(self):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/VSDA/EM/GetImageStack?SimulationID={self.SimulationID}&ScanRegionID={self.ScanRegionID}")
+        QueryList:list = []
+        QueryList.append({
+            "VSDA/Ca/GetImageStack": {
+                "ScanRegionID": self.ScanRegionID,
+                "SimulationID": self.SimulationID
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response["RenderedImages"]
 
 
     def GetImage(self, _ImageHandle:str):
-        Response = self.RequestHandler.MakeAuthenticatedQuery(f"/NES/VSDA/EM/GetImage?SimulationID={self.SimulationID}&ImageHandle={_ImageHandle}")
+        QueryList:list = []
+        QueryList.append({
+            "VSDA/GetImage": {
+                "ImageHandle": _ImageHandle,
+                "SimulationID": self.SimulationID
+            }
+        })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return bytes(Response["ImageData"], 'utf-8')
+
+
+    def GetImages(self, _ImageHandles:list):
     
+        QueryList:list = []
+
+        for ImageHandle in _ImageHandles:
+            QueryList.append({
+                "VSDA/GetImage": {
+                    "SimulationID": self.SimulationID,
+                    "ImageHandle": ImageHandle
+                }
+            })
+        Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")
+        assert(Response != None)
+        
+        ImageBytes:list = []
+        for ImageResponse in Response:
+            ImageBytes.append(bytes(ImageResponse["ImageData"], 'utf-8'))
+        return ImageBytes
+
+
+
 
     def WaitForRender(self):
 
         # Setup Status Information
         StatusInfo:dict = self.GetRenderStatus()
 
 
         # Perform Sanity Check On Render
         if (StatusInfo["RenderStatus"] < 3):
             print("Error during rendering, API reports:\n")
             print(StatusInfo)
 
 
         # Block With Queued Spinner
-        QueueSpinner = yaspin.yaspin(text="Render Operation In Queue, Elapsed Time", color="green", timer=True)
+        QueueSpinner = yaspin.yaspin(text="Calcium Render Operation In Queue, Elapsed Time", color="green", timer=True)
         QueueSpinner.start()
         while (StatusInfo["RenderStatus"] == 3):
 
             # Get Status Info, Wait To Avoid API Spam
             StatusInfo:dict = self.GetRenderStatus()
             time.sleep(0.25)
 
@@ -115,112 +200,64 @@
         # Block Execution Until Render Finishes, Update Bar As We Wait
         while (StatusInfo["RenderStatus"] != 5):
 
             # Update Region Bar
             RegionStatusBar.total = int(StatusInfo["TotalRegions"])
             RegionStatusBar.n = max(int(StatusInfo["CurrentRegion"]), 0)
             RegionStatusBar.refresh()
-            RegionStatusBar.set_description(f"Rendering Region {str(StatusInfo['CurrentRegion']).rjust(5, '0')} / {str(StatusInfo['TotalRegions']).rjust(5, '0')}")
+            RegionStatusBar.set_description(f"Rendering Calcium Region {str(StatusInfo['CurrentRegion']).rjust(5, '0')} / {str(StatusInfo['TotalRegions']).rjust(5, '0')}")
 
 
             # Update Slice Bar
             if (RegionStatusBar.n > LastRegionNumber):
                 LastRegionNumber = RegionStatusBar.n
                 SliceStatusBar.reset()
             SliceStatusBar.total = int(StatusInfo["TotalSlices"])
             SliceStatusBar.n = max(int(StatusInfo["CurrentSlice"]), 0)
             SliceStatusBar.refresh()
-            SliceStatusBar.set_description(f"Rendering Slice {str(StatusInfo['CurrentSlice']).rjust(5, '0')} / {str(StatusInfo['TotalSlices']).rjust(5, '0')}")
+            SliceStatusBar.set_description(f"Rendering Calcium Slice {str(StatusInfo['CurrentSlice']).rjust(5, '0')} / {str(StatusInfo['TotalSlices']).rjust(5, '0')}")
 
 
             # Update Image Bar
             if (SliceStatusBar.n > LastSliceNumber):
                 LastSliceNumber = SliceStatusBar.n
                 ImageStatusBar.reset()
             ImageStatusBar.total = int(StatusInfo["TotalSliceImages"])
             ImageStatusBar.n = max(int(StatusInfo["CurrentSliceImage"]), 0)
             ImageStatusBar.refresh()
-            ImageStatusBar.set_description(f"Rendering Image {str(StatusInfo['CurrentSliceImage']).rjust(5, '0')} / {str(StatusInfo['TotalSliceImages']).rjust(5, '0')}")
+            ImageStatusBar.set_description(f"Rendering Calcium Image {str(StatusInfo['CurrentSliceImage']).rjust(5, '0')} / {str(StatusInfo['TotalSliceImages']).rjust(5, '0')}")
 
 
 
             # Get Status Info, Wait To Avoid API Spam
             StatusInfo:dict = self.GetRenderStatus()
             time.sleep(0.1)
         
     
         # When we're done, rendering is finished - make it look like it truly is, then close the bar
         RegionStatusBar.total = int(StatusInfo["TotalRegions"])
         RegionStatusBar.n = int(StatusInfo["TotalRegions"])
-        RegionStatusBar.set_description(f"Rendering Slice {str(StatusInfo['TotalRegions']).rjust(5, '0')} / {str(StatusInfo['TotalRegions']).rjust(5, '0')}")
+        RegionStatusBar.set_description(f"Rendering Calcium Region {str(StatusInfo['TotalRegions']).rjust(5, '0')} / {str(StatusInfo['TotalRegions']).rjust(5, '0')}")
         RegionStatusBar.refresh()
         RegionStatusBar.close()
         SliceStatusBar.total = int(StatusInfo["TotalSlices"])
         SliceStatusBar.n = int(StatusInfo["TotalSlices"])
-        SliceStatusBar.set_description(f"Rendering Slice {str(StatusInfo['TotalSlices']).rjust(5, '0')} / {str(StatusInfo['TotalSlices']).rjust(5, '0')}")
+        SliceStatusBar.set_description(f"Rendering Calcium Slice {str(StatusInfo['TotalSlices']).rjust(5, '0')} / {str(StatusInfo['TotalSlices']).rjust(5, '0')}")
         SliceStatusBar.refresh()
         SliceStatusBar.close()
         ImageStatusBar.total = int(StatusInfo["TotalSliceImages"])
         ImageStatusBar.n = int(StatusInfo["TotalSliceImages"])
-        ImageStatusBar.set_description(f"Rendering Image {str(StatusInfo['TotalSliceImages']).rjust(5, '0')} / {str(StatusInfo['TotalSliceImages']).rjust(5, '0')}")
+        ImageStatusBar.set_description(f"Rendering Calcium Image {str(StatusInfo['TotalSliceImages']).rjust(5, '0')} / {str(StatusInfo['TotalSliceImages']).rjust(5, '0')}")
         ImageStatusBar.refresh()
         ImageStatusBar.close()
 
 
-    def ThreadedSaveImageStack(self, _ImageStackDirectoryPrefix:str = "", _AsyncImages:int=10):
 
-        # Check That The DirectoryPath Exists
-        if not _ImageStackDirectoryPrefix.endswith("/"):
-            _ImageStackDirectoryPrefix += "/"
-        
-        if not os.path.exists(_ImageStackDirectoryPrefix):
-            os.makedirs(_ImageStackDirectoryPrefix)
-            
 
-        # Get Image Stack Manifest
-        ImageHandles = self.GetImageStack()
-
-        # Setup Progress Bar
-        Bar = tqdm.tqdm("Downloading Image Stack", total=len(ImageHandles))
-        Bar.leave = True
-        Bar.bar_format = "{desc}{percentage:3.0f}%|{bar}| [{elapsed}<{remaining}, {rate_fmt}{postfix}]"
-        Bar.colour = "green"
-
-
-        for i in range(0, len(ImageHandles), _AsyncImages):
-
-            # Make Batch Request URI List
-            RequestURIs:list = []
-            for x in range(i, i + _AsyncImages):
-                RequestURIs.append(f"/NES/VSDA/EM/GetImage?SimulationID={self.SimulationID}&ImageHandle={ImageHandles[x]}")
-
-            # Get Data
-            Images = self.RequestHandler.MakeAuthenticatedAsyncQueries(RequestURIs)
-
-            for Image in Images:
-                ImageData = bytes(Image["ImageData"], 'utf-8')
-                with open(_ImageStackDirectoryPrefix + ImageHandles[i].split("/")[1], "wb") as FileHandler:
-                    FileHandler.write(base64.decodebytes(ImageData))
-
-            Bar.set_description(f"Downloading Image {str(i + 1).rjust(5, '0')} / {str(len(ImageHandles)).rjust(5, '0')}")
-
-            # Count Up Bar
-            Bar.n = i + _AsyncImages
-            Bar.refresh()
-
-        
-        # Finalize Bar
-        Bar.set_description(f"Downloading Image {str(len(ImageHandles)).rjust(5, '0')} / {str(len(ImageHandles)).rjust(5, '0')}")
-        Bar.n = len(ImageHandles)
-        Bar.refresh()
-
-        Bar.close()
-
-
-    def SaveImageStack(self, _ImageStackDirectoryPrefix:str = ""):
+    def SaveImageStack(self, _ImageStackDirectoryPrefix:str = "", _NumImagesPerCall:int = 4):
 
         # Check That The DirectoryPath Exists
         if not _ImageStackDirectoryPrefix.endswith("/"):
             _ImageStackDirectoryPrefix += "/"
         
         if not os.path.exists(_ImageStackDirectoryPrefix):
             os.makedirs(_ImageStackDirectoryPrefix)
@@ -231,22 +268,31 @@
 
         # Setup Progress Bar
         Bar = tqdm.tqdm("Downloading Image Stack", total=len(ImageHandles))
         Bar.leave = True
         Bar.bar_format = "{desc}{percentage:3.0f}%|{bar}| [{elapsed}<{remaining}, {rate_fmt}{postfix}]"
         Bar.colour = "green"
 
+        Total:int = 0
+        for x in range(math.ceil(len(ImageHandles) / _NumImagesPerCall)):
 
-        for i in range(len(ImageHandles)):
-
-            # Save This Image
-            ImageData = self.GetImage(ImageHandles[i])
-            with open(_ImageStackDirectoryPrefix + ImageHandles[i].replace("/", "_").strip("Renders")[1:], "wb") as FileHandler:
-                FileHandler.write(base64.decodebytes(ImageData))
-
-            Bar.set_description(f"Downloading Image {str(i + 1).rjust(5, '0')} / {str(len(ImageHandles)).rjust(5, '0')}")
-
+            BatchHandles:list = []
+            for i in range(_NumImagesPerCall):
+                if (Total < len(ImageHandles)):
+                    BatchHandles.append(ImageHandles[Total])
+                    Total += 1
+
+            # Save These Images
+            ImagesData:list = self.GetImages(BatchHandles)
+
+            for i in range(_NumImagesPerCall):
+                if (i < len(BatchHandles)):
+                    with open(_ImageStackDirectoryPrefix + BatchHandles[i].replace("/", "_").strip("Renders")[1:], "wb") as FileHandler:
+                        FileHandler.write(base64.decodebytes(ImagesData[i]))
+            
             # Count Up Bar
-            Bar.n = i + 1
+            CurrentImageIndex = x * _NumImagesPerCall
+            Bar.set_description(f"Downloading Image {str(CurrentImageIndex + 1).rjust(5, '0')} / {str(len(ImageHandles)).rjust(5, '0')}")
+            Bar.n = CurrentImageIndex + 1
             Bar.refresh()
 
         Bar.close()
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/NES/Visualizer/Visualizer.py` & `pybraingenixclient-2024.4.29/BrainGenix/NES/Visualizer/Visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 "CameraLookAtPositionY_um": _Configuration.CameraLookAtPositionList_um[i][1],
                 "CameraLookAtPositionZ_um": _Configuration.CameraLookAtPositionList_um[i][2],
                 "CameraFOV_deg": _Configuration.CameraFOVList_deg[i],
             })
 
         QueryList:list = []
         QueryList.append({
-            "VisualizerGenerateImage": {
+            "Visualizer/GenerateImages": {
                 "ImageWidth_px": _Configuration.ImageWidth_px,
                 "ImageHeight_px": _Configuration.ImageHeight_px,
                 "Locations": LocationList,
                 "SimulationID": self.SimulationID
             }
         })
         Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
@@ -57,29 +57,29 @@
 
 
 
     def GetStatus(self):
 
         QueryList:list = []
         QueryList.append({
-            "VisualizerGetStatus": {
+            "Visualizer/GetStatus": {
                 "SimulationID": self.SimulationID
             }
         })
         Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return Response["VisualizerStatus"]
 
 
 
     def GetImageHandles(self):
 
         QueryList:list = []
         QueryList.append({
-            "VisualizerGetImageHandles": {
+            "Visualizer/GetImageHandles": {
                 "SimulationID": self.SimulationID
             }
         })
         Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")[0]
         assert(Response != None)
         return json.loads(Response["ImageHandles"])
 
@@ -87,15 +87,15 @@
 
     def GetImages(self, _ImageHandles:list):
     
         QueryList:list = []
 
         for ImageHandle in _ImageHandles:
             QueryList.append({
-                "VisualizerGetImage": {
+                "Visualizer/GetImage": {
                     "SimulationID": self.SimulationID,
                     "ImageHandle": ImageHandle
                 }
             })
         Response = self.RequestHandler.BuildPostQuery(QueryList, "/NES")
         assert(Response != None)
         
@@ -150,11 +150,13 @@
                     Total += 1
 
 
             ImageData:list = self.GetImages(BatchHandles)
 
             for i in range(len(BatchHandles)):
 
-                with open(_Prefix + BatchHandles[i].split("/")[2], "wb") as FileHandler:
-                    FileHandler.write(base64.decodebytes(ImageData[i]))
+                if (i < len(BatchHandles)):
+
+                    with open(_Prefix + BatchHandles[i].split("/")[2], "wb") as FileHandler:
+                        FileHandler.write(base64.decodebytes(ImageData[i]))
 
         WaitSpinner.ok()
```

### Comparing `pyBrainGenixClient-2024.2.9.1/BrainGenix/Tools/Test/Test.py` & `pybraingenixclient-2024.4.29/BrainGenix/Tools/Test/Test.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     assert(ClientInstance.IsReady())
 
     
     # Create A New Simulation
     print(" -- Creating Simulation")
     SimulationCfg = NES.Simulation.Configuration()
     SimulationCfg.Name = "My First Simulation"
+    SimulationCfg.Seed = 0
     MySim = ClientInstance.CreateSimulation(SimulationCfg)
     
 
     # Create Sphere
     print(" -- Creating Sphere")
     SphereCfg = NES.Shapes.Sphere.Configuration()
     SphereCfg.Name = "My Sphere"
```

### Comparing `pyBrainGenixClient-2024.2.9.1/LICENSE.md` & `pybraingenixclient-2024.4.29/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyBrainGenixClient-2024.2.9.1/PKG-INFO` & `pybraingenixclient-2024.4.29/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBrainGenixClient
-Version: 2024.2.9.1
+Version: 2024.4.29
 Summary: Python client for BrainGenix WBE platform.
 Author-email: BrainGenix Team <braingenix@carboncopies.org>
 Project-URL: Homepage, https://gitlab.braingenix.org/carboncopies/BrainGenix/NES/PythonClient
 Project-URL: Bug Tracker, https://gitlab.braingenix.org/carboncopies/BrainGenix/NES/PythonClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -13,12 +13,14 @@
 License-File: LICENSE.md
 Requires-Dist: requests
 Requires-Dist: requests_futures
 Requires-Dist: tqdm
 Requires-Dist: yaspin
 Requires-Dist: pillow
 Requires-Dist: imageio
+Requires-Dist: pandas
+Requires-Dist: joblib
 
 # About
 This directory contains the python implementation as defined in the NES block diagram. Please see the below image for project structure:
 
 ![Image](Overview.png)
```

### Comparing `pyBrainGenixClient-2024.2.9.1/pyBrainGenixClient.egg-info/PKG-INFO` & `pybraingenixclient-2024.4.29/pyBrainGenixClient.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBrainGenixClient
-Version: 2024.2.9.1
+Version: 2024.4.29
 Summary: Python client for BrainGenix WBE platform.
 Author-email: BrainGenix Team <braingenix@carboncopies.org>
 Project-URL: Homepage, https://gitlab.braingenix.org/carboncopies/BrainGenix/NES/PythonClient
 Project-URL: Bug Tracker, https://gitlab.braingenix.org/carboncopies/BrainGenix/NES/PythonClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -13,12 +13,14 @@
 License-File: LICENSE.md
 Requires-Dist: requests
 Requires-Dist: requests_futures
 Requires-Dist: tqdm
 Requires-Dist: yaspin
 Requires-Dist: pillow
 Requires-Dist: imageio
+Requires-Dist: pandas
+Requires-Dist: joblib
 
 # About
 This directory contains the python implementation as defined in the NES block diagram. Please see the below image for project structure:
 
 ![Image](Overview.png)
```

### Comparing `pyBrainGenixClient-2024.2.9.1/pyBrainGenixClient.egg-info/SOURCES.txt` & `pybraingenixclient-2024.4.29/pyBrainGenixClient.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 LICENSE.md
 README.md
 pyproject.toml
+BrainGenix/BG_API.py
 BrainGenix/__init__.py
+BrainGenix/EVM/__init__.py
+BrainGenix/EVM/Debug/DoubleEcho.py
+BrainGenix/EVM/Debug/Echo.py
+BrainGenix/EVM/Debug/__init__.py
 BrainGenix/LibUtils/ConfigCheck.py
 BrainGenix/LibUtils/GetID.py
 BrainGenix/NES/__init__.py
 BrainGenix/NES/Client/Client.py
 BrainGenix/NES/Client/Configuration.py
 BrainGenix/NES/Client/RequestHandler.py
 BrainGenix/NES/Client/__init__.py
@@ -16,25 +21,31 @@
 BrainGenix/NES/Client/Modes/Remote.py
 BrainGenix/NES/Client/Modes/__init__.py
 BrainGenix/NES/Models/__init__.py
 BrainGenix/NES/Models/Compartments/__init__.py
 BrainGenix/NES/Models/Compartments/BS/BS.py
 BrainGenix/NES/Models/Compartments/BS/Configuration.py
 BrainGenix/NES/Models/Compartments/BS/__init__.py
+BrainGenix/NES/Models/Compartments/SC/Configuration.py
+BrainGenix/NES/Models/Compartments/SC/SC.py
+BrainGenix/NES/Models/Compartments/SC/__init__.py
 BrainGenix/NES/Models/Connections/__init__.py
 BrainGenix/NES/Models/Connections/Receptor/Configuration.py
 BrainGenix/NES/Models/Connections/Receptor/Receptor.py
 BrainGenix/NES/Models/Connections/Receptor/__init__.py
 BrainGenix/NES/Models/Connections/Staple/Configuration.py
 BrainGenix/NES/Models/Connections/Staple/Staple.py
 BrainGenix/NES/Models/Connections/Staple/__init__.py
 BrainGenix/NES/Models/Neurons/__init__.py
 BrainGenix/NES/Models/Neurons/BS/BSNeuron.py
 BrainGenix/NES/Models/Neurons/BS/Configuration.py
 BrainGenix/NES/Models/Neurons/BS/__init__.py
+BrainGenix/NES/Models/Neurons/SC/Configuration.py
+BrainGenix/NES/Models/Neurons/SC/SCNeuron.py
+BrainGenix/NES/Models/Neurons/SC/__init__.py
 BrainGenix/NES/Shapes/__init__.py
 BrainGenix/NES/Shapes/Box/Box.py
 BrainGenix/NES/Shapes/Box/Configuration.py
 BrainGenix/NES/Shapes/Box/__init__.py
 BrainGenix/NES/Shapes/Cylinder/Configuration.py
 BrainGenix/NES/Shapes/Cylinder/Cylinder.py
 BrainGenix/NES/Shapes/Cylinder/__init__.py
@@ -58,14 +69,17 @@
 BrainGenix/NES/VSDA/EM/Configuration.py
 BrainGenix/NES/VSDA/EM/EM.py
 BrainGenix/NES/VSDA/EM/__init__.py
 BrainGenix/NES/Visualizer/Configuration.py
 BrainGenix/NES/Visualizer/Visualizer.py
 BrainGenix/NES/Visualizer/__init__.py
 BrainGenix/Tools/__init__.py
+BrainGenix/Tools/NeuroglancerConverter/NeuroglancerConverter.py
+BrainGenix/Tools/NeuroglancerConverter/__init__.py
+BrainGenix/Tools/StackStitcher/CaImagingStackStitcher.py
 BrainGenix/Tools/StackStitcher/StackStitcher.py
 BrainGenix/Tools/StackStitcher/__init__.py
 BrainGenix/Tools/Test/Test.py
 BrainGenix/Tools/Test/__init__.py
 pyBrainGenixClient.egg-info/PKG-INFO
 pyBrainGenixClient.egg-info/SOURCES.txt
 pyBrainGenixClient.egg-info/dependency_links.txt
```

### Comparing `pyBrainGenixClient-2024.2.9.1/pyproject.toml` & `pybraingenixclient-2024.4.29/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.setuptools.packages.find]
 include = ["BrainGenix*"]
 exclude = ["Tests*"]
 
 [project]
 name = "pyBrainGenixClient"
-version = "2024.02.09.1"
+version = "2024.4.29"
 authors = [
   { name="BrainGenix Team", email="braingenix@carboncopies.org" },
 ]
 description = "Python client for BrainGenix WBE platform."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -24,13 +24,15 @@
 ]
 dependencies = [
   "requests",
   "requests_futures",
   "tqdm",
   "yaspin",
   "pillow",
-  "imageio"
+  "imageio",
+  "pandas",
+  "joblib"
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.braingenix.org/carboncopies/BrainGenix/NES/PythonClient"
 "Bug Tracker" = "https://gitlab.braingenix.org/carboncopies/BrainGenix/NES/PythonClient/issues"
```

