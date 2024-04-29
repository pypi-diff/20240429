# Comparing `tmp/janus_core-0.2.0b6.tar.gz` & `tmp/janus_core-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_core-0.2.0b6.tar", max compression
+gzip compressed data, was "janus_core-0.3.0b1.tar", max compression
```

## Comparing `janus_core-0.2.0b6.tar` & `janus_core-0.3.0b1.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0     1533 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/LICENSE
--rw-r--r--   0        0        0     8612 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/README.md
--rw-r--r--   0        0        0       80 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/__init__.py
--rw-r--r--   0        0        0    30268 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/cli.py
--rw-r--r--   0        0        0     4790 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/geom_opt.py
--rw-r--r--   0        0        0     1664 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/janus_types.py
--rw-r--r--   0        0        0     4045 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/log.py
--rw-r--r--   0        0        0    32216 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/md.py
--rw-r--r--   0        0        0     3514 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/mlip_calculators.py
--rw-r--r--   0        0        0    12111 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/single_point.py
--rw-r--r--   0        0        0     3293 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/stats.py
--rw-r--r--   0        0        0     1544 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/utils.py
--rw-r--r--   0        0        0     2553 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/pyproject.toml
--rw-r--r--   0        0        0     9673 1970-01-01 00:00:00.000000 janus_core-0.2.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/LICENSE
+-rw-r--r--   0        0        0     9036 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/README.md
+-rw-r--r--   0        0        0      132 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/janus_core/__init__.py
+-rw-r--r--   0        0        0     4814 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/janus_core/calculations/geom_opt.py
+-rw-r--r--   0        0        0    34723 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/janus_core/calculations/md.py
+-rw-r--r--   0        0        0    12143 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/janus_core/calculations/single_point.py
+-rw-r--r--   0        0        0     6958 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/geomopt.py
+-rw-r--r--   0        0        0      839 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/janus.py
+-rw-r--r--   0        0        0    13206 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/md.py
+-rw-r--r--   0        0        0     5203 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/singlepoint.py
+-rw-r--r--   0        0        0     3481 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/types.py
+-rw-r--r--   0        0        0     3274 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/utils.py
+-rw-r--r--   0        0        0     1686 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/janus_types.py
+-rw-r--r--   0        0        0     4053 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/log.py
+-rw-r--r--   0        0        0     3532 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/mlip_calculators.py
+-rw-r--r--   0        0        0     5838 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/stats.py
+-rw-r--r--   0        0        0     1544 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/utils.py
+-rw-r--r--   0        0        0     2558 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0    10095 1970-01-01 00:00:00.000000 janus_core-0.3.0b1/PKG-INFO
```

### Comparing `janus_core-0.2.0b6/LICENSE` & `janus_core-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b6/README.md` & `janus_core-0.3.0b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 ```
 
 This will generate several output files:
 
 - Thermodynamical statistics every 100 steps, written to `NaCl-npt-T300.0-p1.0-stats.dat`
 - The structure trajectory every 100 steps, written to `NaCl-npt-T300.0-p1.0-traj.xyz`
 - The structure to be able to restart the dynamics every 1000 steps, written to `NaCl-npt-T300.0-p1.0-res-1000.xyz`
+- The final structure written to `NaCl-npt-T300.0-p1.0-final.xyz`
 - A log of the processes carried out, written to `md.log`
 - A summary of the inputs and start/end time, written to `md_summary.yml`.
 
 Additional options may be specified. For example:
 
 ```shell
 janus md --ensemble nvt --struct tests/data/NaCl.cif --steps 1000 --timestep 0.5 --temp 300 --minimize --minimize-every 100 --rescale-velocities --remove-rot --rescale-every 100 --equil-steps 200
@@ -146,24 +147,33 @@
 
 Run an NVT heating simultation from 20K to 300K in steps of 20K, with 10fs at each temperature:
 
 ```shell
 janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10
 ```
 
-This produces the same output files as an MD simulation.
+The produced statistics and trajectory files will indicate the heating range `NaCl-nvt-T20.0-T300.0-stats.dat`, `NaCl-nvt-T20.0-T300.0-traj.xyz`. There will also be final structure files at each temperature point:
 
-MD can also be carried out after heating using the same options as described in #molecular-dynamics. For example:
+```
+NaCl-nvt-T20.0-final.xyz
+NaCl-nvt-T40.0-final.xyz
+...
+NaCl-nvt-T300.0-final.xyz
+```
+
+MD can also be carried out after heating using the same options as described in [Molecular dynamics](#molecular-dynamics). For example:
 
 ```shell
 janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10 --steps 1000 --temp 300
 ```
 
 This performs the same initial heating, before running a further 1000 steps (1 ps) at 300K.
 
+When MD is run with heating the trajectory ```NaCl-nvt-T20.0-T300.0-T300.0-traj.xyz``` and statistics ```NaCl-nvt-T20.0-T300.0-T300.0-stats.dat``` files will indicate the heating range and MD temperature (which may be different). With heating and MD trajectories/statistics within the same files.
+
 
 ### Using configuration files
 
 Default values for all command line options may be specifed through a Yaml 1.1 formatted configuration file by adding the `--config` option. If an option is present in both the command line and configuration file, the command line value takes precedence.
 
 For example, with the following configuration file and command:
 
@@ -183,18 +193,14 @@
 
 This will run a singlepoint energy calculation on `KCl.cif` using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "medium" force-field, saving the results to `KCl-results.cif`.
 
 
 > [!NOTE]
 > `properties` must be passed as a Yaml list, as above, not as a string.
 
-> [!WARNING]
-> If an option in the configuration file does not match any variable names, an error will **not** be raised.
-> Please check the summary file to ensure the configuration has been read correctly.
-
 
 ## License
 
 [BSD 3-Clause License](LICENSE)
 
 ## Funding
```

### Comparing `janus_core-0.2.0b6/janus_core/geom_opt.py` & `janus_core-0.3.0b1/janus_core/calculations/geom_opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 try:
     from ase.filters import FrechetCellFilter as DefaultFilter
 except ImportError:
     from ase.constraints import ExpCellFilter as DefaultFilter
 
 from numpy import linalg
 
-from janus_core.janus_types import ASEOptArgs, ASEWriteArgs
-from janus_core.log import config_logger
-from janus_core.utils import none_to_dict
+from janus_core.helpers.janus_types import ASEOptArgs, ASEWriteArgs
+from janus_core.helpers.log import config_logger
+from janus_core.helpers.utils import none_to_dict
 
 
 def optimize(  # pylint: disable=too-many-arguments,too-many-locals,too-many-branches
     struct: Atoms,
     fmax: float = 0.1,
     steps: int = 1000,
     filter_func: Optional[Callable] = DefaultFilter,
```

### Comparing `janus_core-0.2.0b6/janus_core/janus_types.py` & `janus_core-0.3.0b1/janus_core/helpers/janus_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Module containing types used in Janus-Core.
-"""
+"""Module containing types used in Janus-Core."""
 
 from collections.abc import Sequence
 from enum import Enum
 import logging
 from pathlib import Path, PurePath
 from typing import IO, Literal, Optional, TypedDict, TypeVar, Union
 
@@ -47,15 +45,15 @@
     """Main arugments for ase optimisers."""
 
     restart: Optional[bool]
     logfile: Optional[PathLike]
     trajectory: Optional[str]
 
 
-class LogLevel(Enum):
+class LogLevel(Enum):  # numpydoc ignore=PR01
     """Supported options for logger levels."""
 
     DEBUG = logging.DEBUG
     INFO = logging.INFO
     WARNING = logging.WARNING
     ERROR = logging.ERROR
```

### Comparing `janus_core-0.2.0b6/janus_core/log.py` & `janus_core-0.3.0b1/janus_core/helpers/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Configure logger with yaml-styled format."""
 
 import logging
 from typing import Literal, Optional
 
-from janus_core.janus_types import LogLevel
+from janus_core.helpers.janus_types import LogLevel
 
 
 class YamlFormatter(logging.Formatter):  # numpydoc ignore=PR02
     """
     Custom formatter to convert multiline messages into yaml list.
 
     Parameters
```

### Comparing `janus_core-0.2.0b6/janus_core/md.py` & `janus_core-0.3.0b1/janus_core/calculations/md.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=too-many-lines
 """Run molecular dynamics simulations."""
 
 import datetime
 from pathlib import Path
 import random
 from typing import Any, Optional
 from warnings import warn
@@ -14,17 +15,17 @@
     MaxwellBoltzmannDistribution,
     Stationary,
     ZeroRotation,
 )
 from ase.md.verlet import VelocityVerlet
 import numpy as np
 
-from janus_core.geom_opt import optimize
-from janus_core.janus_types import Ensembles, PathLike
-from janus_core.log import config_logger
+from janus_core.calculations.geom_opt import optimize
+from janus_core.helpers.janus_types import Ensembles, PathLike
+from janus_core.helpers.log import config_logger
 
 DENS_FACT = (units.m / 1.0e2) ** 3 / units.mol
 
 
 class MolecularDynamics:  # pylint: disable=too-many-instance-attributes
     """
     Configure shared molecular dynamics simulation options.
@@ -356,27 +357,81 @@
                     "filename": self.log_kwargs["filename"],
                     "name": self.logger.name,
                     "filemode": "a",
                 }
                 self.logger.info("Minimizing at step %s", self.dyn.nsteps)
             optimize(self.struct, **self.minimize_kwargs)
 
+    @property
+    def _parameter_prefix(self) -> str:
+        """
+        Ensemble parameters for output files.
+
+        Returns
+        -------
+        str
+           Formatted temperature range if heating and target temp if running md.
+        """
+
+        temperature_prefix = ""
+        if self.temp_start and self.temp_end:
+            temperature_prefix = f"-T{self.temp_start}-T{self.temp_end}"
+
+        if self.steps > 0:
+            temperature_prefix += f"-T{self.temp}"
+
+        return temperature_prefix
+
+    @property
+    def _final_file(self) -> str:
+        """
+        Final state file name.
+
+        Returns
+        -------
+        str
+           File name for final state.
+        """
+
+        if not self.restart_stem:
+            return f"{self.file_prefix}-T{self.temp}-final.xyz"
+        # respect the users choice
+        return f"{self.restart_stem}-T{self.temp}-final.xyz"
+
+    @property
+    def _restart_file(self) -> str:
+        """
+        Restart file name.
+
+        Returns
+        -------
+        str
+           File name for restart files.
+        """
+        step = self.offset + self.dyn.nsteps
+        if not self.restart_stem:
+            return f"{self.file_prefix}-T{self.temp}-res-{step}.xyz"
+        return f"{self.restart_stem}-T{self.temp}-res-{step}.xyz"
+
     def configure_filenames(self) -> None:
         """Setup filenames for output files."""
+
         if not self.file_prefix:
-            self.file_prefix = f"{self.struct_name}-{self.ensemble}-T{self.temp}"
+            self.file_prefix = f"{self.struct_name}-{self.ensemble}"
+            data_prefix = f"{self.file_prefix}{self._parameter_prefix}"
+        else:
+            data_prefix = f"{self.file_prefix}"
+            if not self.restart_stem:
+                self.restart_stem = f"{self.file_prefix}"
 
         if not self.stats_file:
-            self.stats_file = f"{self.file_prefix}-stats.dat"
+            self.stats_file = f"{data_prefix}-stats.dat"
 
         if not self.traj_file:
-            self.traj_file = f"{self.file_prefix}-traj.xyz"
-
-        if not self.restart_stem:
-            self.restart_stem = f"{self.file_prefix}-res"
+            self.traj_file = f"{data_prefix}-traj.xyz"
 
     @staticmethod
     def get_log_header() -> str:
         """
         Get header string for molecular dynamics log.
 
         Returns
@@ -467,27 +522,35 @@
             self.dyn.atoms.write(
                 self.traj_file,
                 write_info=True,
                 columns=["symbols", "positions", "momenta", "masses"],
                 append=append,
             )
 
+    def _write_final_state(self) -> None:
+        """Write the final system state."""
+        write(
+            self._final_file,
+            self.struct,
+            write_info=True,
+            columns=["symbols", "positions", "momenta", "masses"],
+        )
+
     def _write_restart(self) -> None:
         """Write restart file and (optionally) rotate files saved."""
         step = self.offset + self.dyn.nsteps
         if step > 0:
-            restart_file = f"{self.restart_stem}-{step}.xyz"
             write(
-                restart_file,
+                self._restart_file,
                 self.struct,
                 write_info=True,
                 columns=["symbols", "positions", "momenta", "masses"],
             )
             if self.rotate_restart:
-                self.restart_files.append(restart_file)
+                self.restart_files.append(self._restart_file)
                 self._rotate_restart_files()
 
     def run(self) -> None:
         """Run molecular dynamics simulation and/or temperature ramp."""
         # Check if restarting simulation
         if self.restart:
             try:
@@ -542,23 +605,25 @@
             temps = [self.temp_start + i * self.temp_step for i in range(n_temps)]
 
             if self.logger:
                 self.logger.info("Beginning temperature ramp at %sK", temps[0])
             for temp in temps:
                 self.temp = temp
                 self.dyn.run(heating_steps)
+                self._write_final_state()
             if self.logger:
                 self.logger.info("Temperature ramp complete at %sK", temps[-1])
 
         # Run MD
         if self.steps > 0:
             if self.logger:
                 self.logger.info("Starting molecular dynamics simulation")
             self.temp = md_temp
             self.dyn.run(self.steps)
+            self._write_final_state()
             if self.logger:
                 self.logger.info("Molecular dynamics simulation complete")
 
 
 class NPT(MolecularDynamics):
     """
     Configure NPT dynamics.
@@ -619,48 +684,80 @@
             Name for thermodynamic ensemble. Default is "npt".
         file_prefix : Optional[PathLike]
             Prefix for output filenames. Default is inferred from structure, ensemble,
             temperature, and pressure.
         **kwargs
             Additional keyword arguments.
         """
+        self.pressure = pressure
         super().__init__(ensemble=ensemble, file_prefix=file_prefix, *args, **kwargs)
 
-        self.pressure = pressure
         self.ttime = thermostat_time * units.fs
         scaled_bulk_modulus = bulk_modulus * units.GPa
         if barostat_time:
             pfactor = (barostat_time * units.fs) ** 2 * scaled_bulk_modulus
         else:
             pfactor = None
 
-        # Reconfigure filenames to include pressure if `file_prefix` not specified
-        # Requires super().__init__ first to determine `self.struct_name`
-        if not file_prefix and not isinstance(self, NVT_NH):
-            self.file_prefix = (
-                f"{self.struct_name}-{self.ensemble}-T{self.temp}-p{self.pressure}"
-            )
-            if not kwargs.get("stats_file"):
-                self.stats_file = ""
-            if not kwargs.get("traj_file"):
-                self.traj_file = ""
-            if not kwargs.get("restart_stem"):
-                self.restart_stem = ""
-            self.configure_filenames()
-
         self.dyn = ASE_NPT(
             self.struct,
             timestep=self.timestep,
             temperature_K=self.temp,
             ttime=self.ttime,
             pfactor=pfactor,
             append_trajectory=self.traj_append,
             externalstress=self.pressure * units.bar,
         )
 
+    @property
+    def _parameter_prefix(self) -> str:
+        """
+        Ensemble parameters for output files.
+
+        Returns
+        -------
+        str
+           Formatted temperature range if heating and target temp if running md.
+        """
+
+        pressure = f"-p{self.pressure}" if not isinstance(self, NVT_NH) else ""
+        return f"{super()._parameter_prefix}{pressure}"
+
+    @property
+    def _final_file(self) -> str:
+        """
+        Final state file name.
+
+        Returns
+        -------
+        str
+           File name for final state, includes pressure.
+        """
+
+        pressure = f"-p{self.pressure}" if not isinstance(self, NVT_NH) else ""
+        if not self.restart_stem:
+            return f"{self.file_prefix}-T{self.temp}{pressure}-final.xyz"
+        return f"{self.restart_stem}-T{self.temp}{pressure}-final.xyz"
+
+    @property
+    def _restart_file(self) -> str:
+        """
+        Restart file name.
+
+        Returns
+        -------
+        str
+           File name for restart file, includes pressure.
+        """
+        step = self.offset + self.dyn.nsteps
+        pressure = f"-p{self.pressure}" if not isinstance(self, NVT_NH) else ""
+        if not self.restart_stem:
+            return f"{self.file_prefix}-T{self.temp}{pressure}-res-{step}.xyz"
+        return f"{self.restart_stem}-T{self.temp}{pressure}-res-{step}.xyz"
+
     def get_log_stats(self) -> str:
         """
         Get thermodynamical statistics to be written to molecular dynamics log.
 
         Returns
         -------
         str
```

### Comparing `janus_core-0.2.0b6/janus_core/mlip_calculators.py` & `janus_core-0.3.0b1/janus_core/helpers/mlip_calculators.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Similar in spirit to matcalc and quacc approaches
 - https://github.com/materialsvirtuallab/matcalc
 - https://github.com/Quantum-Accelerators/quacc.git
 """
 
 from ase.calculators.calculator import Calculator
 
-from .janus_types import Architectures, Devices
+from janus_core.helpers.janus_types import Architectures, Devices
 
 
 def choose_calculator(
     architecture: Architectures = "mace",
     device: Devices = "cpu",
     **kwargs,
 ) -> Calculator:
```

### Comparing `janus_core-0.2.0b6/janus_core/single_point.py` & `janus_core-0.3.0b1/janus_core/calculations/single_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from pathlib import Path
 from typing import Any, Optional
 
 from ase import Atoms
 from ase.io import read, write
 from numpy import isfinite, ndarray
 
-from janus_core.janus_types import (
+from janus_core.helpers.janus_types import (
     Architectures,
     ASEReadArgs,
     ASEWriteArgs,
     CalcResults,
     Devices,
     MaybeList,
     MaybeSequence,
 )
-from janus_core.log import config_logger
-from janus_core.mlip_calculators import choose_calculator
-from janus_core.utils import none_to_dict
+from janus_core.helpers.log import config_logger
+from janus_core.helpers.mlip_calculators import choose_calculator
+from janus_core.helpers.utils import none_to_dict
 
 
 class SinglePoint:
     """
     Prepare and perform single point calculations.
 
     Parameters
```

### Comparing `janus_core-0.2.0b6/janus_core/utils.py` & `janus_core-0.3.0b1/janus_core/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b6/pyproject.toml` & `janus_core-0.3.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-core"
-version = "0.2.0b6"
+version = "0.3.0b1"
 description = "Tools for machine learnt interatomic potentials"
 authors = [
     "Elliott Kasoar",
     "Federica Zanca",
     "Patrick Austin",
     "David Mason",
     "Jacob Wilkins",
@@ -19,21 +19,21 @@
     "Natural Language :: English",
     "Development Status :: 3 - Alpha",
 ]
 repository = "https://github.com/stfc/janus-core/"
 documentation = "https://stfc.github.io/janus-core/"
 
 [tool.poetry.scripts]
-janus = "janus_core.cli:app"
+janus = "janus_core.cli.janus:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ase = "^3.22.1"
 mace-torch = "^0.3.4"
-pyaml = "^23.12.0"
+pyyaml = "^6.0.1"
 typer = "^0.9.0"
 typer-config = "^1.4.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = "^7.4.1"}
 pgtest = "^1.3.2"
 pytest = "^8.0"
```

### Comparing `janus_core-0.2.0b6/PKG-INFO` & `janus_core-0.3.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-core
-Version: 0.2.0b6
+Version: 0.3.0b1
 Summary: Tools for machine learnt interatomic potentials
 Home-page: https://github.com/stfc/janus-core/
 Author: Elliott Kasoar
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ase (>=3.22.1,<4.0.0)
 Requires-Dist: mace-torch (>=0.3.4,<0.4.0)
-Requires-Dist: pyaml (>=23.12.0,<24.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: typer-config (>=1.4.0,<2.0.0)
 Project-URL: Documentation, https://stfc.github.io/janus-core/
 Project-URL: Repository, https://github.com/stfc/janus-core/
 Description-Content-Type: text/markdown
 
 [![Build Status][ci-badge]][ci-link]
@@ -142,14 +142,15 @@
 ```
 
 This will generate several output files:
 
 - Thermodynamical statistics every 100 steps, written to `NaCl-npt-T300.0-p1.0-stats.dat`
 - The structure trajectory every 100 steps, written to `NaCl-npt-T300.0-p1.0-traj.xyz`
 - The structure to be able to restart the dynamics every 1000 steps, written to `NaCl-npt-T300.0-p1.0-res-1000.xyz`
+- The final structure written to `NaCl-npt-T300.0-p1.0-final.xyz`
 - A log of the processes carried out, written to `md.log`
 - A summary of the inputs and start/end time, written to `md_summary.yml`.
 
 Additional options may be specified. For example:
 
 ```shell
 janus md --ensemble nvt --struct tests/data/NaCl.cif --steps 1000 --timestep 0.5 --temp 300 --minimize --minimize-every 100 --rescale-velocities --remove-rot --rescale-every 100 --equil-steps 200
@@ -172,24 +173,33 @@
 
 Run an NVT heating simultation from 20K to 300K in steps of 20K, with 10fs at each temperature:
 
 ```shell
 janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10
 ```
 
-This produces the same output files as an MD simulation.
+The produced statistics and trajectory files will indicate the heating range `NaCl-nvt-T20.0-T300.0-stats.dat`, `NaCl-nvt-T20.0-T300.0-traj.xyz`. There will also be final structure files at each temperature point:
 
-MD can also be carried out after heating using the same options as described in #molecular-dynamics. For example:
+```
+NaCl-nvt-T20.0-final.xyz
+NaCl-nvt-T40.0-final.xyz
+...
+NaCl-nvt-T300.0-final.xyz
+```
+
+MD can also be carried out after heating using the same options as described in [Molecular dynamics](#molecular-dynamics). For example:
 
 ```shell
 janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10 --steps 1000 --temp 300
 ```
 
 This performs the same initial heating, before running a further 1000 steps (1 ps) at 300K.
 
+When MD is run with heating the trajectory ```NaCl-nvt-T20.0-T300.0-T300.0-traj.xyz``` and statistics ```NaCl-nvt-T20.0-T300.0-T300.0-stats.dat``` files will indicate the heating range and MD temperature (which may be different). With heating and MD trajectories/statistics within the same files.
+
 
 ### Using configuration files
 
 Default values for all command line options may be specifed through a Yaml 1.1 formatted configuration file by adding the `--config` option. If an option is present in both the command line and configuration file, the command line value takes precedence.
 
 For example, with the following configuration file and command:
 
@@ -209,18 +219,14 @@
 
 This will run a singlepoint energy calculation on `KCl.cif` using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "medium" force-field, saving the results to `KCl-results.cif`.
 
 
 > [!NOTE]
 > `properties` must be passed as a Yaml list, as above, not as a string.
 
-> [!WARNING]
-> If an option in the configuration file does not match any variable names, an error will **not** be raised.
-> Please check the summary file to ensure the configuration has been read correctly.
-
 
 ## License
 
 [BSD 3-Clause License](LICENSE)
 
 ## Funding
```

