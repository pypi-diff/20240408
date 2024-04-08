# Comparing `tmp/startlit-0.0.1.tar.gz` & `tmp/startlit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "startlit-0.0.1.tar", max compression
+gzip compressed data, was "startlit-0.0.2.tar", max compression
```

## Comparing `startlit-0.0.1.tar` & `startlit-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-05 05:24:49.712398 startlit-0.0.1/LICENSE
--rw-r--r--   0        0        0     1303 2024-04-05 05:24:49.712398 startlit-0.0.1/README.md
--rw-r--r--   0        0        0      520 2024-04-05 05:24:49.712398 startlit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-05 05:24:49.712398 startlit-0.0.1/src/startlit/__init__.py
--rw-r--r--   0        0        0      970 2024-04-05 05:24:49.712398 startlit-0.0.1/src/startlit/start.py
--rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 startlit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 11:02:08.344472 startlit-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2716 2024-04-08 11:02:08.344472 startlit-0.0.2/README.md
+-rw-r--r--   0        0        0      520 2024-04-08 11:02:08.344472 startlit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-08 11:02:08.344472 startlit-0.0.2/src/startlit/__init__.py
+-rw-r--r--   0        0        0     2903 2024-04-08 11:02:08.344472 startlit-0.0.2/src/startlit/start.py
+-rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 startlit-0.0.2/PKG-INFO
```

### Comparing `startlit-0.0.1/LICENSE` & `startlit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `startlit-0.0.1/pyproject.toml` & `startlit-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "startlit"
-version = "0.0.1"
+version = "0.0.2"
 description = "Get started with a streamlit app template code in style"
 authors = ["Indraneel Chakraborty"]
 readme = "README.md"
 homepage = "https://github.com/ineelhere/startlit"
 license = "Apache License - Version 2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `startlit-0.0.1/PKG-INFO` & `startlit-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 Metadata-Version: 2.1
 Name: startlit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get started with a streamlit app template code in style
 Home-page: https://github.com/ineelhere/startlit
 License: Apache License - Version 2.0
 Author: Indraneel Chakraborty
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
-# StartLit
+# StartLit ⭐
+
+**Welcome to StartLit!**
+
+StartLit is your gateway to building Streamlit apps with ease. It brings a simple, streamlined way to start your Streamlit projects. Here's what's included in the latest release:
+
+#### Features:
+- **Package Installation**: Now you can easily install StartLit from PYPI using `pip install startlit`.
+- **Simple Usage**: Import the package and run `hello()` to receive a friendly welcome message.
+- **Basic help**: Use the `help()` function to get started with more support
+-  **Starter App**: Use the `starter()` function to download a very simple starter app template, including an `app.py` file and a `requirements.txt` file.
+-  **Multipage App**: Use the `multipage()` function to download an app template for building multipage Streamlit apps. The files/folders will be available in your working directory.
+-  **Fragments App**: Use the `fragments()` function to download an app that allows you to run independent components in the streamlit app.
+
 
-Get started with a streamlit app template code in style.
 
 ### Install the package from PYPI
 
 ```python
 pip install startlit
 ```
 ### Import the package
@@ -40,14 +52,15 @@
 ```python
 starter()
 ```
 Output - 
 ```
 📥 Starter app downloaded!📥
 👀 Look for 'app.py' and 'requirements.txt' file in your working directory 👀
+💡 Visit https://startlit-starter.streamlit.app/ for a quick look to the starter app
 ```
 
 If you look up in your local/working directory, you should find the 2 files present as mentioned above.
 
 ___
 
 ```bash
@@ -71,13 +84,37 @@
 st.title('Hello, World! 🌎🚀')
 
 # Add a description with an inline comment
 st.write("This is my first app in Streamlit! 📝")  # Comment: Don't forget to smile
 ```
 
 ___
+### Other functions
+```python
+
+# get a list of available ftrs
+help()
+
+# Download a starter app template
+starter()
+
+# Download a multipage app template
+multipage()
+
+# Download a fragment app template
+fragments()
+
+
+```
+___
 
+### Feedback and Contribution:
+Excited to hear your feedback and suggestions for improvements. 
+Feel free to open issues or submit pull requests.
+
+Enjoy your streamlit journey with StartLit and happy coding! 🚀🎉
+___
 
-**© `Indraneel Chakraborty` | 2024** 🧑‍💻[ Email](mailto:hello.indraneel@gmail.com) | [LinkedIn](https://www.linkedin.com/in/indraneelchakraborty/) | [GitHub](https://github.com/ineelhere)
+**© `Indraneel Chakraborty` | 2024** 🧑‍💻[LinkedIn](https://www.linkedin.com/in/indraneelchakraborty/) | [X/Twitter](https://twitter.com/ineelhere)
 
 
 `Collaborations and Contributions are welcome 🤝`
```

