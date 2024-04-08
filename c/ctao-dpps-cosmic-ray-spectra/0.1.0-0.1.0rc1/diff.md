# Comparing `tmp/ctao-dpps-cosmic-ray-spectra-0.1.0.tar.gz` & `tmp/ctao-dpps-cosmic-ray-spectra-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctao-dpps-cosmic-ray-spectra-0.1.0.tar", last modified: Mon Apr  8 16:33:52 2024, max compression
+gzip compressed data, was "ctao-dpps-cosmic-ray-spectra-0.1.0rc1.tar", last modified: Mon Apr  8 13:26:34 2024, max compression
```

## Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0.tar` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1.tar`

### file list

```diff
@@ -1,47 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.153183 ctao-dpps-cosmic-ray-spectra-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3523 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1556 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1313 2024-04-08 16:33:52.153183 ctao-dpps-cosmic-ray-spectra-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.145183 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.145183 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)    22419 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/_static/cta.png
--rw-rw-rw-   0 root         (0) root         (0)    14315 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/_static/cta_dark.png
--rw-rw-rw-   0 root         (0) root         (0)     2659 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/installation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.149183 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/reference/
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/reference/definitions.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/reference/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/reference/index.rst!
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/docs/reference/spectral.rst
--rw-rw-rw-   0 root         (0) root         (0)     2600 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 16:33:52.153183 ctao-dpps-cosmic-ray-spectra-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/sonar-project.properties
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.145183 ctao-dpps-cosmic-ray-spectra-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.149183 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/
--rw-rw-rw-   0 root         (0) root         (0)      850 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-08 16:33:52.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2947 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.149183 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/resources/
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/resources/dampe_p+he_2019.ecsv
--rw-rw-rw-   0 root         (0) root         (0)     1382 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/resources/dampe_p+he_2021.ecsv
--rw-rw-rw-   0 root         (0) root         (0)    18436 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/spectral.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.149183 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/tests/test_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     9746 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/tests/test_spectral.py
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/tests/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)      739 2024-04-08 16:33:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:33:52.149183 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_dpps_cosmic_ray_spectra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1313 2024-04-08 16:33:52.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_dpps_cosmic_ray_spectra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-08 16:33:52.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_dpps_cosmic_ray_spectra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:33:52.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_dpps_cosmic_ray_spectra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      196 2024-04-08 16:33:52.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_dpps_cosmic_ray_spectra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-08 16:33:52.000000 ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_dpps_cosmic_ray_spectra.egg-info/top_level.txt
+drwxr-xr-x   0 mnoethe   (5074) app       (5002)        0 2024-04-08 13:26:34.305750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/
+-rw-r--r--   0 mnoethe   (5074) app       (5002)       47 2024-02-12 09:47:36.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/.dockerignore
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     1861 2024-02-12 09:47:36.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/.gitignore
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     3523 2024-04-08 13:24:05.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/.gitlab-ci.yml
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      709 2024-02-12 12:05:09.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     1386 2024-02-12 09:47:36.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/Dockerfile
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     1556 2024-02-12 09:47:36.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/LICENSE
+-rw-r--r--   0 mnoethe   (5074) app       (5002)       53 2024-02-12 10:01:56.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/MANIFEST.in
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     1267 2024-04-08 13:26:34.301750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      227 2024-02-12 09:56:43.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/README.md
+drwxr-xr-x   0 mnoethe   (5074) app       (5002)        0 2024-04-08 13:26:34.301750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      760 2024-02-12 09:47:36.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/Makefile
+drwxr-xr-x   0 mnoethe   (5074) app       (5002)        0 2024-04-08 13:26:34.301750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/_static/
+-rw-r--r--   0 mnoethe   (5074) app       (5002)    22419 2024-02-12 09:47:36.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/_static/cta.png
+-rw-r--r--   0 mnoethe   (5074) app       (5002)    14315 2024-02-12 09:47:36.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/_static/cta_dark.png
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     2387 2024-02-12 12:04:27.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/conf.py
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      301 2024-02-12 10:04:46.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/index.rst
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      601 2024-02-12 10:07:19.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/installation.rst
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      110 2024-02-12 10:54:10.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/reference.rst
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     2577 2024-04-08 13:17:09.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/pyproject.toml
+-rw-r--r--   0 mnoethe   (5074) app       (5002)       38 2024-04-08 13:26:34.305750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/setup.cfg
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      425 2024-02-12 12:04:27.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/sonar-project.properties
+drwxr-xr-x   0 mnoethe   (5074) app       (5002)        0 2024-04-08 13:26:34.297750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/
+drwxr-xr-x   0 mnoethe   (5074) app       (5002)        0 2024-04-08 13:26:34.301750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      115 2024-02-12 12:04:27.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/__init__.py
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      414 2024-04-08 13:26:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/_version.py
+drwxr-xr-x   0 mnoethe   (5074) app       (5002)        0 2024-04-08 13:26:34.301750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/resources/
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      629 2024-04-08 13:17:09.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/resources/dampe_p+he_2019.ecsv
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     1382 2024-04-08 13:17:09.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/resources/dampe_p+he_2021.ecsv
+-rw-r--r--   0 mnoethe   (5074) app       (5002)    21246 2024-04-08 13:17:09.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/spectral.py
+drwxr-xr-x   0 mnoethe   (5074) app       (5002)        0 2024-04-08 13:26:34.301750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/tests/
+-rw-r--r--   0 mnoethe   (5074) app       (5002)        0 2024-02-12 09:47:36.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/tests/__init__.py
+-rw-r--r--   0 mnoethe   (5074) app       (5002)    11108 2024-04-08 13:17:09.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/tests/test_spectral.py
+-rw-r--r--   0 mnoethe   (5074) app       (5002)       99 2024-02-12 10:54:32.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/tests/test_version.py
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      739 2024-02-12 12:04:27.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/version.py
+drwxr-xr-x   0 mnoethe   (5074) app       (5002)        0 2024-04-08 13:26:34.301750 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_dpps_cosmic_ray_spectra.egg-info/
+-rw-r--r--   0 mnoethe   (5074) app       (5002)     1267 2024-04-08 13:26:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_dpps_cosmic_ray_spectra.egg-info/PKG-INFO
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      905 2024-04-08 13:26:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_dpps_cosmic_ray_spectra.egg-info/SOURCES.txt
+-rw-r--r--   0 mnoethe   (5074) app       (5002)        1 2024-04-08 13:26:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_dpps_cosmic_ray_spectra.egg-info/dependency_links.txt
+-rw-r--r--   0 mnoethe   (5074) app       (5002)      178 2024-04-08 13:26:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_dpps_cosmic_ray_spectra.egg-info/requires.txt
+-rw-r--r--   0 mnoethe   (5074) app       (5002)       16 2024-04-08 13:26:34.000000 ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_dpps_cosmic_ray_spectra.egg-info/top_level.txt
```

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/.gitignore` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/.gitlab-ci.yml` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/.pre-commit-config.yaml` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/Dockerfile` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/Dockerfile`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/LICENSE` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/PKG-INFO` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctao-dpps-cosmic-ray-spectra
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: Common definitions of cosmic ray reference spectra
 Author-email: Maximilian Linhoff <maximilian.linhoff@tu-dortmund.de>
 License: BSD-3-Clause
 Project-URL: repository, https://gitlab.cta-observatory.org/cta-comuting/dpps/cosmic-ray-spectra
 Project-URL: documentation, http://cta-computing.gitlab-pages.cta-observatory.org/dpps/cosmic-ray-spectra
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -15,15 +15,14 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: pydata-sphinx-theme; extra == "doc"
-Requires-Dist: sphinx-automodapi; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Provides-Extra: all
 Requires-Dist: ctao-dpps-cosmic-ray-spectra[dev,doc,test]; extra == "all"
 
 # Cosmic Ray Reference Spectra
```

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/docs/Makefile` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 clean:
-	rm -rf api
+	rm -rf docs/api
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/docs/_static/cta.png` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/_static/cta.png`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/docs/_static/cta_dark.png` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/_static/cta_dark.png`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/docs/conf.py` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.githubpages",
     "sphinx.ext.intersphinx",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
-    "sphinx_automodapi.automodapi",
-    "sphinx_automodapi.smart_resolver",
     "numpydoc",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = []
 
 # List of patterns, relative to source directory, that match files and
@@ -43,15 +41,14 @@
 # have all links automatically associated with the right domain.
 default_role = "py:obj"
 
 
 # intersphinx allows referencing other packages sphinx docs
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3.8", None),
-    "astropy": ("https://docs.astropy.org/en/stable/", None),
 }
 
 # -- Options for HTML output -------------------------------------------------
 
 html_theme = "pydata_sphinx_theme"
 html_theme_options = dict(
     navigation_with_keys=False,
@@ -68,15 +65,7 @@
     navbar_start=["navbar-logo", "version-switcher"],
 )
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
-
-# needed by automodapi
-numpydoc_show_class_members = False
-
-nitpick_ignore = {
-    ("py:obj", "Unit"),
-    ("py:obj", "UnitBase"),
-}
```

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/docs/installation.rst` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/pyproject.toml` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
   "pytest",
   "pytest-cov",
 ]
 doc = [
   "sphinx",
   "numpydoc",
   "pydata-sphinx-theme",
-  "sphinx-automodapi",
 ]
 dev = [
   "setuptools_scm",
   "sphinx-autobuild",
 ]
 
 # we can use self-references to simplify all
```

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/resources/dampe_p+he_2019.ecsv` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/resources/dampe_p+he_2019.ecsv`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/resources/dampe_p+he_2021.ecsv` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/resources/dampe_p+he_2021.ecsv`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/spectral.py` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/spectral.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Functions and classes for calculating spectral weights."""
 from copy import copy
+from importlib.resources import as_file, files
 
 import astropy.units as u
 import numpy as np
 from astropy.table import QTable
 from scipy.interpolate import interp1d
 
 #: Unit of a point source flux
@@ -20,21 +21,28 @@
 __all__ = [
     "POINT_SOURCE_FLUX_UNIT",
     "DIFFUSE_FLUX_UNIT",
     "calculate_event_weights",
     "PowerLaw",
     "LogParabola",
     "PowerLawWithExponentialGaussian",
+    "CRAB_HEGRA",
+    "CRAB_MAGIC_JHEAP2015",
+    "PDG_ALL_PARTICLE",
+    "IRFDOC_PROTON_SPECTRUM",
+    "IRFDOC_ELECTRON_SPECTRUM",
     "TableInterpolationSpectrum",
+    "DAMPE_P_He_SPECTRUM",
 ]
 
 
 @u.quantity_input(angle=u.deg)
 def cone_solid_angle(angle):
     """
+
     Calculate the solid angle of a view cone.
 
     Parameters
     ----------
     angle: astropy.units.Quantity or astropy.coordinates.Angle
         Opening angle of the view cone.
 
@@ -429,14 +437,15 @@
             A string representation of the instance.
         """
         return f"{self.__class__.__name__}({self.normalization} * (E / {self.e_ref})**({self.a} + {self.b} * log10(E / {self.e_ref}))"
 
 
 class PowerLawWithExponentialGaussian(PowerLaw):
     r"""
+
     A power law with an additional Gaussian bump.
 
     Beware that the Gaussian is not normalized!
 
     .. math::
 
         \Phi(E, \Phi_0, \gamma, f, \mu, \sigma, E_\text{ref}) =
@@ -518,27 +527,29 @@
         s = super().__repr__()
         gauss = f"Gauss(log10(E / {self.e_ref}), {self.mu}, {self.sigma})"
         return s[:-1] + f" * (1 + {self.f} * (exp({gauss}) - 1))"
 
 
 class TableInterpolationSpectrum:
     """
-    Spectrum interpolating tabulated values.
+
+    Interpolate flux points to obtain a spectrum.
 
     By default, flux is interpolated linearly in log-log space.
     """
 
     def __init__(
         self,
         energy,
         flux,
         log_energy=True,
         log_flux=True,
         reference_energy=1 * u.TeV,
     ):
+        """Create a new TableInterpolationSpectrum spectrum."""
         self.energy = energy
         self.flux = flux
         self.flux_unit = flux.unit
         self.log_energy = log_energy
         self.log_flux = log_flux
         self.reference_energy = reference_energy
 
@@ -647,7 +658,75 @@
         """
         return cls.from_table(
             QTable.read(path),
             log_energy=log_energy,
             log_flux=log_flux,
             reference_energy=reference_energy,
         )
+
+
+#: Power Law parametrization of the Crab Nebula spectrum as published by HEGRA
+#:
+#: From "The Crab Nebula and Pulsar between 500 GeV and 80 TeV: Observations with the HEGRA stereoscopic air Cherenkov telescopes",
+#: Aharonian et al, 2004, ApJ 614.2
+#: doi.org/10.1086/423931
+CRAB_HEGRA = PowerLaw(
+    normalization=2.83e-11 / (u.TeV * u.cm**2 * u.s),
+    index=-2.62,
+    e_ref=1 * u.TeV,
+)
+
+#: Log-Parabola parametrization of the Crab Nebula spectrum as published by MAGIC
+#:
+#: From "Measurement of the Crab Nebula spectrum over three decades in energy with the MAGIC telescopes",
+#: Aleksìc et al., 2015, JHEAP
+#: https://doi.org/10.1016/j.jheap.2015.01.002
+CRAB_MAGIC_JHEAP2015 = LogParabola(
+    normalization=3.23e-11 / (u.TeV * u.cm**2 * u.s),
+    a=-2.47,
+    b=-0.24,
+)
+
+
+#: All particle spectrum
+#:
+#: (30.2) from "The Review of Particle Physics (2020)"
+#: https://pdg.lbl.gov/2020/reviews/rpp2020-rev-cosmic-rays.pdf
+PDG_ALL_PARTICLE = PowerLaw(
+    normalization=1.8e4 / (u.GeV * u.m**2 * u.s * u.sr),
+    index=-2.7,
+    e_ref=1 * u.GeV,
+)
+
+#: Proton spectrum definition defined in the CTA Prod3b IRF Document
+#:
+#: From "Description of CTA Instrument Response Functions (Production 3b Simulation)", section 4.3.1
+#: https://gitlab.cta-observatory.org/cta-consortium/aswg/documentation/internal_reports/irfs-reports/prod3b-irf-description
+IRFDOC_PROTON_SPECTRUM = PowerLaw(
+    normalization=9.8e-6 / (u.cm**2 * u.s * u.TeV * u.sr),
+    index=-2.62,
+    e_ref=1 * u.TeV,
+)
+
+#: Electron spectrum definition defined in the CTA Prod3b IRF Document
+#:
+#: From "Description of CTA Instrument Response Functions (Production 3b Simulation)", section 4.3.1
+#: https://gitlab.cta-observatory.org/cta-consortium/aswg/documentation/internal_reports/irfs-reports/prod3b-irf-description
+IRFDOC_ELECTRON_SPECTRUM = PowerLawWithExponentialGaussian(
+    normalization=2.385e-9 / (u.TeV * u.cm**2 * u.s * u.sr),
+    index=-3.43,
+    e_ref=1 * u.TeV,
+    mu=-0.101,
+    sigma=0.741,
+    f=1.950,
+)
+
+#: Proton + Helium interpolated from DAMPE measurements
+#:
+#: Datapoints obtained from obtained from:
+#: https://inspirehep.net/files/62efc8374ffced58ea7e3a333bfa1217
+#: Points are from DAMPE, up to  8 TeV.
+#: For higher energies we assume a
+#: flattening of the dF/dE*E^2.7 more or less in the middle of the large
+#: spread of the available data reported on the same proceeding
+with as_file(files("ctao_cr_spectra.resources") / "dampe_p+he_2019.ecsv") as _path:
+    DAMPE_P_He_SPECTRUM = TableInterpolationSpectrum.from_file(_path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/tests/test_spectral.py` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/tests/test_spectral.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 import astropy.units as u
 import numpy as np
 import pytest
 from astropy.table import QTable
 
 from ctao_cr_spectra.spectral import (
+    CRAB_HEGRA,
+    CRAB_MAGIC_JHEAP2015,
+    IRFDOC_ELECTRON_SPECTRUM,
+    IRFDOC_PROTON_SPECTRUM,
+    PDG_ALL_PARTICLE,
     LogParabola,
     PowerLaw,
     PowerLawWithExponentialGaussian,
     TableInterpolationSpectrum,
     calculate_event_weights,
     cone_solid_angle,
 )
@@ -304,7 +309,42 @@
 def test_table_interpolation_spectrum_init():
     spectrum = TableInterpolationSpectrum(energy_values, flux_values)
     assert np.all(spectrum.energy == energy_values)
     assert np.all(spectrum.flux == flux_values)
     assert spectrum.log_energy
     assert spectrum.log_flux
     assert spectrum.reference_energy == reference_energy
+
+
+@pytest.mark.parametrize(
+    ("spectrum", "expected_repr"),
+    [
+        (CRAB_HEGRA, "PowerLaw(2.83e-11 1 / (TeV s cm2) * (E / 1.0 TeV)**-2.62)"),
+        (
+            CRAB_MAGIC_JHEAP2015,
+            "LogParabola(3.23e-11 1 / (TeV s cm2) * (E / 1.0 TeV)**(-2.47 + -0.24 * "
+            "log10(E / 1.0 TeV))",
+        ),
+        (PDG_ALL_PARTICLE, "PowerLaw(18000.0 1 / (GeV s sr m2) * (E / 1.0 GeV)**-2.7)"),
+        (
+            IRFDOC_PROTON_SPECTRUM,
+            "PowerLaw(9.8e-06 1 / (TeV s sr cm2) * (E / 1.0 TeV)**-2.62)",
+        ),
+        (
+            IRFDOC_ELECTRON_SPECTRUM,
+            "PowerLawWithExponentialGaussian(2.385e-09 1 / (TeV s sr cm2) * (E / 1.0 TeV)**-3.43 *"
+            " (1 + 1.95 * (exp(Gauss(log10(E / 1.0 TeV), -0.101, 0.741)) - 1))",
+        ),
+    ],
+)
+def test_spectrum_repr(spectrum, expected_repr):
+    actual_repr = repr(spectrum)
+    assert actual_repr == expected_repr
+
+
+def test_dampe_p_he_spectrum():
+    # Define the path to the ECSV file
+    file_path = "src/ctao_cr_spectra/resources/dampe_p+he_2019.ecsv"
+    # Read the ECSV file using QTable
+    dampe_data = QTable.read(file_path, format="ascii.ecsv")
+    # Assert that the data is read successfully
+    assert len(dampe_data) > 0
```

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_cr_spectra/version.py` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_cr_spectra/version.py`

 * *Files identical despite different names*

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_dpps_cosmic_ray_spectra.egg-info/PKG-INFO` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_dpps_cosmic_ray_spectra.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctao-dpps-cosmic-ray-spectra
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: Common definitions of cosmic ray reference spectra
 Author-email: Maximilian Linhoff <maximilian.linhoff@tu-dortmund.de>
 License: BSD-3-Clause
 Project-URL: repository, https://gitlab.cta-observatory.org/cta-comuting/dpps/cosmic-ray-spectra
 Project-URL: documentation, http://cta-computing.gitlab-pages.cta-observatory.org/dpps/cosmic-ray-spectra
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -15,15 +15,14 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: pydata-sphinx-theme; extra == "doc"
-Requires-Dist: sphinx-automodapi; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Provides-Extra: all
 Requires-Dist: ctao-dpps-cosmic-ray-spectra[dev,doc,test]; extra == "all"
 
 # Cosmic Ray Reference Spectra
```

### Comparing `ctao-dpps-cosmic-ray-spectra-0.1.0/src/ctao_dpps_cosmic_ray_spectra.egg-info/SOURCES.txt` & `ctao-dpps-cosmic-ray-spectra-0.1.0rc1/src/ctao_dpps_cosmic_ray_spectra.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,24 @@
 README.md
 pyproject.toml
 sonar-project.properties
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/installation.rst
+docs/reference.rst
 docs/_static/cta.png
 docs/_static/cta_dark.png
-docs/reference/definitions.rst
-docs/reference/index.rst
-docs/reference/index.rst!
-docs/reference/spectral.rst
 src/ctao_cr_spectra/__init__.py
 src/ctao_cr_spectra/_version.py
-src/ctao_cr_spectra/definitions.py
 src/ctao_cr_spectra/spectral.py
 src/ctao_cr_spectra/version.py
 src/ctao_cr_spectra/resources/dampe_p+he_2019.ecsv
 src/ctao_cr_spectra/resources/dampe_p+he_2021.ecsv
 src/ctao_cr_spectra/tests/__init__.py
-src/ctao_cr_spectra/tests/test_definitions.py
 src/ctao_cr_spectra/tests/test_spectral.py
 src/ctao_cr_spectra/tests/test_version.py
 src/ctao_dpps_cosmic_ray_spectra.egg-info/PKG-INFO
 src/ctao_dpps_cosmic_ray_spectra.egg-info/SOURCES.txt
 src/ctao_dpps_cosmic_ray_spectra.egg-info/dependency_links.txt
 src/ctao_dpps_cosmic_ray_spectra.egg-info/requires.txt
 src/ctao_dpps_cosmic_ray_spectra.egg-info/top_level.txt
```

