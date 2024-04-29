# Comparing `tmp/py50-0.3.6.tar.gz` & `tmp/py50-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py50-0.3.6.tar", max compression
+gzip compressed data, was "py50-1.0.0.tar", max compression
```

## Comparing `py50-0.3.6.tar` & `py50-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-0.3.6/LICENSE
--rw-r--r--   0        0        0     1155 2024-02-15 08:54:24.937954 py50-0.3.6/README_pypi.md
--rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-0.3.6/py50/.DS_Store
--rw-r--r--   0        0        0       74 2024-02-12 05:59:54.494113 py50-0.3.6/py50/__init__.py
--rw-r--r--   0        0        0    17368 2024-02-15 08:21:13.827892 py50-0.3.6/py50/calculator.py
--rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-0.3.6/py50/plot_settings.py
--rw-r--r--   0        0        0    41988 2024-02-15 08:21:23.602608 py50-0.3.6/py50/plotcurve.py
--rw-r--r--   0        0        0     1282 2024-02-12 07:57:00.462410 py50-0.3.6/py50/utils.py
--rw-r--r--   0        0        0      437 2024-02-15 08:57:48.759582 py50-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1847 1970-01-01 00:00:00.000000 py50-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4542 2024-04-29 03:50:21.000706 py50-1.0.0/README_pypi.md
+-rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.0/py50/.DS_Store
+-rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.0/py50/__init__.py
+-rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.0/py50/calculator.py
+-rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.0/py50/plot_settings.py
+-rw-r--r--   0        0        0    43456 2024-04-20 15:15:35.300736 py50-1.0.0/py50/plotcurve.py
+-rw-r--r--   0        0        0    88711 2024-04-29 03:02:08.739556 py50-1.0.0/py50/stats.py
+-rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.0/py50/utils.py
+-rw-r--r--   0        0        0      515 2024-04-29 01:15:06.686222 py50-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5335 1970-01-01 00:00:00.000000 py50-1.0.0/PKG-INFO
```

### Comparing `py50-0.3.6/LICENSE` & `py50-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py50-0.3.6/py50/.DS_Store` & `py50-1.0.0/py50/.DS_Store`

 * *Files identical despite different names*

### Comparing `py50-0.3.6/py50/calculator.py` & `py50-1.0.0/py50/calculator.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,67 +3,184 @@
 from scipy.optimize import curve_fit
 from scipy.interpolate import interp1d
 from py50.plot_settings import CurveSettings
 
 
 class Calculator:
     # Will accept input DataFrame and output said DataFrame for double checking.
-    def __init__(self, df):
-        if not isinstance(df, pd.DataFrame):
+    def __init__(self, data):
+        if not isinstance(data, pd.DataFrame):
             raise ValueError("Input must be a DataFrame")
-        self.df = df
+        self.data = data
+        self.calculation = None
 
-    def show(self):
+    def show(self, rows: int = None):
         """
         show DataFrame
 
+        :param rows: int
+            Indicate the number of rows to display. If none, automatically show 5.
         :return: DataFrame
         """
-        return self.df
 
-    def show_column(self, key):
+        if rows is None:
+            return self.data.head()
+        elif isinstance(rows, int):
+            return self.data.head(rows)
+
+    def show_column(self, key: str = None):
         """
         View specific column from DataFrame
 
-        :param key: column header name.
+        :param  key: String
+            Input column header. Must be a column header found in class input DataFrame.
 
         :return: DataFrame
         """
-        if key not in self.df.columns:
+        if key not in self.data.columns:
             raise ValueError("Column not found")
-        return self.df[key]
+        return self.data[key]
+
+    """Functions for calculations below"""
 
-    def unit_convert(self, ic50, x_intersection=None, input_units=None):
+    def calculate_ic50(
+        self,
+        name_col: str = None,
+        concentration_col: str = None,
+        response_col: str = None,
+        input_units: str = None,
+        verbose: bool = None,
+    ):
         """
-        Converts ic50 to desired input units for the plot_curve class
+        Calculations previously performed in relative_calculation(). The dictionary results are converted into into a
+        pandas DataFrame
 
-        :param ic50:
-        :param x_intersection: Corresponds to the absolute ic50 value. This is calculated from the curve_fit
-        :param input_units:
-        :return:
+        :param name_col: str
+            Name column from DataFrame
+        :param concentration_col: str
+            Concentration column from DataFrame
+        :param response_col: str
+            Response column from DataFrame
+        :param input_units: str
+            Units of input dataset. Default is nM.
+        :param verbose: bool
+            Output drug concentration units.
+
+        :return: DataFrame generated from the list from the relative_calculation method
+        """
+
+        # Set variables from function and convert name_col to np array
+        values = self._relative_calculation(
+            name_col, concentration_col, response_col, input_units, verbose
+        )
+
+        result_df = pd.DataFrame(values)
+
+        self.calculation = result_df
+        return self.calculation
+
+    def calculate_absolute_ic50(
+        self,
+        name_col: str = None,
+        concentration_col: str = None,
+        response_col: str = None,
+        input_units: str = None,
+        verbose: bool = None,
+    ):
+        """
+        Calculations previously performed in absolute_calculation(). The dictionary results are converted into a
+        pandas DataFrame
+
+        :param name_col: str
+            Name column from DataFrame
+        :param concentration_col: str
+            Concentration column from DataFrame
+        :param response_col: str
+            Response column from DataFrame
+        :param input_units: str
+            Units of input dataset. Default is nM.
+        :param verbose: bool
+            Output drug concentration units.
+
+        :return: DataFrame generated from the list from the absolute_calculation method
         """
-        # convert ic50 by input units
-        if input_units == "nM":
-            return ic50, x_intersection, input_units
-        elif input_units == "µM" or input_units == "uM":
-            ic50 = ic50 / 1000
-            if x_intersection is not None:
-                x_intersection = x_intersection / 1000
-            return ic50, x_intersection, input_units
-        elif input_units is None:
-            input_units = "nM"
-            return ic50, x_intersection, input_units
-        else:
-            print("Need nM (Nanomolar) or µM (Micromolar) concentrations!")
 
-    # Define the 4-parameter logistic (4PL) equation
+        values = self._absolute_calculation(
+            name_col=name_col,
+            concentration_col=concentration_col,
+            response_col=response_col,
+            input_units=input_units,
+            verbose=verbose,
+        )
+        result_df = pd.DataFrame(values)
+
+        self.calculation = result_df
+        return self.calculation
+
+    def calculate_pic50(
+        self,
+        name_col: str = None,
+        concentration_col: str = None,
+        response_col: str = None,
+        input_units: str = None,
+        verbose: bool = None,
+    ):
+        """
+        Convert IC50 into pIC50 values. Calculation is performed using the absolute_calculation. As such, two columns
+        will be appended - relative pIC50 and absolute pIC50. Conversion is performed by convert the IC50 values from nM
+        to M levels and then taking the negative log value of said number.
+
+        :param name_col: str
+            Name column from DataFrame
+        :param concentration_col: str
+            Concentration column from DataFrame
+        :param response_col: str
+            Response column from DataFrame
+        :param input_units: str
+            Units of input dataset. Default is nM.
+        :param verbose: bool
+            Output drug concentration units.
+
+        :return: DataFrame from calculate_absolute_ic50 along with the pIC50 values
+        """
+        values = self._absolute_calculation(
+            name_col=name_col,
+            concentration_col=concentration_col,
+            response_col=response_col,
+            input_units=input_units,
+            verbose=verbose,
+        )
+        result_df = pd.DataFrame(values)
+
+        if input_units is None or input_units == "nM":
+            result_df["relative pIC50"] = -np.log10(
+                result_df["relative ic50 (nM)"] * 0.000000001
+            )
+            result_df["absolute pIC50"] = -np.log10(
+                result_df["absolute ic50 (nM)"] * 0.000000001
+            )
+        elif input_units == "µM":
+            result_df["relative pIC50"] = -np.log10(
+                result_df["relative ic50 (µM)"] * 0.000001
+            )
+            result_df["absolute pIC50"] = -np.log10(
+                result_df["absolute ic50 (µM)"] * 0.000001
+            )
+
+        self.calculation = result_df
+        return self.calculation
+
+    """Support functions below"""
+
+    """Define the 4-parameter logistic (4PL) equation"""
+
     @staticmethod
-    def fourpl(concentration, minimum, maximum, ic50, hill_slope):
+    def _fourpl(concentration, minimum, maximum, ic50, hill_slope):
         """
-        Four-Parameter Logistic (4PL) Equation:
+        Four-Parameter Logistic (4PL) Equation for calculating curve fit:
 
 
         :param concentration: concentration
         :param minimum: minimum concentration in drug query (bottom plateau)
         :param maximum: maximum concentration for drug query (top plateau)
         :param ic50: Concentration at inflection point (where curve shifts from up or down)
         :param hill_slope: Steepness of hte curve (Hill Slope)
@@ -71,15 +188,15 @@
         :return: equation
         """
         return minimum + (maximum - minimum) / (
             1 + (concentration / ic50) ** hill_slope
         )
 
     @staticmethod
-    def reverse_fourpl(concentration, minimum, maximum, ic50, hill_slope):
+    def _reverse_fourpl(concentration, minimum, maximum, ic50, hill_slope):
         """
         Four-Parameter Logistic (4PL) Equation. This reverse function will graph the sigmoid curve from 100% to 0%
 
 
         :param concentration: concentration
         :param minimum: minimum concentration in drug query (bottom plateau)
         :param maximum: maximum concentration for drug query (top plateau)
@@ -88,102 +205,119 @@
 
         :return: equation
         """
         return minimum + (maximum - minimum) / (
             1 + (concentration / ic50) ** -hill_slope
         )
 
-    def verbose_calculation(self, drug, input_units, verbose):
+    def _verbose_calculation(
+        self, drug: str = None, input_units: str = None, verbose: bool = True
+    ):
         """
         Logic function to calculate unit concentration for Relative and Absolute IC50 calculation. Information will
-        detail drug name and concentration unit. Units available are nanomolar (nM) or micromolar (µM or uM).
+        detail drug name and concentration unit. Units available a
+        re nanomolar (nM) or micromolar (µM or uM).
 
-        :param drug: Input drug name.
-        :param input_units: Input drug concentration. Units available are nanomolar (nM) or micromolar (uM or µM)
-        :param verbose: Print out information regarding the concentration unit.
+        :param drug: str
+            Input drug name.
+        :param input_units: str
+            Input drug concentration. Units available are nanomolar (nM) or micromolar (uM or µM)
+        :param verbose: bool
+            Print out information regarding the concentration unit.
 
         :return: input_unit concentration
         """
+
         # Verbose conditions
         if verbose is True:
             # Logic to append concentration units to output DataFrame
             if input_units is None:
                 conc_unit = "nM"
             elif input_units == "uM" or input_units == "µM":
                 conc_unit = "µM"
             else:
                 conc_unit = input_units
             print(f"{drug} concentration is in {conc_unit}!")
 
     # This method will be used to reduce the functions in the calculating methods below.
     # This will loop through each drug item.
-    def relative_calculation(
-        self, name_col, concentration_col, response_col, input_units, verbose=None
+    def _relative_calculation(
+        self,
+        name_col: str = None,
+        concentration_col: str = None,
+        response_col: str = None,
+        input_units: str = None,
+        verbose: bool = None,
     ):
         """
         Calculate relative IC50 values for a given drug. Output will be a dictionary that will be converted into a
         pandas dataframe using the calculate_ic50() function.
 
-        :param name_col: Name column from DataFrame.
-        :param concentration_col: Concentration column from DataFrame.
-        :param response_col: Response column from DataFrame.
-        :param input_units: Concentration units for tested drug. By default, units given will be in nM.
-        :param verbose: Output drug concentration units.
+        :param name_col: str
+            Name column from DataFrame.
+        :param concentration_col: str
+            Concentration column from DataFrame.
+        :param response_col: str
+            Response column from DataFrame.
+        :param input_units: str
+            Concentration units for tested drug. By default, units given will be in nM.
+        :param verbose: bool
+            Output drug concentration units.
 
         :return: A dictionary containing drug name, maximum response, minimum response, IC50 (relative) and hill slope.
         """
-        # Set variables from funtion and convert name_col to np array
+        # Set variables from function and convert name_col to np array
         global params, conc_unit
         name_col = name_col
-        name = self.df[name_col].values
+        name = self.data[name_col].values
 
         drug_name = np.unique(name)
 
         values = []
 
         # Loop through each drug name and perform calculation
         for drug in drug_name:
-            drug_query = self.df[self.df[name_col] == drug]
+            drug_query = self.data[self.data[name_col] == drug]
             concentration = drug_query[concentration_col]
             response = drug_query[response_col]
 
             # Set initial guess for 4PL equation
             initial_guess = [
                 max(response),
                 min(response),
-                1.0,
+                0.5 * (max(response) + min(response)),
                 1.0,
             ]  # Max, Min, ic50, and hill_slope
 
             # set a new coy of the DataFrame to avoid warnings
             query = drug_query.copy()
             query.sort_values(by=concentration_col, inplace=True)
 
             # todo Calculate standard deviations from the covariance matrix
             # std_dev = np.sqrt(np.diag(covariance))
 
             # tag response col to determine direction of fourpl equation and fit to 4PL equation
-            reverse, params, covariance = self.calc_logic(
-                df=query,
+            reverse, params, covariance = self._calc_logic(
+                data=query,
                 concentration=concentration,
                 response_col=response_col,
                 initial_guess=initial_guess,
                 response=response,
             )
 
             # If verbose, output info
-            self.verbose_calculation(drug, input_units, verbose)
+            self._verbose_calculation(drug, input_units, verbose)
 
             # Extract parameter values
             maximum, minimum, ic50, hill_slope = params
             # print(drug, ' IC50: ', ic50, f'{input_units}') # For checking
 
             # Confirm ic50 unit output
             # x_intersection is not needed for relative ic50
-            ic50, x_intersection, input_units = self.unit_convert(
+            ic50, x_intersection, input_units = self._unit_convert(
                 ic50, x_intersection=None, input_units=input_units
             )
 
             # Logic to append concentration units to output DataFrame
             if input_units is None:
                 conc_unit = "nM"
             elif input_units == "nM":
@@ -199,43 +333,53 @@
                     "minimum": minimum,
                     f"ic50 ({conc_unit})": ic50,
                     "hill_slope": hill_slope,
                 }
             )
         return values
 
-    def absolute_calculation(
-        self, name_col, concentration_col, response_col, input_units, verbose=None
+    def _absolute_calculation(
+        self,
+        name_col: str = None,
+        concentration_col: str = None,
+        response_col: str = None,
+        input_units: str = None,
+        verbose: bool = None,
     ):
         """
         Calculate relative IC50 values for a given drug. Output will be a dictionary that will be converted into a
         pandas dataframe using the calculate_absolute_ic50() function.
 
-        :param name_col: Name column from DataFrame
-        :param concentration_col: Concentration column from DataFrame
-        :param response_col: Response column from DataFrame
-        :param input_units: Concentration units for tested drug. By default, units given will be in nM.
-        :param verbose:  Output drug concentration units.
+        :param name_col: str
+            Name column from DataFrame.
+        :param concentration_col: str
+            Concentration column from DataFrame.
+        :param response_col: str
+            Response column from DataFrame.
+        :param input_units: str
+            Concentration units for tested drug. By default, units given will be in nM.
+        :param verbose: bool
+            Output drug concentration units.
 
         :return: A dictionary containing drug name, maximum response, minimum response, relative IC50,
          absolute IC50, and hill slope.
         """
 
-        # Set variables from funtion and convert name_col to np array
+        # Set variables from function and convert name_col to np array
         global params, conc_unit
         name_col = name_col
-        name = self.df[name_col].values
+        name = self.data[name_col].values
 
         drug_name = np.unique(name)
 
         values = []
 
         # Loop through each drug name and perform calculation
         for drug in drug_name:
-            drug_query = self.df[self.df[name_col] == drug]
+            drug_query = self.data[self.data[name_col] == drug]
             concentration = drug_query[concentration_col]
             response = drug_query[response_col]
 
             # Set initial guess for 4PL equation
             initial_guess = [
                 max(response),
                 min(response),
@@ -243,16 +387,16 @@
                 1.0,
             ]  # Max, Min, ic50, and hill_slope
 
             # set a new coy of the DataFrame to avoid warnings
             query = drug_query.copy()
             query.sort_values(by=concentration_col, ascending=True, inplace=True)
 
-            reverse, params, covariance = self.calc_logic(
-                df=query,
+            reverse, params, covariance = self._calc_logic(
+                data=query,
                 concentration=concentration,
                 response_col=response_col,
                 initial_guess=initial_guess,
                 response=response,
             )
 
             # If verbose, output info
@@ -267,35 +411,25 @@
             x_fit, input_units = CurveSettings().scale_units(
                 drug_name=drug,
                 xscale_unit=input_units,
                 xscale_ticks=None,
                 verbose=verbose,
             )
 
-            # Calculate from parameters 4PL equation
-            if reverse == 1:
-                y_fit = self.reverse_fourpl(x_fit, maximum, minimum, ic50, hill_slope)
-                y_intersection = 50
-                interpretation = interp1d(
-                    y_fit, x_fit, kind="linear", fill_value="extrapolate"
+            hill_slope, ic50, input_units, x_intersection, y_fit = (
+                self._reverse_absolute_calculation(
+                    hill_slope,
+                    ic50,
+                    input_units,
+                    maximum,
+                    minimum,
+                    params,
+                    reverse,
+                    x_fit,
                 )
-                x_intersection = np.round(
-                    interpretation(y_intersection), 3
-                )  # give results and round to 3 sig figs
-                hill_slope = (
-                    -1 * hill_slope
-                )  # ensure hill_slope is negative # may not be needed if fixed
-            else:
-                y_fit = self.fourpl(x_fit, *params)
-                y_intersection = 50
-                x_intersection = np.interp(y_intersection, y_fit, x_fit)
-
-            # Confirm ic50 unit output
-            ic50, x_intersection, input_units = self.unit_convert(
-                ic50, x_intersection, input_units
             )
 
             # Logic to append concentration units to output DataFrame
             if input_units is None:
                 conc_unit = "nM"
             elif input_units == "nM":
                 conc_unit = "nM"
@@ -311,140 +445,117 @@
                     f"relative ic50 ({conc_unit})": ic50,
                     f"absolute ic50 ({conc_unit})": x_intersection,
                     "hill_slope": hill_slope,
                 }
             )
         return values
 
+    def _reverse_absolute_calculation(
+        self, hill_slope, ic50, input_units, maximum, minimum, params, reverse, x_fit
+    ):
+        """
+        Support function to condense code. Script will allow the generation of reverse curves.
+        """
+        # Calculate from parameters 4PL equation
+        if reverse == 1:
+            y_fit = self._reverse_fourpl(x_fit, maximum, minimum, ic50, hill_slope)
+            y_intersection = 50
+            interpretation = interp1d(
+                y_fit, x_fit, kind="linear", fill_value="extrapolate"
+            )
+            x_intersection = np.round(
+                interpretation(y_intersection), 3
+            )  # give results and round to 3 sig figs
+            hill_slope = (
+                -1 * hill_slope
+            )  # ensure hill_slope is negative # may not be needed if fixed
+        else:
+            y_fit = self._fourpl(x_fit, *params)
+            y_intersection = 50
+            x_intersection = np.interp(y_intersection, y_fit, x_fit)
+        # Confirm ic50 unit output
+        ic50, x_intersection, input_units = self._unit_convert(
+            ic50, x_intersection, input_units
+        )
+        return hill_slope, ic50, input_units, x_intersection, y_fit
+
     # When data is reversed, program is not obtaining correct column.
-    def calc_logic(
+    def _calc_logic(
         self,
-        df,
-        concentration=None,
-        initial_guess=None,
-        response=None,
-        response_col=None,
+        data: pd.DataFrame,
+        concentration: pd.Series = None,
+        initial_guess: list = None,
+        response: pd.Series = None,
+        response_col: str = None,
     ):
         """
         Set logic to determine positive or negative sigmoid curve. This method is called by internally by the
         absolute_calculation() method.
 
-        :param df: Input DataFrame. Must columns with drug name, tested concentration, and Response
-        :param concentration: The concentration column from input DataFrame.
-        :param initial_guess: The initial guesses for the 4PL equation.
-        :param response: The response column from the input Dataframe.
-        :param response_col: Name of the response column.
+        :param data: pd.DataFrame
+            Input DataFrame. Must columns with drug name, tested concentration, and Response
+        :param concentration: pd. Series
+            The concentration column from input DataFrame.
+        :param initial_guess: list
+            The initial guesses for the 4PL equation.
+        :param response: pd.Series
+            The response column from the input Dataframe.
+        :param response_col: str
+            Name of the response column.
 
         :return: variables for further calculation. This includes: reverse, params, covariance
         """
         global reverse, params, covariance
         if (
-            df[response_col].iloc[0] > df[response_col].iloc[-1]
+            data[response_col].iloc[0] > data[response_col].iloc[-1]
         ):  # Sigmoid curve 100% to 0%
             params, covariance, *_ = curve_fit(
-                self.reverse_fourpl,
+                self._reverse_fourpl,
                 concentration,
                 response,
                 p0=[initial_guess],
                 maxfev=100000,
             )
             reverse = 1  # Tag direction of sigmoid curve
 
         elif (
-            df[response_col].iloc[0] < df[response_col].iloc[-1]
+            data[response_col].iloc[0] < data[response_col].iloc[-1]
         ):  # sigmoid curve 0% to 100%
             params, covariance, *_ = curve_fit(
-                self.fourpl, concentration, response, p0=[initial_guess], maxfev=100000
+                self._fourpl, concentration, response, p0=[initial_guess], maxfev=100000
             )
             reverse = 0  # Tag direction of sigmoid curve
         return reverse, params, covariance
 
-    def calculate_ic50(
-        self, name_col, concentration_col, response_col, input_units=None, verbose=None
-    ):
-        """
-        Calculations previously performed in relative_calculation(). The dictionary results are converted into into a
-        pandas DataFrame
-
-        :param name_col: Name column from DataFrame
-        :param concentration_col: Concentration column from DataFrame
-        :param response_col: Response column from DataFrame
-        :param input_units:
-        :param verbose: Output drug concentration units.
-
-        :return: DataFrame generated from the list from the relative_calculation method
-        """
-
-        # Set variables from funtion and convert name_col to np array
-        values = self.relative_calculation(
-            name_col, concentration_col, response_col, input_units, verbose
-        )
-
-        df = pd.DataFrame(values)
-        return df
-
-    def calculate_absolute_ic50(
-        self, name_col, concentration_col, response_col, input_units=None, verbose=None
+    def _unit_convert(
+        self, ic50: int = None, x_intersection: int = None, input_units: str = None
     ):
         """
-        Calculations previously performed in absolute_calculation(). The dictionary results are converted into into a
-        pandas DataFrame
-
-        :param name_col: Name column from DataFrame
-        :param concentration_col: Concentration column from DataFrame
-        :param response_col: Response column from DataFrame
-        :param input_units: Concentration units for tested drug. By default, units given will be in nM.
-        :param verbose:  Output drug concentration units.
-
-        :return: DataFrame generated from the list from the absolute_calculation method
-        """
-
-        values = self.absolute_calculation(
-            name_col=name_col,
-            concentration_col=concentration_col,
-            response_col=response_col,
-            input_units=input_units,
-            verbose=verbose,
-        )
-        df = pd.DataFrame(values)
-
-        return df
-
-    def calculate_pic50(
-        self, name_col, concentration_col, response_col, input_units=None, verbose=None
-    ):
-        """
-        Convert IC50 into pIC50 values. Calculation is performed using the absolute_calculation. As such, two columns
-        will be appended - relative pIC50 and absolute pIC50. Conversion is performed by convert the IC50 values from nM
-        to M levels and then taking the negative log value of said number.
-
-        :param name_col: Name column from DataFrame
-        :param concentration_col: Concentration column from DataFrame
-        :param response_col: Response column from DataFrame
-        :param input_units: Concentration units for tested drug. By default, units given will be in nM.
-        :param verbose:  Output drug concentration units.
+        Converts ic50 to desired input units for the plot_curve class
 
-        :return: DataFrame from calculate_absolute_ic50 along with the pIC50 values
+        :param ic50: int
+            IC50 value for conversion. Obtained from the curve parameter values.
+        :param x_intersection: int
+            This value will correspond to the absolute ic50 value. This is calculated from the curve_fit.
+        :param input_units: str
+            Unites for the converted IC50 value. Only "nM" or "µM" are supported.
+        :return:
         """
-        values = self.absolute_calculation(
-            name_col=name_col,
-            concentration_col=concentration_col,
-            response_col=response_col,
-            input_units=input_units,
-            verbose=verbose,
-        )
-        df = pd.DataFrame(values)
-
-        if input_units is None or input_units == "nM":
-            df["relative pIC50"] = -np.log10(df["relative ic50 (nM)"] * 0.000000001)
-            df["absolute pIC50"] = -np.log10(df["absolute ic50 (nM)"] * 0.000000001)
-        elif input_units == "µM":
-            df["relative pIC50"] = -np.log10(df["relative ic50 (µM)"] * 0.000001)
-            df["absolute pIC50"] = -np.log10(df["absolute ic50 (µM)"] * 0.000001)
-
-        return df
+        # convert ic50 by input units
+        if input_units == "nM":
+            return ic50, x_intersection, input_units
+        elif input_units == "µM" or input_units == "uM":
+            ic50 = ic50 / 1000
+            if x_intersection is not None:
+                x_intersection = x_intersection / 1000
+            return ic50, x_intersection, input_units
+        elif input_units is None:
+            input_units = "nM"
+            return ic50, x_intersection, input_units
+        else:
+            print("Need to be in 'nM' (Nanomolar) or 'µM' (Micromolar) concentrations!")
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `py50-0.3.6/py50/plot_settings.py` & `py50-1.0.0/py50/plot_settings.py`

 * *Files identical despite different names*

### Comparing `py50-0.3.6/py50/plotcurve.py` & `py50-1.0.0/py50/plotcurve.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,145 +1,166 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.lines as mlines
-import pandas as pd
 import itertools
 from scipy.interpolate import interp1d
 from py50.plot_settings import CBMARKERS, CBPALETTE, CurveSettings
 from py50.calculator import Calculator
 
 
 class PlotCurve:
     # Will accept input DataFrame and output said DataFrame for double checking.
-    def __init__(self, df):
-        if not isinstance(df, pd.DataFrame):
-            raise ValueError("Input must be a DataFrame")
-        self.df = df
+    def __init__(self, data):
+        self.data = data
 
-    def show(self):
+    def show(self, rows: int = None):
         """
-        Show DataFrame
+        show DataFrame
 
+        :param rows: int
+            Indicate the number of rows to display. If none, automatically show 5.
         :return: DataFrame
         """
-        return self.df
 
-    def show_column(self, key):
-        """
-        View specific column from DataFrame
-
-        :param key: column header name.
-
-        :return: DataFrame
-        """
-
-        if key not in self.df.columns:
-            raise ValueError("Column not found")
-        return self.df[key]
+        if rows is None:
+            return self.data.head()
+        elif isinstance(rows, int):
+            return self.data.head(rows)
 
     # Filter input data based on Compound Name to generate single plot
-    def filter_dataframe(self, drug_name):
+    def _filter_dataframe(self, drug_name: str = None):
         """
         Filter input DataFrame by query drug name.
 
-        :param drug_name:
-
+        :param drug_name: str
+            Column name containing drug name.
         :return: DataFrame
         """
         # Filter row based on drug name input. Row must match drug name somewhere
-        filtered_df = self.df[self.df.apply(lambda row: drug_name in str(row), axis=1)]
+        filtered_df = self.data[
+            self.data.apply(lambda row: drug_name in str(row), axis=1)
+        ]
         return filtered_df
 
     # todo rename function to curve_plot
     # todo fix verbose issue - box info will also print
     def single_curve_plot(
         self,
-        concentration_col,
-        response_col,
-        drug_name=None,
-        plot_title=None,
-        plot_title_size=16,
-        xlabel=None,
-        ylabel=None,
-        axis_fontsize=14,
-        conc_unit="nM",
-        xscale="log",
-        xscale_ticks=None,
-        ymax=None,
-        ymin=None,
-        line_color="black",
-        line_width=1.5,
-        marker=None,
-        legend=False,
-        legend_loc="best",
-        box=False,
-        box_color="gray",
-        box_intercept=50,
-        conc_target=None,
-        hline=None,
-        hline_color="gray",
-        vline=None,
-        vline_color="gray",
-        figsize=(6.4, 4.8),
-        output_filename=None,
-        verbose=None,
+        concentration_col: str = None,
+        response_col: str = None,
+        drug_name: str = None,
+        plot_title: str = None,
+        plot_title_size: int = 16,
+        xlabel: str = None,
+        ylabel: str = None,
+        axis_fontsize: int = 14,
+        conc_unit: str = "nM",
+        xscale: str = "log",
+        xscale_ticks: tuple = None,
+        ymax: int = None,
+        ymin: int = None,
+        line_color: str = "black",
+        line_width: int = 1.5,
+        marker: bool = None,
+        legend: bool = False,
+        legend_loc: str = "best",
+        box: bool = False,
+        box_color: str = "gray",
+        box_intercept: int = 50,
+        conc_target: int = None,
+        hline: int = None,
+        hline_color: str = "gray",
+        vline: int = None,
+        vline_color: str = "gray",
+        figsize: tuple = (6.4, 4.8),
+        output_filename: str = None,
+        verbose: bool = None,
         **kwargs,
     ):
         """
         Generate a dose-response curve for a single drug target. Because a data table can contain multiple drugs, user
         must specify specific target.
 
-        :param concentration_col: Concentration column from DataFrame
-        :param response_col: Response column from DataFrame
-        :param drug_name: Name of drug for plotting
-        :param plot_title: Title of the figure
-        :param plot_title_size: Modify plot title font size
-        :param xlabel: Title of the X-axis
-        :param ylabel: Title of the Y-axis
-        :param axis_fontsize: Modify axis label font size
-        :param conc_unit: Input unit of concentration. Can accept nanomolar (nM) and micromolar (uM or µM). If the \
+        :param concentration_col: str
+            Concentration column from DataFrame
+        :param response_col: str
+            Response column from DataFrame
+        :param drug_name: str
+            Column containing drug name for plotting
+        :param plot_title: str
+            Title of the figure
+        :param plot_title_size: tuple
+            Modify plot title font size
+        :param xlabel: str
+            Title of the X-axis
+        :param ylabel: str
+            Title of the Y-axis
+        :param axis_fontsize: int
+            Modify axis label font size
+        :param conc_unit: str
+            Input unit of concentration. Can accept nanomolar (nM) and micromolar (uM or µM). If the \
         units are different, for example in the DataFrame units are in nM, but the units for the graph are µM, the \
         units from the DataFrame will be converted to match the conc_unit input. The final plot will scale based on \
         the conc_unit input. By default, it will assume input concentration will be in nM.
-        :param xscale: Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
-        :param xscale_ticks: Set the scale of the X-axis
-        :param ymax: Give a set maximum limit for the Y-Axis
-        :param ymin: Give a set minimum limit for the Y-Axis
-        :param line_color: Optional. Takes a list of colors. By default, it uses the CBPALETTE. List can contain name \
-        of colors or colors in hex code.
-        :param line_width: Set width of lines in plot.
-        :param marker: Optional. Takes a list of for point markers.
-        :param legend: Optional. Denotes a figure legend.
-        :param legend_loc: Determine legend location. Default is best. Matplotlib options can be found here \
+        :param xscale: int
+            Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
+        :param xscale_ticks: tuple
+            Set the scale of the X-axis
+        :param ymax: int
+            Give a set maximum limit for the Y-Axis
+        :param ymin: int
+            Give a set minimum limit for the Y-Axis
+        :param line_color: str.
+            Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of colors or colors in hex\
+        code.
+        :param line_width: int
+            Set width of lines in plot.
+        :param marker: Optional, list
+            Takes a list of for point markers.
+        :param legend: Optional, bool
+            Denotes a figure legend.
+        :param legend_loc: str
+        Determine legend location. Default is best. Matplotlib options can be found here \
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
-        :param box: Optional. Draw a box to highlight a specific location. If box = True, then the box_color, \
+        :param box: Optional bool.
+            Draw a box to highlight a specific location. If box = True, then the box_color, \
         box_intercept, and x_concentration MUST ALSO BE GIVEN.
-        :param box_color: Set color of box. Default is gray.
-        :param box_intercept: Set horizontal location of box. By default, it is set at 50% of the Y-axis.
-        :param conc_target: Set vertical location of the box. By default, this is set to None. For example, if the \
+        :param box_color: str
+            Set color of box. Default is gray.
+        :param box_intercept: int
+            Set horizontal location of box. By default, it is set at 50% of the Y-axis.
+        :param conc_target: int
+            Set vertical location of the box. By default, this is set to None. For example, if the \
         box_intercept is set to 50%, then the x_concentration must be the Absolute IC50 value. If there is an input to \
         x_concentration, it will override the box_intercept and the response data will move accordingly. Finally, the \
         number must be in the same unit as the X-axis. i.e., if the axis is in µM, then the number for the \
         x_concentration should be in µM and vice versa.
-        :param hline: Int or float for horizontal line. This line will stretch across the length of the plot. This is \
+        :param hline: Int or float
+            Draw a horizontal line across the graph. This line will stretch across the length of the plot. This is \
         optional and set to 0 by default.
-        :param hline_color: Set color of horizontal line. Default color is gray.
-        :param vline: This line will stretch across the height of the plot. This is  optional and set to 0 by default.
-        :param vline_color: Set color of vertical line. Default color is gray.
-        :param figsize: Set figure size.
-        :param output_filename: File path for save location.
-        :param verbose: Output information about the plot.
+        :param hline_color: str
+            Set color of horizontal line. Default color is gray.
+        :param vline: int or float
+            This line will stretch across the height of the plot. This is  optional and set to 0 by default.
+        :param vline_color: str
+            Set color of vertical line. Default color is gray.
+        :param figsize: tuple
+            Set figure size.
+        :param output_filename: str
+            File path for save location.
+        :param verbose: bool
+            Output information about the plot.
 
 
         :return: Figure
         """
 
         global x_fit, drug_query, y_intersection, x_intersection, reverse
         if drug_name is not None:
-            drug_query = self.filter_dataframe(drug_name=drug_name)
+            drug_query = self._filter_dataframe(drug_name=drug_name)
             if len(drug_query) > 0:
                 pass
             elif len(drug_query) == 0:
                 print("Drug not found!")
         else:
             print("Drug not found!")
 
@@ -172,55 +193,50 @@
         )
 
         # Function to scale the concentration by nM or µM
         concentration = CurveSettings().conc_scale(
             xscale_unit, concentration, verbose=verbose
         )
 
-        reverse, params, covariance = calculator.calc_logic(
-            df=query,
+        reverse, params, covariance = calculator._calc_logic(
+            data=query,
             concentration=concentration,
             response_col=response_col,
             initial_guess=initial_guess,
             response=response,
         )
         # Extract parameter values
         maximum, minimum, ic50, hill_slope = params
         # print(drug_name, ' IC50: ', ic50, 'µM') # For checking
 
-        # todo extract into a method
-        # Calculate from parameters 4PL equation
-        if reverse == 1:
-            y_fit = calculator.reverse_fourpl(x_fit, maximum, minimum, ic50, hill_slope)
-            y_intersection = 50
-            interpretation = interp1d(
-                y_fit, x_fit, kind="linear", fill_value="extrapolate"
+        hill_slope, ic50, final_unit, x_intersection, y_fit = (
+            calculator._reverse_absolute_calculation(
+                hill_slope,
+                ic50,
+                conc_unit,
+                maximum,
+                minimum,
+                params,
+                reverse,
+                x_fit,
             )
-            x_intersection = np.round(
-                interpretation(y_intersection), 3
-            )  # give results and round to 3 sig figs
-            hill_slope = (
-                -1 * hill_slope
-            )  # ensure hill_slope is negative # may not be needed if fixed
-        else:
-            y_fit = calculator.fourpl(x_fit, *params)
-            y_intersection = 50
-            x_intersection = np.interp(y_intersection, y_fit, x_fit)
-
-        # Confirm ic50 unit output
-        ic50, x_intersection, final_unit = calculator.unit_convert(
-            ic50, x_intersection, conc_unit
         )
 
         # Boolean check for marker
         if marker is not None:
             marker = marker
         else:
             marker = "o"
 
+        # Check for xscale label:
+        if xscale == "log" or xscale == "linear":
+            pass
+        else:
+            raise ValueError("xscale must be 'log' or 'linear'")
+
         # Create the plot
         fig, ax = plt.subplots(figsize=figsize)
         ax.set_ylim(top=100)  # Set maximum y axis limit
         ax.scatter(concentration, response, marker=marker, color=line_color)
         ax.plot(x_fit, y_fit, color=line_color, linewidth=line_width)
         ax.set_xscale(xscale)  # Use a logarithmic scale for the x-axis
         ax.set_xlabel(xlabel, fontsize=axis_fontsize)
@@ -248,17 +264,14 @@
                 min_value = min_value - 5
             else:
                 min_value = 0
         else:
             min_value = ymin
         ax.set_ylim(min_value, max_value)
 
-        # todo change box_intercept is None to box
-        # todo Only print the Box X and Y intersection if Box is True
-        # todo nest additional if/else statement for box_intercept to match input accordingly
         # Plot box to IC50 on curve
         # Interpolate to find the x-value (Concentration) at the intersection point
         if box_intercept is None:
             print("Input Inhibition % target")
         elif box_intercept and conc_target is None and reverse == 1:
             y_intersection = box_intercept
             interpretation = interp1d(
@@ -321,97 +334,123 @@
         else:
             plt.savefig(
                 output_filename, dpi=300
             )  # Save the plot to a file with the specified filename
 
         return fig
 
-    # todo include conc_target from single_curve_plot
-    # todo include axis_fontsize as seen from other 2 plots
     def multi_curve_plot(
         self,
-        concentration_col,
-        response_col,
-        name_col,
-        plot_title=None,
-        plot_title_size=12,
-        xlabel=None,
-        ylabel=None,
-        conc_unit="nM",
-        xscale="log",
-        xscale_ticks=None,
-        ymax=None,
-        ymin=None,
-        axis_fontsize=10,
-        line_color=CBPALETTE,
-        marker=CBMARKERS,
-        line_width=1.5,
-        legend=False,
-        legend_loc="best",
-        box_target=None,
-        box_color="gray",
-        box_intercept=50,
-        hline=None,
-        hline_color="gray",
-        vline=None,
-        vline_color="gray",
-        figsize=(6.4, 4.8),
-        output_filename=None,
-        verbose=None,
+        concentration_col: str = None,
+        response_col: str = None,
+        name_col: str = None,
+        plot_title: str = None,
+        plot_title_size: int = 12,
+        xlabel: str = None,
+        ylabel: str = None,
+        conc_unit: str = "nM",
+        xscale: str = "log",
+        xscale_ticks: tuple = None,
+        ymax: int = None,
+        ymin: int = None,
+        axis_fontsize: int = 10,
+        line_color: list = CBPALETTE,
+        marker: list = CBMARKERS,
+        line_width: int = 1.5,
+        legend: bool = False,
+        legend_loc: str = "best",
+        box_target: str = None,
+        box_color: str = "gray",
+        box_intercept: int = 50,
+        hline: int = None,
+        hline_color: str = "gray",
+        vline: int = None,
+        vline_color: str = "gray",
+        figsize: tuple = (6.4, 4.8),
+        output_filename: str = None,
+        verbose: bool = None,
         **kwargs,
     ):
         """
         Generate a dose-response plot for multiple drug targets. Curves will be placed into a single plot.
 
-        :param concentration_col: Concentration column from DataFrame
-        :param response_col: Response column from DataFrame
-        :param name_col: Name column from DataFrame
-        :param plot_title: Title of the figure
-        :param plot_title_size: Modify plot title font size
-        :param xlabel: Title of the X-axis
-        :param ylabel: Title of the Y-axis
-        :param conc_unit: Input will assume that the concentration will be in nM. \
+        :param concentration_col: str
+            Concentration column from DataFrame
+        :param response_col: str
+            Response column from DataFrame
+        :param name_col:
+            Column containing name of drug from DataFrame
+        :param plot_title: str
+            Title of the figure
+        :param plot_title_size: int
+            Modify plot title font size
+        :param xlabel: str
+            Title of the X-axis
+        :param ylabel: str
+            Title of the Y-axis
+        :param conc_unit: str
+            Input will assume that the concentration will be in nM. \
         Thus, it will be automatically converted into µM. \
         If xscale_unit is given as nM, no conversion will be performed.
-        :param xscale: Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
-        :param xscale_ticks: Set the scale of the X-axis
-        :param ymax: Give a set maximum limit for the Y-Axis
-        :param ymin: Give a set minimum limit for the Y-Axis
-        :param axis_fontsize: Modify axis label font size
-        :param line_color: Optional. Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of \
+        :param xscale: str
+            Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
+        :param xscale_ticks: tuple
+            Set the scale of the X-axis
+        :param ymax: int
+            Give a set maximum limit for the Y-Axis
+        :param ymin: int
+            Give a set minimum limit for the Y-Axis
+        :param axis_fontsize:int
+            Modify axis label font size
+        :param line_color: str
+        Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of \
         colors or colors in hex code.
-        :param line_width: Set width of lines in plot.
-        :param marker: Optional. Takes a list for point markers. Marker options can be found here: \
+        :param line_width: int
+            Set width of lines in plot.
+        :param marker: list
+        Takes a list for point markers. Marker options can be found here: \
         https://matplotlib.org/stable/api/markers_api.html
-        :param legend: Optional. Denotes a figure legend.
-        :param legend_loc: Determine legend location. Matplotlib options can be found here \
+        :param legend: bool
+            Denotes a figure legend.
+        :param legend_loc: str
+            Determine legend location. Matplotlib options can be found here \
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
-        :param box_target: Optional. Draw a box to highlight a specific location.
-        :param box_color: Set color of box. Default color is gray.
-        :param box_intercept: Set horizontal location of box. By default, it is set at Absolute IC50.
-        :param hline: Int or float for horizontal line. This line will stretch across the length of the plot. This is \
+        :param box_target: str
+            Draw a box to highlight a specific drug curve. Must use specific drug name.
+        :param box_color: str
+            Set color of box. Default color is gray.
+        :param box_intercept: int
+            Set horizontal location of box. By default, it is set at Absolute IC50.
+        :param hline: int or float
+            Draw a horizontal line that will stretch across the length of the plot. This is \
         optional and set to 0 by default.
-        :param hline_color: Set color of horizontal line. Default color is gray.
-        :param vline: This line will stretch across the height of the plot. This is  optional and set to 0 by default.
-        :param vline_color: Set color of vertical line. Default color is gray.
-        :param figsize: Set figure size.
-        :param output_filename: File path for save location.
-        :param verbose: Output information about the plot.
+        :param hline_color: str
+            Set color of horizontal line. Default color is gray.
+        :param vline: int or float
+            Draw a line that will stretch across the height of the plot. This is  optional and set to 0 by default.
+        :param vline_color: str
+            Set color of vertical line. Default color is gray.
+        :param figsize: tuple
+            Set figure size.
+        :param output_filename: str
+            File path for save location.
+        :param verbose: bool
+            Output information about the plot.
 
         :return: Figure
         """
         global response, x_fit, y_fit, y_intersection, x_intersection, reverse, params
-        name_list = np.unique(self.df[name_col])
+        name_list = np.unique(self.data[name_col])
 
         concentration_list = []
         response_list = []
         y_fit_list = []
 
         for drug in name_list:
-            drug_query = self.filter_dataframe(drug)
+            drug_query = self._filter_dataframe(drug)
 
             # Create variables for inputs. Extract column from Dataframe
             concentration = drug_query[concentration_col]
             response = drug_query[response_col]
 
             # Set initial guess for 4PL equation
             initial_guess = [
@@ -439,28 +478,28 @@
             )
 
             # Function to scale the concentration by nM or µM
             concentration = CurveSettings().conc_scale(
                 xscale_unit, concentration, verbose=verbose
             )
 
-            reverse, params, covariance = calculator.calc_logic(
-                df=query,
+            reverse, params, covariance = calculator._calc_logic(
+                data=query,
                 concentration=concentration,
                 response_col=response_col,
                 initial_guess=initial_guess,
                 response=response,
             )
             # Extract parameter values
             maximum, minimum, ic50, hill_slope = params
             # print(drug, ' IC50: ', ic50, 'nM') # For checking
 
             # Calculate from parameters 4PL equation
             if reverse == 1:
-                y_fit = calculator.reverse_fourpl(
+                y_fit = calculator._reverse_fourpl(
                     x_fit, maximum, minimum, ic50, hill_slope
                 )
                 y_intersection = 50
                 interpretation = interp1d(
                     y_fit, x_fit, kind="linear", fill_value="extrapolate"
                 )
                 x_intersection = np.round(
@@ -468,15 +507,15 @@
                 )  # give results and round to 3 sig figs
                 hill_slope = (
                     -1 * hill_slope
                 )  # ensure hill_slope is negative # may not be needed if fixed
                 y_fit_list.append(y_fit)
 
             else:
-                y_fit = calculator.fourpl(x_fit, *params)
+                y_fit = calculator._fourpl(x_fit, *params)
                 y_intersection = 50
                 x_intersection = np.interp(y_intersection, y_fit, x_fit)
                 y_fit_list.append(y_fit)
 
             # This script is from single_curve_plot. It is not needed for multi-curve
             # Confirm ic50 unit output
             # ic50, x_intersection = calculator.unit_convert(ic50, x_intersection, conc_unit)
@@ -497,14 +536,20 @@
             line_color = line_color
 
         if marker is CBMARKERS:
             pass
         else:
             marker = marker
 
+        # Check for xscale label:
+        if xscale == "log" or xscale == "linear":
+            pass
+        else:
+            raise ValueError("xscale must be 'log' or 'linear'")
+
         # Plotting the data for each line
         legend_handles = (
             []
         )  # Store data for each line as a dictionary inside a list for the legend
         for i, (
             y_fit_point,
             concentration_point,
@@ -544,15 +589,15 @@
             # Append scatter plot handle to the legend
             legend_piece = {"marker": mark, "name": name, "line_color": color}
             legend_handles.append(legend_piece)
 
         # Set y-axis limit
         # Y-axis limit will be limited to the largest response number and add 10 for spacing
         if ymax is None:
-            max_y = self.df[response_col].max()
+            max_y = self.data[response_col].max()
             max_value = max_y + 10
         else:
             max_value = ymax
 
         if ymin is None:
             min_value = min(response)
             if min_value < 0:
@@ -562,15 +607,15 @@
         else:
             min_value = ymin
 
         ax.set_ylim(min_value, max_value)
 
         # Plot box to IC50 on curve
         # Interpolate to find the x-value (Concentration) at the intersection point
-        if box_intercept == None:
+        if box_intercept is None:
             y_intersection = 50
         else:
             y_intersection = box_intercept
 
         # Specify box target
         if box_target in name_list:
             if isinstance(box_target, str) and reverse == 1:
@@ -677,93 +722,116 @@
         if output_filename is None:
             pass
         else:
             plt.savefig(output_filename, dpi=300)
 
         return fig
 
-    # todo include conc_target from single_curve_plot
     def grid_curve_plot(
         self,
-        concentration_col,
-        response_col,
-        name_col,
-        column_num=2,
-        plot_title=None,
-        plot_title_size=20,
-        xlabel=None,
-        ylabel=None,
-        conc_unit="nM",
-        xscale="log",
-        xscale_ticks=None,
-        ymax=None,
-        ymin=None,
-        line_color=CBPALETTE,
-        line_width=1.5,
-        box=False,
-        box_color="gray",
-        box_intercept=50,
-        hline=None,
-        hline_color="gray",
-        vline=None,
-        vline_color="gray",
-        figsize=(8.4, 4.8),
-        output_filename=None,
-        verbose=None,
+        concentration_col: str = None,
+        response_col: str = None,
+        name_col: str = None,
+        column_num: int = 2,
+        plot_title: str = None,
+        plot_title_size: int = 20,
+        xlabel: str = None,
+        ylabel: str = None,
+        conc_unit: str = "nM",
+        xscale: str = "log",
+        xscale_ticks: tuple = None,
+        ymax: int = None,
+        ymin: int = None,
+        line_color: list = CBPALETTE,
+        line_width: int = 1.5,
+        box: bool = False,
+        box_color: str = "gray",
+        box_intercept: int = 50,
+        hline: int = None,
+        hline_color: str = "gray",
+        vline: int = None,
+        vline_color: str = "gray",
+        figsize: tuple = (8.4, 4.8),
+        output_filename: str = None,
+        verbose: bool = None,
         **kwargs,
     ):
         """
         Generate a dose-response curve for mutliple drugs. Each curve will be placed in its own plot which is then
         placed in a grid.
 
-        :param concentration_col: Concentration column from DataFrame
-        :param response_col: Response column from DataFrame
-        :param name_col: Name column from DataFrame
-        :param column_num: Set number of column grid
-        :param plot_title: Title of the figure
-        :param plot_title_size: Modify plot title font size
-        :param xlabel: Title of the X-axis
-        :param ylabel: Title of the Y-axis
-        :param ymax: Give a set maximum limit for the Y-Axis
-        :param ymin: Give a set minimum limit for the Y-Axis
-        :param conc_unit: Input will assume that the concentration will be in nM. \
-        Thus, it will be automatically converted into µM. \
+        :param concentration_col: str
+            Concentration column from DataFrame
+        :param response_col: str
+            Response column from DataFrame
+        :param name_col: str
+            Name column from DataFrame
+        :param column_num: int
+            Set number of column grid
+        :param plot_title: str
+            Title of the figure
+        :param plot_title_size: int
+            Modify plot title font size
+        :param xlabel:str
+            Title of the X-axis
+        :param ylabel: str
+            Title of the Y-axis
+        :param ymax: int
+            Give a set maximum limit for the Y-Axis
+        :param ymin: int
+            Give a set minimum limit for the Y-Axis
+        :param conc_unit: str
+            Input will assume that the concentration will be in nM. Thus, it will be automatically converted into µM. \
         If xscale_unit is given as nM, no conversion will be performed.
-        :param xscale: Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
-        :param xscale_ticks: Set the scale of the X-axis
-        :param line_color: Optional. Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of \
+        :param xscale: str
+            Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
+        :param xscale_ticks: tuple
+            Set the scale of the X-axis
+        :param line_color: list
+            Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of \
         colors or colors in hex code.
-        :param line_width: Set width of lines in plot.
-        :param box: Optional. Draw a box to highlight a specific location. If box = True, then the box_color, \
-        and box_intercept MUST ALSO BE GIVEN.
-        :param box_color: Set color of box. Default color is gray.
-        :param box_intercept: Set horizontal location of box. By default, it is set at Absolute IC50.
-        :param hline: Int or float for horizontal line. This line will stretch across the length of the plot. This is \
-        optional and set to 0 by default.
-        :param hline_color: Set color of horizontal line. Default color is gray.
-        :param vline: This line will stretch across the height of the plot. This is  optional and set to 0 by default.
-        :param vline_color: Set color of vertical line. Default color is gray.
-        :param figsize: Set figure size for subplot.
-        :param output_filename: File path for save location.
-        :param verbose: Output information about the plot.
+        :param line_width: int
+            Set width of lines in plot.
+        :param box: bool
+        Draw a box to highlight a specific location. If box = True, then the box_color, and box_intercept MUST ALSO BE \
+        GIVEN.
+        :param box_color: str
+            Set color of box. Default color is gray.
+        :param box_intercept: int
+            Set horizontal location of box. By default, it is set at Absolute IC50.
+        :param hline: int or float
+            Draw horizontal line that will stretch across the length of the plot. This is optional and set to 0 by \
+            default.
+        :param hline_color: str
+            Set color of horizontal line. Default color is gray.
+        :param vline: int or float
+            Draw a line thatwill stretch across the height of the plot. This is  optional and set to 0 by default.
+        :param vline_color: str
+            Set color of vertical line. Default color is gray.
+        :param figsize: tuple
+            Set figure size for subplot.
+        :param output_filename: str
+            File path for save location.
+        :param verbose: bool
+            Output information about the plot.
 
         :return: Figure
         """
 
         global x_fit, reverse, params, response, concentration
-        name_list = np.unique(self.df[name_col])
+        name_list = np.unique(self.data[name_col])
 
         # Generate lists for modifying plots (vline, box, etc)
         concentration_list = []
         response_list = []
         y_fit_list = []
         x_fit_list = []
 
         for drug in name_list:
-            drug_query = self.filter_dataframe(drug)
+            drug_query = self._filter_dataframe(drug)
 
             # Create variables for inputs. Extract column from Dataframe
             concentration = drug_query[concentration_col]
             response = drug_query[response_col]
 
             # Set initial guess for 4PL equation
             initial_guess = [
@@ -792,43 +860,43 @@
             x_fit_list.append(x_fit)
 
             # Function to scale the concentration by nM or µM
             concentration = CurveSettings().conc_scale(
                 xscale_unit, concentration, verbose=verbose
             )
 
-            reverse, params, covariance = calculator.calc_logic(
-                df=query,
+            reverse, params, covariance = calculator._calc_logic(
+                data=query,
                 concentration=concentration,
                 response_col=response_col,
                 initial_guess=initial_guess,
                 response=response,
             )
             # Extract parameter values
             maximum, minimum, ic50, hill_slope = params
             # print(drug, ' IC50: ', ic50, 'nM') # For checking
 
             # Calculate from parameters 4PL equation
             if reverse == 1:
-                y_fit = calculator.reverse_fourpl(
+                y_fit = calculator._reverse_fourpl(
                     x_fit, maximum, minimum, ic50, hill_slope
                 )
                 y_intersection = 50
                 interpretation = interp1d(
                     y_fit, x_fit, kind="linear", fill_value="extrapolate"
                 )
                 x_intersection = np.round(
                     interpretation(y_intersection), 3
                 )  # give results and round to 3 sig figs
                 hill_slope = (
                     -1 * hill_slope
                 )  # ensure hill_slope is negative # may not be needed if fixed
                 y_fit_list.append(y_fit)
             else:
-                y_fit = calculator.fourpl(x_fit, *params)
+                y_fit = calculator._fourpl(x_fit, *params)
                 y_intersection = 50
                 x_intersection = np.interp(y_intersection, y_fit, x_fit)
                 y_fit_list.append(y_fit)
 
             """Appended list will contain concentrations in nM or µM depending on user input"""
             # Append values for each drug into list
             concentration_for_list = concentration.values  # Convert into np.array
@@ -854,14 +922,20 @@
             # If user only gives a string of 1 color, duplicate color name to match length of drug names
             elif len(line_color) is not len(name_list):
                 line_color_list = tuple([line_color] * len(name_list))
                 line_color = line_color_list
         else:
             pass
 
+        # Check for xscale label:
+        if xscale == "log" or xscale == "linear":
+            pass
+        else:
+            raise ValueError("xscale must be 'log' or 'linear'")
+
         # Generate figure in grid layout
         # Calculate the number of rows needed
         num_plots = len(name_list)  # determine total plots to make
         row_num = -(-num_plots // column_num)  # Round up to the nearest integer
         # Squeeze to handle possible 1D array
         fig, axes = plt.subplots(row_num, column_num, figsize=figsize, squeeze=False)
         fig.suptitle(plot_title, fontsize=plot_title_size)
```

