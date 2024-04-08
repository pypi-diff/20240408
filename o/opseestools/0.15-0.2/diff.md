# Comparing `tmp/opseestools-0.15.tar.gz` & `tmp/opseestools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opseestools-0.15.tar", last modified: Wed Mar 20 12:44:22 2024, max compression
+gzip compressed data, was "opseestools-0.2.tar", last modified: Mon Apr  8 15:44:01 2024, max compression
```

## Comparing `opseestools-0.15.tar` & `opseestools-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 12:44:22.313467 opseestools-0.15/
--rw-rw-rw-   0        0        0     4755 2024-03-20 12:44:22.312456 opseestools-0.15/PKG-INFO
--rw-rw-rw-   0        0        0     4298 2024-03-16 22:25:04.000000 opseestools-0.15/README.md
-drwxrwxrwx   0        0        0        0 2024-03-20 12:44:22.298822 opseestools-0.15/opseestools/
--rw-rw-rw-   0        0        0     5696 2024-03-16 20:46:05.000000 opseestools-0.15/opseestools/Lib_frag.py
--rw-rw-rw-   0        0        0       91 2024-03-16 16:37:45.000000 opseestools-0.15/opseestools/__init__.py
--rw-rw-rw-   0        0        0   105610 2024-03-16 22:19:04.000000 opseestools-0.15/opseestools/analisis.py
--rw-rw-rw-   0        0        0    91076 2024-03-11 19:44:11.000000 opseestools-0.15/opseestools/analisis3D.py
--rw-rw-rw-   0        0        0    19939 2024-03-06 21:36:46.000000 opseestools-0.15/opseestools/utilidades.py
-drwxrwxrwx   0        0        0        0 2024-03-20 12:44:22.310951 opseestools-0.15/opseestools.egg-info/
--rw-rw-rw-   0        0        0     4755 2024-03-20 12:44:22.000000 opseestools-0.15/opseestools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-03-20 12:44:22.000000 opseestools-0.15/opseestools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 12:44:22.000000 opseestools-0.15/opseestools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-03-20 12:44:22.000000 opseestools-0.15/opseestools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-20 12:44:22.000000 opseestools-0.15/opseestools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-20 12:44:22.313467 opseestools-0.15/setup.cfg
--rw-rw-rw-   0        0        0      900 2024-03-20 12:38:02.000000 opseestools-0.15/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:44:01.458608 opseestools-0.2/
+-rw-rw-rw-   0        0        0     4903 2024-04-08 15:44:01.457607 opseestools-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4416 2024-04-08 15:30:07.000000 opseestools-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 15:44:01.444071 opseestools-0.2/opseestools/
+-rw-rw-rw-   0        0        0     7214 2024-04-08 15:37:47.000000 opseestools-0.2/opseestools/Lib_frag.py
+-rw-rw-rw-   0        0        0       91 2024-03-16 16:37:45.000000 opseestools-0.2/opseestools/__init__.py
+-rw-rw-rw-   0        0        0   105586 2024-03-20 20:17:26.000000 opseestools-0.2/opseestools/analisis.py
+-rw-rw-rw-   0        0        0    91076 2024-03-20 20:44:02.000000 opseestools-0.2/opseestools/analisis3D.py
+-rw-rw-rw-   0        0        0    19939 2024-03-06 21:36:46.000000 opseestools-0.2/opseestools/utilidades.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:44:01.457607 opseestools-0.2/opseestools.egg-info/
+-rw-rw-rw-   0        0        0     4903 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 15:44:01.000000 opseestools-0.2/opseestools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:44:01.458608 opseestools-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      926 2024-04-08 15:43:14.000000 opseestools-0.2/setup.py
```

### Comparing `opseestools-0.15/PKG-INFO` & `opseestools-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: opseestools
-Version: 0.15
+Version: 0.2
 Summary: A collection of OpenSeesPy routines for performing several types of analyses and other tools
-Home-page: https://github.com/odarroyo/opstools
+Home-page: https://github.com/odarroyo/opseestools
 Author: Orlando Arroyo
 Author-email: odarroyo@uc.cl
 License: LICENSE
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: openseespy>=3.5
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy>=1.11
+Requires-Dist: pandas>=2.0
 
 # opseestools
 
 This is a library to be used with OpenSeesPy.
 
 It includes a collection of analysis functions that are useful if you are analyzing frames or wall buildings both in two and three dimensions, storing the results in Python variables. 
 It also includes another useful tools for processing results and creating scripts
@@ -40,15 +41,16 @@
 
 import opstools.utilidades as ut (or any other name)
 
 4) A library to calculate and plot fragility functions. You can import it as:
 
 import opstools.Lib_frag as ut (or any other name)
 
-The full documentation is available on the GitHub website: https://github.com/odarroyo/opstools 
+The full documentation is available on the GitHub website: https://github.com/odarroyo/opseestools 
+Tutorials of how to use the functions are available in: https://github.com/odarroyo/openseespy_starting_tutorials
 
 ## 2D Analysis functions
 
 Here's a brief description of some of the functions:
 
 ### gravedad()
 To perform gravity analysis of a model you created. In a more general sense, it runs a static analysis, but returns no output. The idea of this script is to perform the gravity analysis before a pushover or other nonlinear analysis.
```

### Comparing `opseestools-0.15/README.md` & `opseestools-0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 import opstools.utilidades as ut (or any other name)
 
 4) A library to calculate and plot fragility functions. You can import it as:
 
 import opstools.Lib_frag as ut (or any other name)
 
-The full documentation is available on the GitHub website: https://github.com/odarroyo/opstools 
+The full documentation is available on the GitHub website: https://github.com/odarroyo/opseestools 
+Tutorials of how to use the functions are available in: https://github.com/odarroyo/openseespy_starting_tutorials
 
 ## 2D Analysis functions
 
 Here's a brief description of some of the functions:
 
 ### gravedad()
 To perform gravity analysis of a model you created. In a more general sense, it runs a static analysis, but returns no output. The idea of this script is to perform the gravity analysis before a pushover or other nonlinear analysis.
```

### Comparing `opseestools-0.15/opseestools/Lib_frag.py` & `opseestools-0.2/opseestools/Lib_frag.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np                                                              # Importa librería estándar para operaciones matematicas.
                                                          # Importa librería estándar de análisis de datos.
 import matplotlib.pyplot as plt                                                 # Importa librería estándar para plotear otras cosasy poder crear figuras.
                                        # Importa librería estándar que tiene un conjunto de herramientas para proporcionar una canalización ligera en Python
 # Ajuste de distribuciones
 # ==============================================================================
 from scipy import stats, optimize
-
+import pandas as pd
 
 #%% CURVAS DE FRAGILIDAD AJUSTE FUNCIÓN LOGNORMAL
 #-----Example calculations to demonstrate the use of fragility fitting
 #-----functions. These calculations are based on the following paper:
 #-----Baker, J. W. (2015). “Efficient analytical fragility function fitting 
 #-----using dynamic structural analysis.” Earthquake Spectra, 31(1), 579-599.
 
@@ -109,8 +109,48 @@
                 bins_indices[i].append(index)
                 break
     
     # Convert lists to NumPy arrays for numerical operations
     bins_values = [np.array(bin) for bin in bins_values]
     bins_indices = [np.array(bin) for bin in bins_indices]
     
-    return bins_values, bins_indices, bin_midpoints, bin_counts, bin_edges
+    return bins_values, bins_indices, bin_midpoints, bin_counts, bin_edges
+
+def calculate_fragility(df,limit_name,limits,IM_column,EDP_column,plot=True):
+    ''' Function to calculate fragility based on a dataframe.
+    The dataframe must have a column named bin which containst the values for
+    the intensity measure. It also must have a column that you 
+    
+    Inputs:
+        df: dataframe
+        limit_name: how you want to name your limits
+        limits: values to define the limits
+        column_limit: dataframe column to check the exceedance of the values in limits
+        plot: by default is True, meaning that it returns the plots. Set to false if you do not want them
+    
+    Outputs:
+        thetas: median of the lognormal distribution
+        betas: deviation of the lognormal distribution
+    
+    '''
+    ngm = df[IM_column].value_counts().to_numpy()
+    
+    for i in range(len(limits)):
+        df[limit_name[i]] = df[EDP_column] > limits[i]
+
+    true_counts = df.groupby(IM_column)[limit_name].apply(lambda x: x.sum()).reset_index()
+    thetas, betas = [],[]
+    
+    for i,lim in enumerate(limit_name):
+        theta,beta = fn_mle_pc(true_counts[IM_column], ngm, true_counts[lim])
+        thetas.append(theta)
+        betas.append(beta)
+        if plot==True:
+            plt.plot(true_counts[IM_column],true_counts[lim]/ngm[i],'x')
+            plotfrag(theta, beta)
+        
+    if plot==True:
+        plt.xlabel('Sa(g)')
+        plt.ylabel('Probability')
+        plt.show()
+    
+    return thetas,betas
```

### Comparing `opseestools-0.15/opseestools/analisis.py` & `opseestools-0.2/opseestools/analisis.py`

 * *Files 0% similar despite different names*

```diff
@@ -2487,15 +2487,15 @@
     unicos = np.unique(kfails)                                                  # Para encontrar los valores únicos donde se producen fallas de la mamposteria
     unicos2 = unicos[unicos<1e8]                                                # Para quitar los valores de 1e9 que hicimos para el artificio
     
     # retornar tiempo, desplazamiento de recho, Fuerzas globales,fuerza en el 
     # puntal A, fuerza en el puntal B, Desplazamiento, velocidad, aceleración, 
     # deriva, instante de tiempo en el que el muro falla
     
-    return tiempo,techo,Eds,f_puntalA,f_puntalB,node_disp,node_vel,node_acel,drift,unicos2, Prot, fiber_s, fiber_c
+    return tiempo,techo,Eds,f_puntalA,f_puntalB,node_disp,node_vel,node_acel,drift,unicos2
 
 #%% ============================ FUNCIONES REMOVAL ============================
 
 def removal(nodeI,nodeJ,ele,der):
     fuerza=0
     d1= nodeDisp(nodeI,1)
     d2= nodeDisp(nodeJ,1)
```

### Comparing `opseestools-0.15/opseestools/analisis3D.py` & `opseestools-0.2/opseestools/analisis3D.py`

 * *Files identical despite different names*

### Comparing `opseestools-0.15/opseestools/utilidades.py` & `opseestools-0.2/opseestools/utilidades.py`

 * *Files identical despite different names*

### Comparing `opseestools-0.15/opseestools.egg-info/PKG-INFO` & `opseestools-0.2/opseestools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: opseestools
-Version: 0.15
+Version: 0.2
 Summary: A collection of OpenSeesPy routines for performing several types of analyses and other tools
-Home-page: https://github.com/odarroyo/opstools
+Home-page: https://github.com/odarroyo/opseestools
 Author: Orlando Arroyo
 Author-email: odarroyo@uc.cl
 License: LICENSE
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: openseespy>=3.5
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy>=1.11
+Requires-Dist: pandas>=2.0
 
 # opseestools
 
 This is a library to be used with OpenSeesPy.
 
 It includes a collection of analysis functions that are useful if you are analyzing frames or wall buildings both in two and three dimensions, storing the results in Python variables. 
 It also includes another useful tools for processing results and creating scripts
@@ -40,15 +41,16 @@
 
 import opstools.utilidades as ut (or any other name)
 
 4) A library to calculate and plot fragility functions. You can import it as:
 
 import opstools.Lib_frag as ut (or any other name)
 
-The full documentation is available on the GitHub website: https://github.com/odarroyo/opstools 
+The full documentation is available on the GitHub website: https://github.com/odarroyo/opseestools 
+Tutorials of how to use the functions are available in: https://github.com/odarroyo/openseespy_starting_tutorials
 
 ## 2D Analysis functions
 
 Here's a brief description of some of the functions:
 
 ### gravedad()
 To perform gravity analysis of a model you created. In a more general sense, it runs a static analysis, but returns no output. The idea of this script is to perform the gravity analysis before a pushover or other nonlinear analysis.
```

### Comparing `opseestools-0.15/setup.py` & `opseestools-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 @author: HOME
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='opseestools',
-    version='0.15',
+    version='0.2',
     author='Orlando Arroyo',
     author_email='odarroyo@uc.cl',
     packages=find_packages(),
     description='A collection of OpenSeesPy routines for performing several types of analyses and other tools',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'openseespy>=3.5',  # Requires a version of OpenSeesPy later than 3.5
         'matplotlib',  # Any version of matplotlib
         'numpy',  # Any version of numpy
-        'scipy>=1.11'
+        'scipy>=1.11',
+        'pandas>=2.0'
     ],
     python_requires='>=3.9', # Adjust based on your compatibility
-    url='https://github.com/odarroyo/opstools',
+    url='https://github.com/odarroyo/opseestools',
     license='LICENSE', # If you have a license file
 )
```

