# Comparing `tmp/unesco_reader-0.3.1.tar.gz` & `tmp/unesco_reader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unesco_reader-0.3.1.tar", max compression
+gzip compressed data, was "unesco_reader-1.0.0.tar", max compression
```

## Comparing `unesco_reader-0.3.1.tar` & `unesco_reader-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-03-17 11:27:27.988247 unesco_reader-0.3.1/LICENSE
--rw-r--r--   0        0        0     6279 2023-03-17 11:27:27.988247 unesco_reader-0.3.1/README.md
--rw-r--r--   0        0        0     1241 2023-03-17 11:27:27.988247 unesco_reader-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      117 2023-03-17 11:27:27.988247 unesco_reader-0.3.1/src/unesco_reader/__init__.py
--rw-r--r--   0        0        0     2797 2023-03-17 11:27:27.988247 unesco_reader-0.3.1/src/unesco_reader/common.py
--rw-r--r--   0        0        0      980 2023-03-17 11:27:27.988247 unesco_reader-0.3.1/src/unesco_reader/config.py
--rw-r--r--   0        0        0      269 2023-03-17 11:27:27.988247 unesco_reader-0.3.1/src/unesco_reader/glossaries/uis_datasets.csv
--rw-r--r--   0        0        0    17569 2023-03-17 11:27:27.988247 unesco_reader-0.3.1/src/unesco_reader/uis.py
--rw-r--r--   0        0        0     6900 1970-01-01 00:00:00.000000 unesco_reader-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-08 07:52:49.180888 unesco_reader-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7429 2024-04-08 07:52:49.180888 unesco_reader-1.0.0/README.md
+-rw-r--r--   0        0        0      694 2024-04-08 07:52:49.180888 unesco_reader-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-04-08 07:52:49.180888 unesco_reader-1.0.0/src/unesco_reader/__init__.py
+-rw-r--r--   0        0        0     1054 2024-04-08 07:52:49.180888 unesco_reader-1.0.0/src/unesco_reader/config.py
+-rw-r--r--   0        0        0    12421 2024-04-08 07:52:49.180888 unesco_reader-1.0.0/src/unesco_reader/formatting.py
+-rw-r--r--   0        0        0     5823 2024-04-08 07:52:49.180888 unesco_reader-1.0.0/src/unesco_reader/read.py
+-rw-r--r--   0        0        0    13777 2024-04-08 07:52:49.180888 unesco_reader-1.0.0/src/unesco_reader/uis.py
+-rw-r--r--   0        0        0     8075 1970-01-01 00:00:00.000000 unesco_reader-1.0.0/PKG-INFO
```

### Comparing `unesco_reader-0.3.1/LICENSE` & `unesco_reader-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unesco_reader-0.3.1/README.md` & `unesco_reader-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,131 +5,173 @@
 [![Documentation Status](https://readthedocs.org/projects/unesco-reader/badge/?version=latest)](https://unesco-reader.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/lpicci96/unesco_reader/branch/main/graph/badge.svg)](https://codecov.io/gh/lpicci96/unesco_reader)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 
 Pythonic access to UNESCO data
 
-`unesco_reader` is a Python package providing a simple interface to access UNESCO data. 
-UNESCO does not currently provide an API to access its data, particularly the widely used 
-UNESCO Institute for Statistics (UIS) data. Users must download the data from the UIS bulk download
-services as a zipped file, and then extract the data from the zip file. This requires several manual steps,
-and some of the datasets are too large to be read easily with a standard spreadsheet program
-and must be read programmatically. UNESCO provides some guidance on how to do this in their 
-[python tutorial](https://apiportal.uis.unesco.org/bdds-tutorial).
-
-With `unesco_reader`, users don't need to worry about downloading the data, extracting it from the zip file,
-and following the python tutorial - this is all taken care of. This package handles accessing the data directly from the UNESCO website, and provides a simple interface to
-explore the data.
-
-<b>Note</b>:
-
-This package is currently in development, and only supports UIS datasets.
-It contains basic functionality to extract and interact with the data, 
-and will be expanded to include more analytical functionality in the future.
-All feedback, suggestions, and contributions are welcome!
-
+`unesco_reader` is a Python package that provides a simple interface to access UNESCO Institute of Statistics (UIS)
+data. UIS currently does not offer API access to its data. Users must download zipped files and extract the data.
+This process requires several manual steps explained in their [python tutorial](https://apiportal.uis.unesco.org/bdds-tutorial). This package simplifies the process by providing a simple
+interface to access, explore, and analyze the data, already structured and formatted through pandas DataFrames. This package also
+allows users to view dataset documentation and other information such as the date of last update, as well as retrieve
+information about all available datasets from UIS.
+
+### Note</b>: 
+UIS data is expected to be accessible through the [DataCommons](https://datacommons.org/) API in the future and should
+be the preferred method to access the data. Future versions of this package may include support for the API,
+or may be deprecated and remain as a legacy package.
+
+This package is designed to scrape data from the UIS website. As a result of this approach
+the package may be subject to breakage if the website structure or data file formats change without notice. 
+Please report any unexpected errors or issues you encounter. All feedback, suggestions, and contributions are welcome!
 
 ## Installation
 
 ```bash
 $ pip install unesco-reader
 ```
 
 ## Usage
 
-To access UIS data, import the `uis` module from `unesco_reader`
+Importing the package
 ```python
-from unesco_reader import uis
+import unesco_reader as uis
 ```
 
+Retrieve information about all the available datasets from UIS.
+```python
+uis.info()
+```
+This function will display all available datasets and relevant information about them.
+```
+>>>
+name                                                               latest_update    theme
+-----------------------------------------------------------------  ---------------  ---------
+SDG Global and Thematic Indicators                                 February 2024    Education
+Other Policy Relevant Indicators (OPRI)                            February 2024    Education
+Research and Development (R&D) SDG 9.5                             February 2024    Science
+Research and Development (R&D) – Other Policy Relevant Indicators  February 2024    Science
+...
+```
 
-You can see available datasets or retrieve information for a particular dataset. 
-To see all available datasets from UIS, run the following function:
-
+Retrieve a list of all available datasets from UIS.
 ```python
 uis.available_datasets()
 ```
-The output will be a list of available dataset codes `['SDG', 'OPRI', 'SCI', 'SDG11', 'DEM']`.
 
-Optionally you can return available datasets as names, and see available 
-datasets that belong to a particular category.
+```
+>>> ['SDG Global and Thematic Indicators',
+     'Other Policy Relevant Indicators (OPRI)',
+     'Research and Development (R&D) SDG 9.5',
+     ...]
+```
 
+Optionally you can specify a theme to filter the datasets.
 ```python
-uis.available_datasets(as_names=True, category='education')
+uis.available_datasets(theme='Education')
 ```
 
-To see details about a particular dataset, call the `dataset_info()` 
-function passing in either the dataset code or name.
+
+To access data for a particular dataset, use the `UIS` class passing the name of the dataset. 
+A `UIS` object allows a user to easily access, explore, and analyse the data.
+On instantiation, the data will be extracted from the UIS website, or if it has already been 
+extracted, it will be read from the cache (more on caching below)
 
 ```python
-uis.dataset_info('SDG')
+from unesco_reader import UIS
+
+sdg = UIS("SDG Global and Thematic Indicators")
 ```
 
-Information about the dataset will be printed:
+Basic information about the dataset can be accessed using the `info` method.
+```python
+sdg.info()
 ```
-----------------  -----------------------------------------------
-dataset_name      SDG Global and Thematic Indicators
-dataset_code      SDG
-dataset_category  education
-----------------  -----------------------------------------------
+This will display information about the dataset, such as the name, and the latest update, and theme
+
+```
+>>>
+-------------  ----------------------------------
+name           SDG Global and Thematic Indicators
+latest update  February 2024
+theme          Education
+-------------  ----------------------------------
 ```
 
-To extract and explore the data in a particular dataset, use the `UIS` class. 
-A `UIS` object allows a user to extract the data, either from directly from
-UIS bulk download services, or from a zipped file downloaded locally, 
-and explore and analyze the data easily.
+Information is also accessible through the attributes of the object.
+```python
+name = sdg.name
+update = sdg.latest_update
+theme = sdg.theme
+documentation = sdg.readme
+```
 
-To use, first create an instance of `UIS`, passing either the dataset code or name. 
-Here we create an object for the "SDG" dataset.
+The `readme` attribute contains the dataset documentation. To display the documentation, use the `display_readme` method.
+```python
+sdg.display_readme()
+```
 
+Various methods exist to access the data.
+To access country data:
 ```python
-sdg = uis.UIS("SDG")
+df = sdg.get_country_data()
 ```
+This will return a pandas DataFrame with the country data, in a structured and expected format.
+By default the dataframe will not contain metadata. To include metadata in the output, set the `include_metadata` parameter to `True`.
+Countries may also be filtered for a specific region by specifying the region's ID in the `region` parameter.
+To see available regions use the `get_regions` method.
 
-Once instantiated, you can retrieve relevant information about the dataset
+```python
+df = sdg.get_country_data(include_metadata=True, region='WB: World')
+```
 
+To access regional data:
 ```python
-sdg.dataset_name # SDG Global and Thematic Indicators
-sdg.dataset_code # SDG
-sdg.dataset_category # education
-sdg.link # https://apimgmtstzgjpfeq2u763lag.blob.core.windows.net/uisdatastore/SDG.zip
+df = sdg.get_region_data()
 ```
+This will return a pandas DataFrame with the regional data, in a structured and expected format. Note that not all datasets contain regional data.
+If the dataset does not contain regional data, an error will be raised. This is the same for any other data that is not available for the particular dataset.
+By default the dataframe will not contain metadata. To include metadata in the output, set the `include_metadata` parameter to `True`.
 
-To access and start exploring the data, you need to load the data to the object
-using the `load_data` method. This will download the data from the UNESCO website,
-clean it, and format it as a pandas DataFrame stored in the object. Optionally,
-if you have downloaded the zipped file locally, you can pass the path to the file.
+Metadata, available countries, available regions, and variables are also accessible through class objects.
+```python
+metadata_df = sdg.get_metadata()
+countries_df = sdg.get_countries()
+regions_df = sdg.get_regions()
+variables_df = sdg.get_variables()
+```
 
+To refresh the data and extract the latest data from the UIS website, use the `refresh` method.
 ```python
-sdg = UIS("SDG")
-sdg.load_data()
+sdg.refresh()
 ```
 
-Once the data is loaded, you can access it using the `get_data` method.
+### Caching
+
+Caching is used to prevent unnecessary requests to the UIS website and enhance performance.
+To refresh data returned by functions, use the `refresh` parameter. Caching using the LRU 
+(Least Recently Used) algorithm approach and stores data in RAM. The cache is cleared when the
+program is terminated.
 
 ```python
-df = sdg.get_data()
-print(df)
+uis.info(refresh=True)
+uis.available_datasets(refresh=True)
 ```
-The result will be a pandas DataFrame with the data. Here is a sample what the data looks like:
-
-| INDICATOR_ID           | INDICATOR_NAME                                   | COUNTRY_ID | COUNTRY_NAME | YEAR | VALUE |
-| ---------------------- | ------------------------------------------------ | ---------- | ------------ | ---- | ----- |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2014 | 0.0   |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2015 | 0.0   |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2016 | 0.0   |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2017 | 0.0   |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2018 | 0.0   |
+`refresh=True` will clear the cache and force extraction of the data and information from the UIS website.
 
-In the `get_data` you can specify whether you want to return country or regional (if available) data,
-and whether to include metadata in the dataframe. 
+For the `UIS` class, the `refresh` method will clear the cache and extract the latest data from the UIS website.
+```python
+sdg.refresh()
+```
 
-Several other tools are available to explore the data. 
-Please see the [documentation](https://unesco-reader.readthedocs.io/en/latest/) for more details.
+To clear all cached data, use the `clear_all_caches` method.
+```python
+uis.clear_all_caches()
+```
 
 
 ## Contributing
 
 All contributions are welcome! If you find a bug, 
 or have a suggestion for a new feature, or an 
 improvement on the documentation please open an issue.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `unesco_reader-0.3.1/src/unesco_reader/config.py` & `unesco_reader-1.0.0/src/unesco_reader/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-"""Configuration file for unesco_reader"""
+"""Configuration file for unesco_reader
+
+This file contains the configuration for the logger used in the unesco_reader package and
+the custom exceptions used in the package.
+
+"""
 
-from pathlib import Path
 import logging
 
 
-class PATHS:
-    """Paths"""
+# Custom Exceptions
 
-    package = Path(__file__).resolve().parent.parent
 
-    DATASETS = package / "unesco_reader" / "glossaries"
+class NoDataError(Exception):
+    """This is a custom exception that is raised when no UIS data exists"""
 
-    TEST_FILES = package / "tests" / "test_files"
+    pass
 
 
-# =========================================
 # Configure Logging
-# =========================================
-
 logger = logging.getLogger(__name__)
-# Create terminal handler
-shell_handler = logging.StreamHandler()
-# Set levels for the logger, shell and file
-logger.setLevel(logging.DEBUG)
-shell_handler.setLevel(logging.DEBUG)
-# Format the outputs
-fmt_file = "%(levelname)s (%(asctime)s): %(message)s"
-fmt_shell = (
-    "%(levelname)s %(asctime)s [%(filename)s:%(funcName)s:%(lineno)d] %(message)s"
-)
-# Create formatters
-shell_formatter = logging.Formatter(fmt_shell)
-# Add formatters to handlers
-shell_handler.setFormatter(shell_formatter)
-# Add handlers to the logger
-logger.addHandler(shell_handler)
+shell_handler = logging.StreamHandler()  # Create terminal handler
+logger.setLevel(logging.INFO)  # Set levels for the logger, shell and file
+shell_handler.setLevel(logging.INFO)  # Set levels for the logger, shell and file
+
+# Format the outputs   "%(levelname)s (%(asctime)s): %(message)s"
+fmt_file = "%(levelname)s: %(message)s"
+
+# "%(levelname)s %(asctime)s [%(filename)s:%(funcName)s:%(lineno)d] %(message)s"
+fmt_shell = "%(levelname)s: %(message)s"
+
+shell_formatter = logging.Formatter(fmt_shell)  # Create formatters
+shell_handler.setFormatter(shell_formatter)  # Add formatters to handlers
+logger.addHandler(shell_handler)  # Add handlers to the logger
```

### Comparing `unesco_reader-0.3.1/PKG-INFO` & `unesco_reader-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,153 +1,196 @@
 Metadata-Version: 2.1
 Name: unesco-reader
-Version: 0.3.1
+Version: 1.0.0
 Summary: Pythonic access to UNESCO data
 License: MIT
 Author: Luca Picci
-Requires-Python: >=3.8,<4
+Author-email: lpicci96@gmail.com
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bs4 (>=0.0.2,<0.0.3)
+Requires-Dist: myst-parser (>=2.0.0,<3.0.0)
+Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # unesco_reader
 
 [![PyPI](https://img.shields.io/pypi/v/unesco_reader.svg)](https://pypi.org/project/unesco_reader/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unesco_reader.svg)](https://pypi.org/project/unesco_reader/)
 [![Documentation Status](https://readthedocs.org/projects/unesco-reader/badge/?version=latest)](https://unesco-reader.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/lpicci96/unesco_reader/branch/main/graph/badge.svg)](https://codecov.io/gh/lpicci96/unesco_reader)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 
 Pythonic access to UNESCO data
 
-`unesco_reader` is a Python package providing a simple interface to access UNESCO data. 
-UNESCO does not currently provide an API to access its data, particularly the widely used 
-UNESCO Institute for Statistics (UIS) data. Users must download the data from the UIS bulk download
-services as a zipped file, and then extract the data from the zip file. This requires several manual steps,
-and some of the datasets are too large to be read easily with a standard spreadsheet program
-and must be read programmatically. UNESCO provides some guidance on how to do this in their 
-[python tutorial](https://apiportal.uis.unesco.org/bdds-tutorial).
-
-With `unesco_reader`, users don't need to worry about downloading the data, extracting it from the zip file,
-and following the python tutorial - this is all taken care of. This package handles accessing the data directly from the UNESCO website, and provides a simple interface to
-explore the data.
-
-<b>Note</b>:
-
-This package is currently in development, and only supports UIS datasets.
-It contains basic functionality to extract and interact with the data, 
-and will be expanded to include more analytical functionality in the future.
-All feedback, suggestions, and contributions are welcome!
-
+`unesco_reader` is a Python package that provides a simple interface to access UNESCO Institute of Statistics (UIS)
+data. UIS currently does not offer API access to its data. Users must download zipped files and extract the data.
+This process requires several manual steps explained in their [python tutorial](https://apiportal.uis.unesco.org/bdds-tutorial). This package simplifies the process by providing a simple
+interface to access, explore, and analyze the data, already structured and formatted through pandas DataFrames. This package also
+allows users to view dataset documentation and other information such as the date of last update, as well as retrieve
+information about all available datasets from UIS.
+
+### Note</b>: 
+UIS data is expected to be accessible through the [DataCommons](https://datacommons.org/) API in the future and should
+be the preferred method to access the data. Future versions of this package may include support for the API,
+or may be deprecated and remain as a legacy package.
+
+This package is designed to scrape data from the UIS website. As a result of this approach
+the package may be subject to breakage if the website structure or data file formats change without notice. 
+Please report any unexpected errors or issues you encounter. All feedback, suggestions, and contributions are welcome!
 
 ## Installation
 
 ```bash
 $ pip install unesco-reader
 ```
 
 ## Usage
 
-To access UIS data, import the `uis` module from `unesco_reader`
+Importing the package
 ```python
-from unesco_reader import uis
+import unesco_reader as uis
 ```
 
+Retrieve information about all the available datasets from UIS.
+```python
+uis.info()
+```
+This function will display all available datasets and relevant information about them.
+```
+>>>
+name                                                               latest_update    theme
+-----------------------------------------------------------------  ---------------  ---------
+SDG Global and Thematic Indicators                                 February 2024    Education
+Other Policy Relevant Indicators (OPRI)                            February 2024    Education
+Research and Development (R&D) SDG 9.5                             February 2024    Science
+Research and Development (R&D) – Other Policy Relevant Indicators  February 2024    Science
+...
+```
 
-You can see available datasets or retrieve information for a particular dataset. 
-To see all available datasets from UIS, run the following function:
-
+Retrieve a list of all available datasets from UIS.
 ```python
 uis.available_datasets()
 ```
-The output will be a list of available dataset codes `['SDG', 'OPRI', 'SCI', 'SDG11', 'DEM']`.
 
-Optionally you can return available datasets as names, and see available 
-datasets that belong to a particular category.
+```
+>>> ['SDG Global and Thematic Indicators',
+     'Other Policy Relevant Indicators (OPRI)',
+     'Research and Development (R&D) SDG 9.5',
+     ...]
+```
 
+Optionally you can specify a theme to filter the datasets.
 ```python
-uis.available_datasets(as_names=True, category='education')
+uis.available_datasets(theme='Education')
 ```
 
-To see details about a particular dataset, call the `dataset_info()` 
-function passing in either the dataset code or name.
+
+To access data for a particular dataset, use the `UIS` class passing the name of the dataset. 
+A `UIS` object allows a user to easily access, explore, and analyse the data.
+On instantiation, the data will be extracted from the UIS website, or if it has already been 
+extracted, it will be read from the cache (more on caching below)
 
 ```python
-uis.dataset_info('SDG')
+from unesco_reader import UIS
+
+sdg = UIS("SDG Global and Thematic Indicators")
 ```
 
-Information about the dataset will be printed:
+Basic information about the dataset can be accessed using the `info` method.
+```python
+sdg.info()
 ```
-----------------  -----------------------------------------------
-dataset_name      SDG Global and Thematic Indicators
-dataset_code      SDG
-dataset_category  education
-----------------  -----------------------------------------------
+This will display information about the dataset, such as the name, and the latest update, and theme
+
+```
+>>>
+-------------  ----------------------------------
+name           SDG Global and Thematic Indicators
+latest update  February 2024
+theme          Education
+-------------  ----------------------------------
 ```
 
-To extract and explore the data in a particular dataset, use the `UIS` class. 
-A `UIS` object allows a user to extract the data, either from directly from
-UIS bulk download services, or from a zipped file downloaded locally, 
-and explore and analyze the data easily.
+Information is also accessible through the attributes of the object.
+```python
+name = sdg.name
+update = sdg.latest_update
+theme = sdg.theme
+documentation = sdg.readme
+```
 
-To use, first create an instance of `UIS`, passing either the dataset code or name. 
-Here we create an object for the "SDG" dataset.
+The `readme` attribute contains the dataset documentation. To display the documentation, use the `display_readme` method.
+```python
+sdg.display_readme()
+```
 
+Various methods exist to access the data.
+To access country data:
 ```python
-sdg = uis.UIS("SDG")
+df = sdg.get_country_data()
 ```
+This will return a pandas DataFrame with the country data, in a structured and expected format.
+By default the dataframe will not contain metadata. To include metadata in the output, set the `include_metadata` parameter to `True`.
+Countries may also be filtered for a specific region by specifying the region's ID in the `region` parameter.
+To see available regions use the `get_regions` method.
 
-Once instantiated, you can retrieve relevant information about the dataset
+```python
+df = sdg.get_country_data(include_metadata=True, region='WB: World')
+```
 
+To access regional data:
 ```python
-sdg.dataset_name # SDG Global and Thematic Indicators
-sdg.dataset_code # SDG
-sdg.dataset_category # education
-sdg.link # https://apimgmtstzgjpfeq2u763lag.blob.core.windows.net/uisdatastore/SDG.zip
+df = sdg.get_region_data()
 ```
+This will return a pandas DataFrame with the regional data, in a structured and expected format. Note that not all datasets contain regional data.
+If the dataset does not contain regional data, an error will be raised. This is the same for any other data that is not available for the particular dataset.
+By default the dataframe will not contain metadata. To include metadata in the output, set the `include_metadata` parameter to `True`.
 
-To access and start exploring the data, you need to load the data to the object
-using the `load_data` method. This will download the data from the UNESCO website,
-clean it, and format it as a pandas DataFrame stored in the object. Optionally,
-if you have downloaded the zipped file locally, you can pass the path to the file.
+Metadata, available countries, available regions, and variables are also accessible through class objects.
+```python
+metadata_df = sdg.get_metadata()
+countries_df = sdg.get_countries()
+regions_df = sdg.get_regions()
+variables_df = sdg.get_variables()
+```
 
+To refresh the data and extract the latest data from the UIS website, use the `refresh` method.
 ```python
-sdg = UIS("SDG")
-sdg.load_data()
+sdg.refresh()
 ```
 
-Once the data is loaded, you can access it using the `get_data` method.
+### Caching
+
+Caching is used to prevent unnecessary requests to the UIS website and enhance performance.
+To refresh data returned by functions, use the `refresh` parameter. Caching using the LRU 
+(Least Recently Used) algorithm approach and stores data in RAM. The cache is cleared when the
+program is terminated.
 
 ```python
-df = sdg.get_data()
-print(df)
+uis.info(refresh=True)
+uis.available_datasets(refresh=True)
 ```
-The result will be a pandas DataFrame with the data. Here is a sample what the data looks like:
-
-| INDICATOR_ID           | INDICATOR_NAME                                   | COUNTRY_ID | COUNTRY_NAME | YEAR | VALUE |
-| ---------------------- | ------------------------------------------------ | ---------- | ------------ | ---- | ----- |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2014 | 0.0   |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2015 | 0.0   |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2016 | 0.0   |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2017 | 0.0   |
-| ADMI.ENDOFLOWERSEC.MAT | Administration of a nationally-representative... | ABW        | Aruba        | 2018 | 0.0   |
+`refresh=True` will clear the cache and force extraction of the data and information from the UIS website.
 
-In the `get_data` you can specify whether you want to return country or regional (if available) data,
-and whether to include metadata in the dataframe. 
+For the `UIS` class, the `refresh` method will clear the cache and extract the latest data from the UIS website.
+```python
+sdg.refresh()
+```
 
-Several other tools are available to explore the data. 
-Please see the [documentation](https://unesco-reader.readthedocs.io/en/latest/) for more details.
+To clear all cached data, use the `clear_all_caches` method.
+```python
+uis.clear_all_caches()
+```
 
 
 ## Contributing
 
 All contributions are welcome! If you find a bug, 
 or have a suggestion for a new feature, or an 
 improvement on the documentation please open an issue.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

