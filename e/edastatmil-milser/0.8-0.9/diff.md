# Comparing `tmp/edastatmil_milser-0.8.tar.gz` & `tmp/edastatmil_milser-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edastatmil_milser-0.8.tar", last modified: Sun Apr  7 16:52:14 2024, max compression
+gzip compressed data, was "edastatmil_milser-0.9.tar", last modified: Mon Apr  8 16:37:28 2024, max compression
```

## Comparing `edastatmil_milser-0.8.tar` & `edastatmil_milser-0.9.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 16:52:14.579613 edastatmil_milser-0.8/
--rw-rw-rw-   0        0        0    11558 2024-04-06 18:06:27.000000 edastatmil_milser-0.8/LICENSE
--rw-rw-rw-   0        0        0       70 2024-04-06 18:06:27.000000 edastatmil_milser-0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3886 2024-04-07 16:52:14.579613 edastatmil_milser-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3254 2024-04-07 16:48:02.000000 edastatmil_milser-0.8/README.md
--rw-rw-rw-   0        0        0      517 2024-04-07 16:47:44.000000 edastatmil_milser-0.8/pyproject.toml
--rw-rw-rw-   0        0        0      538 2024-04-07 16:52:14.581615 edastatmil_milser-0.8/setup.cfg
--rw-rw-rw-   0        0        0      613 2024-04-07 16:50:47.000000 edastatmil_milser-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:52:14.512598 edastatmil_milser-0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 16:52:14.543605 edastatmil_milser-0.8/src/edastatmil_milser/
--rw-rw-rw-   0        0        0       63 2024-04-06 18:06:27.000000 edastatmil_milser-0.8/src/edastatmil_milser/__init__.py
--rw-rw-rw-   0        0        0      277 2024-04-06 18:11:47.000000 edastatmil_milser-0.8/src/edastatmil_milser/commandline.py
--rw-rw-rw-   0        0        0    26233 2024-04-07 16:34:25.000000 edastatmil_milser-0.8/src/edastatmil_milser/edas_tatmil.py
--rw-rw-rw-   0        0        0      175 2024-04-07 16:44:37.000000 edastatmil_milser-0.8/src/edastatmil_milser/version.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:52:14.577623 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/
--rw-rw-rw-   0        0        0     3886 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:37:28.908364 edastatmil_milser-0.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-06 18:06:27.000000 edastatmil_milser-0.9/LICENSE
+-rw-rw-rw-   0        0        0       70 2024-04-06 18:06:27.000000 edastatmil_milser-0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      630 2024-04-08 16:37:28.907365 edastatmil_milser-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-04-08 16:37:02.000000 edastatmil_milser-0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      538 2024-04-08 16:37:28.913366 edastatmil_milser-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      613 2024-04-08 16:36:59.000000 edastatmil_milser-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:37:28.820320 edastatmil_milser-0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:37:28.879342 edastatmil_milser-0.9/src/edastatmil_milser/
+-rw-rw-rw-   0        0        0       63 2024-04-06 18:06:27.000000 edastatmil_milser-0.9/src/edastatmil_milser/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-04-06 18:11:47.000000 edastatmil_milser-0.9/src/edastatmil_milser/commandline.py
+-rw-rw-rw-   0        0        0    26328 2024-04-08 16:36:38.000000 edastatmil_milser-0.9/src/edastatmil_milser/edas_tatmil.py
+-rw-rw-rw-   0        0        0      175 2024-04-08 16:36:55.000000 edastatmil_milser-0.9/src/edastatmil_milser/version.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:37:28.906365 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/
+-rw-rw-rw-   0        0        0      630 2024-04-08 16:37:28.000000 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-04-08 16:37:28.000000 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:37:28.000000 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-08 16:37:28.000000 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/top_level.txt
```

### Comparing `edastatmil_milser-0.8/LICENSE` & `edastatmil_milser-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edastatmil_milser-0.8/pyproject.toml` & `edastatmil_milser-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "edastatmil_milser"
-version = "0.8"
+version = "0.9"
 authors = [
   { name="TatianaCC y milser", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `edastatmil_milser-0.8/setup.cfg` & `edastatmil_milser-0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6461 7374 6174 6d69 6c5f 6d69   = edastatmil_mi
 00000020: 6c73 6572 0d0a 7665 7273 696f 6e20 3d20  lser..version = 
-00000030: 302e 380d 0a61 7574 686f 7220 3d20 5461  0.8..author = Ta
+00000030: 302e 390d 0a61 7574 686f 7220 3d20 5461  0.9..author = Ta
 00000040: 7469 616e 6143 4320 7920 6d69 6c73 6572  tianaCC y milser
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2061 7574 686f 7240 6578 616d 706c 652e   author@example.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2041 2073 6d61 6c6c 2065 7861 6d70   = A small examp
 00000090: 6c65 2070 6163 6b61 6765 0d0a 6c6f 6e67  le package..long
 000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `edastatmil_milser-0.8/setup.py` & `edastatmil_milser-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='edastatmil_milser',
-    version='0.8',
+    version='0.9',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     author='Tatiana Cazorla y Rubén Serrano',
     description='Tu EDA mas sencillo',
     url='https://github.com/milser/edas_tatianamilser',
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `edastatmil_milser-0.8/src/edastatmil_milser/edas_tatmil.py` & `edastatmil_milser-0.9/src/edastatmil_milser/edas_tatmil.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     
         str: 'Numeric': If they are numeric.
              'Categorical': If they are categorical.
     """
     series_ = series.copy()
     
     if pd.api.types.is_numeric_dtype(series_):
-        return 'Numeric'
+        return 'Numerical'
     else:
         return 'Categorical'
 
 def explore(data_frame: pd.DataFrame) -> Tuple[List[str], List[str]]:
     """
     Explores a pandas DataFrame and prints information about its characteristics.
 
@@ -366,22 +366,24 @@
     Parameters::
 
         df (pandas.DataFrame): The pandas DataFrame containing the data.
         variables_list (List[str]): List of variable names for which correlation will be calculated.
 
     Returns::
 
-        None
+        pd.DataFrame: The pandas DataFrame with the factorized categorical variables.
     """
     df_ = df.copy()
     variables_list_ = variables_list.copy()
     
     fz_df_ = factorize_categorical(df_, variables_list_)
     sns.heatmap(fz_df_.corr(), annot = True, fmt = ".2f")
 
+    return fz_df_
+
 def numerical_box(variables: List[str], data_frame: pd.DataFrame, color: str = '#1295a6') -> None:
     """
     Crea diagramas de caja para variables numéricas en un DataFrame de pandas.
 
     Esta función crea `diagramas` de caja para variables `numéricas` en el DataFrame de pandas proporcionado.
     Los diagramas se muestran en una cuadrícula, con hasta 3 gráficos por fila.
 
@@ -436,15 +438,15 @@
             'mean': Outliers are REPLACED by the MEAN.
             'median': Outliers are REPLACED by the MEDIAN.
 
     Returns::
 
         tuple: A tuple containing two DataFrames.
                The first DataFrame contains the identified outliers.
-               The second DataFrame contains the original data with outliers treated according to the option specified in 'Do_'.
+               The second DataFrame contains the original data with outliers treated according to the option specified in 'Do'.
     """    
     df_ = df.copy()
     var_ = var
     sigma_ = sigma
     Do_ = Do
   
     descr_ = df_[var_].describe()
```

