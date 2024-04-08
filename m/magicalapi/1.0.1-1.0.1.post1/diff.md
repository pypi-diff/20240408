# Comparing `tmp/magicalapi-1.0.1.tar.gz` & `tmp/magicalapi-1.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicalapi-1.0.1.tar", max compression
+gzip compressed data, was "magicalapi-1.0.1.post1.tar", max compression
```

## Comparing `magicalapi-1.0.1.tar` & `magicalapi-1.0.1.post1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1067 2024-02-07 06:23:11.026629 magicalapi-1.0.1/LICENSE
--rw-r--r--   0        0        0     7845 2024-04-07 10:59:53.439999 magicalapi-1.0.1/README.md
--rw-r--r--   0        0        0       59 2024-02-07 06:23:11.033296 magicalapi-1.0.1/magicalapi/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 06:23:11.033296 magicalapi-1.0.1/magicalapi/abstractions/__init__.py
--rw-r--r--   0        0        0      413 2024-03-26 12:02:10.739930 magicalapi-1.0.1/magicalapi/abstractions/base_service.py
--rw-r--r--   0        0        0     3045 2024-03-27 12:47:18.029273 magicalapi-1.0.1/magicalapi/client.py
--rw-r--r--   0        0        0      270 2024-02-07 06:23:11.036629 magicalapi-1.0.1/magicalapi/errors.py
--rw-r--r--   0        0        0      693 2024-03-26 12:02:10.743263 magicalapi-1.0.1/magicalapi/services/__init__.py
--rw-r--r--   0        0        0     5238 2024-04-07 09:21:20.663262 magicalapi-1.0.1/magicalapi/services/base_service.py
--rw-r--r--   0        0        0     1275 2024-04-03 12:54:00.959978 magicalapi-1.0.1/magicalapi/services/company_data_service.py
--rw-r--r--   0        0        0     1433 2024-04-07 08:52:02.996638 magicalapi-1.0.1/magicalapi/services/profile_data_service.py
--rw-r--r--   0        0        0     1366 2024-04-07 08:52:02.999971 magicalapi-1.0.1/magicalapi/services/resume_parser_service.py
--rw-r--r--   0        0        0     1224 2024-03-27 12:42:51.355949 magicalapi-1.0.1/magicalapi/services/resume_review_service.py
--rw-r--r--   0        0        0     1458 2024-03-27 12:42:51.365949 magicalapi-1.0.1/magicalapi/services/resume_score_service.py
--rw-r--r--   0        0        0     1119 2024-03-27 12:42:51.365949 magicalapi-1.0.1/magicalapi/services/youtube_seo_service.py
--rw-r--r--   0        0        0     1766 2024-03-27 12:42:51.269282 magicalapi-1.0.1/magicalapi/services/youtube_suggestions_service.py
--rw-r--r--   0        0        0     3693 2024-03-27 12:42:51.272616 magicalapi-1.0.1/magicalapi/services/youtube_top_keywords_service.py
--rw-r--r--   0        0        0      982 2024-03-27 12:32:32.425971 magicalapi-1.0.1/magicalapi/settings.py
--rw-r--r--   0        0        0      292 2024-04-03 13:44:11.699802 magicalapi-1.0.1/magicalapi/types/__init__.py
--rw-r--r--   0        0        0      881 2024-04-07 09:21:20.663262 magicalapi-1.0.1/magicalapi/types/base.py
--rw-r--r--   0        0        0     1288 2024-03-26 12:02:10.743263 magicalapi-1.0.1/magicalapi/types/company_data.py
--rw-r--r--   0        0        0     3757 2024-04-07 08:52:02.999971 magicalapi-1.0.1/magicalapi/types/profile_data.py
--rw-r--r--   0        0        0     2028 2024-04-07 08:52:03.003305 magicalapi-1.0.1/magicalapi/types/resume_parser.py
--rw-r--r--   0        0        0      710 2024-04-07 08:52:03.003305 magicalapi-1.0.1/magicalapi/types/resume_review.py
--rw-r--r--   0        0        0      434 2024-03-26 12:02:10.746596 magicalapi-1.0.1/magicalapi/types/resume_score.py
--rw-r--r--   0        0        0      398 2024-04-03 14:43:20.342928 magicalapi-1.0.1/magicalapi/types/schemas.py
--rw-r--r--   0        0        0     2773 2024-04-03 14:43:20.342928 magicalapi-1.0.1/magicalapi/types/youtube_seo.py
--rw-r--r--   0        0        0      641 2024-03-26 12:02:10.746596 magicalapi-1.0.1/magicalapi/types/youtube_suggestions.py
--rw-r--r--   0        0        0      591 2024-03-26 12:02:10.746596 magicalapi-1.0.1/magicalapi/types/youtube_top_keywords.py
--rw-r--r--   0        0        0     1002 2024-03-26 12:02:10.746596 magicalapi-1.0.1/magicalapi/utils/logger.py
--rw-r--r--   0        0        0     1694 2024-04-07 11:29:38.163320 magicalapi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     9276 1970-01-01 00:00:00.000000 magicalapi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-07 06:23:11.026629 magicalapi-1.0.1.post1/LICENSE
+-rw-r--r--   0        0        0     8211 2024-04-08 09:37:28.653039 magicalapi-1.0.1.post1/README.md
+-rw-r--r--   0        0        0       59 2024-02-07 06:23:11.033296 magicalapi-1.0.1.post1/magicalapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 06:23:11.033296 magicalapi-1.0.1.post1/magicalapi/abstractions/__init__.py
+-rw-r--r--   0        0        0      413 2024-03-26 12:02:10.739930 magicalapi-1.0.1.post1/magicalapi/abstractions/base_service.py
+-rw-r--r--   0        0        0     3045 2024-03-27 12:47:18.029273 magicalapi-1.0.1.post1/magicalapi/client.py
+-rw-r--r--   0        0        0      270 2024-02-07 06:23:11.036629 magicalapi-1.0.1.post1/magicalapi/errors.py
+-rw-r--r--   0        0        0      693 2024-03-26 12:02:10.743263 magicalapi-1.0.1.post1/magicalapi/services/__init__.py
+-rw-r--r--   0        0        0     5238 2024-04-07 17:50:06.966654 magicalapi-1.0.1.post1/magicalapi/services/base_service.py
+-rw-r--r--   0        0        0     1275 2024-04-03 12:54:00.959978 magicalapi-1.0.1.post1/magicalapi/services/company_data_service.py
+-rw-r--r--   0        0        0     1433 2024-04-07 08:52:02.996638 magicalapi-1.0.1.post1/magicalapi/services/profile_data_service.py
+-rw-r--r--   0        0        0     1366 2024-04-07 08:52:02.999971 magicalapi-1.0.1.post1/magicalapi/services/resume_parser_service.py
+-rw-r--r--   0        0        0     1224 2024-03-27 12:42:51.355949 magicalapi-1.0.1.post1/magicalapi/services/resume_review_service.py
+-rw-r--r--   0        0        0     1458 2024-03-27 12:42:51.365949 magicalapi-1.0.1.post1/magicalapi/services/resume_score_service.py
+-rw-r--r--   0        0        0     1119 2024-03-27 12:42:51.365949 magicalapi-1.0.1.post1/magicalapi/services/youtube_seo_service.py
+-rw-r--r--   0        0        0     1766 2024-03-27 12:42:51.269282 magicalapi-1.0.1.post1/magicalapi/services/youtube_suggestions_service.py
+-rw-r--r--   0        0        0     3693 2024-03-27 12:42:51.272616 magicalapi-1.0.1.post1/magicalapi/services/youtube_top_keywords_service.py
+-rw-r--r--   0        0        0      982 2024-03-27 12:32:32.425971 magicalapi-1.0.1.post1/magicalapi/settings.py
+-rw-r--r--   0        0        0      292 2024-04-03 13:44:11.699802 magicalapi-1.0.1.post1/magicalapi/types/__init__.py
+-rw-r--r--   0        0        0      881 2024-04-07 17:50:06.966654 magicalapi-1.0.1.post1/magicalapi/types/base.py
+-rw-r--r--   0        0        0     1288 2024-03-26 12:02:10.743263 magicalapi-1.0.1.post1/magicalapi/types/company_data.py
+-rw-r--r--   0        0        0     3757 2024-04-07 08:52:02.999971 magicalapi-1.0.1.post1/magicalapi/types/profile_data.py
+-rw-r--r--   0        0        0     2028 2024-04-07 08:52:03.003305 magicalapi-1.0.1.post1/magicalapi/types/resume_parser.py
+-rw-r--r--   0        0        0      710 2024-04-07 08:52:03.003305 magicalapi-1.0.1.post1/magicalapi/types/resume_review.py
+-rw-r--r--   0        0        0      434 2024-03-26 12:02:10.746596 magicalapi-1.0.1.post1/magicalapi/types/resume_score.py
+-rw-r--r--   0        0        0      398 2024-04-03 14:43:20.342928 magicalapi-1.0.1.post1/magicalapi/types/schemas.py
+-rw-r--r--   0        0        0     2773 2024-04-03 14:43:20.342928 magicalapi-1.0.1.post1/magicalapi/types/youtube_seo.py
+-rw-r--r--   0        0        0      641 2024-03-26 12:02:10.746596 magicalapi-1.0.1.post1/magicalapi/types/youtube_suggestions.py
+-rw-r--r--   0        0        0      591 2024-03-26 12:02:10.746596 magicalapi-1.0.1.post1/magicalapi/types/youtube_top_keywords.py
+-rw-r--r--   0        0        0     1002 2024-03-26 12:02:10.746596 magicalapi-1.0.1.post1/magicalapi/utils/logger.py
+-rw-r--r--   0        0        0     1696 2024-04-08 09:42:07.306365 magicalapi-1.0.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     9648 1970-01-01 00:00:00.000000 magicalapi-1.0.1.post1/PKG-INFO
```

### Comparing `magicalapi-1.0.1/LICENSE` & `magicalapi-1.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/README.md` & `magicalapi-1.0.1.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 <a name="readme-top"></a>
 
 <!-- PROJECT SHIELDS -->
 
-![Tests][tests-shield]
-![PyPI - Version][pypi-version-shields]
-![PyPI - Python Version][pypi-python-versions-shields]
+[![PyPI - Version][pypi-version-shields]][pypi-url]
+[![PyPI - Python Version][pypi-python-versions-shields]][pypi-url]
+[![Downloads](https://static.pepy.tech/badge/magicalapi)][pypi-url]
+<!-- (https://pepy.tech/project/magicalapi) -->
 
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
+<!--[![Contributors][contributors-shield]][contributors-url]-->
+<!-- [![Forks][forks-shield]][forks-url]-->
+
+[![Tests][tests-shield]][github-repo-url]
 [![Issues][issues-shield]][issues-url]
+[![Stargazers][stars-shield]][stars-url]
 [![MIT License][license-shield]][license-url]
 
+
+
+
 <!-- PROJECT LOGO -->
 
 <br />
 <div align="center">
   <a href="https://github.com/magicalapi/magicalapi-python">
-    <img src="images/logo.png" alt="Logo" width="80" height="80">
+    <img src="https://raw.githubusercontent.com/magicalapi/magicalapi-python/master/docs/logo.png?raw=true" alt="Logo" width="80" height="80">
   </a>
 
 <h3 align="center">MagicalAPI Python Client</h3>
 
   <p align="center">
     An Async and Type Annotated Python Client to Easy Access <a href="https://magicalapi.com">MagicalAPI.com</a> Service.
     <br />
@@ -208,32 +214,35 @@
 ## License
 
 Distributed under the MIT License. See [`LICENSE`](./LICENSE) for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- MARKDOWN LINKS & IMAGES -->
-
-
+<!-- SHIELDS -->
 [contributors-shield]: https://img.shields.io/github/contributors/magicalapi/magicalapi-python.svg?style=for-the-badge
-[contributors-url]: https://github.com/magicalapi/magicalapi-python/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/magicalapi/magicalapi-python.svg?style=for-the-badge
+[stars-shield]: https://img.shields.io/github/stars/magicalapi/magicalapi-python?style=flat&color=green
+[issues-shield]: https://img.shields.io/github/issues/magicalapi/magicalapi-python.svg
+[license-shield]: https://img.shields.io/github/license/magicalapi/magicalapi-python.svg
+<!-- other links -->
+[contributors-url]: https://github.com/magicalapi/magicalapi-python/graphs/contributors
 [forks-url]: https://github.com/magicalapi/magicalapi-python/network/members
-[stars-shield]: https://img.shields.io/github/stars/magicalapi/magicalapi-python.svg?style=for-the-badge
 [stars-url]: https://github.com/magicalapi/magicalapi-python/stargazers
-[issues-shield]: https://img.shields.io/github/issues/magicalapi/magicalapi-python.svg?style=for-the-badge
 [issues-url]: https://github.com/magicalapi/magicalapi-python/issues
-[license-shield]: https://img.shields.io/github/license/magicalapi/magicalapi-python.svg?style=for-the-badge
 [license-url]: https://github.com/magicalapi/magicalapi-python/blob/master/LICENSE
-
+[pypi-url]: https://pypi.org/project/magicalapi
+[github-repo-url]: https://github.com/magicalapi/magicalapi-python
 <!-- [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555 -->
 
 <!-- [linkedin-url]: https://linkedin.com/company/MagicalAPI -->
 
 <!-- [product-screenshot]: images/screenshot.png -->
 
 [Pydantic.badge]: https://img.shields.io/badge/pydantic-black?style=for-the-badge&logo=pydantic&logoColor=red
 [Httpx.badge]: https://img.shields.io/badge/Httpx-gray?style=for-the-badge
 [tests-shield]: https://github.com/magicalapi/magicalapi-python/actions/workflows/tests.yml/badge.svg
 [pypi-version-shields]: https://img.shields.io/pypi/v/magicalapi
 [pypi-python-versions-shields]: https://img.shields.io/pypi/pyversions/magicalapi
 [website-url]: https://magicalapi.com
+
+
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-![Tests][tests-shield] ![PyPI - Version][pypi-version-shields] ![PyPI - Python
-Version][pypi-python-versions-shields] [![Contributors][contributors-shield]]
-[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url]
+[![PyPI - Version][pypi-version-shields]][pypi-url] [![PyPI - Python Version]
+[pypi-python-versions-shields]][pypi-url] [![Downloads](https://
+static.pepy.tech/badge/magicalapi)][pypi-url] [![Tests][tests-shield]][github-
+repo-url] [![Issues][issues-shield]][issues-url] [![Stargazers][stars-shield]]
+[stars-url] [![MIT License][license-shield]][license-url]
                                     _[_L_o_g_o_]
                       ******** MMaaggiiccaallAAPPII PPyytthhoonn CClliieenntt ********
     An Async and Type Annotated Python Client to Easy Access _M_a_g_i_c_a_l_A_P_I_._c_o_m
                                    Service.
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _W_h_a_t_ _i_s_ _M_a_g_i_c_a_l_A_P_I
@@ -65,25 +65,27 @@
 **greatly appreciated**. Here is the [Contributing Guidelines](./
 CONTRIBUTING.rst). Don't forget to give the project a star! Thanks again!
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See [`LICENSE`](./LICENSE) for
 more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/magicalapi/
-magicalapi-python.svg?style=for-the-badge [contributors-url]: https://
-github.com/magicalapi/magicalapi-python/graphs/contributors [forks-shield]:
-https://img.shields.io/github/forks/magicalapi/magicalapi-python.svg?style=for-
-the-badge [forks-url]: https://github.com/magicalapi/magicalapi-python/network/
-members [stars-shield]: https://img.shields.io/github/stars/magicalapi/
-magicalapi-python.svg?style=for-the-badge [stars-url]: https://github.com/
-magicalapi/magicalapi-python/stargazers [issues-shield]: https://
-img.shields.io/github/issues/magicalapi/magicalapi-python.svg?style=for-the-
-badge [issues-url]: https://github.com/magicalapi/magicalapi-python/issues
-[license-shield]: https://img.shields.io/github/license/magicalapi/magicalapi-
-python.svg?style=for-the-badge [license-url]: https://github.com/magicalapi/
-magicalapi-python/blob/master/LICENSE [Pydantic.badge]: https://img.shields.io/
-badge/pydantic-black?style=for-the-badge&logo=pydantic&logoColor=red
-[Httpx.badge]: https://img.shields.io/badge/Httpx-gray?style=for-the-badge
-[tests-shield]: https://github.com/magicalapi/magicalapi-python/actions/
-workflows/tests.yml/badge.svg [pypi-version-shields]: https://img.shields.io/
-pypi/v/magicalapi [pypi-python-versions-shields]: https://img.shields.io/pypi/
-pyversions/magicalapi [website-url]: https://magicalapi.com
+magicalapi-python.svg?style=for-the-badge [forks-shield]: https://
+img.shields.io/github/forks/magicalapi/magicalapi-python.svg?style=for-the-
+badge [stars-shield]: https://img.shields.io/github/stars/magicalapi/
+magicalapi-python?style=flat&color=green [issues-shield]: https://
+img.shields.io/github/issues/magicalapi/magicalapi-python.svg [license-shield]:
+https://img.shields.io/github/license/magicalapi/magicalapi-python.svg
+[contributors-url]: https://github.com/magicalapi/magicalapi-python/graphs/
+contributors [forks-url]: https://github.com/magicalapi/magicalapi-python/
+network/members [stars-url]: https://github.com/magicalapi/magicalapi-python/
+stargazers [issues-url]: https://github.com/magicalapi/magicalapi-python/issues
+[license-url]: https://github.com/magicalapi/magicalapi-python/blob/master/
+LICENSE [pypi-url]: https://pypi.org/project/magicalapi [github-repo-url]:
+https://github.com/magicalapi/magicalapi-python [Pydantic.badge]: https://
+img.shields.io/badge/pydantic-black?style=for-the-
+badge&logo=pydantic&logoColor=red [Httpx.badge]: https://img.shields.io/badge/
+Httpx-gray?style=for-the-badge [tests-shield]: https://github.com/magicalapi/
+magicalapi-python/actions/workflows/tests.yml/badge.svg [pypi-version-shields]:
+https://img.shields.io/pypi/v/magicalapi [pypi-python-versions-shields]: https:
+//img.shields.io/pypi/pyversions/magicalapi [website-url]: https://
+magicalapi.com
```

### Comparing `magicalapi-1.0.1/magicalapi/client.py` & `magicalapi-1.0.1.post1/magicalapi/client.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/__init__.py` & `magicalapi-1.0.1.post1/magicalapi/services/__init__.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/base_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/base_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/company_data_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/company_data_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/profile_data_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/profile_data_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/resume_parser_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/resume_parser_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/resume_review_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/resume_review_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/resume_score_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/resume_score_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/youtube_seo_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/youtube_seo_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/youtube_suggestions_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/youtube_suggestions_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/services/youtube_top_keywords_service.py` & `magicalapi-1.0.1.post1/magicalapi/services/youtube_top_keywords_service.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/settings.py` & `magicalapi-1.0.1.post1/magicalapi/settings.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/types/base.py` & `magicalapi-1.0.1.post1/magicalapi/types/base.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/types/company_data.py` & `magicalapi-1.0.1.post1/magicalapi/types/company_data.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/types/profile_data.py` & `magicalapi-1.0.1.post1/magicalapi/types/profile_data.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/types/resume_parser.py` & `magicalapi-1.0.1.post1/magicalapi/types/resume_parser.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/types/resume_review.py` & `magicalapi-1.0.1.post1/magicalapi/types/resume_review.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/types/youtube_seo.py` & `magicalapi-1.0.1.post1/magicalapi/types/youtube_seo.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/types/youtube_suggestions.py` & `magicalapi-1.0.1.post1/magicalapi/types/youtube_suggestions.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/types/youtube_top_keywords.py` & `magicalapi-1.0.1.post1/magicalapi/types/youtube_top_keywords.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/magicalapi/utils/logger.py` & `magicalapi-1.0.1.post1/magicalapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `magicalapi-1.0.1/pyproject.toml` & `magicalapi-1.0.1.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magicalapi"
-version = "1.0.1"
+version = "1.0.1-1"
 description = "This is a Python client that provides easy access to the MagicalAPI.com services, fully type annotated, and asynchronous."
 authors = ["MagicalAPI <info@magicalapi.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/magicalapi/magicalapi-python"
 homepage = "https://github.com/magicalapi/magicalapi-python"
 classifiers = [
```

### Comparing `magicalapi-1.0.1/PKG-INFO` & `magicalapi-1.0.1.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicalapi
-Version: 1.0.1
+Version: 1.0.1.post1
 Summary: This is a Python client that provides easy access to the MagicalAPI.com services, fully type annotated, and asynchronous.
 Home-page: https://github.com/magicalapi/magicalapi-python
 License: MIT
 Author: MagicalAPI
 Author-email: info@magicalapi.com
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
@@ -32,30 +32,36 @@
 Project-URL: Repository, https://github.com/magicalapi/magicalapi-python
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
 <!-- PROJECT SHIELDS -->
 
-![Tests][tests-shield]
-![PyPI - Version][pypi-version-shields]
-![PyPI - Python Version][pypi-python-versions-shields]
+[![PyPI - Version][pypi-version-shields]][pypi-url]
+[![PyPI - Python Version][pypi-python-versions-shields]][pypi-url]
+[![Downloads](https://static.pepy.tech/badge/magicalapi)][pypi-url]
+<!-- (https://pepy.tech/project/magicalapi) -->
 
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
+<!--[![Contributors][contributors-shield]][contributors-url]-->
+<!-- [![Forks][forks-shield]][forks-url]-->
+
+[![Tests][tests-shield]][github-repo-url]
 [![Issues][issues-shield]][issues-url]
+[![Stargazers][stars-shield]][stars-url]
 [![MIT License][license-shield]][license-url]
 
+
+
+
 <!-- PROJECT LOGO -->
 
 <br />
 <div align="center">
   <a href="https://github.com/magicalapi/magicalapi-python">
-    <img src="images/logo.png" alt="Logo" width="80" height="80">
+    <img src="https://raw.githubusercontent.com/magicalapi/magicalapi-python/master/docs/logo.png?raw=true" alt="Logo" width="80" height="80">
   </a>
 
 <h3 align="center">MagicalAPI Python Client</h3>
 
   <p align="center">
     An Async and Type Annotated Python Client to Easy Access <a href="https://magicalapi.com">MagicalAPI.com</a> Service.
     <br />
@@ -242,33 +248,36 @@
 ## License
 
 Distributed under the MIT License. See [`LICENSE`](./LICENSE) for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- MARKDOWN LINKS & IMAGES -->
-
-
+<!-- SHIELDS -->
 [contributors-shield]: https://img.shields.io/github/contributors/magicalapi/magicalapi-python.svg?style=for-the-badge
-[contributors-url]: https://github.com/magicalapi/magicalapi-python/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/magicalapi/magicalapi-python.svg?style=for-the-badge
+[stars-shield]: https://img.shields.io/github/stars/magicalapi/magicalapi-python?style=flat&color=green
+[issues-shield]: https://img.shields.io/github/issues/magicalapi/magicalapi-python.svg
+[license-shield]: https://img.shields.io/github/license/magicalapi/magicalapi-python.svg
+<!-- other links -->
+[contributors-url]: https://github.com/magicalapi/magicalapi-python/graphs/contributors
 [forks-url]: https://github.com/magicalapi/magicalapi-python/network/members
-[stars-shield]: https://img.shields.io/github/stars/magicalapi/magicalapi-python.svg?style=for-the-badge
 [stars-url]: https://github.com/magicalapi/magicalapi-python/stargazers
-[issues-shield]: https://img.shields.io/github/issues/magicalapi/magicalapi-python.svg?style=for-the-badge
 [issues-url]: https://github.com/magicalapi/magicalapi-python/issues
-[license-shield]: https://img.shields.io/github/license/magicalapi/magicalapi-python.svg?style=for-the-badge
 [license-url]: https://github.com/magicalapi/magicalapi-python/blob/master/LICENSE
-
+[pypi-url]: https://pypi.org/project/magicalapi
+[github-repo-url]: https://github.com/magicalapi/magicalapi-python
 <!-- [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555 -->
 
 <!-- [linkedin-url]: https://linkedin.com/company/MagicalAPI -->
 
 <!-- [product-screenshot]: images/screenshot.png -->
 
 [Pydantic.badge]: https://img.shields.io/badge/pydantic-black?style=for-the-badge&logo=pydantic&logoColor=red
 [Httpx.badge]: https://img.shields.io/badge/Httpx-gray?style=for-the-badge
 [tests-shield]: https://github.com/magicalapi/magicalapi-python/actions/workflows/tests.yml/badge.svg
 [pypi-version-shields]: https://img.shields.io/pypi/v/magicalapi
 [pypi-python-versions-shields]: https://img.shields.io/pypi/pyversions/magicalapi
 [website-url]: https://magicalapi.com
 
+
+
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: magicalapi Version: 1.0.1 Summary: This is a Python
-client that provides easy access to the MagicalAPI.com services, fully type
-annotated, and asynchronous. Home-page: https://github.com/magicalapi/
+Metadata-Version: 2.1 Name: magicalapi Version: 1.0.1.post1 Summary: This is a
+Python client that provides easy access to the MagicalAPI.com services, fully
+type annotated, and asynchronous. Home-page: https://github.com/magicalapi/
 magicalapi-python License: MIT Author: MagicalAPI Author-email:
 info@magicalapi.com Requires-Python: >=3.10 Classifier: Development Status :: 4
 - Beta Classifier: Framework :: AsyncIO Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 2 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -12,20 +12,20 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Internet Classifier: Topic :: Software Development Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Typing :: Typed Requires-Dist: httpx
 (>=0.26.0,<0.27.0) Requires-Dist: pydantic (>=2.5.3,<3.0.0) Requires-Dist:
 pydantic-settings (>=2.1.0,<3.0.0) Project-URL: Repository, https://github.com/
-magicalapi/magicalapi-python Description-Content-Type: text/markdown ![Tests]
-[tests-shield] ![PyPI - Version][pypi-version-shields] ![PyPI - Python Version]
-[pypi-python-versions-shields] [![Contributors][contributors-shield]]
-[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url]
+magicalapi/magicalapi-python Description-Content-Type: text/markdown [![PyPI -
+Version][pypi-version-shields]][pypi-url] [![PyPI - Python Version][pypi-
+python-versions-shields]][pypi-url] [![Downloads](https://static.pepy.tech/
+badge/magicalapi)][pypi-url] [![Tests][tests-shield]][github-repo-url] [!
+[Issues][issues-shield]][issues-url] [![Stargazers][stars-shield]][stars-url]
+[![MIT License][license-shield]][license-url]
                                     _[_L_o_g_o_]
                       ******** MMaaggiiccaallAAPPII PPyytthhoonn CClliieenntt ********
     An Async and Type Annotated Python Client to Easy Access _M_a_g_i_c_a_l_A_P_I_._c_o_m
                                    Service.
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _W_h_a_t_ _i_s_ _M_a_g_i_c_a_l_A_P_I
@@ -84,25 +84,27 @@
 **greatly appreciated**. Here is the [Contributing Guidelines](./
 CONTRIBUTING.rst). Don't forget to give the project a star! Thanks again!
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See [`LICENSE`](./LICENSE) for
 more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/magicalapi/
-magicalapi-python.svg?style=for-the-badge [contributors-url]: https://
-github.com/magicalapi/magicalapi-python/graphs/contributors [forks-shield]:
-https://img.shields.io/github/forks/magicalapi/magicalapi-python.svg?style=for-
-the-badge [forks-url]: https://github.com/magicalapi/magicalapi-python/network/
-members [stars-shield]: https://img.shields.io/github/stars/magicalapi/
-magicalapi-python.svg?style=for-the-badge [stars-url]: https://github.com/
-magicalapi/magicalapi-python/stargazers [issues-shield]: https://
-img.shields.io/github/issues/magicalapi/magicalapi-python.svg?style=for-the-
-badge [issues-url]: https://github.com/magicalapi/magicalapi-python/issues
-[license-shield]: https://img.shields.io/github/license/magicalapi/magicalapi-
-python.svg?style=for-the-badge [license-url]: https://github.com/magicalapi/
-magicalapi-python/blob/master/LICENSE [Pydantic.badge]: https://img.shields.io/
-badge/pydantic-black?style=for-the-badge&logo=pydantic&logoColor=red
-[Httpx.badge]: https://img.shields.io/badge/Httpx-gray?style=for-the-badge
-[tests-shield]: https://github.com/magicalapi/magicalapi-python/actions/
-workflows/tests.yml/badge.svg [pypi-version-shields]: https://img.shields.io/
-pypi/v/magicalapi [pypi-python-versions-shields]: https://img.shields.io/pypi/
-pyversions/magicalapi [website-url]: https://magicalapi.com
+magicalapi-python.svg?style=for-the-badge [forks-shield]: https://
+img.shields.io/github/forks/magicalapi/magicalapi-python.svg?style=for-the-
+badge [stars-shield]: https://img.shields.io/github/stars/magicalapi/
+magicalapi-python?style=flat&color=green [issues-shield]: https://
+img.shields.io/github/issues/magicalapi/magicalapi-python.svg [license-shield]:
+https://img.shields.io/github/license/magicalapi/magicalapi-python.svg
+[contributors-url]: https://github.com/magicalapi/magicalapi-python/graphs/
+contributors [forks-url]: https://github.com/magicalapi/magicalapi-python/
+network/members [stars-url]: https://github.com/magicalapi/magicalapi-python/
+stargazers [issues-url]: https://github.com/magicalapi/magicalapi-python/issues
+[license-url]: https://github.com/magicalapi/magicalapi-python/blob/master/
+LICENSE [pypi-url]: https://pypi.org/project/magicalapi [github-repo-url]:
+https://github.com/magicalapi/magicalapi-python [Pydantic.badge]: https://
+img.shields.io/badge/pydantic-black?style=for-the-
+badge&logo=pydantic&logoColor=red [Httpx.badge]: https://img.shields.io/badge/
+Httpx-gray?style=for-the-badge [tests-shield]: https://github.com/magicalapi/
+magicalapi-python/actions/workflows/tests.yml/badge.svg [pypi-version-shields]:
+https://img.shields.io/pypi/v/magicalapi [pypi-python-versions-shields]: https:
+//img.shields.io/pypi/pyversions/magicalapi [website-url]: https://
+magicalapi.com
```

