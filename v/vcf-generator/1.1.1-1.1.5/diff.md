# Comparing `tmp/vcf_generator-1.1.1.tar.gz` & `tmp/vcf_generator-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf_generator-1.1.1.tar", max compression
+gzip compressed data, was "vcf_generator-1.1.5.tar", max compression
```

## Comparing `vcf_generator-1.1.1.tar` & `vcf_generator-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/LICENSE
--rw-r--r--   0        0        0     3054 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/README.md
--rw-r--r--   0        0        0      906 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      896 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/addres_test.py
--rw-r--r--   0        0        0     3196 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/contact_test.py
--rw-r--r--   0        0        0      175 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/email_test.py
--rw-r--r--   0        0        0     4872 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/gen_contacts_test.py
--rw-r--r--   0        0        0     3716 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/gen_vcards_test.py
--rw-r--r--   0        0        0      323 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/phone_number_test.py
--rw-r--r--   0        0        0       90 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/__main__.py
--rw-r--r--   0        0        0      619 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/address.py
--rw-r--r--   0        0        0     1694 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/contact.py
--rw-r--r--   0        0        0      258 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/email.py
--rw-r--r--   0        0        0     3515 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/gen_contacts.py
--rw-r--r--   0        0        0     2619 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/gen_vcards.py
--rw-r--r--   0        0        0      754 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/phone_number.py
--rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 vcf_generator-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/LICENSE
+-rw-r--r--   0        0        0     3054 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/README.md
+-rw-r--r--   0        0        0      906 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      896 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/tests/addres_test.py
+-rw-r--r--   0        0        0     3196 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/tests/contact_test.py
+-rw-r--r--   0        0        0      175 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/tests/email_test.py
+-rw-r--r--   0        0        0     4872 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/tests/gen_contacts_test.py
+-rw-r--r--   0        0        0     3716 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/tests/gen_vcards_test.py
+-rw-r--r--   0        0        0      323 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/tests/phone_number_test.py
+-rw-r--r--   0        0        0       90 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/vcf_generator/__init__.py
+-rw-r--r--   0        0        0     1496 2024-04-08 04:08:48.842960 vcf_generator-1.1.5/vcf_generator/__main__.py
+-rw-r--r--   0        0        0      619 2024-04-08 04:08:48.846960 vcf_generator-1.1.5/vcf_generator/address.py
+-rw-r--r--   0        0        0     1694 2024-04-08 04:08:48.846960 vcf_generator-1.1.5/vcf_generator/contact.py
+-rw-r--r--   0        0        0      258 2024-04-08 04:08:48.846960 vcf_generator-1.1.5/vcf_generator/email.py
+-rw-r--r--   0        0        0     3515 2024-04-08 04:08:48.846960 vcf_generator-1.1.5/vcf_generator/gen_contacts.py
+-rw-r--r--   0        0        0     2619 2024-04-08 04:08:48.846960 vcf_generator-1.1.5/vcf_generator/gen_vcards.py
+-rw-r--r--   0        0        0      754 2024-04-08 04:08:48.846960 vcf_generator-1.1.5/vcf_generator/phone_number.py
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 vcf_generator-1.1.5/PKG-INFO
```

### Comparing `vcf_generator-1.1.1/LICENSE` & `vcf_generator-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/README.md` & `vcf_generator-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/pyproject.toml` & `vcf_generator-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vcf-generator"
-version = "1.1.1"
+version = "1.1.5"
 description = "A simple VCF generator. Generate VCF files with random data."
 authors = ["Bryan Wodi <pypi.envy443@dralias.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/talk2bryan/vcf-generator"
 keywords = ["vcf", "generator", "vcard", "contacts", "faker", "python"]
 include = [
```

### Comparing `vcf_generator-1.1.1/tests/addres_test.py` & `vcf_generator-1.1.5/tests/addres_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/tests/contact_test.py` & `vcf_generator-1.1.5/tests/contact_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/tests/gen_contacts_test.py` & `vcf_generator-1.1.5/tests/gen_contacts_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/tests/gen_vcards_test.py` & `vcf_generator-1.1.5/tests/gen_vcards_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/vcf_generator/__main__.py` & `vcf_generator-1.1.5/vcf_generator/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,13 +37,12 @@
             output_file (str | None, optional): Output file path. Defaults to None.
         """
         gen_vcards(num_contacts=num_contacts, output_file=output_file)
 
 
 def main():
     """CLI module for vcf_generator package."""
-    # Fire up the CLI module.
     fire.Fire(Contacts)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vcf_generator-1.1.1/vcf_generator/address.py` & `vcf_generator-1.1.5/vcf_generator/address.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/vcf_generator/contact.py` & `vcf_generator-1.1.5/vcf_generator/contact.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/vcf_generator/gen_contacts.py` & `vcf_generator-1.1.5/vcf_generator/gen_contacts.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/vcf_generator/gen_vcards.py` & `vcf_generator-1.1.5/vcf_generator/gen_vcards.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/vcf_generator/phone_number.py` & `vcf_generator-1.1.5/vcf_generator/phone_number.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.1/PKG-INFO` & `vcf_generator-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf-generator
-Version: 1.1.1
+Version: 1.1.5
 Summary: A simple VCF generator. Generate VCF files with random data.
 Home-page: https://github.com/talk2bryan/vcf-generator
 License: MIT
 Keywords: vcf,generator,vcard,contacts,faker,python
 Author: Bryan Wodi
 Author-email: pypi.envy443@dralias.com
 Requires-Python: >=3.10,<4.0
```

