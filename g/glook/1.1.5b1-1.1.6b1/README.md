# Comparing `tmp/glook-1.1.5b1-py3-none-any.whl.zip` & `tmp/glook-1.1.6b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 54315 bytes, number of entries: 18
+Zip file size: 55468 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat     3200 b- defN 24-Apr-24 16:04 glook/GLook.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 17:39 glook/__init__.py
 -rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-25 18:24 glook/cli.py
 -rw-rw-rw-  2.0 fat    25002 b- defN 24-Apr-10 10:33 glook/pages/10_Unsupervised_learning.py
 -rw-rw-rw-  2.0 fat    96985 b- defN 24-Apr-27 21:03 glook/pages/11_Custom_Model_Training.py
--rw-rw-rw-  2.0 fat     6170 b- defN 24-Apr-28 06:13 glook/pages/1_General_Data_Insights.py
+-rw-rw-rw-  2.0 fat     6157 b- defN 24-Apr-28 06:49 glook/pages/1_General_Data_Insights.py
 -rw-rw-rw-  2.0 fat    19725 b- defN 24-Apr-27 19:10 glook/pages/2_Univariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-24 16:05 glook/pages/3_Bivariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7707 b- defN 24-Apr-28 06:03 glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-  2.0 fat   130608 b- defN 24-Apr-27 20:33 glook/pages/5_Pre_Processing.py
+-rw-rw-rw-  2.0 fat   112037 b- defN 24-Apr-29 14:17 glook/pages/5_Pre_Processing.py
 -rw-rw-rw-  2.0 fat     3315 b- defN 24-Apr-27 20:41 glook/pages/6_Split_Data.py
 -rw-rw-rw-  2.0 fat     4588 b- defN 24-Apr-11 19:05 glook/pages/7_Dimensionality_Reduction.py
 -rw-rw-rw-  2.0 fat    59951 b- defN 24-Apr-27 20:43 glook/pages/8_Supervised_Learning.py
--rw-rw-rw-  2.0 fat     7141 b- defN 24-Apr-28 06:30 glook-1.1.5b1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 06:30 glook-1.1.5b1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-28 06:30 glook-1.1.5b1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-28 06:30 glook-1.1.5b1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1537 b- defN 24-Apr-28 06:30 glook-1.1.5b1.dist-info/RECORD
-18 files, 374268 bytes uncompressed, 51787 bytes compressed:  86.2%
+-rw-rw-rw-  2.0 fat     7241 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1537 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/RECORD
+18 files, 355784 bytes uncompressed, 52940 bytes compressed:  85.1%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: glook/pages/7_Dimensionality_Reduction.py
 Comment: 
 
 Filename: glook/pages/8_Supervised_Learning.py
 Comment: 
 
-Filename: glook-1.1.5b1.dist-info/METADATA
+Filename: glook-1.1.6b1.dist-info/METADATA
 Comment: 
 
-Filename: glook-1.1.5b1.dist-info/WHEEL
+Filename: glook-1.1.6b1.dist-info/WHEEL
 Comment: 
 
-Filename: glook-1.1.5b1.dist-info/entry_points.txt
+Filename: glook-1.1.6b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: glook-1.1.5b1.dist-info/top_level.txt
+Filename: glook-1.1.6b1.dist-info/top_level.txt
 Comment: 
 
-Filename: glook-1.1.5b1.dist-info/RECORD
+Filename: glook-1.1.6b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## glook/pages/1_General_Data_Insights.py

```diff
@@ -123,15 +123,15 @@
 				]
 			)
 			.highlight_max(axis=0, props='background-color: darkgreen; color: white;')  # Highlight max values with specific color
 			.highlight_min(axis=0, props='background-color: yellowgreen; color: black;')  # Highlight min values with another color
 			# .format("{:.2f}")
 		)
 
-		st.dataframe(styled_df_info1, width = 720)
+		st.dataframe(styled_df_info1)
 	except ValueError:
 		st.dataframe()
 	# Display the insights
 	st.subheader(f"Data dimensions: :green[{num_rows} rows, {num_columns} columns]")
 	st.subheader(f"Number of rows: :green[{num_rows}]")
 	st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
 	st.subheader(f"Deep Memory usage: :green[{memory_usage:.3f} MB]")
```

## glook/pages/5_Pre_Processing.py

```diff
@@ -1,3049 +1,3395 @@
-# page2.py
 import streamlit as st
-st.set_page_config(
-		page_title="ML-Automation", 
-		page_icon="🏗️", 
-		layout="wide", 
-		initial_sidebar_state = "expanded")
-
+st.set_page_config(page_title='ML-Automation', page_icon='🏗️', layout=
+	'wide', initial_sidebar_state='expanded')
+print(1)
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 import plotly.express as px
 import plotly.graph_objects as go
 import numpy as np
 import statsmodels.api as sm
+# st.set_option('deprecation.showPyplotGlobalUse', False)
 st.set_option('deprecation.showPyplotGlobalUse', False)
-# from wordcloud import WordCloud
+print(2)
 from scipy.stats.mstats import winsorize
 from sklearn.impute import SimpleImputer
 from scipy.stats import boxcox, yeojohnson
 from sklearn.preprocessing import OneHotEncoder, LabelEncoder, KBinsDiscretizer
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
-# import matplotlib.pyplot as plt
-# import matplotlib
-# matplotlib.use('TkAgg')
-# st.title("1️⃣Univariate Analysis")
+import joblib
 Confirm_Change = False
+
+
 def limit_unique_values(series, limit=20):
 	if series.nunique() > limit:
 		top_categories = series.value_counts().index[:limit]
 		return series.apply(lambda x: x if x in top_categories else 'Other')
 	else:
 		return series
 
+
 def limit_unique_values_cloud(series, limit=200):
 	if series.nunique() > limit:
 		top_categories = series.value_counts().index[:limit]
 		return top_categories
 	else:
 		return series.unique()
 
-# def limit_unique_values_cloud(series, limit=200):
-# 	if series.nunique() > limit:
-# 		top_categories = series.value_counts().index[:limit]
-# 		return series.apply(lambda x: x if x in top_categories else 'Other')
-# 	else:
-# 		return series
+
 def change_dtype(df, column_name, new_dtype):
 	try:
 		df[column_name] = pd.to_numeric(df[column_name], errors='coerce')
 		df[column_name] = df[column_name].astype(new_dtype)
-		# st.success(f"Successfully changed data type of column '{column_name}' to {new_dtype}.")
-		st.warning(f"Data type of column '{column_name}' changed to {new_dtype}, but these changes won't be saved until you press the 'Confirm Changes' button below.")
+		st.warning(
+			f"Data type of column '{column_name}' changed to {new_dtype}, but these changes won't be saved until you press the 'Confirm Changes' button below."
+			)
+		print(3)
 	except Exception as e:
-		st.warning("Select Proper Column")
-		st.error(f"Error occurred: {e}")
+		st.warning('Select Proper Column')
+		print(4)
+		st.error(f'Error occurred: {e}')
+		print(5)
+
 
-# Function to preprocess column by dropping it
 def drop_column(df, column_name):
 	try:
 		df.drop(column_name, axis=1, inplace=True)
+		print(6)
 		st.warning(
 			f"Column '{column_name}' has been dropped, but changes won't be saved until you press the 'Confirm Changes' button below."
-		)
+			)
+		print(7)
 	except Exception as e:
-		st.error(f"Error occurred: {e}")
+		st.error(f'Error occurred: {e}')
+		print(8)
+
 
-# Function to preprocess by dropping duplicates
 def drop_duplicates(df):
 	try:
 		original_rows = len(df)
 		df.drop_duplicates(inplace=True)
+		print(9)
 		new_rows = len(df)
-		st.warning(f"Dropped {original_rows - new_rows} duplicate rows, but changes will not be saved until you press the 'Confirm Changes' button below.")
+		st.warning(
+			f"Dropped {original_rows - new_rows} duplicate rows, but changes will not be saved until you press the 'Confirm Changes' button below."
+			)
+		print(10)
 	except Exception as e:
-		st.error(f"Error occurred: {e}")
+		st.error(f'Error occurred: {e}')
+		print(11)
 
 
-# Function to preprocess by treating outliers
-def treat_outliers(df, column_name, method):
+def treat_outliers(df, column_name, method, z_score_threshold, lower_limit,
+	upper_limit):
 	try:
-		if method == "Delete Outliers":
-			# Define your outlier detection and deletion method here
-			# For example, you can use z-score method to detect and delete outliers
-			z_scores = np.abs((df[column_name] - df[column_name].mean()) / df[column_name].std())
-			df = df[z_scores < 3]  # Remove rows with z-scores greater than 3
-			
-			# st.success("Outliers deleted successfully.")
-			st.warning("Outliers deleted. Changes will not be saved until you press the 'Confirm Changes' button below.")
+		if method == 'Delete Outliers':
+			z_scores = np.abs((df[column_name] - df[column_name].mean()) /
+				df[column_name].std())
+			df = df[z_scores < float(z_score_threshold)]
+			st.warning(
+				"Outliers deleted. Changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(12)
 			return df
-		elif method == "Winsorization":
-			print(0)
-			# df[column_name] = pd.to_numeric(df[column_name], errors='coerce')
-			# df = df.reset_index()
-			# ser = pd.Series([2, pd.NA], dtype=pd.Int64Dtype())
-			# df[column_name] = pd.Series(df[column_name], dtype=pd.Int64Dtype)
-			# df[column_name] = df[column_name].astype(pd.Int64Dtype())
-			# Slider for selecting the lower limit for Winsorization
-			print(2)
-			lower_limit = st.slider("Select Lower Limit", min_value=0.0, max_value=0.1, step=0.01, value=0.05)
-			# Slider for selecting the upper limit for Winsorization
-			upper_limit = st.slider("Select Upper Limit", min_value=0.0, max_value=0.1, step=0.01, value=0.05)
-
-			# Apply Winsorization to the column
-			modified_column = winsorize(df[column_name], limits=[lower_limit, upper_limit])
-			print(3)
+		elif method == 'Winsorization':
+			modified_column = winsorize(df[column_name], limits=[
+				lower_limit, upper_limit])
 			df[column_name] = modified_column
-			
-			st.warning("Outliers have been treated using Winsorization, but changes will not be saved until the 'Confirm Changes' button is pressed.")
+			st.warning(
+				"Outliers have been treated using Winsorization, but changes will not be saved until the 'Confirm Changes' button is pressed."
+				)
+			print(13)
 			return df
 	except Exception as e:
 		print(e)
-		# st.error(f"Error occurred: {e}")
-		# st.error("🚨 Select Proper Numerical Column")
-		st.warning("Select Proper Numerical Column")
+		print(14)
+		st.warning('Select Proper Numerical Column')
+		print(15)
 		return df
-	
-# Function to preprocess by treating outliers
-def treat_outliers_full_df(df, method, z_score_threshold=3, lower_limit=0.05, upper_limit=0.05):
+
+
+def treat_outliers_full_df(df, method, z_score_threshold=3, lower_limit=
+	0.05, upper_limit=0.05):
 	"""
 	Treat outliers in a given DataFrame.
 
 	:param df: DataFrame to process
 	:param method: Method to use for outlier treatment ("Delete Outliers", "Winsorization")
 	:param z_score_threshold: Z-score threshold for identifying outliers (used for "Delete Outliers")
 	:param lower_limit: Lower limit for Winsorization
 	:param upper_limit: Upper limit for Winsorization
 	:return: DataFrame with outliers treated
 	"""
+	print(16)
 	try:
-		# Get a list of all numerical columns
-		numerical_columns = df.select_dtypes(include=[np.number]).columns.tolist()
-
-		if method == "Delete Outliers":
-			# Remove rows with z-scores greater than the specified threshold for each numerical column
+		numerical_columns = df.select_dtypes(include=[np.number]
+			).columns.tolist()
+		if method == 'Delete Outliers':
 			for column_name in numerical_columns:
-				z_scores = np.abs((df[column_name] - df[column_name].mean()) / df[column_name].std())
-				df = df[z_scores < z_score_threshold]  # Retain rows with z-scores less than the threshold
-			# st.success("Outliers deleted successfully.")
-			st.warning("Outliers deleted. Changes will not be saved until you press the 'Confirm Changes' button below.")
+				z_scores = np.abs((df[column_name] - df[column_name].mean()
+					) / df[column_name].std())
+				df = df[z_scores < float(z_score_threshold)]
+			st.warning(
+				"Outliers deleted. Changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(17)
 			return df
-
-		elif method == "Winsorization":
-			# Apply Winsorization to each numerical column with the specified limits
+		elif method == 'Winsorization':
 			for column_name in numerical_columns:
-				df[column_name] = winsorize(df[column_name], limits=[lower_limit, upper_limit])
-			# st.success("Outliers treated using Winsorization successfully.")
-			st.warning("Outliers have been treated using Winsorization, but changes will not be saved until the 'Confirm Changes' button is pressed.")
+				df[column_name] = winsorize(df[column_name], limits=[
+					lower_limit, upper_limit])
+			st.warning(
+				"Outliers have been treated using Winsorization, but changes will not be saved until the 'Confirm Changes' button is pressed."
+				)
+			print(18)
 			return df
-
 		else:
-			st.error("Invalid method specified for treating outliers.")
+			st.error('Invalid method specified for treating outliers.')
+			print(19)
 			return df
-
 	except Exception as e:
-		st.warning(f"Error occurred: {e}")
+		st.warning(f'Error occurred: {e}')
+		print(20)
 		return df
 
-# Function to preprocess by treating missing values
+
 def treat_missing_values(df, column_name, method):
 	try:
-		if method == "Delete Missing Values":
+		if method == 'Delete Missing Values':
 			df.dropna(subset=[column_name], inplace=True)
-			# st.success("Missing values deleted successfully.")
-			st.warning("Missing values have been deleted, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			print(21)
+			st.warning(
+				"Missing values have been deleted, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(22)
 			return df
-		elif method == "Mean Imputation":
-			imputer = SimpleImputer(strategy="mean")
+		elif method == 'Mean Imputation':
+			imputer = SimpleImputer(strategy='mean')
 			df[column_name] = imputer.fit_transform(df[[column_name]])
-			# st.success("Missing values imputed using mean successfully.")
-			st.warning("Missing values have been imputed using the mean, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Missing values have been imputed using the mean, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(23)
 			return df
-		elif method == "Median Imputation":
-			imputer = SimpleImputer(strategy="median")
+		elif method == 'Median Imputation':
+			imputer = SimpleImputer(strategy='median')
 			df[column_name] = imputer.fit_transform(df[[column_name]])
-			# st.success("Missing values imputed using median successfully.")
-			st.warning("Missing values have been imputed using the median, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Missing values have been imputed using the median, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(24)
 			return df
-		elif method == "Mode Imputation":
-			imputer = SimpleImputer(strategy="most_frequent")
+		elif method == 'Mode Imputation':
+			imputer = SimpleImputer(strategy='most_frequent')
 			df[column_name] = imputer.fit_transform(df[[column_name]])
-			# st.success("Missing values imputed using mode successfully.")
-			st.warning("Missing values have been imputed using the mode, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Missing values have been imputed using the mode, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(25)
 			return df
 	except Exception as e:
-		st.error(f"Error occurred: {e}")
+		st.error(f'Error occurred: {e}')
+		print(26)
 		return df
 
-# Function to preprocess by applying transformation techniques
+
 def apply_transformation(df, column_name, method):
 	try:
-		if method == "Log Transformation":
+		if method == 'Log Transformation':
 			df[column_name] = np.log1p(df[column_name])
-			# st.success("Log transformation applied successfully.")
-			st.warning("Log transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Log transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(27)
 			return df
-		elif method == "Exponential Transformation":
+		elif method == 'Exponential Transformation':
 			df[column_name] = np.exp(df[column_name])
-			# st.success("Exponential transformation applied successfully.")
-			st.warning("Exponential transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Exponential transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(28)
 			return df
-		elif method == "Square Root Transformation":
+		elif method == 'Square Root Transformation':
 			df[column_name] = np.sqrt(df[column_name])
-			# st.success("Square root transformation applied successfully.")
-			st.warning("Square root transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Square root transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(29)
 			return df
-		elif method == "Box-Cox Transformation":
-			transformed_data, _ = boxcox(df[column_name] + 1)  # Adding 1 to avoid non-positive values
+		elif method == 'Box-Cox Transformation':
+			transformed_data, _ = boxcox(df[column_name] + 1)
 			df[column_name] = transformed_data
-			# st.success("Box-Cox transformation applied successfully.")
-			st.warning("Box-Cox transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Box-Cox transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(30)
 			return df
-		elif method == "Yeo-Johnson Transformation":
-			transformed_data, _ = yeojohnson(df[column_name] + 1)  # Adding 1 to avoid non-positive values
+		elif method == 'Yeo-Johnson Transformation':
+			transformed_data, _ = yeojohnson(df[column_name] + 1)
 			df[column_name] = transformed_data
-			# st.success("Yeo-Johnson transformation applied successfully.")
-			st.warning("Yeo-Johnson transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Yeo-Johnson transformation applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(31)
 			return df
 	except Exception as e:
-		st.warning("Select Proper Column")
-		st.error(f"Error occurred: {e}")
+		st.warning('Select Proper Column')
+		print(32)
+		st.error(f'Error occurred: {e}')
+		print(33)
 		return df
 
 
-# Function to preprocess by creating dummy variables
-def create_dummy_variables(df, method):
+def create_dummy_variables(df, method, opt):
 	try:
-		if method == "One-Hot Encoding":
-			# Perform one-hot encoding for all categorical columns
-			opt = st.toggle("drop_first")
+		if method == 'One-Hot Encoding':
+			
 			cat_columns = df.select_dtypes(include=['object']).columns
-			encoded_df = pd.get_dummies(df, columns=cat_columns, drop_first=opt)
-			encoded_df.replace({True: 1, False: 0}, inplace=True)
-			# st.success("One-hot encoding applied successfully.")
-			st.warning("One-hot encoding applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			encoded_df = pd.get_dummies(df, columns=cat_columns, drop_first=opt
+				)
+			encoded_df.replace({(True): 1, (False): 0}, inplace=True)
+			print(34)
+			st.warning(
+				"One-hot encoding applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(35)
 			return encoded_df
-		elif method == "Label Encoding":
-			# Perform label encoding for all categorical columns
+		elif method == 'Label Encoding':
 			encoded_df = df.copy()
 			label_encoder = LabelEncoder()
 			for column in encoded_df.select_dtypes(include=['object']).columns:
-				encoded_df[column] = label_encoder.fit_transform(encoded_df[column])
-			# st.success("Label encoding applied successfully.")
-			st.warning("Label encoding applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+				encoded_df[column] = label_encoder.fit_transform(encoded_df
+					[column])
+			st.warning(
+				"Label encoding applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(36)
 			return encoded_df
 	except Exception as e:
-		st.error(f"Error occurred: {e}")
+		st.error(f'Error occurred: {e}')
+		print(37)
 		return df
 
 
-# Function to preprocess by creating dummy variables
-def create_dummy_variables_for_col(df, column_name, method):
+def create_dummy_variables_for_col(df, column_name, method, opt):
 	try:
-		if method == "One-Hot Encoding":
-			# Perform one-hot encoding
-			encoded_df = pd.get_dummies(df[column_name], prefix=column_name)
+		if method == 'One-Hot Encoding':
+			encoded_df = pd.get_dummies(df[column_name], prefix=column_name, drop_first=opt)
 			df = pd.concat([df, encoded_df], axis=1)
 			df.drop(column_name, axis=1, inplace=True)
-			df.replace({True: 1, False: 0}, inplace=True)
-			# st.success("One-hot encoding applied successfully.")
-			st.warning("One-hot encoding applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			print(38)
+			df.replace({(True): 1, (False): 0}, inplace=True)
+			print(39)
+			st.warning(
+				"One-hot encoding applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(40)
 			return df
-		elif method == "Label Encoding":
-			# Perform label encoding
+		elif method == 'Label Encoding':
 			label_encoder = LabelEncoder()
 			df[column_name] = label_encoder.fit_transform(df[column_name])
-			# st.success("Label encoding applied successfully.")
-			st.warning("Label encoding applied, but changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Label encoding applied, but changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(41)
 			return df
 	except Exception as e:
-		st.error(f"Error occurred: {e}")
+		st.error(f'Error occurred: {e}')
+		print(42)
 		return df
 
 
-# Function to preprocess by applying scaling
 def apply_scaling(df, method):
 	try:
-		if method == "Standardize Scaling":
+		if method == 'Standardize Scaling':
 			scaler = StandardScaler()
 			scaled_data = scaler.fit_transform(df)
 			scaled_df = pd.DataFrame(scaled_data, columns=df.columns)
-			# st.success("Robust scaling applied successfully.")
-			st.warning("Standardize scaling has been applied, but the changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Standardize scaling has been applied, but the changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(43)
 			return scaled_df
-		elif method == "Min-Max Scaling":
+		elif method == 'Min-Max Scaling':
 			scaler = MinMaxScaler()
 			scaled_data = scaler.fit_transform(df)
 			scaled_df = pd.DataFrame(scaled_data, columns=df.columns)
-			# st.success("Robust scaling applied successfully.")
-			st.warning("Min-Max scaling has been applied, but the changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Min-Max scaling has been applied, but the changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(44)
 			return scaled_df
-		elif method == "Robust Scaling":
+		elif method == 'Robust Scaling':
 			scaler = RobustScaler()
 			scaled_data = scaler.fit_transform(df)
 			scaled_df = pd.DataFrame(scaled_data, columns=df.columns)
-			# st.success("Robust scaling applied successfully.")
-			st.warning("Robust scaling has been applied, but the changes will not be saved until you press the 'Confirm Changes' button below.")
+			st.warning(
+				"Robust scaling has been applied, but the changes will not be saved until you press the 'Confirm Changes' button below."
+				)
+			print(45)
 			return scaled_df
 	except Exception as e:
-		st.warning("Only Numerical Columns Should be present.")
-		st.error(f"Error occurred: {e}")
+		st.warning('Only Numerical Columns Should be present.')
+		print(46)
+		st.error(f'Error occurred: {e}')
+		print(47)
 		return df
 
 
-# Function to discretize output variable
-# Function to discretize output variable
 def discretize_output(df, column_name, bins, strategy):
 	try:
-		discretizer = KBinsDiscretizer(n_bins=bins, encode='ordinal', strategy=strategy)
+		discretizer = KBinsDiscretizer(n_bins=bins, encode='ordinal',
+			strategy=strategy)
 		df[column_name] = discretizer.fit_transform(df[[column_name]])
-		# st.success(f"Output variable '{column_name}' discretized successfully.")
-		st.warning(f"Output variable '{column_name}' discretized, but changes will not be saved until you press the 'Confirm Changes' button below.")
+		st.warning(
+			f"Output variable '{column_name}' discretized, but changes will not be saved until you press the 'Confirm Changes' button below."
+			)
+		print(48)
 		return df
 	except Exception as e:
-		st.warning("Works for only numerical columns")
-		st.error(f"Error occurred: {e}")
+		st.warning('Works for only numerical columns')
+		print(49)
+		st.error(f'Error occurred: {e}')
+		print(50)
 		return df
 
+
 def calculate_insights(column_data):
 	try:
 		insights = {}
-
-		# Count of distinct values
 		insights['Distinct'] = len(column_data.dropna().unique())
-
-		# Percentage of distinct values
-		insights['Distinct (%)'] = len(column_data.dropna().unique()) / len(column_data.dropna()) * 100
-
-		# Count of missing values
+		insights['Distinct (%)'] = len(column_data.dropna().unique()) / len(
+			column_data.dropna()) * 100
 		insights['Missing'] = column_data.isnull().sum()
-
-		# Percentage of missing values
-		insights['Missing (%)'] = column_data.isnull().sum() / len(column_data) * 100
-
-		# Count of infinite values
+		insights['Missing (%)'] = column_data.isnull().sum() / len(column_data
+			) * 100
 		insights['Infinite'] = np.isinf(column_data).sum()
-
-		# Percentage of infinite values
-		insights['Infinite (%)'] = np.isinf(column_data).sum() / len(column_data) * 100
-
-		# Mean
+		insights['Infinite (%)'] = np.isinf(column_data).sum() / len(
+			column_data) * 100
 		insights['Mean'] = column_data.mean()
-
-		# Median
 		insights['Median'] = column_data.median()
-
-		# Mode
 		insights['Mode'] = column_data.mode().iloc[0]
-
-		# Minimum
 		insights['Minimum'] = column_data.min()
-
-		# Maximum
 		insights['Maximum'] = column_data.max()
-
-		# Zeros count
 		insights['Zeros'] = (column_data == 0).sum()
-
-		# Percentage of zeros
-		insights['Zeros (%)'] = (column_data == 0).sum() / len(column_data) * 100
-
-		# Negative values count
+		insights['Zeros (%)'] = (column_data == 0).sum() / len(column_data
+			) * 100
 		insights['Negative'] = (column_data < 0).sum()
-
-		# Percentage of negative values
-		insights['Negative (%)'] = (column_data < 0).sum() / len(column_data) * 100
-
-		# Memory size
+		insights['Negative (%)'] = (column_data < 0).sum() / len(column_data
+			) * 100
 		insights['Memory size'] = column_data.memory_usage(deep=True)
-
-		# 5th percentile
 		insights['5-th percentile'] = np.percentile(column_data.dropna(), 5)
-
-		# Q1 (25th percentile)
 		insights['Q1'] = np.percentile(column_data.dropna(), 25)
-
-		# Median
 		insights['Median'] = np.median(column_data.dropna())
-
-		# Q3 (75th percentile)
 		insights['Q3'] = np.percentile(column_data.dropna(), 75)
-
-		# 95th percentile
 		insights['95-th percentile'] = np.percentile(column_data.dropna(), 95)
-
-		# Range
 		insights['Range'] = insights['Maximum'] - insights['Minimum']
-
-		# Interquartile range (IQR)
 		insights['Interquartile range'] = insights['Q3'] - insights['Q1']
-
-		# Descriptive statistics
 		insights['Descriptive statistics'] = column_data.describe()
-
-		# Standard deviation
 		insights['Standard deviation'] = column_data.std()
-
-		# Coefficient of variation (CV)
 		if insights['Mean'] != 0:
-			insights['Coefficient of variation (CV)'] = insights['Standard deviation'] / insights['Mean']
+			insights['Coefficient of variation (CV)'] = insights[
+				'Standard deviation'] / insights['Mean']
 		else:
 			insights['Coefficient of variation (CV)'] = float('NaN')
-
-		# Kurtosis
 		insights['Kurtosis'] = column_data.kurtosis()
-
-		# Median Absolute Deviation (MAD)
-		mad = np.median(np.abs(column_data.dropna() - np.median(column_data.dropna())))
+		mad = np.median(np.abs(column_data.dropna() - np.median(column_data
+			.dropna())))
 		insights['Median Absolute Deviation (MAD)'] = mad
-
-		# Skewness
 		insights['Skewness'] = column_data.skew()
-
-		# Sum
 		insights['Sum'] = column_data.sum()
-
-		# Variance
 		insights['Variance'] = column_data.var()
-
-		# Monotonicity (not calculated)
 	except Exception as e:
-		print("_e:=_", e)
+		print('_e:=_', e)
+		print(51)
 		st.write(e)
-		
-
+		print(52)
 	return insights
 
 
-
-# Initialize state
-if "button_clicked" not in st.session_state:
+if 'button_clicked' not in st.session_state:
 	st.session_state.button_clicked = False
+
+
 def callback():
-	# Button was clicked!
 	st.session_state.button_clicked = True
 
 
-st.subheader(":green[Try Best Pre-Processing Step]")
+st.header(':green[Try Best Pre-Processing Step]')
+print(53)
 try:
-	st.write("Session State:->", st.session_state["shared"])
-	if "df" in st.session_state:
+	st.write('Session State:->', st.session_state['shared'])
+	print(54)
+	if 'df' in st.session_state:
 		df = st.session_state.df
 		print(1)
-		# int_columns = df.select_dtypes(include='int').columns
-		# df[int_columns] = df[int_columns].astype(pd.Int64Dtype())
-		selected_column = st.selectbox("Select a column", df.columns)
+		print(55)
+		selected_column = st.selectbox('Select a column', df.columns)
 		print(2)
-		st.subheader(f"Insights for column ':green[{selected_column}]':")
+		print(56)
+		html_content = (
+			f"<div class='column-header'>Insights for column:<code>{selected_column}</code></div>"
+			)
+		css_style = """
+		<style>
+		.column-header {
+			margin-bottom: 10px;
+			font-weight: bold;
+			font-size: 26px;
+			color: green; /* Change color as needed */
+		}
+		</style>
+		"""
+		st.markdown(css_style, unsafe_allow_html=True)
+		print(57)
+		st.markdown(html_content, unsafe_allow_html=True)
+		print(58)
 		print(3)
+		print(59)
 		if df[selected_column].dtype == 'object':
 			col1, col2 = st.columns(2)
 			print(4)
+			print(60)
 			with col1:
 				unique_values = df[selected_column].nunique()
 				print(5)
-				st.write(f"  - Data Type: :green[{df[selected_column].dtype}]")
+				print(61)
+				st.write(f'  - Data Type: :green[{df[selected_column].dtype}]')
+				print(62)
 				print(6)
-				st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+				print(63)
+				st.write(
+					f'  - Number of Unique Values: :green[{unique_values}]')
+				print(64)
 				print(7)
+				print(65)
 				if unique_values <= 20:
 					print(8)
-					st.write(f"  - Unique Values: :green[{', '.join(map(str, df[selected_column].unique()))}]")
+					print(66)
+					st.write(
+						f"  - Unique Values: :green[{', '.join(map(str, df[selected_column].unique()))}]"
+						)
+					print(67)
 				else:
 					print(9)
-					st.write(f"  - Top 20 Unique Values:")
+					print(68)
+					st.write(f'  - Top 20 Unique Values:')
+					print(69)
 					print(10)
-					st.write(f":green[{', '.join(map(str, df[selected_column].value_counts().head(20).index))}]")
+					print(70)
+					st.write(
+						f":green[{', '.join(map(str, df[selected_column].value_counts().head(20).index))}]"
+						)
+					print(71)
 			with col2:
 				print(10)
+				print(72)
 				plt.figure(figsize=(10, 6))
+				print(73)
 				print(11)
+				print(74)
 				try:
 					print(12)
-					sns.countplot(x=limit_unique_values(df[selected_column]), data=df, color="green")
+					print(75)
+					sns.countplot(x=limit_unique_values(df[selected_column]
+						), data=df, color='green')
+					print(76)
 				except:
 					print(13)
-					sns.countplot(x=df[selected_column], data=df, color="green")
+					print(77)
+					sns.countplot(x=df[selected_column], data=df, color='green'
+						)
+					print(78)
 				plt.xticks(rotation=45)
+				print(79)
 				st.pyplot()
+				print(80)
 				plt.close()
-			with st.expander("More Info"):
+				print(81)
+			with st.expander('More Info'):
 				print(14)
-				tab1, tab2 = st.tabs(["Insights", "Donut chart"])
+				print(82)
+				tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
 				print(15)
+				print(83)
 				with tab1:
 					print(16)
+					print(84)
 					col7, col8, col9 = st.columns(3)
 					with col7:
 						print(17)
-						# Insights
-						st.write("## Insights")
-						approximate_distinct_count = df[selected_column].nunique()
-						approximate_unique_percent = (approximate_distinct_count / len(df)) * 100
+						print(85)
+						st.write('## Insights')
+						print(86)
+						approximate_distinct_count = df[selected_column
+							].nunique()
+						approximate_unique_percent = (
+							approximate_distinct_count / len(df) * 100)
 						missing = df[selected_column].isna().sum()
-						missing_percent = (missing / len(df)) * 100
-						memory_size = df[selected_column].memory_usage(deep=True)
-						st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-						st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-						st.write(f"Missing: :green[{missing}]")
-						st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-						st.write(f"Memory Size: :green[{memory_size}]")
+						missing_percent = missing / len(df) * 100
+						memory_size = df[selected_column].memory_usage(deep
+							=True)
+						st.write(
+							f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+							)
+						print(87)
+						st.write(
+							f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+							)
+						print(88)
+						st.write(f'Missing: :green[{missing}]')
+						print(89)
+						st.write(f'Missing (%): :green[{missing_percent:.2f}%]'
+							)
+						print(90)
+						st.write(f'Memory Size: :green[{memory_size}]')
+						print(91)
 						print(18)
-						# st.header("An owl")
-						# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
+						print(92)
 					with col8:
 						print(19)
-						# Mode and Standard Deviation
-						st.write("## Mode")
-						# if df[selected_column].dtype == 'object':
-						mode = df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-						st.write(f"Mode: :green[{mode}]")
-							# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-						# else:
-							# mode = df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-							# std_dev = df[selected_column].astype(float).std()
-							# st.write(f"Mode: {mode}")
-							# st.write(f"Standard Deviation: {std_dev}")
+						print(93)
+						st.write('## Mode')
+						print(94)
+						mode = df[selected_column].mode().iloc[0]
+						st.write(f'Mode: :green[{mode}]')
+						print(95)
 						print(20)
+						print(96)
 					with col9:
 						print(21)
-						# First 5 Sample Rows
-						st.write("## First 5 Sample Rows")
+						print(97)
+						st.write('## First 5 Sample Rows')
+						print(98)
 						st.write(df[selected_column].head())
+						print(99)
 						print(22)
+						print(100)
 				with tab2:
 					print(23)
-					# Prepare data for donut chart
-					data = limit_unique_values(df[selected_column]).value_counts().reset_index()
+					print(101)
+					data = limit_unique_values(df[selected_column]
+						).value_counts().reset_index()
 					data.columns = [selected_column, 'count']
-
-					fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-					fig.update_traces(textposition='inside', textinfo='percent+label')
-					fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
+					fig = px.pie(data, values='count', names=
+						selected_column, hole=0.5)
+					fig.update_traces(textposition='inside', textinfo=
+						'percent+label')
+					print(102)
+					fig.update_layout(legend=dict(orientation='h', yanchor=
+						'bottom', y=1.02, xanchor='right', x=1))
+					print(103)
 					st.plotly_chart(fig)
+					print(104)
 					print(24)
-					# st.header("An owl")
-					# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-				
+					print(105)
 		elif pd.api.types.is_numeric_dtype(df[selected_column]):
 			print(25)
+			print(106)
 			col3, col4 = st.columns(2)
 			print(26)
+			print(107)
 			with col3:
 				print(27)
-				st.write(f"  - Data Type: :green[{df[selected_column].dtype}]")
-				st.write(f"  - Mean: :green[{df[selected_column].mean()}]")
-				st.write(f"  - Standard Deviation: :green[{df[selected_column].std()}]")
-				st.write(f"  - Min Value: :green[{df[selected_column].min()}]")
-				st.write(f"  - Max Value: :green[{df[selected_column].max()}]")
+				print(108)
+				st.write(f'  - Data Type: :green[{df[selected_column].dtype}]')
+				print(109)
+				st.write(f'  - Mean: :green[{df[selected_column].mean()}]')
+				print(110)
+				st.write(
+					f'  - Standard Deviation: :green[{df[selected_column].std()}]'
+					)
+				print(111)
+				st.write(f'  - Min Value: :green[{df[selected_column].min()}]')
+				print(112)
+				st.write(f'  - Max Value: :green[{df[selected_column].max()}]')
+				print(113)
 				print(28)
+				print(114)
 			with col4:
 				plt.figure(figsize=(10, 6))
-				sns.histplot(df[selected_column], kde=True, color="green")
+				print(115)
+				sns.histplot(df[selected_column], kde=True, color='green')
+				print(116)
 				st.pyplot()
+				print(117)
 				plt.close()
+				print(118)
 				print(29)
-			with st.expander("More Info"):
+				print(119)
+			with st.expander('More Info'):
 				print(30)
-				tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+				print(120)
+				tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot', 'QQ plot'])
 				with tab1:
 					print(31)
+					print(121)
 					col4, col5, col6 = st.columns(3)
 					with col4:
 						print(32)
-						st.write("#### Basic Statistics")
+						print(122)
+						st.write('#### Basic Statistics')
+						print(123)
 						insights = calculate_insights(df[selected_column])
-						basic_stats = {key: value for key, value in insights.items() if key in [
-							'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
+						basic_stats = {key: value for key, value in
+							insights.items() if key in ['Mean', 'Median',
+							'Mode', 'Standard deviation', 'Variance',
+							'Kurtosis', 'Skewness']}
 						for key, value in basic_stats.items():
-							st.write(f"**{key}:** :green[{value:.3f}]")
-						st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-						st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-						st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
+							st.write(f'**{key}:** :green[{value:.3f}]')
+							print(124)
+						st.write(
+							f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+							)
+						print(125)
+						st.write(
+							f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+							)
+						print(126)
+						st.write(
+							f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+							)
+						print(127)
 						print(33)
+						print(128)
 					with col5:
 						print(34)
-						st.write("#### Percentiles")
-						descriptive_stats = insights.get('Descriptive statistics')
+						print(129)
+						st.write('#### Percentiles')
+						print(130)
+						descriptive_stats = insights.get(
+							'Descriptive statistics')
 						if descriptive_stats is not None:
-							percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
+							percentiles = descriptive_stats.loc[['min',
+								'25%', '50%', '75%', 'max']]
 							if '5%' in descriptive_stats.index:
 								percentiles['5%'] = descriptive_stats['5%']
 							if '95%' in descriptive_stats.index:
 								percentiles['95%'] = descriptive_stats['95%']
 							st.write(percentiles)
+							print(131)
 						print(35)
-
+						print(132)
 					with col6:
 						print(36)
-						st.write("#### Additional Statistics")
-						additional_stats = {key: value for key, value in insights.items() if key in [
-							'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
+						print(133)
+						st.write('#### Additional Statistics')
+						print(134)
+						additional_stats = {key: value for key, value in
+							insights.items() if key in ['Distinct',
+							'Distinct (%)', 'Missing', 'Missing (%)',
+							'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
 						for key, value in additional_stats.items():
-							st.write(f"**{key}:** :green[{value:.3f}]")
-						# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-						# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-						# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-						st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-						st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-						st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+							st.write(f'**{key}:** :green[{value:.3f}]')
+							print(135)
+						st.write(
+							f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+							)
+						print(136)
+						st.write(
+							f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+							)
+						print(137)
+						st.write(
+							f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+							)
+						print(138)
 						print(37)
+						print(139)
 				with tab2:
 					print(38)
+					print(140)
 					fig = px.box(df, y=selected_column)
 					st.plotly_chart(fig)
+					print(141)
 					print(39)
+					print(142)
 				with tab3:
 					print(40)
+					print(143)
 					plt.figure(figsize=(10, 6))
-					qqplot_data = sm.qqplot(df[selected_column], line='s').gca().lines
+					print(144)
+					qqplot_data = sm.qqplot(df[selected_column], line='s').gca(
+						).lines
 					fig = go.Figure()
-					fig.add_trace({
-						'type': 'scatter',
-						'x': qqplot_data[0].get_xdata(),
-						'y': qqplot_data[0].get_ydata(),
-						'mode': 'markers',
-						'marker': {'color': '#19d3f3'}
-					})
-					fig.add_trace({
-						'type': 'scatter',
-						'x': qqplot_data[1].get_xdata(),
-						'y': qqplot_data[1].get_ydata(),
-						'mode': 'lines',
-						'line': {'color': '#636efa'}
-					})
+					fig.add_trace({'type': 'scatter', 'x': qqplot_data[0].
+						get_xdata(), 'y': qqplot_data[0].get_ydata(),
+						'mode': 'markers', 'marker': {'color': '#19d3f3'}})
+					print(145)
+					fig.add_trace({'type': 'scatter', 'x': qqplot_data[1].
+						get_xdata(), 'y': qqplot_data[1].get_ydata(),
+						'mode': 'lines', 'line': {'color': '#636efa'}})
+					print(146)
 					x_min = min(qqplot_data[0].get_xdata())
 					x_max = max(qqplot_data[0].get_xdata())
 					y_min = min(qqplot_data[0].get_ydata())
 					y_max = max(qqplot_data[0].get_ydata())
-					fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-					fig.update_layout({
-						'title': f'QQ Plot for {selected_column}',
-						'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
+					fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min,
+						y_max], mode='lines', line=dict(color='red', width=
+						2), name='Identity Line'))
+					print(147)
+					fig.update_layout({'title':
+						f'QQ Plot for {selected_column}', 'xaxis': {'title':
+						'Theoretical Quantiles', 'zeroline': False},
 						'yaxis': {'title': 'Sample Quantiles'},
-						'showlegend': False,
-						'width': 800,
-						'height': 700,
-					})
+						'showlegend': False, 'width': 800, 'height': 700})
+					print(148)
 					st.plotly_chart(fig)
+					print(149)
 					print(41)
-		# st.write("---")
+					print(150)
 	else:
-		st.write("DataFrame not found.")
-	# st.write("``")
+		st.write('DataFrame not found.')
+		print(151)
 except ZeroDivisionError:
 	pass
 except Exception as e:
 	st.error(e)
-	st.subheader("⚠️Please upload a file⚠️")
+	print(152)
+	st.subheader('⚠️Please upload a file⚠️')
+	print(153)
 	pass
-
-# Function to preprocess column by changing data type
-
-
-
-# Select column to preprocess
-# selected_column = st.selectbox("Select a column", df.columns)
-		
 print(42)
-
-# Select preprocessing action
-preprocessing_action = st.sidebar.radio("Select preprocessing action", 
-									[
-										"Select Pre-Processing Step⬇️",
-										"Change Data Type", 
-										"Drop Column", 
-										"Drop Duplicates", 
-										"Treat Outliers", 
-										"Treat Outliers on full DF",
-										"Treat Missing Values",
-										"Traat Missing from full DF",
-										"Apply Transformation",
-										"Create Dummy Variables",
-										"Column to Dummy Variable",
-										"Apply Scaling",
-										"Discretize Output Variable",
-										"Column Unique Value Replacement"
-									]
-									)
-
-# modified_df = pd.DataFrame()
+print(154)
+preprocessing_action = st.sidebar.radio('Select preprocessing action', [
+	'Select Pre-Processing Step⬇️', 'Drop Column', 'Treat Missing Values',
+	'Traat Missing from full DF', 'Change Data Type', 'Drop Duplicates',
+	'Treat Outliers', 'Treat Outliers on full DF', 'Apply Transformation',
+	'Create Dummy Variables', 'Column to Dummy Variable', 'Apply Scaling',
+	'Discretize Output Variable', 'Column Unique Value Replacement'])
 try:
-	if preprocessing_action == "Select Pre-Processing Step⬇️":
-		print("You have successfuly reached Pre-Proceaaing Phase")
-
-	elif preprocessing_action == "Change Data Type":
-		dtype_options = [
-			"int", "int32", "Int32", "int64", "Int64",
-			"float", "float32", "Float32", "float64", "Float64",
-			"str", "bool"
-		]
-		new_dtype = st.selectbox("Select new data type", dtype_options)
-		# Apply = st.button('Apply')
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
-		# if Apply:
-			# Make a copy of the original DataFrame to preserve undo functionality
+	if preprocessing_action == 'Select Pre-Processing Step⬇️':
+		print('You have successfuly reached Pre-Proceaaing Phase')
+		print(155)
+	elif preprocessing_action == 'Change Data Type':
+		dtype_options = ['int', 'int32', 'Int32', 'int64', 'Int64', 'float',
+			'float32', 'Float32', 'float64', 'Float64', 'str', 'bool']
+		new_dtype = st.selectbox('Select new data type', dtype_options)
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			
 			change_dtype(modified_df, selected_column, new_dtype)
-			st.write("Modified DataFrame:")
+			print(156)
+			st.write('Modified DataFrame:')
+			print(157)
 			st.write(modified_df)
-			# st.session_state.df = modified_df  # Store modified DataFrame in session state
-			# st.session_state.modified_df = modified_df
+			print(158)
 			try:
 				if modified_df[selected_column].dtype == 'object':
 					col1, col2 = st.columns(2)
 					with col1:
 						unique_values = modified_df[selected_column].nunique()
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(159)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(160)
 						if unique_values <= 20:
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(161)
 						else:
-							st.write(f"  - Top 20 Unique Values:")
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
+							st.write(f'  - Top 20 Unique Values:')
+							print(162)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(163)
 					with col2:
 						plt.figure(figsize=(10, 6))
+						print(164)
 						try:
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(165)
 						except:
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(166)
 						plt.xticks(rotation=45)
+						print(167)
 						st.pyplot()
+						print(168)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2 = st.tabs(["Insights", "Donut chart"])
+						print(169)
+					with st.expander('More Info'):
+						tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
 						with tab1:
 							col7, col8, col9 = st.columns(3)
 							with col7:
-								# Insights
-								st.write("## Insights")
-								approximate_distinct_count = modified_df[selected_column].nunique()
-								approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-								missing = modified_df[selected_column].isna().sum()
-								missing_percent = (missing / len(modified_df)) * 100
-								memory_size = modified_df[selected_column].memory_usage(deep=True)
-								st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-								st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-								st.write(f"Missing: :green[{missing}]")
-								st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-								st.write(f"Memory Size: :green[{memory_size}]")
-
-								# st.header("An owl")
-								# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
+								st.write('## Insights')
+								print(170)
+								approximate_distinct_count = modified_df[
+									selected_column].nunique()
+								approximate_unique_percent = (
+									approximate_distinct_count / len(
+									modified_df) * 100)
+								missing = modified_df[selected_column].isna(
+									).sum()
+								missing_percent = missing / len(modified_df
+									) * 100
+								memory_size = modified_df[selected_column
+									].memory_usage(deep=True)
+								st.write(
+									f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+									)
+								print(171)
+								st.write(
+									f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+									)
+								print(172)
+								st.write(f'Missing: :green[{missing}]')
+								print(173)
+								st.write(
+									f'Missing (%): :green[{missing_percent:.2f}%]'
+									)
+								print(174)
+								st.write(f'Memory Size: :green[{memory_size}]')
+								print(175)
 							with col8:
-								# Mode and Standard Deviation
-								st.write("## Mode")
-								# if modified_df[selected_column].dtype == 'object':
-								mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-								st.write(f"Mode: :green[{mode}]")
-									# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-								# else:
-									# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-									# std_dev = modified_df[selected_column].astype(float).std()
-									# st.write(f"Mode: {mode}")
-									# st.write(f"Standard Deviation: {std_dev}")
+								st.write('## Mode')
+								print(176)
+								mode = modified_df[selected_column].mode(
+									).iloc[0]
+								st.write(f'Mode: :green[{mode}]')
+								print(177)
 							with col9:
-								# First 5 Sample Rows
-								st.write("## First 5 Sample Rows")
+								st.write('## First 5 Sample Rows')
+								print(178)
 								st.write(modified_df[selected_column].head())
-
+								print(179)
 						with tab2:
-							# Prepare data for donut chart
-							data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
+							data = limit_unique_values(modified_df[
+								selected_column]).value_counts().reset_index()
 							data.columns = [selected_column, 'count']
-
-							fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-							fig.update_traces(textposition='inside', textinfo='percent+label')
-							fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-							st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+							fig = px.pie(data, values='count', names=
+								selected_column, hole=0.5)
+							fig.update_traces(textposition='inside',
+								textinfo='percent+label')
+							print(180)
+							fig.update_layout(legend=dict(orientation='h',
+								yanchor='bottom', y=1.02, xanchor='right', x=1)
+								)
+							print(181)
+							st.plotly_chart(fig)
+							print(182)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
 					col3, col4 = st.columns(2)
 					with col3:
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(183)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(184)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(185)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(186)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(187)
 					with col4:
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(188)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(189)
 						st.pyplot()
+						print(190)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+						print(191)
+					with st.expander('More Info'):
+						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot',
+							'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								st.write("#### Basic Statistics")
-								insights = calculate_insights(modified_df[selected_column])
-								basic_stats = {key: value for key, value in insights.items() if key in [
-									'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
+								st.write('#### Basic Statistics')
+								print(192)
+								insights = calculate_insights(modified_df[
+									selected_column])
+								basic_stats = {key: value for key, value in
+									insights.items() if key in ['Mean',
+									'Median', 'Mode', 'Standard deviation',
+									'Variance', 'Kurtosis', 'Skewness']}
 								for key, value in basic_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-								st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-								st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(193)
+								st.write(
+									f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+									)
+								print(194)
+								st.write(
+									f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+									)
+								print(195)
+								st.write(
+									f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+									)
+								print(196)
 							with col5:
-								st.write("#### Percentiles")
-								descriptive_stats = insights.get('Descriptive statistics')
+								st.write('#### Percentiles')
+								print(197)
+								descriptive_stats = insights.get(
+									'Descriptive statistics')
 								if descriptive_stats is not None:
-									percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
+									percentiles = descriptive_stats.loc[[
+										'min', '25%', '50%', '75%', 'max']]
 									if '5%' in descriptive_stats.index:
 										percentiles['5%'] = descriptive_stats['5%']
 									if '95%' in descriptive_stats.index:
-										percentiles['95%'] = descriptive_stats['95%']
+										percentiles['95%'] = descriptive_stats[
+											'95%']
 									st.write(percentiles)
-
+									print(198)
 							with col6:
-								st.write("#### Additional Statistics")
-								additional_stats = {key: value for key, value in insights.items() if key in [
-									'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
+								st.write('#### Additional Statistics')
+								print(199)
+								additional_stats = {key: value for key,
+									value in insights.items() if key in [
+									'Distinct', 'Distinct (%)', 'Missing',
+									'Missing (%)', 'Zeros', 'Zeros (%)',
+									'Negative', 'Negative (%)']}
 								for key, value in additional_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-								# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-								# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-								st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-								st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-								st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(200)
+								st.write(
+									f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+									)
+								print(201)
+								st.write(
+									f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+									)
+								print(202)
+								st.write(
+									f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+									)
+								print(203)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
+							print(204)
 						with tab3:
 							plt.figure(figsize=(10, 6))
-							qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
+							print(205)
+							qqplot_data = sm.qqplot(modified_df[
+								selected_column], line='s').gca().lines
 							fig = go.Figure()
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[0].get_xdata(),
-								'y': qqplot_data[0].get_ydata(),
-								'mode': 'markers',
-								'marker': {'color': '#19d3f3'}
-							})
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[1].get_xdata(),
-								'y': qqplot_data[1].get_ydata(),
-								'mode': 'lines',
-								'line': {'color': '#636efa'}
-							})
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[0].get_xdata(), 'y':
+								qqplot_data[0].get_ydata(), 'mode':
+								'markers', 'marker': {'color': '#19d3f3'}})
+							print(206)
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[1].get_xdata(), 'y':
+								qqplot_data[1].get_ydata(), 'mode': 'lines',
+								'line': {'color': '#636efa'}})
+							print(207)
 							x_min = min(qqplot_data[0].get_xdata())
 							x_max = max(qqplot_data[0].get_xdata())
 							y_min = min(qqplot_data[0].get_ydata())
 							y_max = max(qqplot_data[0].get_ydata())
-							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-							fig.update_layout({
-								'title': f'QQ Plot for {selected_column}',
-								'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-								'yaxis': {'title': 'Sample Quantiles'},
-								'showlegend': False,
-								'width': 800,
-								'height': 700,
-							})
-							st.plotly_chart(fig)
-					st.write("---")
+							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[
+								y_min, y_max], mode='lines', line=dict(
+								color='red', width=2), name='Identity Line'))
+							print(208)
+							fig.update_layout({'title':
+								f'QQ Plot for {selected_column}', 'xaxis':
+								{'title': 'Theoretical Quantiles',
+								'zeroline': False}, 'yaxis': {'title':
+								'Sample Quantiles'}, 'showlegend': False,
+								'width': 800, 'height': 700})
+							print(209)
+							st.plotly_chart(fig)
+							print(210)
+					st.write('---')
+					print(211)
 				else:
-					st.write("DataFrame not found.")
-				st.write("``")
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+					st.write('DataFrame not found.')
+					print(212)
+				st.write('``')
+				print(213)
 			except ZeroDivisionError:
 				pass
 			except Exception as e:
 				st.error(e)
-				st.subheader("⚠️Please upload a file⚠️")
+				print(214)
+				st.subheader('⚠️Please upload a file⚠️')
+				print(215)
 				pass
-
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
 				st.session_state.df = modified_df
+				pipeline = {'column': f'{selected_column}', 'new_dtype':
+					f'{new_dtype}'}
+				with open('datatype_pipeline.pkl', 'wb') as f:
+					joblib.dump(pipeline, f)
+					print(216)
 				st.rerun()
-
-
-	elif preprocessing_action == "Drop Column":
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
-		# if Apply:
-			# Make a copy of the original DataFrame to preserve undo functionality
+				print(217)
+	elif preprocessing_action == 'Drop Column':
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			
 			drop_column(modified_df, selected_column)
-			st.write("Modified DataFrame:")
+			print(218)
+			st.write('Modified DataFrame:')
+			print(219)
 			st.write(modified_df)
-			# st.session_state.df = modified_df  # Store modified DataFrame in session state
-			# st.session_state.modified_df = modified_df
+			print(220)
 			try:
 				if modified_df[selected_column].dtype == 'object':
 					col1, col2 = st.columns(2)
 					with col1:
 						unique_values = modified_df[selected_column].nunique()
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(221)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(222)
 						if unique_values <= 20:
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(223)
 						else:
-							st.write(f"  - Top 20 Unique Values:")
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
+							st.write(f'  - Top 20 Unique Values:')
+							print(224)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(225)
 					with col2:
 						plt.figure(figsize=(10, 6))
+						print(226)
 						try:
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(227)
 						except:
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(228)
 						plt.xticks(rotation=45)
+						print(229)
 						st.pyplot()
+						print(230)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2 = st.tabs(["Insights", "Donut chart"])
+						print(231)
+					with st.expander('More Info'):
+						tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
 						with tab1:
 							col7, col8, col9 = st.columns(3)
 							with col7:
-								# Insights
-								st.write("## Insights")
-								approximate_distinct_count = modified_df[selected_column].nunique()
-								approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-								missing = modified_df[selected_column].isna().sum()
-								missing_percent = (missing / len(modified_df)) * 100
-								memory_size = modified_df[selected_column].memory_usage(deep=True)
-								st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-								st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-								st.write(f"Missing: :green[{missing}]")
-								st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-								st.write(f"Memory Size: :green[{memory_size}]")
-
-								# st.header("An owl")
-								# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
+								st.write('## Insights')
+								print(232)
+								approximate_distinct_count = modified_df[
+									selected_column].nunique()
+								approximate_unique_percent = (
+									approximate_distinct_count / len(
+									modified_df) * 100)
+								missing = modified_df[selected_column].isna(
+									).sum()
+								missing_percent = missing / len(modified_df
+									) * 100
+								memory_size = modified_df[selected_column
+									].memory_usage(deep=True)
+								st.write(
+									f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+									)
+								print(233)
+								st.write(
+									f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+									)
+								print(234)
+								st.write(f'Missing: :green[{missing}]')
+								print(235)
+								st.write(
+									f'Missing (%): :green[{missing_percent:.2f}%]'
+									)
+								print(236)
+								st.write(f'Memory Size: :green[{memory_size}]')
+								print(237)
 							with col8:
-								# Mode and Standard Deviation
-								st.write("## Mode")
-								# if modified_df[selected_column].dtype == 'object':
-								mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-								st.write(f"Mode: :green[{mode}]")
-									# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-								# else:
-									# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-									# std_dev = modified_df[selected_column].astype(float).std()
-									# st.write(f"Mode: {mode}")
-									# st.write(f"Standard Deviation: {std_dev}")
+								st.write('## Mode')
+								print(238)
+								mode = modified_df[selected_column].mode(
+									).iloc[0]
+								st.write(f'Mode: :green[{mode}]')
+								print(239)
 							with col9:
-								# First 5 Sample Rows
-								st.write("## First 5 Sample Rows")
+								st.write('## First 5 Sample Rows')
+								print(240)
 								st.write(modified_df[selected_column].head())
-
+								print(241)
 						with tab2:
-							# Prepare data for donut chart
-							data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
+							data = limit_unique_values(modified_df[
+								selected_column]).value_counts().reset_index()
 							data.columns = [selected_column, 'count']
-
-							fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-							fig.update_traces(textposition='inside', textinfo='percent+label')
-							fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-							st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+							fig = px.pie(data, values='count', names=
+								selected_column, hole=0.5)
+							fig.update_traces(textposition='inside',
+								textinfo='percent+label')
+							print(242)
+							fig.update_layout(legend=dict(orientation='h',
+								yanchor='bottom', y=1.02, xanchor='right', x=1)
+								)
+							print(243)
+							st.plotly_chart(fig)
+							print(244)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
 					col3, col4 = st.columns(2)
 					with col3:
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(245)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(246)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(247)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(248)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(249)
 					with col4:
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(250)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(251)
 						st.pyplot()
+						print(252)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+						print(253)
+					with st.expander('More Info'):
+						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot',
+							'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								st.write("#### Basic Statistics")
-								insights = calculate_insights(modified_df[selected_column])
-								basic_stats = {key: value for key, value in insights.items() if key in [
-									'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
+								st.write('#### Basic Statistics')
+								print(254)
+								insights = calculate_insights(modified_df[
+									selected_column])
+								basic_stats = {key: value for key, value in
+									insights.items() if key in ['Mean',
+									'Median', 'Mode', 'Standard deviation',
+									'Variance', 'Kurtosis', 'Skewness']}
 								for key, value in basic_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-								st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-								st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(255)
+								st.write(
+									f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+									)
+								print(256)
+								st.write(
+									f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+									)
+								print(257)
+								st.write(
+									f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+									)
+								print(258)
 							with col5:
-								st.write("#### Percentiles")
-								descriptive_stats = insights.get('Descriptive statistics')
+								st.write('#### Percentiles')
+								print(259)
+								descriptive_stats = insights.get(
+									'Descriptive statistics')
 								if descriptive_stats is not None:
-									percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
+									percentiles = descriptive_stats.loc[[
+										'min', '25%', '50%', '75%', 'max']]
 									if '5%' in descriptive_stats.index:
 										percentiles['5%'] = descriptive_stats['5%']
 									if '95%' in descriptive_stats.index:
-										percentiles['95%'] = descriptive_stats['95%']
+										percentiles['95%'] = descriptive_stats[
+											'95%']
 									st.write(percentiles)
-
+									print(260)
 							with col6:
-								st.write("#### Additional Statistics")
-								additional_stats = {key: value for key, value in insights.items() if key in [
-									'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
+								st.write('#### Additional Statistics')
+								print(261)
+								additional_stats = {key: value for key,
+									value in insights.items() if key in [
+									'Distinct', 'Distinct (%)', 'Missing',
+									'Missing (%)', 'Zeros', 'Zeros (%)',
+									'Negative', 'Negative (%)']}
 								for key, value in additional_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-								# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-								# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-								st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-								st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-								st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(262)
+								st.write(
+									f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+									)
+								print(263)
+								st.write(
+									f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+									)
+								print(264)
+								st.write(
+									f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+									)
+								print(265)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
+							print(266)
 						with tab3:
 							plt.figure(figsize=(10, 6))
-							qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
+							print(267)
+							qqplot_data = sm.qqplot(modified_df[
+								selected_column], line='s').gca().lines
 							fig = go.Figure()
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[0].get_xdata(),
-								'y': qqplot_data[0].get_ydata(),
-								'mode': 'markers',
-								'marker': {'color': '#19d3f3'}
-							})
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[1].get_xdata(),
-								'y': qqplot_data[1].get_ydata(),
-								'mode': 'lines',
-								'line': {'color': '#636efa'}
-							})
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[0].get_xdata(), 'y':
+								qqplot_data[0].get_ydata(), 'mode':
+								'markers', 'marker': {'color': '#19d3f3'}})
+							print(268)
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[1].get_xdata(), 'y':
+								qqplot_data[1].get_ydata(), 'mode': 'lines',
+								'line': {'color': '#636efa'}})
+							print(269)
 							x_min = min(qqplot_data[0].get_xdata())
 							x_max = max(qqplot_data[0].get_xdata())
 							y_min = min(qqplot_data[0].get_ydata())
 							y_max = max(qqplot_data[0].get_ydata())
-							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-							fig.update_layout({
-								'title': f'QQ Plot for {selected_column}',
-								'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-								'yaxis': {'title': 'Sample Quantiles'},
-								'showlegend': False,
-								'width': 800,
-								'height': 700,
-							})
-							st.plotly_chart(fig)
-					st.write("---")
+							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[
+								y_min, y_max], mode='lines', line=dict(
+								color='red', width=2), name='Identity Line'))
+							print(270)
+							fig.update_layout({'title':
+								f'QQ Plot for {selected_column}', 'xaxis':
+								{'title': 'Theoretical Quantiles',
+								'zeroline': False}, 'yaxis': {'title':
+								'Sample Quantiles'}, 'showlegend': False,
+								'width': 800, 'height': 700})
+							print(271)
+							st.plotly_chart(fig)
+							print(272)
+					st.write('---')
+					print(273)
 				else:
-					st.write("DataFrame not found.")
-				st.write("``")
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+					st.write('DataFrame not found.')
+					print(274)
+				st.write('``')
+				print(275)
 			except ZeroDivisionError:
 				pass
 			except Exception as e:
-				# st.error(e)
-				# st.subheader("⚠️Please upload a file⚠️")
 				pass
-
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline1 = {'column': f'{selected_column}'}
+				with open('drop_pipeline.pkl', 'wb') as f:
+					joblib.dump(pipeline1, f)
+					print(276)
 				st.session_state.df = modified_df
 				st.rerun()
-
-
-	elif preprocessing_action == "Drop Duplicates":
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+				print(277)
+	elif preprocessing_action == 'Drop Duplicates':
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			
 			drop_duplicates(modified_df)
-			st.write("Modified DataFrame:")
+			print(278)
+			st.write('Modified DataFrame:')
+			print(279)
 			st.write(modified_df)
-
+			print(280)
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline2 = {'action': 'drop_duplicates'}
+				with open('drop_dup_pipeline.pkl', 'wb') as f:
+					joblib.dump(pipeline2, f)
+					print(281)
 				st.session_state.df = modified_df
 				st.rerun()
-
-
-	elif preprocessing_action == "Treat Outliers":
-		outlier_method = st.radio("Select Outlier Treatment Method", ["Delete Outliers", "Winsorization"])
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+				print(282)
+	elif preprocessing_action == 'Treat Outliers':
+		outlier_method = st.radio('Select Outlier Treatment Method', [
+			'Delete Outliers', 'Winsorization'])
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			
-			modified_df = treat_outliers(modified_df, selected_column, outlier_method)
-			st.write("Modified DataFrame:")
+			if outlier_method == 'Winsorization':
+				lower_limit = st.slider('Select Lower Limit', min_value=0.0,
+					max_value=0.1, step=0.01, value=0.05)
+				upper_limit = st.slider('Select Upper Limit', min_value=0.0,
+					max_value=0.1, step=0.01, value=0.05)
+			else:
+				lower_limit = 0.05
+				upper_limit = 0.05
+			if outlier_method == 'Delete Outliers':
+				z_score_threshold = st.slider('Select Z-Score Threshold',
+					min_value=1.0, max_value=5.0, step=0.1, value=3.0)
+			else:
+				z_score_threshold = 3.0
+			modified_df = treat_outliers(modified_df, selected_column,
+				outlier_method, z_score_threshold, lower_limit, upper_limit)
+			st.write('Modified DataFrame:')
+			print(283)
 			st.write(modified_df)
+			print(284)
 			try:
 				if modified_df[selected_column].dtype == 'object':
 					col1, col2 = st.columns(2)
 					with col1:
 						unique_values = modified_df[selected_column].nunique()
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(285)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(286)
 						if unique_values <= 20:
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(287)
 						else:
-							st.write(f"  - Top 20 Unique Values:")
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
+							st.write(f'  - Top 20 Unique Values:')
+							print(288)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(289)
 					with col2:
 						plt.figure(figsize=(10, 6))
+						print(290)
 						try:
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(291)
 						except:
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(292)
 						plt.xticks(rotation=45)
+						print(293)
 						st.pyplot()
+						print(294)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2 = st.tabs(["Insights", "Donut chart"])
+						print(295)
+					with st.expander('More Info'):
+						tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
 						with tab1:
 							col7, col8, col9 = st.columns(3)
 							with col7:
-								# Insights
-								st.write("## Insights")
-								approximate_distinct_count = modified_df[selected_column].nunique()
-								approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-								missing = modified_df[selected_column].isna().sum()
-								missing_percent = (missing / len(modified_df)) * 100
-								memory_size = modified_df[selected_column].memory_usage(deep=True)
-								st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-								st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-								st.write(f"Missing: :green[{missing}]")
-								st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-								st.write(f"Memory Size: :green[{memory_size}]")
-
-								# st.header("An owl")
-								# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
+								st.write('## Insights')
+								print(296)
+								approximate_distinct_count = modified_df[
+									selected_column].nunique()
+								approximate_unique_percent = (
+									approximate_distinct_count / len(
+									modified_df) * 100)
+								missing = modified_df[selected_column].isna(
+									).sum()
+								missing_percent = missing / len(modified_df
+									) * 100
+								memory_size = modified_df[selected_column
+									].memory_usage(deep=True)
+								st.write(
+									f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+									)
+								print(297)
+								st.write(
+									f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+									)
+								print(298)
+								st.write(f'Missing: :green[{missing}]')
+								print(299)
+								st.write(
+									f'Missing (%): :green[{missing_percent:.2f}%]'
+									)
+								print(300)
+								st.write(f'Memory Size: :green[{memory_size}]')
+								print(301)
 							with col8:
-								# Mode and Standard Deviation
-								st.write("## Mode")
-								# if modified_df[selected_column].dtype == 'object':
-								mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-								st.write(f"Mode: :green[{mode}]")
-									# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-								# else:
-									# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-									# std_dev = modified_df[selected_column].astype(float).std()
-									# st.write(f"Mode: {mode}")
-									# st.write(f"Standard Deviation: {std_dev}")
+								st.write('## Mode')
+								print(302)
+								mode = modified_df[selected_column].mode(
+									).iloc[0]
+								st.write(f'Mode: :green[{mode}]')
+								print(303)
 							with col9:
-								# First 5 Sample Rows
-								st.write("## First 5 Sample Rows")
+								st.write('## First 5 Sample Rows')
+								print(304)
 								st.write(modified_df[selected_column].head())
-
+								print(305)
 						with tab2:
-							# Prepare data for donut chart
-							data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
+							data = limit_unique_values(modified_df[
+								selected_column]).value_counts().reset_index()
 							data.columns = [selected_column, 'count']
-
-							fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-							fig.update_traces(textposition='inside', textinfo='percent+label')
-							fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-							st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+							fig = px.pie(data, values='count', names=
+								selected_column, hole=0.5)
+							fig.update_traces(textposition='inside',
+								textinfo='percent+label')
+							print(306)
+							fig.update_layout(legend=dict(orientation='h',
+								yanchor='bottom', y=1.02, xanchor='right', x=1)
+								)
+							print(307)
+							st.plotly_chart(fig)
+							print(308)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
 					col3, col4 = st.columns(2)
 					with col3:
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(309)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(310)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(311)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(312)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(313)
 					with col4:
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(314)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(315)
 						st.pyplot()
+						print(316)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+						print(317)
+					with st.expander('More Info'):
+						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot',
+							'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								st.write("#### Basic Statistics")
-								insights = calculate_insights(modified_df[selected_column])
-								basic_stats = {key: value for key, value in insights.items() if key in [
-									'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
+								st.write('#### Basic Statistics')
+								print(318)
+								insights = calculate_insights(modified_df[
+									selected_column])
+								basic_stats = {key: value for key, value in
+									insights.items() if key in ['Mean',
+									'Median', 'Mode', 'Standard deviation',
+									'Variance', 'Kurtosis', 'Skewness']}
 								for key, value in basic_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-								st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-								st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(319)
+								st.write(
+									f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+									)
+								print(320)
+								st.write(
+									f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+									)
+								print(321)
+								st.write(
+									f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+									)
+								print(322)
 							with col5:
-								st.write("#### Percentiles")
-								descriptive_stats = insights.get('Descriptive statistics')
+								st.write('#### Percentiles')
+								print(323)
+								descriptive_stats = insights.get(
+									'Descriptive statistics')
 								if descriptive_stats is not None:
-									percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
+									percentiles = descriptive_stats.loc[[
+										'min', '25%', '50%', '75%', 'max']]
 									if '5%' in descriptive_stats.index:
 										percentiles['5%'] = descriptive_stats['5%']
 									if '95%' in descriptive_stats.index:
-										percentiles['95%'] = descriptive_stats['95%']
+										percentiles['95%'] = descriptive_stats[
+											'95%']
 									st.write(percentiles)
-
+									print(324)
 							with col6:
-								st.write("#### Additional Statistics")
-								additional_stats = {key: value for key, value in insights.items() if key in [
-									'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
+								st.write('#### Additional Statistics')
+								print(325)
+								additional_stats = {key: value for key,
+									value in insights.items() if key in [
+									'Distinct', 'Distinct (%)', 'Missing',
+									'Missing (%)', 'Zeros', 'Zeros (%)',
+									'Negative', 'Negative (%)']}
 								for key, value in additional_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-								# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-								# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-								st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-								st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-								st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(326)
+								st.write(
+									f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+									)
+								print(327)
+								st.write(
+									f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+									)
+								print(328)
+								st.write(
+									f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+									)
+								print(329)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
+							print(330)
 						with tab3:
 							plt.figure(figsize=(10, 6))
-							qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
+							print(331)
+							qqplot_data = sm.qqplot(modified_df[
+								selected_column], line='s').gca().lines
 							fig = go.Figure()
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[0].get_xdata(),
-								'y': qqplot_data[0].get_ydata(),
-								'mode': 'markers',
-								'marker': {'color': '#19d3f3'}
-							})
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[1].get_xdata(),
-								'y': qqplot_data[1].get_ydata(),
-								'mode': 'lines',
-								'line': {'color': '#636efa'}
-							})
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[0].get_xdata(), 'y':
+								qqplot_data[0].get_ydata(), 'mode':
+								'markers', 'marker': {'color': '#19d3f3'}})
+							print(332)
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[1].get_xdata(), 'y':
+								qqplot_data[1].get_ydata(), 'mode': 'lines',
+								'line': {'color': '#636efa'}})
+							print(333)
 							x_min = min(qqplot_data[0].get_xdata())
 							x_max = max(qqplot_data[0].get_xdata())
 							y_min = min(qqplot_data[0].get_ydata())
 							y_max = max(qqplot_data[0].get_ydata())
-							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-							fig.update_layout({
-								'title': f'QQ Plot for {selected_column}',
-								'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-								'yaxis': {'title': 'Sample Quantiles'},
-								'showlegend': False,
-								'width': 800,
-								'height': 700,
-							})
-							st.plotly_chart(fig)
-					st.write("---")
+							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[
+								y_min, y_max], mode='lines', line=dict(
+								color='red', width=2), name='Identity Line'))
+							print(334)
+							fig.update_layout({'title':
+								f'QQ Plot for {selected_column}', 'xaxis':
+								{'title': 'Theoretical Quantiles',
+								'zeroline': False}, 'yaxis': {'title':
+								'Sample Quantiles'}, 'showlegend': False,
+								'width': 800, 'height': 700})
+							print(335)
+							st.plotly_chart(fig)
+							print(336)
+					st.write('---')
+					print(337)
 				else:
-					st.write("DataFrame not found.")
-				st.write("``")
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+					st.write('DataFrame not found.')
+					print(338)
+				st.write('``')
+				print(339)
 			except ZeroDivisionError:
 				pass
 			except Exception as e:
 				st.error(e)
-				st.subheader("⚠️Please upload a file⚠️")
+				print(340)
+				st.subheader('⚠️Please upload a file⚠️')
+				print(341)
 				pass
-
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline3 = {'method': f'{outlier_method}', 'column':
+					f'{selected_column}', 'lower_limit': f'{lower_limit}',
+					'upper_limit': f'{upper_limit}'}
+				with open('outliers_for_col_pipeline.pkl', 'wb') as f:
+					joblib.dump(pipeline3, f)
+					print(342)
 				st.session_state.df = modified_df
 				st.rerun()
-
-
-
-	elif preprocessing_action == "Treat Outliers on full DF":
-		# outlier_method = st.radio("Select Outlier Treatment Method", ["Delete Outliers", "Winsorization"])
-		method = st.selectbox("Select Method to Treat Outliers", ["Delete Outliers", "Winsorization"])
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+				print(343)
+	elif preprocessing_action == 'Treat Outliers on full DF':
+		method = st.selectbox('Select Method to Treat Outliers', [
+			'Delete Outliers', 'Winsorization'])
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			# Z-score threshold input for "Delete Outliers"
-			if method == "Delete Outliers":
-				z_score_threshold = st.slider(
-					"Select Z-Score Threshold",
-					min_value=1.0,
-					max_value=5.0,
-					step=0.1,
-					value=3.0,
-				)
+			if method == 'Delete Outliers':
+				z_score_threshold = st.slider('Select Z-Score Threshold',
+					min_value=1.0, max_value=5.0, step=0.1, value=3.0)
 			else:
-				z_score_threshold = 3.0  # Default value if not used
-			if method == "Winsorization":
-
-				# method = st.selectbox("Select Method to Treat Outliers", ["Delete Outliers", "Winsorization"])
-				lower_limit = st.slider("Select Lower Limit:", min_value=0.0, max_value=0.1, step=0.01, value=0.05)
-				# Slider for selecting the upper limit for Winsorization
-				upper_limit = st.slider("Select Upper Limit:", min_value=0.0, max_value=0.1, step=0.01, value=0.05)
+				z_score_threshold = 3.0
+			if method == 'Winsorization':
+				lower_limit = st.slider('Select Lower Limit:', min_value=
+					0.0, max_value=0.1, step=0.01, value=0.05)
+				upper_limit = st.slider('Select Upper Limit:', min_value=
+					0.0, max_value=0.1, step=0.01, value=0.05)
 			else:
 				lower_limit = upper_limit = 0.05
-			modified_df = treat_outliers_full_df(modified_df, method, z_score_threshold=3, lower_limit=lower_limit, upper_limit=upper_limit)
-			st.write("Modified DataFrame:")
+			modified_df = treat_outliers_full_df(modified_df, method,
+				z_score_threshold=3, lower_limit=lower_limit, upper_limit=
+				upper_limit)
+			st.write('Modified DataFrame:')
+			print(344)
 			st.write(modified_df)
-
+			print(345)
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
 				st.session_state.df = modified_df
+				pipeline4 = {'method': f'{method}', 'lower_limit':
+					f'{lower_limit}', 'upper_limit': f'{upper_limit}',
+					'z_score_threshold': f'{z_score_threshold}'}
+				with open('outliers_for_full_df_pipeline.pkl', 'wb') as f:
+					joblib.dump(pipeline4, f)
+					print(346)
 				st.rerun()
-
-
-
-
-
-	elif preprocessing_action == "Treat Missing Values":
-		missing_method = st.radio("Select Missing Value Treatment Method", ["Delete Missing Values", "Mean Imputation", "Median Imputation", "Mode Imputation"])
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+				print(347)
+	elif preprocessing_action == 'Treat Missing Values':
+		missing_method = st.radio('Select Missing Value Treatment Method',
+			['Delete Missing Values', 'Mean Imputation',
+			'Median Imputation', 'Mode Imputation'])
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			modified_df = treat_missing_values(modified_df, selected_column, missing_method)
-			st.write("Modified DataFrame:")
+			modified_df = treat_missing_values(modified_df, selected_column,
+				missing_method)
+			st.write('Modified DataFrame:')
+			print(348)
 			st.write(modified_df)
+			print(349)
 			try:
 				if modified_df[selected_column].dtype == 'object':
 					col1, col2 = st.columns(2)
 					with col1:
 						unique_values = modified_df[selected_column].nunique()
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(350)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(351)
 						if unique_values <= 20:
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(352)
 						else:
-							st.write(f"  - Top 20 Unique Values:")
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
+							st.write(f'  - Top 20 Unique Values:')
+							print(353)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(354)
 					with col2:
 						plt.figure(figsize=(10, 6))
+						print(355)
 						try:
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(356)
 						except:
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(357)
 						plt.xticks(rotation=45)
+						print(358)
 						st.pyplot()
+						print(359)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2 = st.tabs(["Insights", "Donut chart"])
+						print(360)
+					with st.expander('More Info'):
+						tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
 						with tab1:
 							col7, col8, col9 = st.columns(3)
 							with col7:
-								# Insights
-								st.write("## Insights")
-								approximate_distinct_count = modified_df[selected_column].nunique()
-								approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-								missing = modified_df[selected_column].isna().sum()
-								missing_percent = (missing / len(modified_df)) * 100
-								memory_size = modified_df[selected_column].memory_usage(deep=True)
-								st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-								st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-								st.write(f"Missing: :green[{missing}]")
-								st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-								st.write(f"Memory Size: :green[{memory_size}]")
-
-								# st.header("An owl")
-								# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
+								st.write('## Insights')
+								print(361)
+								approximate_distinct_count = modified_df[
+									selected_column].nunique()
+								approximate_unique_percent = (
+									approximate_distinct_count / len(
+									modified_df) * 100)
+								missing = modified_df[selected_column].isna(
+									).sum()
+								missing_percent = missing / len(modified_df
+									) * 100
+								memory_size = modified_df[selected_column
+									].memory_usage(deep=True)
+								st.write(
+									f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+									)
+								print(362)
+								st.write(
+									f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+									)
+								print(363)
+								st.write(f'Missing: :green[{missing}]')
+								print(364)
+								st.write(
+									f'Missing (%): :green[{missing_percent:.2f}%]'
+									)
+								print(365)
+								st.write(f'Memory Size: :green[{memory_size}]')
+								print(366)
 							with col8:
-								# Mode and Standard Deviation
-								st.write("## Mode")
-								# if modified_df[selected_column].dtype == 'object':
-								mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-								st.write(f"Mode: :green[{mode}]")
-									# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-								# else:
-									# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-									# std_dev = modified_df[selected_column].astype(float).std()
-									# st.write(f"Mode: {mode}")
-									# st.write(f"Standard Deviation: {std_dev}")
+								st.write('## Mode')
+								print(367)
+								mode = modified_df[selected_column].mode(
+									).iloc[0]
+								st.write(f'Mode: :green[{mode}]')
+								print(368)
 							with col9:
-								# First 5 Sample Rows
-								st.write("## First 5 Sample Rows")
+								st.write('## First 5 Sample Rows')
+								print(369)
 								st.write(modified_df[selected_column].head())
-
+								print(370)
 						with tab2:
-							# Prepare data for donut chart
-							data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
+							data = limit_unique_values(modified_df[
+								selected_column]).value_counts().reset_index()
 							data.columns = [selected_column, 'count']
-
-							fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-							fig.update_traces(textposition='inside', textinfo='percent+label')
-							fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-							st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+							fig = px.pie(data, values='count', names=
+								selected_column, hole=0.5)
+							fig.update_traces(textposition='inside',
+								textinfo='percent+label')
+							print(371)
+							fig.update_layout(legend=dict(orientation='h',
+								yanchor='bottom', y=1.02, xanchor='right', x=1)
+								)
+							print(372)
+							st.plotly_chart(fig)
+							print(373)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
 					col3, col4 = st.columns(2)
 					with col3:
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(374)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(375)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(376)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(377)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(378)
 					with col4:
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(379)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(380)
 						st.pyplot()
+						print(381)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+						print(382)
+					with st.expander('More Info'):
+						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot',
+							'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								st.write("#### Basic Statistics")
-								insights = calculate_insights(modified_df[selected_column])
-								basic_stats = {key: value for key, value in insights.items() if key in [
-									'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
+								st.write('#### Basic Statistics')
+								print(383)
+								insights = calculate_insights(modified_df[
+									selected_column])
+								basic_stats = {key: value for key, value in
+									insights.items() if key in ['Mean',
+									'Median', 'Mode', 'Standard deviation',
+									'Variance', 'Kurtosis', 'Skewness']}
 								for key, value in basic_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-								st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-								st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(384)
+								st.write(
+									f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+									)
+								print(385)
+								st.write(
+									f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+									)
+								print(386)
+								st.write(
+									f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+									)
+								print(387)
 							with col5:
-								st.write("#### Percentiles")
-								descriptive_stats = insights.get('Descriptive statistics')
+								st.write('#### Percentiles')
+								print(388)
+								descriptive_stats = insights.get(
+									'Descriptive statistics')
 								if descriptive_stats is not None:
-									percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
+									percentiles = descriptive_stats.loc[[
+										'min', '25%', '50%', '75%', 'max']]
 									if '5%' in descriptive_stats.index:
 										percentiles['5%'] = descriptive_stats['5%']
 									if '95%' in descriptive_stats.index:
-										percentiles['95%'] = descriptive_stats['95%']
+										percentiles['95%'] = descriptive_stats[
+											'95%']
 									st.write(percentiles)
-
+									print(389)
 							with col6:
-								st.write("#### Additional Statistics")
-								additional_stats = {key: value for key, value in insights.items() if key in [
-									'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
+								st.write('#### Additional Statistics')
+								print(390)
+								additional_stats = {key: value for key,
+									value in insights.items() if key in [
+									'Distinct', 'Distinct (%)', 'Missing',
+									'Missing (%)', 'Zeros', 'Zeros (%)',
+									'Negative', 'Negative (%)']}
 								for key, value in additional_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-								# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-								# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-								st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-								st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-								st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(391)
+								st.write(
+									f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+									)
+								print(392)
+								st.write(
+									f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+									)
+								print(393)
+								st.write(
+									f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+									)
+								print(394)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
+							print(395)
 						with tab3:
 							plt.figure(figsize=(10, 6))
-							qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
+							print(396)
+							qqplot_data = sm.qqplot(modified_df[
+								selected_column], line='s').gca().lines
 							fig = go.Figure()
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[0].get_xdata(),
-								'y': qqplot_data[0].get_ydata(),
-								'mode': 'markers',
-								'marker': {'color': '#19d3f3'}
-							})
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[1].get_xdata(),
-								'y': qqplot_data[1].get_ydata(),
-								'mode': 'lines',
-								'line': {'color': '#636efa'}
-							})
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[0].get_xdata(), 'y':
+								qqplot_data[0].get_ydata(), 'mode':
+								'markers', 'marker': {'color': '#19d3f3'}})
+							print(397)
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[1].get_xdata(), 'y':
+								qqplot_data[1].get_ydata(), 'mode': 'lines',
+								'line': {'color': '#636efa'}})
+							print(398)
 							x_min = min(qqplot_data[0].get_xdata())
 							x_max = max(qqplot_data[0].get_xdata())
 							y_min = min(qqplot_data[0].get_ydata())
 							y_max = max(qqplot_data[0].get_ydata())
-							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-							fig.update_layout({
-								'title': f'QQ Plot for {selected_column}',
-								'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-								'yaxis': {'title': 'Sample Quantiles'},
-								'showlegend': False,
-								'width': 800,
-								'height': 700,
-							})
-							st.plotly_chart(fig)
-					st.write("---")
+							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[
+								y_min, y_max], mode='lines', line=dict(
+								color='red', width=2), name='Identity Line'))
+							print(399)
+							fig.update_layout({'title':
+								f'QQ Plot for {selected_column}', 'xaxis':
+								{'title': 'Theoretical Quantiles',
+								'zeroline': False}, 'yaxis': {'title':
+								'Sample Quantiles'}, 'showlegend': False,
+								'width': 800, 'height': 700})
+							print(400)
+							st.plotly_chart(fig)
+							print(401)
+					st.write('---')
+					print(402)
 				else:
-					st.write("DataFrame not found.")
-				st.write("``")
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+					st.write('DataFrame not found.')
+					print(403)
+				st.write('``')
+				print(404)
 			except ZeroDivisionError:
 				pass
 			except Exception as e:
 				st.error(e)
-				st.subheader("⚠️Please upload a file⚠️")
+				print(405)
+				st.subheader('⚠️Please upload a file⚠️')
+				print(406)
 				pass
-
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline5 = {'method': f'{missing_method}', 'column':
+					f'{selected_column}'}
+				with open('treat_missing_vaues_for_col.pkl', 'wb') as f:
+					joblib.dump(pipeline5, f)
+					print(407)
 				st.session_state.df = modified_df
 				st.rerun()
-
-
-	elif preprocessing_action == "Traat Missing from full DF":
-		st.write("hi")
-		# Determine numeric and categorical columns
+				print(408)
+	elif preprocessing_action == 'Traat Missing from full DF':
+		st.write('hi')
+		print(409)
 		numeric_columns = df.select_dtypes(include=np.number).columns
-		categorical_columns = df.select_dtypes(include=['object', 'category']).columns
-		
-		# Ask user for treatment options for numeric columns
-		numeric_treatment = st.selectbox("Select treatment for missing values in numeric columns", ["Mean", "Median", "Mode", "Random"])
+		categorical_columns = df.select_dtypes(include=['object', 'category']
+			).columns
+		numeric_treatment = st.selectbox(
+			'Select treatment for missing values in numeric columns', [
+			'Mean', 'Median', 'Mode', 'Random'])
 		numeric_strategy = None
-		if numeric_treatment == "Random":
-			numeric_strategy = st.text_input("Enter strategy for random value generation (e.g., 'uniform', 'normal')")
-
-		# Ask user for treatment options for categorical columns
-		categorical_treatment = st.selectbox("Select treatment for missing values in categorical columns", ["Mode", "Random"])
+		if numeric_treatment == 'Random':
+			numeric_strategy = st.text_input(
+				"Enter strategy for random value generation (e.g., 'uniform', 'normal')"
+				)
+		categorical_treatment = st.selectbox(
+			'Select treatment for missing values in categorical columns', [
+			'Mode', 'Random'])
 		categorical_strategy = None
-		if categorical_treatment == "Random":
-			categorical_strategy = st.text_input("Enter strategy for random value generation (e.g., 'uniform', 'normal')")
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+		if categorical_treatment == 'Random':
+			categorical_strategy = st.text_input(
+				"Enter strategy for random value generation (e.g., 'uniform', 'normal')"
+				)
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			# Apply treatment for numeric columns
 			for column in numeric_columns:
-				if numeric_treatment == "Mean":
-					modified_df[column].fillna(modified_df[column].mean(), inplace=True)
-				elif numeric_treatment == "Median":
-					modified_df[column].fillna(modified_df[column].median(), inplace=True)
-				elif numeric_treatment == "Mode":
-					modified_df[column].fillna(modified_df[column].mode()[0], inplace=True)
-				elif numeric_treatment == "Random":
-					modified_df[column].fillna(np.random.RandomState().choice(modified_df[column].dropna()), inplace=True)
-			# Apply treatment for categorical columns
+				if numeric_treatment == 'Mean':
+					modified_df[column].fillna(modified_df[column].mean(),
+						inplace=True)
+					print(410)
+				elif numeric_treatment == 'Median':
+					modified_df[column].fillna(modified_df[column].median(),
+						inplace=True)
+					print(411)
+				elif numeric_treatment == 'Mode':
+					modified_df[column].fillna(modified_df[column].mode()[0
+						], inplace=True)
+					print(412)
+				elif numeric_treatment == 'Random':
+					modified_df[column].fillna(np.random.RandomState().
+						choice(modified_df[column].dropna()), inplace=True)
+					print(413)
 			for column in categorical_columns:
-				if categorical_treatment == "Mode":
-					modified_df[column].fillna(modified_df[column].mode()[0], inplace=True)
-				elif categorical_treatment == "Random":
-					modified_df[column].fillna(np.random.RandomState().choice(modified_df[column].dropna()), inplace=True)
-
-			st.write("Modified DataFrame:")
+				if categorical_treatment == 'Mode':
+					modified_df[column].fillna(modified_df[column].mode()[0
+						], inplace=True)
+					print(414)
+				elif categorical_treatment == 'Random':
+					modified_df[column].fillna(np.random.RandomState().
+						choice(modified_df[column].dropna()), inplace=True)
+					print(415)
+			st.write('Modified DataFrame:')
+			print(416)
 			st.write(modified_df)
+			print(417)
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				modified_df.to_csv('data.csv', index=False)
-				# st.session_state.df = modified_df
+				pipeline6 = {'numeric_treatment': f'{numeric_treatment}',
+					'numeric_strategy': f'{numeric_strategy}',
+					'categorical_treatment': f'{numeric_strategy}',
+					'categorical_strategy': f'{categorical_strategy}'}
+				with open('treat_missing_vaues_in_full_df.pkl', 'wb') as f:
+					joblib.dump(pipeline6, f)
+					print(418)
 				st.session_state.df = modified_df
 				st.rerun()
-
-
-	elif preprocessing_action == "Apply Transformation":
-		transformation_method = st.selectbox("Select Transformation Technique", ["Log Transformation", "Exponential Transformation", "Square Root Transformation", "Box-Cox Transformation", "Yeo-Johnson Transformation"])
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+				print(419)
+	elif preprocessing_action == 'Apply Transformation':
+		transformation_method = st.selectbox('Select Transformation Technique',
+			['Log Transformation', 'Exponential Transformation',
+			'Square Root Transformation', 'Box-Cox Transformation',
+			'Yeo-Johnson Transformation'])
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			modified_df = apply_transformation(modified_df, selected_column, transformation_method)
-			st.write("Modified DataFrame:")
+			modified_df = apply_transformation(modified_df, selected_column,
+				transformation_method)
+			st.write('Modified DataFrame:')
+			print(420)
 			st.write(modified_df)
+			print(421)
 			try:
 				if modified_df[selected_column].dtype == 'object':
 					col1, col2 = st.columns(2)
 					with col1:
 						unique_values = modified_df[selected_column].nunique()
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(422)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(423)
 						if unique_values <= 20:
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(424)
 						else:
-							st.write(f"  - Top 20 Unique Values:")
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
+							st.write(f'  - Top 20 Unique Values:')
+							print(425)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(426)
 					with col2:
 						plt.figure(figsize=(10, 6))
+						print(427)
 						try:
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(428)
 						except:
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(429)
 						plt.xticks(rotation=45)
+						print(430)
 						st.pyplot()
+						print(431)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2 = st.tabs(["Insights", "Donut chart"])
+						print(432)
+					with st.expander('More Info'):
+						tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
 						with tab1:
 							col7, col8, col9 = st.columns(3)
 							with col7:
-								# Insights
-								st.write("## Insights")
-								approximate_distinct_count = modified_df[selected_column].nunique()
-								approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-								missing = modified_df[selected_column].isna().sum()
-								missing_percent = (missing / len(modified_df)) * 100
-								memory_size = modified_df[selected_column].memory_usage(deep=True)
-								st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-								st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-								st.write(f"Missing: :green[{missing}]")
-								st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-								st.write(f"Memory Size: :green[{memory_size}]")
-
-								# st.header("An owl")
-								# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
+								st.write('## Insights')
+								print(433)
+								approximate_distinct_count = modified_df[
+									selected_column].nunique()
+								approximate_unique_percent = (
+									approximate_distinct_count / len(
+									modified_df) * 100)
+								missing = modified_df[selected_column].isna(
+									).sum()
+								missing_percent = missing / len(modified_df
+									) * 100
+								memory_size = modified_df[selected_column
+									].memory_usage(deep=True)
+								st.write(
+									f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+									)
+								print(434)
+								st.write(
+									f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+									)
+								print(435)
+								st.write(f'Missing: :green[{missing}]')
+								print(436)
+								st.write(
+									f'Missing (%): :green[{missing_percent:.2f}%]'
+									)
+								print(437)
+								st.write(f'Memory Size: :green[{memory_size}]')
+								print(438)
 							with col8:
-								# Mode and Standard Deviation
-								st.write("## Mode")
-								# if modified_df[selected_column].dtype == 'object':
-								mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-								st.write(f"Mode: :green[{mode}]")
-									# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-								# else:
-									# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-									# std_dev = modified_df[selected_column].astype(float).std()
-									# st.write(f"Mode: {mode}")
-									# st.write(f"Standard Deviation: {std_dev}")
+								st.write('## Mode')
+								print(439)
+								mode = modified_df[selected_column].mode(
+									).iloc[0]
+								st.write(f'Mode: :green[{mode}]')
+								print(440)
 							with col9:
-								# First 5 Sample Rows
-								st.write("## First 5 Sample Rows")
+								st.write('## First 5 Sample Rows')
+								print(441)
 								st.write(modified_df[selected_column].head())
-
+								print(442)
 						with tab2:
-							# Prepare data for donut chart
-							data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
+							data = limit_unique_values(modified_df[
+								selected_column]).value_counts().reset_index()
 							data.columns = [selected_column, 'count']
-
-							fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-							fig.update_traces(textposition='inside', textinfo='percent+label')
-							fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-							st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+							fig = px.pie(data, values='count', names=
+								selected_column, hole=0.5)
+							fig.update_traces(textposition='inside',
+								textinfo='percent+label')
+							print(443)
+							fig.update_layout(legend=dict(orientation='h',
+								yanchor='bottom', y=1.02, xanchor='right', x=1)
+								)
+							print(444)
+							st.plotly_chart(fig)
+							print(445)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
 					col3, col4 = st.columns(2)
 					with col3:
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(446)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(447)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(448)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(449)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(450)
 					with col4:
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(451)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(452)
 						st.pyplot()
+						print(453)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+						print(454)
+					with st.expander('More Info'):
+						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot',
+							'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								st.write("#### Basic Statistics")
-								insights = calculate_insights(modified_df[selected_column])
-								basic_stats = {key: value for key, value in insights.items() if key in [
-									'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
+								st.write('#### Basic Statistics')
+								print(455)
+								insights = calculate_insights(modified_df[
+									selected_column])
+								basic_stats = {key: value for key, value in
+									insights.items() if key in ['Mean',
+									'Median', 'Mode', 'Standard deviation',
+									'Variance', 'Kurtosis', 'Skewness']}
 								for key, value in basic_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-								st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-								st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(456)
+								st.write(
+									f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+									)
+								print(457)
+								st.write(
+									f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+									)
+								print(458)
+								st.write(
+									f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+									)
+								print(459)
 							with col5:
-								st.write("#### Percentiles")
-								descriptive_stats = insights.get('Descriptive statistics')
+								st.write('#### Percentiles')
+								print(460)
+								descriptive_stats = insights.get(
+									'Descriptive statistics')
 								if descriptive_stats is not None:
-									percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
+									percentiles = descriptive_stats.loc[[
+										'min', '25%', '50%', '75%', 'max']]
 									if '5%' in descriptive_stats.index:
 										percentiles['5%'] = descriptive_stats['5%']
 									if '95%' in descriptive_stats.index:
-										percentiles['95%'] = descriptive_stats['95%']
+										percentiles['95%'] = descriptive_stats[
+											'95%']
 									st.write(percentiles)
-
+									print(461)
 							with col6:
-								st.write("#### Additional Statistics")
-								additional_stats = {key: value for key, value in insights.items() if key in [
-									'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
+								st.write('#### Additional Statistics')
+								print(462)
+								additional_stats = {key: value for key,
+									value in insights.items() if key in [
+									'Distinct', 'Distinct (%)', 'Missing',
+									'Missing (%)', 'Zeros', 'Zeros (%)',
+									'Negative', 'Negative (%)']}
 								for key, value in additional_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-								# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-								# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-								st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-								st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-								st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(463)
+								st.write(
+									f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+									)
+								print(464)
+								st.write(
+									f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+									)
+								print(465)
+								st.write(
+									f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+									)
+								print(466)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
+							print(467)
 						with tab3:
 							plt.figure(figsize=(10, 6))
-							qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
+							print(468)
+							qqplot_data = sm.qqplot(modified_df[
+								selected_column], line='s').gca().lines
 							fig = go.Figure()
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[0].get_xdata(),
-								'y': qqplot_data[0].get_ydata(),
-								'mode': 'markers',
-								'marker': {'color': '#19d3f3'}
-							})
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[1].get_xdata(),
-								'y': qqplot_data[1].get_ydata(),
-								'mode': 'lines',
-								'line': {'color': '#636efa'}
-							})
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[0].get_xdata(), 'y':
+								qqplot_data[0].get_ydata(), 'mode':
+								'markers', 'marker': {'color': '#19d3f3'}})
+							print(469)
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[1].get_xdata(), 'y':
+								qqplot_data[1].get_ydata(), 'mode': 'lines',
+								'line': {'color': '#636efa'}})
+							print(470)
 							x_min = min(qqplot_data[0].get_xdata())
 							x_max = max(qqplot_data[0].get_xdata())
 							y_min = min(qqplot_data[0].get_ydata())
 							y_max = max(qqplot_data[0].get_ydata())
-							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-							fig.update_layout({
-								'title': f'QQ Plot for {selected_column}',
-								'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-								'yaxis': {'title': 'Sample Quantiles'},
-								'showlegend': False,
-								'width': 800,
-								'height': 700,
-							})
-							st.plotly_chart(fig)
-					st.write("---")
+							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[
+								y_min, y_max], mode='lines', line=dict(
+								color='red', width=2), name='Identity Line'))
+							print(471)
+							fig.update_layout({'title':
+								f'QQ Plot for {selected_column}', 'xaxis':
+								{'title': 'Theoretical Quantiles',
+								'zeroline': False}, 'yaxis': {'title':
+								'Sample Quantiles'}, 'showlegend': False,
+								'width': 800, 'height': 700})
+							print(472)
+							st.plotly_chart(fig)
+							print(473)
+					st.write('---')
+					print(474)
 				else:
-					st.write("DataFrame not found.")
-				st.write("``")
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+					st.write('DataFrame not found.')
+					print(475)
+				st.write('``')
+				print(476)
 			except ZeroDivisionError:
 				pass
 			except Exception as e:
 				st.error(e)
-				st.subheader("⚠️Please upload a file⚠️")
+				print(477)
+				st.subheader('⚠️Please upload a file⚠️')
+				print(478)
 				pass
-
-	# col11, col22 = st.columns(2)
-	# with col11:
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline7 = {
+					"method": f'{transformation_method}',
+					"column_name": f'{selected_column}',
+				}
+
+				# Save the pipeline to a serialized object
+				with open("apply_transformation_on_col.pkl", "wb") as f:
+					joblib.dump(pipeline7, f)
 				st.session_state.df = modified_df
 				st.rerun()
 
-	elif preprocessing_action == "Create Dummy Variables":
-		encoding_method = st.selectbox("Select encoding method", ["One-Hot Encoding", "Label Encoding"])
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+	elif preprocessing_action == 'Create Dummy Variables':
+		encoding_method = st.selectbox('Select encoding method', [
+			'One-Hot Encoding', 'Label Encoding'])
+		opt = st.toggle('drop_first')
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			modified_df = create_dummy_variables(modified_df, encoding_method)
-			st.write("Modified DataFrame:")
+			modified_df = create_dummy_variables(modified_df, encoding_method, opt)
+			st.write('Modified DataFrame:')
+			print(480)
 			st.write(modified_df)
+			print(481)
 			try:
+				print(110000)
 				if modified_df[selected_column].dtype == 'object':
-					col1, col2 = st.columns(2)
-					with col1:
-						unique_values = modified_df[selected_column].nunique()
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
-						if unique_values <= 20:
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
-						else:
-							st.write(f"  - Top 20 Unique Values:")
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
-					with col2:
-						plt.figure(figsize=(10, 6))
-						try:
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
-						except:
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
-						plt.xticks(rotation=45)
-						st.pyplot()
-						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2 = st.tabs(["Insights", "Donut chart"])
-						with tab1:
-							col7, col8, col9 = st.columns(3)
-							with col7:
-								# Insights
-								st.write("## Insights")
-								approximate_distinct_count = modified_df[selected_column].nunique()
-								approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-								missing = modified_df[selected_column].isna().sum()
-								missing_percent = (missing / len(modified_df)) * 100
-								memory_size = modified_df[selected_column].memory_usage(deep=True)
-								st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-								st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-								st.write(f"Missing: :green[{missing}]")
-								st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-								st.write(f"Memory Size: :green[{memory_size}]")
-
-								# st.header("An owl")
-								# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-							with col8:
-								# Mode and Standard Deviation
-								st.write("## Mode")
-								# if modified_df[selected_column].dtype == 'object':
-								mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-								st.write(f"Mode: :green[{mode}]")
-									# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-								# else:
-									# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-									# std_dev = modified_df[selected_column].astype(float).std()
-									# st.write(f"Mode: {mode}")
-									# st.write(f"Standard Deviation: {std_dev}")
-							with col9:
-								# First 5 Sample Rows
-								st.write("## First 5 Sample Rows")
-								st.write(modified_df[selected_column].head())
-
-						with tab2:
-							# Prepare data for donut chart
-							data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
-							data.columns = [selected_column, 'count']
-
-							fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-							fig.update_traces(textposition='inside', textinfo='percent+label')
-							fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-							st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+					print(210000)
+				# 	col1, col2 = st.columns(2)
+				# 	with col1:
+				# 		unique_values = modified_df[selected_column].nunique()
+				# 		st.write(
+				# 			f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+				# 			)
+				# 		print(482)
+				# 		st.write(
+				# 			f'  - Number of Unique Values: :green[{unique_values}]'
+				# 			)
+				# 		print(483)
+				# 		if unique_values <= 20:
+				# 			st.write(
+				# 				f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+				# 				)
+				# 			print(484)
+				# 		else:
+				# 			st.write(f'  - Top 20 Unique Values:')
+				# 			print(485)
+				# 			st.write(
+				# 				f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+				# 				)
+				# 			print(486)
+				# 	with col2:
+				# 		plt.figure(figsize=(10, 6))
+				# 		print(487)
+				# 		try:
+				# 			sns.countplot(x=limit_unique_values(modified_df
+				# 				[selected_column]), data=modified_df, color
+				# 				='green')
+				# 			print(488)
+				# 		except:
+				# 			sns.countplot(x=modified_df[selected_column],
+				# 				data=modified_df, color='green')
+				# 			print(489)
+				# 		plt.xticks(rotation=45)
+				# 		print(490)
+				# 		st.pyplot()
+				# 		print(491)
+				# 		plt.close()
+				# 		print(492)
+				# 	with st.expander('More Info'):
+				# 		tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
+				# 		with tab1:
+				# 			col7, col8, col9 = st.columns(3)
+				# 			with col7:
+				# 				st.write('## Insights')
+				# 				print(493)
+				# 				approximate_distinct_count = modified_df[
+				# 					selected_column].nunique()
+				# 				approximate_unique_percent = (
+				# 					approximate_distinct_count / len(
+				# 					modified_df) * 100)
+				# 				missing = modified_df[selected_column].isna(
+				# 					).sum()
+				# 				missing_percent = missing / len(modified_df
+				# 					) * 100
+				# 				memory_size = modified_df[selected_column
+				# 					].memory_usage(deep=True)
+				# 				st.write(
+				# 					f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+				# 					)
+				# 				print(494)
+				# 				st.write(
+				# 					f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+				# 					)
+				# 				print(495)
+				# 				st.write(f'Missing: :green[{missing}]')
+				# 				print(496)
+				# 				st.write(
+				# 					f'Missing (%): :green[{missing_percent:.2f}%]'
+				# 					)
+				# 				print(497)
+				# 				st.write(f'Memory Size: :green[{memory_size}]')
+				# 				print(498)
+				# 			with col8:
+				# 				st.write('## Mode')
+				# 				print(499)
+				# 				mode = modified_df[selected_column].mode(
+				# 					).iloc[0]
+				# 				st.write(f'Mode: :green[{mode}]')
+				# 				print(500)
+				# 			with col9:
+				# 				st.write('## First 5 Sample Rows')
+				# 				print(501)
+				# 				st.write(modified_df[selected_column].head())
+				# 				print(502)
+				# 		with tab2:
+				# 			data = limit_unique_values(modified_df[
+				# 				selected_column]).value_counts().reset_index()
+				# 			data.columns = [selected_column, 'count']
+				# 			fig = px.pie(data, values='count', names=
+				# 				selected_column, hole=0.5)
+				# 			fig.update_traces(textposition='inside',
+				# 				textinfo='percent+label')
+				# 			print(503)
+				# 			fig.update_layout(legend=dict(orientation='h',
+				# 				yanchor='bottom', y=1.02, xanchor='right', x=1)
+				# 				)
+				# 			print(504)
+				# 			st.plotly_chart(fig)
+				# 			print(505)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
+					print(10000)
+					modified_df.to_csv("heha.csv")
 					col3, col4 = st.columns(2)
-					with col3:
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+				# 	with col3:
+				# 		st.write(
+				# 			f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+				# 			)
+				# # 		print(506)
+				# 		st.write(
+				# 			f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+				# 			)
+				# 		print(507)
+				# 		st.write(
+				# 			f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+				# 			)
+				# 		print(508)
+				# 		st.write(
+				# 			f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+				# 			)
+				# 		print(509)
+				# 		st.write(
+				# 			f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+				# 			)
+				# 		print(510)
 					with col4:
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(511)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(512)
 						st.pyplot()
+						print(513)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+						print(514)
+					with st.expander('More Info'):
+						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot', 'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								st.write("#### Basic Statistics")
-								insights = calculate_insights(modified_df[selected_column])
-								basic_stats = {key: value for key, value in insights.items() if key in [
-									'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
-								for key, value in basic_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-								st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-								st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
+								# st.write('#### Basic Statistics')
+								print(515)
+								# insights = calculate_insights(modified_df[selected_column])
+								# basic_stats = {key: value for key, value in
+								# 	insights.items() if key in ['Mean',
+								# 	'Median', 'Mode', 'Standard deviation',
+								# 	'Variance', 'Kurtosis', 'Skewness']}
+								# for key, value in basic_stats.items():
+									# st.write(f'**{key}:** :green[{value:.3f}]')
+									# print(516)
+								# st.write(
+								# 	f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+								# 	)
+								# print(517)
+								# st.write(
+								# 	f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+								# 	)
+								# print(518)
+								# st.write(
+								# 	f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+								# 	)
+								print(519)
 							with col5:
-								st.write("#### Percentiles")
-								descriptive_stats = insights.get('Descriptive statistics')
-								if descriptive_stats is not None:
-									percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
-									if '5%' in descriptive_stats.index:
-										percentiles['5%'] = descriptive_stats['5%']
-									if '95%' in descriptive_stats.index:
-										percentiles['95%'] = descriptive_stats['95%']
-									st.write(percentiles)
-
+								st.write('#### Percentiles')
+								print(520)
+								# descriptive_stats = insights.get(
+								# 	'Descriptive statistics')
+								# if descriptive_stats is not None:
+								# 	percentiles = descriptive_stats.loc[[
+								# 		'min', '25%', '50%', '75%', 'max']]
+								# 	if '5%' in descriptive_stats.index:
+								# 		percentiles['5%'] = descriptive_stats['5%']
+								# 	if '95%' in descriptive_stats.index:
+								# 		percentiles['95%'] = descriptive_stats[
+								# 			'95%']
+								# 	st.write(percentiles)
+									# print(521)
 							with col6:
-								st.write("#### Additional Statistics")
-								additional_stats = {key: value for key, value in insights.items() if key in [
-									'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
-								for key, value in additional_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-								# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-								# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-								st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-								st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-								st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+								st.write('#### Additional Statistics')
+								# print(522)
+								# additional_stats = {key: value for key,
+								# 	value in insights.items() if key in [
+								# 	'Distinct', 'Distinct (%)', 'Missing',
+								# 	'Missing (%)', 'Zeros', 'Zeros (%)',
+								# 	'Negative', 'Negative (%)']}
+								# for key, value in additional_stats.items():
+								# # 	st.write(f'**{key}:** :green[{value:.3f}]')
+									# print(523)
+								# st.write(
+								# 	f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+								# 	)
+								# print(524)
+								# st.write(
+								# 	f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+								# 	)
+								# print(525)
+								# st.write(
+								# 	f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+								# 	)
+								print(526)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
+							print(527)
 						with tab3:
 							plt.figure(figsize=(10, 6))
-							qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
+							print(528)
+							qqplot_data = sm.qqplot(modified_df[
+								selected_column], line='s').gca().lines
 							fig = go.Figure()
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[0].get_xdata(),
-								'y': qqplot_data[0].get_ydata(),
-								'mode': 'markers',
-								'marker': {'color': '#19d3f3'}
-							})
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[1].get_xdata(),
-								'y': qqplot_data[1].get_ydata(),
-								'mode': 'lines',
-								'line': {'color': '#636efa'}
-							})
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[0].get_xdata(), 'y':
+								qqplot_data[0].get_ydata(), 'mode':
+								'markers', 'marker': {'color': '#19d3f3'}})
+							print(529)
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[1].get_xdata(), 'y':
+								qqplot_data[1].get_ydata(), 'mode': 'lines',
+								'line': {'color': '#636efa'}})
+							print(530)
 							x_min = min(qqplot_data[0].get_xdata())
 							x_max = max(qqplot_data[0].get_xdata())
 							y_min = min(qqplot_data[0].get_ydata())
 							y_max = max(qqplot_data[0].get_ydata())
-							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-							fig.update_layout({
-								'title': f'QQ Plot for {selected_column}',
-								'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-								'yaxis': {'title': 'Sample Quantiles'},
-								'showlegend': False,
-								'width': 800,
-								'height': 700,
-							})
-							st.plotly_chart(fig)
-					st.write("---")
+							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[
+								y_min, y_max], mode='lines', line=dict(
+								color='red', width=2), name='Identity Line'))
+							print(531)
+							fig.update_layout({'title':
+								f'QQ Plot for {str(selected_column)}', 'xaxis':
+								{'title': 'Theoretical Quantiles',
+								'zeroline': False}, 'yaxis': {'title':
+								'Sample Quantiles'}, 'showlegend': False,
+								'width': 800, 'height': 700})
+							print(532)
+							st.plotly_chart(fig)
+							print(533)
+					st.write('---')
+					print(534)
 				else:
-					st.write("DataFrame not found.")
-				st.write("``")
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+					st.write('DataFrame not found.')
+					print(535)
+				st.write('``')
+				print(536)
 			except ZeroDivisionError:
 				pass
 			except Exception as e:
-				# st.error(e)
-				# st.subheader("⚠️Please upload a file⚠️")
 				pass
-
-	# col11, col22 = st.columns(2)
-	# with col11:
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline8 = {
+					"method": f'{encoding_method}',
+					"param": opt
+				}
+
+				# Save the pipeline to a serialized object
+				with open("apply_encoding_on_df.pkl", "wb") as f:
+					joblib.dump(pipeline8, f)
 				st.session_state.df = modified_df
 				st.rerun()
+				print(537)
 
-
-	elif preprocessing_action == "Column to Dummy Variable":
-		encoding_method = st.selectbox("Select encoding method", ["One-Hot Encoding", "Label Encoding"])
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+	elif preprocessing_action == 'Column to Dummy Variable':
+		encoding_method = st.selectbox('Select encoding method', [
+			'One-Hot Encoding', 'Label Encoding'])
+		opt = st.toggle('drop_first')
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			modified_df = create_dummy_variables_for_col(modified_df, selected_column, encoding_method)
-			st.write("Modified DataFrame:")
+			modified_df = create_dummy_variables_for_col(modified_df,
+				selected_column, encoding_method, opt)
+			st.write('Modified DataFrame:')
+			print(538)
 			st.write(modified_df)
+			print(539)
 			try:
 				if modified_df[selected_column].dtype == 'object':
 					col1, col2 = st.columns(2)
 					with col1:
 						unique_values = modified_df[selected_column].nunique()
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(540)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(541)
 						if unique_values <= 20:
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(542)
 						else:
-							st.write(f"  - Top 20 Unique Values:")
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
+							st.write(f'  - Top 20 Unique Values:')
+							print(543)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(544)
 					with col2:
 						plt.figure(figsize=(10, 6))
+						print(545)
 						try:
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(546)
 						except:
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(547)
 						plt.xticks(rotation=45)
+						print(548)
 						st.pyplot()
+						print(549)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2 = st.tabs(["Insights", "Donut chart"])
+						print(550)
+					with st.expander('More Info'):
+						tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
 						with tab1:
 							col7, col8, col9 = st.columns(3)
 							with col7:
-								# Insights
-								st.write("## Insights")
-								approximate_distinct_count = modified_df[selected_column].nunique()
-								approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-								missing = modified_df[selected_column].isna().sum()
-								missing_percent = (missing / len(modified_df)) * 100
-								memory_size = modified_df[selected_column].memory_usage(deep=True)
-								st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-								st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-								st.write(f"Missing: :green[{missing}]")
-								st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-								st.write(f"Memory Size: :green[{memory_size}]")
-
-								# st.header("An owl")
-								# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
+								st.write('## Insights')
+								print(551)
+								approximate_distinct_count = modified_df[
+									selected_column].nunique()
+								approximate_unique_percent = (
+									approximate_distinct_count / len(
+									modified_df) * 100)
+								missing = modified_df[selected_column].isna(
+									).sum()
+								missing_percent = missing / len(modified_df
+									) * 100
+								memory_size = modified_df[selected_column
+									].memory_usage(deep=True)
+								st.write(
+									f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+									)
+								print(552)
+								st.write(
+									f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+									)
+								print(553)
+								st.write(f'Missing: :green[{missing}]')
+								print(554)
+								st.write(
+									f'Missing (%): :green[{missing_percent:.2f}%]'
+									)
+								print(555)
+								st.write(f'Memory Size: :green[{memory_size}]')
+								print(556)
 							with col8:
-								# Mode and Standard Deviation
-								st.write("## Mode")
-								# if modified_df[selected_column].dtype == 'object':
-								mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-								st.write(f"Mode: :green[{mode}]")
-									# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-								# else:
-									# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-									# std_dev = modified_df[selected_column].astype(float).std()
-									# st.write(f"Mode: {mode}")
-									# st.write(f"Standard Deviation: {std_dev}")
+								st.write('## Mode')
+								print(557)
+								mode = modified_df[selected_column].mode(
+									).iloc[0]
+								st.write(f'Mode: :green[{mode}]')
+								print(558)
 							with col9:
-								# First 5 Sample Rows
-								st.write("## First 5 Sample Rows")
+								st.write('## First 5 Sample Rows')
+								print(559)
 								st.write(modified_df[selected_column].head())
-
+								print(560)
 						with tab2:
-							# Prepare data for donut chart
-							data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
+							data = limit_unique_values(modified_df[
+								selected_column]).value_counts().reset_index()
 							data.columns = [selected_column, 'count']
-
-							fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-							fig.update_traces(textposition='inside', textinfo='percent+label')
-							fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-							st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+							fig = px.pie(data, values='count', names=
+								selected_column, hole=0.5)
+							fig.update_traces(textposition='inside',
+								textinfo='percent+label')
+							print(561)
+							fig.update_layout(legend=dict(orientation='h',
+								yanchor='bottom', y=1.02, xanchor='right', x=1)
+								)
+							print(562)
+							st.plotly_chart(fig)
+							print(563)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
 					col3, col4 = st.columns(2)
 					with col3:
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(564)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(565)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(566)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(567)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(568)
 					with col4:
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(569)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(570)
 						st.pyplot()
+						print(571)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+						print(572)
+					with st.expander('More Info'):
+						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot',
+							'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								st.write("#### Basic Statistics")
-								insights = calculate_insights(modified_df[selected_column])
-								basic_stats = {key: value for key, value in insights.items() if key in [
-									'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
+								st.write('#### Basic Statistics')
+								print(573)
+								insights = calculate_insights(modified_df[
+									selected_column])
+								basic_stats = {key: value for key, value in
+									insights.items() if key in ['Mean',
+									'Median', 'Mode', 'Standard deviation',
+									'Variance', 'Kurtosis', 'Skewness']}
 								for key, value in basic_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-								st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-								st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(574)
+								st.write(
+									f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+									)
+								print(575)
+								st.write(
+									f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+									)
+								print(576)
+								st.write(
+									f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+									)
+								print(577)
 							with col5:
-								st.write("#### Percentiles")
-								descriptive_stats = insights.get('Descriptive statistics')
+								st.write('#### Percentiles')
+								print(578)
+								descriptive_stats = insights.get(
+									'Descriptive statistics')
 								if descriptive_stats is not None:
-									percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
+									percentiles = descriptive_stats.loc[[
+										'min', '25%', '50%', '75%', 'max']]
 									if '5%' in descriptive_stats.index:
 										percentiles['5%'] = descriptive_stats['5%']
 									if '95%' in descriptive_stats.index:
-										percentiles['95%'] = descriptive_stats['95%']
+										percentiles['95%'] = descriptive_stats[
+											'95%']
 									st.write(percentiles)
-
+									print(579)
 							with col6:
-								st.write("#### Additional Statistics")
-								additional_stats = {key: value for key, value in insights.items() if key in [
-									'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
+								st.write('#### Additional Statistics')
+								print(580)
+								additional_stats = {key: value for key,
+									value in insights.items() if key in [
+									'Distinct', 'Distinct (%)', 'Missing',
+									'Missing (%)', 'Zeros', 'Zeros (%)',
+									'Negative', 'Negative (%)']}
 								for key, value in additional_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-								# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-								# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-								st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-								st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-								st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(581)
+								st.write(
+									f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+									)
+								print(582)
+								st.write(
+									f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+									)
+								print(583)
+								st.write(
+									f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+									)
+								print(584)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
+							print(585)
 						with tab3:
 							plt.figure(figsize=(10, 6))
-							qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
+							print(586)
+							qqplot_data = sm.qqplot(modified_df[
+								selected_column], line='s').gca().lines
 							fig = go.Figure()
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[0].get_xdata(),
-								'y': qqplot_data[0].get_ydata(),
-								'mode': 'markers',
-								'marker': {'color': '#19d3f3'}
-							})
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[1].get_xdata(),
-								'y': qqplot_data[1].get_ydata(),
-								'mode': 'lines',
-								'line': {'color': '#636efa'}
-							})
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[0].get_xdata(), 'y':
+								qqplot_data[0].get_ydata(), 'mode':
+								'markers', 'marker': {'color': '#19d3f3'}})
+							print(587)
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[1].get_xdata(), 'y':
+								qqplot_data[1].get_ydata(), 'mode': 'lines',
+								'line': {'color': '#636efa'}})
+							print(588)
 							x_min = min(qqplot_data[0].get_xdata())
 							x_max = max(qqplot_data[0].get_xdata())
 							y_min = min(qqplot_data[0].get_ydata())
 							y_max = max(qqplot_data[0].get_ydata())
-							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-							fig.update_layout({
-								'title': f'QQ Plot for {selected_column}',
-								'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-								'yaxis': {'title': 'Sample Quantiles'},
-								'showlegend': False,
-								'width': 800,
-								'height': 700,
-							})
-							st.plotly_chart(fig)
-					st.write("---")
+							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[
+								y_min, y_max], mode='lines', line=dict(
+								color='red', width=2), name='Identity Line'))
+							print(589)
+							fig.update_layout({'title':
+								f'QQ Plot for {selected_column}', 'xaxis':
+								{'title': 'Theoretical Quantiles',
+								'zeroline': False}, 'yaxis': {'title':
+								'Sample Quantiles'}, 'showlegend': False,
+								'width': 800, 'height': 700})
+							print(590)
+							st.plotly_chart(fig)
+							print(591)
+					st.write('---')
+					print(592)
 				else:
-					st.write("DataFrame not found.")
-				st.write("``")
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+					st.write('DataFrame not found.')
+					print(593)
+				st.write('``')
+				print(594)
 			except ZeroDivisionError:
 				pass
 			except Exception as e:
-				# st.error(e)
-				# st.subheader("⚠️Please upload a file⚠️")
 				pass
-
-	# col11, col22 = st.columns(2)
-	# with col11:
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline9 = {
+					"method": f'{encoding_method}',
+					"column_name": f'{selected_column}',
+					"param": opt
+				}
+
+				# Save the pipeline to a serialized object
+				with open("apply_encoding_on_col.pkl", "wb") as f:
+					joblib.dump(pipeline9, f)
 				st.session_state.df = modified_df
 				st.rerun()
-
-
-	elif preprocessing_action == "Apply Scaling":
-		scaling_method = st.selectbox("Select scaling method", ["Standardize Scaling", "Min-Max Scaling", "Robust Scaling"])
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+				print(595)
+	elif preprocessing_action == 'Apply Scaling':
+		scaling_method = st.selectbox('Select scaling method', [
+			'Standardize Scaling', 'Min-Max Scaling', 'Robust Scaling'])
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
 			modified_df = apply_scaling(modified_df, scaling_method)
-			st.write("Modified DataFrame:")
+			st.write('Modified DataFrame:')
+			print(596)
 			st.write(modified_df)
-
-	# col11, col22 = st.columns(2)
-	# with col11:
+			print(597)
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline10 = {
+					"method": f'{scaling_method}',
+				}
+
+				# Save the pipeline to a serialized object
+				with open("apply_scaling_on_df.pkl", "wb") as f:
+					joblib.dump(pipeline10, f)
 				st.session_state.df = modified_df
-				# modified_df.to_csv('data4.csv', index=False)
 				st.rerun()
-
-
-
-	elif preprocessing_action == "Discretize Output Variable":
-		# output_column = st.selectbox("Select output variable", df.columns)
-		bins = st.slider("Select the number of bins", min_value=2, max_value=20, value=5)
-		strategy = st.selectbox("Select the strategy for binning", ["uniform", "quantile", "kmeans"])
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
+				print(598)
+	elif preprocessing_action == 'Discretize Output Variable':
+		bins = st.slider('Select the number of bins', min_value=2,
+			max_value=20, value=5)
+		strategy = st.selectbox('Select the strategy for binning', [
+			'uniform', 'quantile', 'kmeans'])
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
 			modified_df = df.copy()
-			modified_df = discretize_output(modified_df, selected_column, bins, strategy)		
-			st.write("Modified DataFrame:")
+			modified_df = discretize_output(modified_df, selected_column,
+				bins, strategy)
+			st.write('Modified DataFrame:')
+			print(599)
 			st.write(modified_df)
+			print(600)
 			try:
 				if modified_df[selected_column].dtype == 'object':
 					col1, col2 = st.columns(2)
 					with col1:
 						unique_values = modified_df[selected_column].nunique()
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(601)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(602)
 						if unique_values <= 20:
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(603)
 						else:
-							st.write(f"  - Top 20 Unique Values:")
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
+							st.write(f'  - Top 20 Unique Values:')
+							print(604)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(605)
 					with col2:
 						plt.figure(figsize=(10, 6))
+						print(606)
 						try:
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(607)
 						except:
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(608)
 						plt.xticks(rotation=45)
+						print(609)
 						st.pyplot()
+						print(610)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2 = st.tabs(["Insights", "Donut chart"])
+						print(611)
+					with st.expander('More Info'):
+						tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
 						with tab1:
 							col7, col8, col9 = st.columns(3)
 							with col7:
-								# Insights
-								st.write("## Insights")
-								approximate_distinct_count = modified_df[selected_column].nunique()
-								approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-								missing = modified_df[selected_column].isna().sum()
-								missing_percent = (missing / len(modified_df)) * 100
-								memory_size = modified_df[selected_column].memory_usage(deep=True)
-								st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-								st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-								st.write(f"Missing: :green[{missing}]")
-								st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-								st.write(f"Memory Size: :green[{memory_size}]")
-
-								# st.header("An owl")
-								# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
+								st.write('## Insights')
+								print(612)
+								approximate_distinct_count = modified_df[
+									selected_column].nunique()
+								approximate_unique_percent = (
+									approximate_distinct_count / len(
+									modified_df) * 100)
+								missing = modified_df[selected_column].isna(
+									).sum()
+								missing_percent = missing / len(modified_df
+									) * 100
+								memory_size = modified_df[selected_column
+									].memory_usage(deep=True)
+								st.write(
+									f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+									)
+								print(613)
+								st.write(
+									f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+									)
+								print(614)
+								st.write(f'Missing: :green[{missing}]')
+								print(615)
+								st.write(
+									f'Missing (%): :green[{missing_percent:.2f}%]'
+									)
+								print(616)
+								st.write(f'Memory Size: :green[{memory_size}]')
+								print(617)
 							with col8:
-								# Mode and Standard Deviation
-								st.write("## Mode")
-								# if modified_df[selected_column].dtype == 'object':
-								mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-								st.write(f"Mode: :green[{mode}]")
-									# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-								# else:
-									# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-									# std_dev = modified_df[selected_column].astype(float).std()
-									# st.write(f"Mode: {mode}")
-									# st.write(f"Standard Deviation: {std_dev}")
+								st.write('## Mode')
+								print(618)
+								mode = modified_df[selected_column].mode(
+									).iloc[0]
+								st.write(f'Mode: :green[{mode}]')
+								print(619)
 							with col9:
-								# First 5 Sample Rows
-								st.write("## First 5 Sample Rows")
+								st.write('## First 5 Sample Rows')
+								print(620)
 								st.write(modified_df[selected_column].head())
-
+								print(621)
 						with tab2:
-							# Prepare data for donut chart
-							data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
+							data = limit_unique_values(modified_df[
+								selected_column]).value_counts().reset_index()
 							data.columns = [selected_column, 'count']
-
-							fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-							fig.update_traces(textposition='inside', textinfo='percent+label')
-							fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-							st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+							fig = px.pie(data, values='count', names=
+								selected_column, hole=0.5)
+							fig.update_traces(textposition='inside',
+								textinfo='percent+label')
+							print(622)
+							fig.update_layout(legend=dict(orientation='h',
+								yanchor='bottom', y=1.02, xanchor='right', x=1)
+								)
+							print(623)
+							st.plotly_chart(fig)
+							print(624)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
 					col3, col4 = st.columns(2)
 					with col3:
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(625)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(626)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(627)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(628)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(629)
 					with col4:
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(630)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(631)
 						st.pyplot()
+						print(632)
 						plt.close()
-					with st.expander("More Info"):
-						tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
+						print(633)
+					with st.expander('More Info'):
+						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot',
+							'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								st.write("#### Basic Statistics")
-								insights = calculate_insights(modified_df[selected_column])
-								basic_stats = {key: value for key, value in insights.items() if key in [
-									'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
+								st.write('#### Basic Statistics')
+								print(634)
+								insights = calculate_insights(modified_df[
+									selected_column])
+								basic_stats = {key: value for key, value in
+									insights.items() if key in ['Mean',
+									'Median', 'Mode', 'Standard deviation',
+									'Variance', 'Kurtosis', 'Skewness']}
 								for key, value in basic_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-								st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-								st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(635)
+								st.write(
+									f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+									)
+								print(636)
+								st.write(
+									f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+									)
+								print(637)
+								st.write(
+									f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+									)
+								print(638)
 							with col5:
-								st.write("#### Percentiles")
-								descriptive_stats = insights.get('Descriptive statistics')
+								st.write('#### Percentiles')
+								print(639)
+								descriptive_stats = insights.get(
+									'Descriptive statistics')
 								if descriptive_stats is not None:
-									percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
+									percentiles = descriptive_stats.loc[[
+										'min', '25%', '50%', '75%', 'max']]
 									if '5%' in descriptive_stats.index:
 										percentiles['5%'] = descriptive_stats['5%']
 									if '95%' in descriptive_stats.index:
-										percentiles['95%'] = descriptive_stats['95%']
+										percentiles['95%'] = descriptive_stats[
+											'95%']
 									st.write(percentiles)
-
+									print(640)
 							with col6:
-								st.write("#### Additional Statistics")
-								additional_stats = {key: value for key, value in insights.items() if key in [
-									'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
+								st.write('#### Additional Statistics')
+								print(641)
+								additional_stats = {key: value for key,
+									value in insights.items() if key in [
+									'Distinct', 'Distinct (%)', 'Missing',
+									'Missing (%)', 'Zeros', 'Zeros (%)',
+									'Negative', 'Negative (%)']}
 								for key, value in additional_stats.items():
-									st.write(f"**{key}:** :green[{value:.3f}]")
-								# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-								# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-								# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-								st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-								st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-								st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(642)
+								st.write(
+									f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+									)
+								print(643)
+								st.write(
+									f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+									)
+								print(644)
+								st.write(
+									f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+									)
+								print(645)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
+							print(646)
 						with tab3:
 							plt.figure(figsize=(10, 6))
-							qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
+							print(647)
+							qqplot_data = sm.qqplot(modified_df[
+								selected_column], line='s').gca().lines
 							fig = go.Figure()
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[0].get_xdata(),
-								'y': qqplot_data[0].get_ydata(),
-								'mode': 'markers',
-								'marker': {'color': '#19d3f3'}
-							})
-							fig.add_trace({
-								'type': 'scatter',
-								'x': qqplot_data[1].get_xdata(),
-								'y': qqplot_data[1].get_ydata(),
-								'mode': 'lines',
-								'line': {'color': '#636efa'}
-							})
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[0].get_xdata(), 'y':
+								qqplot_data[0].get_ydata(), 'mode':
+								'markers', 'marker': {'color': '#19d3f3'}})
+							print(648)
+							fig.add_trace({'type': 'scatter', 'x':
+								qqplot_data[1].get_xdata(), 'y':
+								qqplot_data[1].get_ydata(), 'mode': 'lines',
+								'line': {'color': '#636efa'}})
+							print(649)
 							x_min = min(qqplot_data[0].get_xdata())
 							x_max = max(qqplot_data[0].get_xdata())
 							y_min = min(qqplot_data[0].get_ydata())
 							y_max = max(qqplot_data[0].get_ydata())
-							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-							fig.update_layout({
-								'title': f'QQ Plot for {selected_column}',
-								'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-								'yaxis': {'title': 'Sample Quantiles'},
-								'showlegend': False,
-								'width': 800,
-								'height': 700,
-							})
-							st.plotly_chart(fig)
-					st.write("---")
+							fig.add_trace(go.Scatter(x=[x_min, x_max], y=[
+								y_min, y_max], mode='lines', line=dict(
+								color='red', width=2), name='Identity Line'))
+							print(650)
+							fig.update_layout({'title':
+								f'QQ Plot for {selected_column}', 'xaxis':
+								{'title': 'Theoretical Quantiles',
+								'zeroline': False}, 'yaxis': {'title':
+								'Sample Quantiles'}, 'showlegend': False,
+								'width': 800, 'height': 700})
+							print(651)
+							st.plotly_chart(fig)
+							print(652)
+					st.write('---')
+					print(653)
 				else:
-					st.write("DataFrame not found.")
-				st.write("``")
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+					st.write('DataFrame not found.')
+					print(654)
+				st.write('``')
+				print(655)
 			except ZeroDivisionError:
 				pass
 			except Exception as e:
 				st.error(e)
-				st.subheader("⚠️Please upload a file⚠️")
+				print(656)
+				st.subheader('⚠️Please upload a file⚠️')
+				print(657)
 				pass
-
-	# col11, col22 = st.columns(2)
-	# with col11:
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline11 = {
+					"column_name": f'{selected_column}',
+					"bins": bins,
+					"strategy": strategy
+				}
+				with open("discretize_output_col.pkl", "wb") as f:
+					joblib.dump(pipeline11, f)
 				st.session_state.df = modified_df
 				st.rerun()
-
-	elif preprocessing_action == "Column Unique Value Replacement":
+				print(658)
+	elif preprocessing_action == 'Column Unique Value Replacement':
 		print(43)
-		select = st.selectbox("Convert type:", ["Convert to Str:", "Convert to int:", "Convert to float:"])
-		
-		# Select a categorical column
-		# selected_column = st.selectbox("Select a categorical column", categorical_columns)
-
-		# Get distinct categorical values
+		print(659)
+		select = st.selectbox('Convert type:', ['Convert to Str:',
+			'Convert to int:', 'Convert to float:'])
 		print(44)
+		print(660)
 		distinct_values = df[selected_column].unique()
 		print(45)
-		# Display distinct categorical values and input box for replacement
+		print(661)
 		replacements = {}
 		for value in distinct_values:
 			print(46)
-			if select == "Convert to Str:":
+			print(662)
+			if select == 'Convert to Str:':
 				print(47)
+				print(663)
 				replacements[value] = st.text_input(f"Replace '{value}' with:", value=str(value))
-			elif select == "Convert to int:":
+			elif select == 'Convert to int:':
 				try:
 					print(48)
-					replacements[value] = st.number_input(f"Replace '{value}' with:", value=int(value), step=1)
+					print(664)
+					replacements[value] = st.number_input(
+						f"Replace '{value}' with:", value=int(value), step=1)
 				except:
 					print(49)
-					replacements[value] = st.number_input(f"Replace '{value}' with:", step=1)
-			elif select == "Convert to float:":
+					print(665)
+					replacements[value] = st.number_input(
+						f"Replace '{value}' with:", step=1)
+			elif select == 'Convert to float:':
 				try:
 					print(50)
-					replacements[value] = st.number_input(f"Replace '{value}' with:", value=float(value), step=0.01)
+					print(666)
+					replacements[value] = st.number_input(f"Replace '{value}' with:", value=float(value),step=0.01)
 				except:
 					print(51)
+					print(667)
 					replacements[value] = st.number_input(f"Replace '{value}' with:", step=0.01)
-		# if st.button("Apply :)"):
-		if (
-			st.button("Apply", on_click=callback)
-				or st.session_state.button_clicked
-				):
-			st.warning(f""""{select}" is applied, but changes will not be saved until you press the 'Confirm Changes' button below.""")
+		if st.button('Apply', on_click=callback
+			) or st.session_state.button_clicked:
+			st.warning(
+				f'"{select}" is applied, but changes will not be saved until you press the \'Confirm Changes\' button below.'
+				)
+			print(668)
 			print(52)
+			print(669)
 			modified_df = df.copy()
-			# Replace categorical values
 			print(53)
+			print(670)
+			print("replacements:=_", replacements)
 			modified_df[selected_column].replace(replacements, inplace=True)
+			print(671)
 			print(54)
-			st.write("Modified DataFrame:")
+			print(672)
+			st.write('Modified DataFrame:')
+			print(673)
 			print(55)
+			print(674)
 			st.write(modified_df)
+			print(675)
 			print(56)
-			# Explicitly convert the column to the desired data type
-			if select == "Convert to int:":
+			print(676)
+			if select == 'Convert to int:':
 				print(57)
-				# modified_df[selected_column] = modified_df[selected_column].astype(int)
+				print(677)
 				modified_df[selected_column] = modified_df[selected_column].astype(pd.Int64Dtype())
 				print(58)
-			elif select == "Convert to float:":
+				print(678)
+			elif select == 'Convert to float:':
 				print(59)
-				modified_df[selected_column] = modified_df[selected_column].astype(float)
-
-			# Display data type of the modified column
-			# st.write(f"Data Type after conversion: :green[{modified_df[selected_column].dtype}]")
+				print(679)
+				modified_df[selected_column] = modified_df[selected_column
+					].astype(float)
 			try:
 				print(60)
+				print(680)
 				if modified_df[selected_column].dtype == 'object':
 					print(61)
+					print(681)
 					col1, col2 = st.columns(2)
 					with col1:
 						print(62)
+						print(682)
 						unique_values = modified_df[selected_column].nunique()
 						print(63)
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
+						print(683)
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(684)
 						print(64)
-						st.write(f"  - Number of Unique Values: :green[{unique_values}]")
+						print(685)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(686)
 						print(65)
+						print(687)
 						if unique_values <= 20:
 							print(66)
-							st.write(f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]")
+							print(688)
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(689)
 							print(67)
+							print(690)
 						else:
 							print(68)
-							st.write(f"  - Top 20 Unique Values:")
+							print(691)
+							st.write(f'  - Top 20 Unique Values:')
+							print(692)
 							print(69)
-							st.write(f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]")
+							print(693)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(694)
 							print(70)
+							print(695)
 					with col2:
 						print(71)
+						print(696)
 						plt.figure(figsize=(10, 6))
+						print(697)
 						try:
 							print(72)
-							sns.countplot(x=limit_unique_values(modified_df[selected_column]), data=modified_df, color="green")
+							print(698)
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(699)
 						except:
 							print(73)
-							sns.countplot(x=modified_df[selected_column], data=modified_df, color="green")
+							print(700)
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(701)
 						plt.xticks(rotation=45)
+						print(702)
 						st.pyplot()
+						print(703)
 						plt.close()
+						print(704)
 						print(74)
-					# with st.expander("More Info"):
-					# 	print(75)
-					# 	tab1, tab2 = st.tabs(["Insights", "Donut chart"])
-					# 	with tab1:
-					# 		print(76)
-					# 		col7, col8, col9 = st.columns(3)
-					# 		with col7:
-					# 			# Insights
-					# 			print(77)
-					# 			st.write("## Insights")
-					# 			approximate_distinct_count = modified_df[selected_column].nunique()
-					# 			approximate_unique_percent = (approximate_distinct_count / len(modified_df)) * 100
-					# 			missing = modified_df[selected_column].isna().sum()
-					# 			missing_percent = (missing / len(modified_df)) * 100
-					# 			memory_size = modified_df[selected_column].memory_usage(deep=True)
-					# 			st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-					# 			st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-					# 			st.write(f"Missing: :green[{missing}]")
-					# 			st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-					# 			st.write(f"Memory Size: :green[{memory_size}]")
-					# 			print(78)
-
-					# 			# st.header("An owl")
-					# 			# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-					# 		with col8:
-					# 			print(79)
-					# 			# Mode and Standard Deviation
-					# 			st.write("## Mode")
-					# 			# if modified_df[selected_column].dtype == 'object':
-					# 			mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-					# 			st.write(f"Mode: :green[{mode}]")
-					# 				# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-					# 			# else:
-					# 				# mode = modified_df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-					# 				# std_dev = modified_df[selected_column].astype(float).std()
-					# 				# st.write(f"Mode: {mode}")
-					# 				# st.write(f"Standard Deviation: {std_dev}")
-					# 		with col9:
-					# 			print(80)
-					# 			# First 5 Sample Rows
-					# 			st.write("## First 5 Sample Rows")
-					# 			st.write(modified_df[selected_column].head())
-
-					# 	with tab2:
-					# 		print(81)
-					# 		# Prepare data for donut chart
-					# 		data = limit_unique_values(modified_df[selected_column]).value_counts().reset_index()
-					# 		data.columns = [selected_column, 'count']
-					# 		print(82)
-					# 		fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-					# 		fig.update_traces(textposition='inside', textinfo='percent+label')
-					# 		fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-					# 		st.plotly_chart(fig)
-
-							# st.header("An owl")
-							# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-						
-				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]):
+						print(705)
+				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
+					):
 					print(83)
+					print(706)
 					col3, col4 = st.columns(2)
 					with col3:
 						print(84)
-						st.write(f"  - Data Type: :green[{modified_df[selected_column].dtype}]")
-						st.write(f"  - Mean: :green[{modified_df[selected_column].mean()}]")
-						st.write(f"  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]")
-						st.write(f"  - Min Value: :green[{modified_df[selected_column].min()}]")
-						st.write(f"  - Max Value: :green[{modified_df[selected_column].max()}]")
+						print(707)
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(708)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(709)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(710)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(711)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(712)
 					with col4:
 						print(85)
+						print(713)
 						plt.figure(figsize=(10, 6))
-						sns.histplot(modified_df[selected_column], kde=True, color="green")
+						print(714)
+						sns.histplot(modified_df[selected_column], kde=True,
+							color='green')
+						print(715)
 						st.pyplot()
+						print(716)
 						plt.close()
-					# with st.expander("More Info"):
-					# 	print(86)
-					# 	tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
-					# 	with tab1:
-					# 		print(87)
-					# 		col4, col5, col6 = st.columns(3)
-					# 		with col4:
-					# 			print(88)
-					# 			st.write("#### Basic Statistics")
-					# 			insights = calculate_insights(modified_df[selected_column])
-					# 			basic_stats = {key: value for key, value in insights.items() if key in [
-					# 				'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
-					# 			print(89)
-					# 			for key, value in basic_stats.items():
-					# 				st.write(f"**{key}:** :green[{value:.3f}]")
-					# 			print(90)
-					# 			st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-					# 			st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-					# 			st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-					# 			print(91)
-					# 		with col5:
-					# 			print(92)
-					# 			st.write("#### Percentiles")
-					# 			descriptive_stats = insights.get('Descriptive statistics')
-					# 			print(93)
-					# 			if descriptive_stats is not None:
-					# 				print(94)
-					# 				percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
-					# 				if '5%' in descriptive_stats.index:
-					# 					percentiles['5%'] = descriptive_stats['5%']
-					# 				if '95%' in descriptive_stats.index:
-					# 					percentiles['95%'] = descriptive_stats['95%']
-					# 				st.write(percentiles)
-
-					# 		with col6:
-					# 			print(95)
-					# 			st.write("#### Additional Statistics")
-					# 			additional_stats = {key: value for key, value in insights.items() if key in [
-					# 				'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
-					# 			print(96)
-					# 			for key, value in additional_stats.items():
-					# 				st.write(f"**{key}:** :green[{value:.3f}]")
-					# 			# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-					# 			# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-					# 			# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-					# 			# try:
-					# 			# 	print(97)
-					# 			# 	st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-					# 			# 	print(98)
-					# 			# 	st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-					# 			# 	print(99)
-					# 			# 	st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
-					# 			# 	print(100)
-					# 			# except Exception as e:
-					# 			# 	print(e)
-						
-					# 	with tab2:
-					# 		print(101)
-					# 		try:
-					# 			fig = px.box(modified_df, y=selected_column)
-					# 		except Exception as e:
-					# 			print(e)
-					# 		st.plotly_chart(fig)
-					# 		print(102)
-						
-					# 	with tab3:
-					# 		print(103)
-					# 		plt.figure(figsize=(10, 6))
-					# 		print(103)
-					# 		qqplot_data = sm.qqplot(modified_df[selected_column], line='s').gca().lines
-					# 		print(104)
-					# 		try:
-					# 			fig = go.Figure()
-					# 			fig.add_trace({
-					# 				'type': 'scatter',
-					# 				'x': qqplot_data[0].get_xdata(),
-					# 				'y': qqplot_data[0].get_ydata(),
-					# 				'mode': 'markers',
-					# 				'marker': {'color': '#19d3f3'}
-					# 			})
-					# 			fig.add_trace({
-					# 				'type': 'scatter',
-					# 				'x': qqplot_data[1].get_xdata(),
-					# 				'y': qqplot_data[1].get_ydata(),
-					# 				'mode': 'lines',
-					# 				'line': {'color': '#636efa'}
-					# 			})
-					# 			x_min = min(qqplot_data[0].get_xdata())
-					# 			x_max = max(qqplot_data[0].get_xdata())
-					# 			y_min = min(qqplot_data[0].get_ydata())
-					# 			y_max = max(qqplot_data[0].get_ydata())
-					# 			fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-					# 			fig.update_layout({
-					# 				'title': f'QQ Plot for {selected_column}',
-					# 				'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-					# 				'yaxis': {'title': 'Sample Quantiles'},
-					# 				'showlegend': False,
-					# 				'width': 800,
-					# 				'height': 700,
-					# 			})
-					# 			st.plotly_chart(fig)
-					# 		except Exception as e:
-					# 			print(e)
-					
-
-					# 		print(105)
-					st.write("---")
+						print(717)
+					st.write('---')
+					print(718)
 					print(106)
+					print(719)
 				else:
 					print(107)
-					st.write("DataFrame not found.")
+					print(720)
+					st.write('DataFrame not found.')
+					print(721)
 					print(108)
-				st.write("``")
+					print(722)
+				st.write('``')
+				print(723)
 				print(109)
-				# col11, col22 = st.columns(2)
-				# with col11:
-				# 	if st.button("Confirm Change"):
-				# st.session_state.df = modified_df 
-				# 		st.session_state.df = modified_df  # Store modified DataFrame in session state
-				# 		st.rerun()
-
-				# with col22:
-				# 	# Undo functionality
-				# 	# if "modified_df" in st.session_state:
-				# 	if st.button("Undo", type='primary'):
-				# 		st.rerun()
-				# 		# if "copyy" in st.session_state:
-				# 		# 	# copyy = st.session_state.copyy
-				# 		# 	# st.session_state.df = copyy  # Revert to original DataFrame
-				# 		# 	st.session_state.df = st.session_state.copyy
-				# 		# 	st.write("Undo successful.")
-				# 		# else:
-				# 		# 	st.write("hi")
+				print(724)
 			except ZeroDivisionError:
 				print(110)
+				print(725)
 				pass
 			except Exception as e:
 				print(111)
+				print(726)
 				st.error(e)
-				st.subheader("⚠️Please upload a file⚠️")
+				print(727)
+				st.subheader('⚠️Please upload a file⚠️')
+				print(728)
 				pass
-
-	# col11, col22 = st.columns(2)
-	# with col11:
 			confirm_change = st.button('Confirm Change')
-
 			if confirm_change:
-				# st.session_state.df = modified_df
+				pipeline12 = {
+					"column_name": f'{selected_column}',
+					"replacements": replacements,
+					"select": select
+				}
+
+				# Save the pipeline to a serialized object
+				with open("column_unique_value_replacement.pkl", "wb") as f:
+					joblib.dump(pipeline12, f)
 				st.session_state.df = modified_df
-				# modified_df.to_csv('data3.csv', index=False)
+				modified_df.to_csv("heha.csv")
 				st.rerun()
+				print(729)
 except Exception as e:
-	print("e:=_", e)
+	print('e:=_', e)
+	print(730)
 	st.error(e)
-
-
-	# Update the checkbox value to False after the action
-	# st.session_state.confirm_change = False
-		
-
-# with col22:
-	# Undo functionality
-	# if "modified_df" in st.session_state:
-# if st.button("Undo", type='primary'):                              # IIMP
-# 	st.rerun()
-	# if "copyy" in st.session_state:
-		# copyy = st.session_state.copyy
-		# st.session_state.df = copyy  # Revert to original DataFrame
-	# st.session_state.df = ccc
-	# st.write("Undo successful.")
-	# else:
-		# st.write("hi")
-	# col11, col22 = st.columns(2)
-	# with col11:
-	# 	if st.button("Confirm Change"):
-	# 		st.session_state.df = modified_df 
-	# 		# st.rerun()
-
-	# with col22:
-	# 	# Undo functionality
-	# 	if "modified_df" in st.session_state:
-	# 		if st.button("Undo", type='primary'):
-	# 			st.session_state.df = df  # Revert to original DataFrame
-	# 			st.write("Undo successful.")
-
-
-
-# try:
-# 	if df[selected_column].dtype == 'object':
-# 		col1, col2 = st.columns(2)
-# 		with col1:
-# 			unique_values = df[selected_column].nunique()
-# 			st.write(f"  - Data Type: :green[{df[selected_column].dtype}]")
-# 			st.write(f"  - Number of Unique Values: :green[{unique_values}]")
-# 			if unique_values <= 20:
-# 				st.write(f"  - Unique Values: :green[{', '.join(map(str, df[selected_column].unique()))}]")
-# 			else:
-# 				st.write(f"  - Top 20 Unique Values:")
-# 				st.write(f":green[{', '.join(map(str, df[selected_column].value_counts().head(20).index))}]")
-# 		with col2:
-# 			plt.figure(figsize=(10, 6))
-# 			try:
-# 				sns.countplot(x=limit_unique_values(df[selected_column]), data=df, color="green")
-# 			except:
-# 				sns.countplot(x=df[selected_column], data=df, color="green")
-# 			plt.xticks(rotation=45)
-# 			st.pyplot()
-# 			plt.close()
-# 		with st.expander("More Info"):
-# 			tab1, tab2, tab3 = st.tabs(["Insights", "Donut chart", "WordCloud"])
-# 			with tab1:
-# 				col7, col8, col9 = st.columns(3)
-# 				with col7:
-# 					# Insights
-# 					st.write("## Insights")
-# 					approximate_distinct_count = df[selected_column].nunique()
-# 					approximate_unique_percent = (approximate_distinct_count / len(df)) * 100
-# 					missing = df[selected_column].isna().sum()
-# 					missing_percent = (missing / len(df)) * 100
-# 					memory_size = df[selected_column].memory_usage(deep=True)
-# 					st.write(f"Approximate Distinct Count: :green[{approximate_distinct_count}]")
-# 					st.write(f"Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]")
-# 					st.write(f"Missing: :green[{missing}]")
-# 					st.write(f"Missing (%): :green[{missing_percent:.2f}%]")
-# 					st.write(f"Memory Size: :green[{memory_size}]")
-
-# 					# st.header("An owl")
-# 					# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-# 				with col8:
-# 					# Mode and Standard Deviation
-# 					st.write("## Mode")
-# 					# if df[selected_column].dtype == 'object':
-# 					mode = df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-# 					st.write(f"Mode: :green[{mode}]")
-# 						# st.write("Standard Deviation cannot be calculated for non-numeric data.")
-# 					# else:
-# 						# mode = df[selected_column].mode().iloc[0]  # Mode can return multiple values, taking the first one
-# 						# std_dev = df[selected_column].astype(float).std()
-# 						# st.write(f"Mode: {mode}")
-# 						# st.write(f"Standard Deviation: {std_dev}")
-# 				with col9:
-# 					# First 5 Sample Rows
-# 					st.write("## First 5 Sample Rows")
-# 					st.write(df[selected_column].head())
-
-# 			with tab2:
-# 				# Prepare data for donut chart
-# 				data = limit_unique_values(df[selected_column]).value_counts().reset_index()
-# 				data.columns = [selected_column, 'count']
-
-# 				fig = px.pie(data, values='count', names=selected_column, hole=0.5)
-# 				fig.update_traces(textposition='inside', textinfo='percent+label')
-# 				fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
-# 				st.plotly_chart(fig)
-
-# 				# st.header("An owl")
-# 				# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
-
-# 			with tab3:
-# 				# Concatenate all values of the column into a single string
-# 				cleanstrng = ' '.join(df[selected_column].dropna())
-
-# 				# Check if there are words to plot
-# 				if cleanstrng:
-# 					# Generate word cloud
-# 					word_freq = pd.Series(cleanstrng.split()).value_counts()
-					
-# 					# Select top 200 words if available, otherwise take the exact number of words
-# 					if len(word_freq) >= 50:
-# 						top_words = word_freq.head(50)
-# 					else:
-# 						top_words = word_freq
-
-# 					words_dict = top_words.to_dict()
-					
-# 					try:
-# 						# Generate word cloud from frequencies
-# 						wordcloud_ip = WordCloud(background_color='white', width=2800, height=2400).generate_from_frequencies(words_dict)
-
-# 						# Display word cloud
-# 						plt.figure(figsize=(10, 7))
-# 						plt.imshow(wordcloud_ip, interpolation='bilinear')
-# 						plt.title(f'Word Cloud for {selected_column}')
-# 						plt.axis('off')
-# 						plt.show()
-# 						st.pyplot(plt, use_container_width=True)
-# 					except Exception as e:
-# 						st.write(f"Error generating word cloud: {e}")
-# 				else:
-# 					st.write(f"No words to plot for column '{selected_column}'")
-# 	elif pd.api.types.is_numeric_dtype(df[selected_column]):
-# 		col3, col4 = st.columns(2)
-# 		with col3:
-# 			st.write(f"  - Data Type: :green[{df[selected_column].dtype}]")
-# 			st.write(f"  - Mean: :green[{df[selected_column].mean()}]")
-# 			st.write(f"  - Standard Deviation: :green[{df[selected_column].std()}]")
-# 			st.write(f"  - Min Value: :green[{df[selected_column].min()}]")
-# 			st.write(f"  - Max Value: :green[{df[selected_column].max()}]")
-# 		with col4:
-# 			plt.figure(figsize=(10, 6))
-# 			sns.histplot(df[selected_column], kde=True, color="green")
-# 			st.pyplot()
-# 			plt.close()
-# 		with st.expander("More Info"):
-# 			tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
-# 			with tab1:
-# 				col4, col5, col6 = st.columns(3)
-# 				with col4:
-# 					st.write("#### Basic Statistics")
-# 					insights = calculate_insights(df[selected_column])
-# 					basic_stats = {key: value for key, value in insights.items() if key in [
-# 						'Mean', 'Median', 'Mode', 'Standard deviation', 'Variance', 'Kurtosis', 'Skewness']}
-# 					for key, value in basic_stats.items():
-# 						st.write(f"**{key}:** :green[{value:.3f}]")
-# 					st.write(f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]")
-# 					st.write(f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]")
-# 					st.write(f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]")
-
-# 				with col5:
-# 					st.write("#### Percentiles")
-# 					descriptive_stats = insights.get('Descriptive statistics')
-# 					if descriptive_stats is not None:
-# 						percentiles = descriptive_stats.loc[['min', '25%', '50%', '75%', 'max']]
-# 						if '5%' in descriptive_stats.index:
-# 							percentiles['5%'] = descriptive_stats['5%']
-# 						if '95%' in descriptive_stats.index:
-# 							percentiles['95%'] = descriptive_stats['95%']
-# 						st.write(percentiles)
-
-# 				with col6:
-# 					st.write("#### Additional Statistics")
-# 					additional_stats = {key: value for key, value in insights.items() if key in [
-# 						'Distinct', 'Distinct (%)', 'Missing', 'Missing (%)', 'Zeros', 'Zeros (%)', 'Negative', 'Negative (%)']}
-# 					for key, value in additional_stats.items():
-# 						st.write(f"**{key}:** :green[{value:.3f}]")
-# 					# st.write(f"**Memory size:** {insights.get('Memory size', 'N/A')}")
-# 					# st.write(f"**Range:** {insights.get('Range', 'N/A')}")
-# 					# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
-# 					st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
-# 					st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
-# 					st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
-# 			with tab2:
-# 				fig = px.box(df, y=selected_column)
-# 				st.plotly_chart(fig)
-# 			with tab3:
-# 				plt.figure(figsize=(10, 6))
-# 				qqplot_data = sm.qqplot(df[selected_column], line='s').gca().lines
-# 				fig = go.Figure()
-# 				fig.add_trace({
-# 					'type': 'scatter',
-# 					'x': qqplot_data[0].get_xdata(),
-# 					'y': qqplot_data[0].get_ydata(),
-# 					'mode': 'markers',
-# 					'marker': {'color': '#19d3f3'}
-# 				})
-# 				fig.add_trace({
-# 					'type': 'scatter',
-# 					'x': qqplot_data[1].get_xdata(),
-# 					'y': qqplot_data[1].get_ydata(),
-# 					'mode': 'lines',
-# 					'line': {'color': '#636efa'}
-# 				})
-# 				x_min = min(qqplot_data[0].get_xdata())
-# 				x_max = max(qqplot_data[0].get_xdata())
-# 				y_min = min(qqplot_data[0].get_ydata())
-# 				y_max = max(qqplot_data[0].get_ydata())
-# 				fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
-# 				fig.update_layout({
-# 					'title': f'QQ Plot for {selected_column}',
-# 					'xaxis': {'title': 'Theoretical Quantiles', 'zeroline': False},
-# 					'yaxis': {'title': 'Sample Quantiles'},
-# 					'showlegend': False,
-# 					'width': 800,
-# 					'height': 700,
-# 				})
-# 				st.plotly_chart(fig)
-# 		st.write("---")
-# 	else:
-# 		st.write("DataFrame not found.")
-# 	st.write("``")
-# except ZeroDivisionError:
-# 	pass
-# except Exception as e:
-# 	st.error(e)
-# 	st.subheader("⚠️Please upload a file⚠️")
-# 	pass
+	print(731)
```

## Comparing `glook-1.1.5b1.dist-info/METADATA` & `glook-1.1.6b1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 1.1.5b1
+Version: 1.1.6b1
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com
 License: MIT
@@ -34,14 +34,17 @@
 Requires-Dist: plotly ==5.19.0
 Requires-Dist: scipy ==1.10.0
 Requires-Dist: seaborn ==0.13.2
 Requires-Dist: statsmodels ==0.14.1
 Requires-Dist: streamlit ==1.31.1
 Requires-Dist: wordcloud ==1.9.3
 Requires-Dist: openpyxl ==3.1.2
+Requires-Dist: joblib ==1.3.2
+Requires-Dist: scikit-learn ==1.3.2
+Requires-Dist: xgboost ==2.0.3
 
 
 ![G-Look](https://raw.githubusercontent.com/gaurang157/glook/main/assets/pixelcut-export.png)
 ---
 
 <p align="center">
   <a href="LICENSE"><img src="https://img.shields.io/pypi/l/glook?style=flat-square"/></a>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glook Version: 1.1.5b1 Summary: Auto EDA. Home-
+Metadata-Version: 2.1 Name: glook Version: 1.1.6b1 Summary: Auto EDA. Home-
 page: https://github.com/gaurang157/glook Author: Gaurang Ingle Author-email:
 gaurang.ingle@gmail.com Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com License: MIT Project-URL: Bug
 Reports, https://github.com/gaurang157/glook/issues Project-URL: Source, https:
 //github.com/gaurang157/glook Project-URL: Documentation, https://github.com/
 gaurang157/glook/blob/main/README.md Project-URL: Say Thanks!, https://
 github.com/gaurang157/glook/issues/new?assignees=&labels=&template=thanks.yml
@@ -17,17 +17,18 @@
 License :: OSI Approved :: MIT License Classifier: Topic :: Software
 Development :: Libraries :: Application Frameworks Classifier: Topic ::
 Software Development :: User Interfaces Classifier: Topic :: Utilities
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist:
 matplotlib ==3.7.4 Requires-Dist: numpy ==1.24.4 Requires-Dist: pandas ==2.0.3
 Requires-Dist: plotly ==5.19.0 Requires-Dist: scipy ==1.10.0 Requires-Dist:
 seaborn ==0.13.2 Requires-Dist: statsmodels ==0.14.1 Requires-Dist: streamlit
-==1.31.1 Requires-Dist: wordcloud ==1.9.3 Requires-Dist: openpyxl ==3.1.2 ![G-
-Look](https://raw.githubusercontent.com/gaurang157/glook/main/assets/pixelcut-
-export.png) ---
+==1.31.1 Requires-Dist: wordcloud ==1.9.3 Requires-Dist: openpyxl ==3.1.2
+Requires-Dist: joblib ==1.3.2 Requires-Dist: scikit-learn ==1.3.2 Requires-
+Dist: xgboost ==2.0.3 ![G-Look](https://raw.githubusercontent.com/gaurang157/
+glook/main/assets/pixelcut-export.png) ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_g_l_o_o_k_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
               _p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_g_l_o_o_k_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_d_o_w_n_l_o_a_d_s_]
 ## Releases
      RReeppoo VVeerrssiioonn                         DDoowwnnllooaaddss
      PyPI _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/ _[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_g_l_o_o_k_]
           _g_l_o_o_k_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
 # G-Look: Auto EDA glook is a Python library that provides a graphical user
```

## Comparing `glook-1.1.5b1.dist-info/RECORD` & `glook-1.1.6b1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 glook/GLook.py,sha256=qNCnTY0f4myhVXkZHf1mMgpN4yfHCaVXq4uz4uC85_s,3200
 glook/__init__.py,sha256=8NahmY4XQHJYMnFDvkZnHpjVBHwxrYrnDFlTTuyXbB0,51
 glook/cli.py,sha256=zBVCZyNNyRj_Zy4Tdnbrb1TrgRhEqAEEdZbk_vrLmi4,339
 glook/pages/10_Unsupervised_learning.py,sha256=_RAtRgR8asoxaIsu-KlITcFlVOV0nRHZl1qWT33OU4k,25002
 glook/pages/11_Custom_Model_Training.py,sha256=4FtzOYYLxySsy7tgV2m6B8IHVaO9KOCVJ1GVHqgmCbs,96985
-glook/pages/1_General_Data_Insights.py,sha256=-L3YAeg_HMYGvMfX3YrjOiRIDlXdNhsqzQLoVbqfboo,6170
+glook/pages/1_General_Data_Insights.py,sha256=MTFJNDNfE6k7dBBeWMlN-dfromzX4oKEWWClmSTHc9w,6157
 glook/pages/2_Univariate_Analysis.py,sha256=eGA6zjAwmlMNDIqm1dN-eq_4EVOW1ispoq8BL3o2ypU,19725
 glook/pages/3_Bivariate_Analysis.py,sha256=_eUSH35csf_Uljg9HvW7szmfXjrgNwrsVJA0gLMDNEA,7813
 glook/pages/4_Trivariate_Analysis.py,sha256=lChxNbGt1nyga-Zf69oL7hUH-z_xLJPq1o0b-pjrtTw,7707
-glook/pages/5_Pre_Processing.py,sha256=k2W_GJTcPA3lH2QMlgofCtAiCUW7TreL1SnYFC5Yzjs,130608
+glook/pages/5_Pre_Processing.py,sha256=usaMfyFrgKcYVK_wfxuTDY7825tyo384matx087qj9I,112037
 glook/pages/6_Split_Data.py,sha256=y-3Qo16H5vZeADRxKR8oSs8PViSm89O-iCstK-YPhSs,3315
 glook/pages/7_Dimensionality_Reduction.py,sha256=Eq9Et3k7Q-MsS7e5EYiI6P4Vat5P9VBTCziM6KdidIo,4588
 glook/pages/8_Supervised_Learning.py,sha256=Bg3qK4w8RRfWhpMzaYeTwPgfzeBO4PgO7rkgB9wzuCQ,59951
-glook-1.1.5b1.dist-info/METADATA,sha256=wsQUUDQWy7h_HCHZT5BxqlSROiNK-u7UWRtEwqonCEM,7141
-glook-1.1.5b1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-glook-1.1.5b1.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
-glook-1.1.5b1.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
-glook-1.1.5b1.dist-info/RECORD,,
+glook-1.1.6b1.dist-info/METADATA,sha256=TFhxkNQ-fJfx1Hckvn9CfGmziX843Xw_3070bab1u_8,7241
+glook-1.1.6b1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+glook-1.1.6b1.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
+glook-1.1.6b1.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
+glook-1.1.6b1.dist-info/RECORD,,
```

