# Comparing `tmp/vcf_generator-1.1.0.tar.gz` & `tmp/vcf_generator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf_generator-1.1.0.tar", max compression
+gzip compressed data, was "vcf_generator-1.1.1.tar", max compression
```

## Comparing `vcf_generator-1.1.0.tar` & `vcf_generator-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2024-04-07 15:31:43.843531 vcf_generator-1.1.0/LICENSE
--rw-r--r--   0        0        0     3067 2024-04-07 15:31:43.843531 vcf_generator-1.1.0/README.md
--rw-r--r--   0        0        0      906 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      896 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/addres_test.py
--rw-r--r--   0        0        0     3196 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/contact_test.py
--rw-r--r--   0        0        0      175 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/email_test.py
--rw-r--r--   0        0        0     4872 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/gen_contacts_test.py
--rw-r--r--   0        0        0     3844 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/gen_vcards_test.py
--rw-r--r--   0        0        0      323 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/phone_number_test.py
--rw-r--r--   0        0        0       90 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/__main__.py
--rw-r--r--   0        0        0      619 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/address.py
--rw-r--r--   0        0        0     1694 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/contact.py
--rw-r--r--   0        0        0      258 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/email.py
--rw-r--r--   0        0        0     3515 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/gen_contacts.py
--rw-r--r--   0        0        0     2655 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/gen_vcards.py
--rw-r--r--   0        0        0      754 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/phone_number.py
--rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 vcf_generator-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3054 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/README.md
+-rw-r--r--   0        0        0      906 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      896 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/addres_test.py
+-rw-r--r--   0        0        0     3196 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/contact_test.py
+-rw-r--r--   0        0        0      175 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/email_test.py
+-rw-r--r--   0        0        0     4872 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/gen_contacts_test.py
+-rw-r--r--   0        0        0     3716 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/gen_vcards_test.py
+-rw-r--r--   0        0        0      323 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/tests/phone_number_test.py
+-rw-r--r--   0        0        0       90 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/__main__.py
+-rw-r--r--   0        0        0      619 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/address.py
+-rw-r--r--   0        0        0     1694 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/contact.py
+-rw-r--r--   0        0        0      258 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/email.py
+-rw-r--r--   0        0        0     3515 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/gen_contacts.py
+-rw-r--r--   0        0        0     2619 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/gen_vcards.py
+-rw-r--r--   0        0        0      754 2024-04-07 15:54:34.728924 vcf_generator-1.1.1/vcf_generator/phone_number.py
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 vcf_generator-1.1.1/PKG-INFO
```

### Comparing `vcf_generator-1.1.0/LICENSE` & `vcf_generator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/README.md` & `vcf_generator-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 The above command will generate 1 contact as a VCF string and print the content to the console:
 
 ```bash
 BEGIN:VCARD
 VERSION:4.0
 N:None;Laura;Valerie;;Miss
 FN:Laura Valerie
-ORG:Miss Co.
 TITLE:Miss
 TEL;TYPE#HOME,voice;VALUE#uri:tel:+859-422-5863580
 TEL;TYPE#MOBILE,voice;VALUE#uri:tel:+528-463-7642962
 TEL;TYPE#MOBILE,voice;VALUE#uri:tel:+51-666-1415776
 ADR;TYPE#WORK;PREF#1;LABEL#13962 Casey Spring Suite 931
 Xavierfurt, VT 65391
 Suriname:;;13962 Casey Spring Suite 931;Xavierfurt;VT;65391;Suriname
```

### Comparing `vcf_generator-1.1.0/pyproject.toml` & `vcf_generator-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vcf-generator"
-version = "1.1.0"
+version = "1.1.1"
 description = "A simple VCF generator. Generate VCF files with random data."
 authors = ["Bryan Wodi <pypi.envy443@dralias.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/talk2bryan/vcf-generator"
 keywords = ["vcf", "generator", "vcard", "contacts", "faker", "python"]
 include = [
```

### Comparing `vcf_generator-1.1.0/tests/addres_test.py` & `vcf_generator-1.1.1/tests/addres_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/tests/contact_test.py` & `vcf_generator-1.1.1/tests/contact_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/tests/gen_contacts_test.py` & `vcf_generator-1.1.1/tests/gen_contacts_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/tests/gen_vcards_test.py` & `vcf_generator-1.1.1/tests/gen_vcards_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 
 def test_serialize_contact(contact):
     vcard = serialize_contact(contact)
     assert "BEGIN:VCARD" in vcard
     assert "VERSION:4.0" in vcard
     assert "N:Doe;John;M;;Mr" in vcard
     assert "FN:John M Doe" in vcard
-    assert "ORG:Mr Co." in vcard
     assert "TITLE:Mr" in vcard
     assert "TEL;TYPE#WORK,voice;VALUE#uri:tel:+1-123-4567890" in vcard
     assert (
         "ADR;TYPE#HOME;PREF#1;LABEL#123 Main St\nAnytown, NY 12345\nUSA:;;123 Main St;Anytown;NY;12345;USA"
         in vcard
     )
     assert "BDAY:1980-01-01" in vcard
@@ -97,29 +96,27 @@
     contact.phone_numbers = []
     contact.addresses = []
     vcard = serialize_contact(contact)
     assert "BEGIN:VCARD" in vcard
     assert "VERSION:4.0" in vcard
     assert "N:Doe;John;M;;Mr" in vcard
     assert "FN:John M Doe" in vcard
-    assert "ORG:Mr Co." in vcard
     assert "TITLE:Mr" in vcard
     assert "BDAY:1980-01-01" in vcard
     assert "EMAIL:test@example.com" in vcard
 
 
 def test_serialize_contacts(contacts):
     vcards = serialize_contacts(contacts)
     assert len(vcards) == 2
     for vcard in vcards:
         assert "BEGIN:VCARD" in vcard
         assert "VERSION:4.0" in vcard
         assert "N:" in vcard
         assert "FN:" in vcard
-        assert "ORG:" in vcard
         assert "TITLE:" in vcard
         assert "TEL;TYPE#WORK,voice;VALUE#uri:tel:+1-123-4567890" in vcard
         assert (
             "ADR;TYPE#HOME;PREF#1;LABEL#123 Main St\nAnytown, NY 12345\nUSA:;;123 Main St;Anytown;NY;12345;USA"
             in vcard
         )
         assert "BDAY:" in vcard
@@ -137,10 +134,9 @@
     vcards_str = gen_vcards_str(num_contacts=len(contacts))
     assert len(vcards_str) == len(contacts)
     for vcard in vcards_str:
         assert "BEGIN:VCARD" in vcard
         assert "VERSION:4.0" in vcard
         assert "N:" in vcard
         assert "FN:" in vcard
-        assert "ORG:" in vcard
         assert "TITLE:" in vcard
         assert "BDAY:" in vcard
```

### Comparing `vcf_generator-1.1.0/vcf_generator/__main__.py` & `vcf_generator-1.1.1/vcf_generator/__main__.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/vcf_generator/address.py` & `vcf_generator-1.1.1/vcf_generator/address.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/vcf_generator/contact.py` & `vcf_generator-1.1.1/vcf_generator/contact.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/vcf_generator/gen_contacts.py` & `vcf_generator-1.1.1/vcf_generator/gen_contacts.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/vcf_generator/gen_vcards.py` & `vcf_generator-1.1.1/vcf_generator/gen_vcards.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 def serialize_contact(contact: Contact) -> str:
     """Serialize a contact to a vCard string."""
     vcard = [
         "BEGIN:VCARD",
         "VERSION:4.0",
         f"N:{contact.last_name};{contact.first_name};{contact.middle_name};;{contact.title}",
         f"FN:{contact.full_name}",
-        f"ORG:{contact.title} Co.",
         f"TITLE:{contact.title}",
     ]
     if contact.phone_numbers:
         for i, phone in enumerate(contact.phone_numbers, start=1):
             vcard.append(
                 f"TEL;TYPE#{phone.type},voice;VALUE#uri:tel:+{phone.country_code}-{phone.area_code}-{phone.subscriber_number}",
             )
```

### Comparing `vcf_generator-1.1.0/vcf_generator/phone_number.py` & `vcf_generator-1.1.1/vcf_generator/phone_number.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.1.0/PKG-INFO` & `vcf_generator-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf-generator
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple VCF generator. Generate VCF files with random data.
 Home-page: https://github.com/talk2bryan/vcf-generator
 License: MIT
 Keywords: vcf,generator,vcard,contacts,faker,python
 Author: Bryan Wodi
 Author-email: pypi.envy443@dralias.com
 Requires-Python: >=3.10,<4.0
@@ -75,15 +75,14 @@
 The above command will generate 1 contact as a VCF string and print the content to the console:
 
 ```bash
 BEGIN:VCARD
 VERSION:4.0
 N:None;Laura;Valerie;;Miss
 FN:Laura Valerie
-ORG:Miss Co.
 TITLE:Miss
 TEL;TYPE#HOME,voice;VALUE#uri:tel:+859-422-5863580
 TEL;TYPE#MOBILE,voice;VALUE#uri:tel:+528-463-7642962
 TEL;TYPE#MOBILE,voice;VALUE#uri:tel:+51-666-1415776
 ADR;TYPE#WORK;PREF#1;LABEL#13962 Casey Spring Suite 931
 Xavierfurt, VT 65391
 Suriname:;;13962 Casey Spring Suite 931;Xavierfurt;VT;65391;Suriname
```

