# Comparing `tmp/avrotize-1.0.3.tar.gz` & `tmp/avrotize-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.0.3.tar` & `avrotize-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0    18924 2024-04-07 09:39:19.835150 avrotize-1.0.3/README.md
--rw-r--r--   0        0        0      924 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-07 09:39:23.979235 avrotize-1.0.3/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/asn1toavro.py
--rw-r--r--   0        0        0     9463 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotize.py
--rw-r--r--   0        0        0    18100 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22185 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotoproto.py
--rw-r--r--   0        0        0     9514 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12136 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    91241 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15532 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-07 09:39:19.839150 avrotize-1.0.3/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    15752 2024-04-07 09:39:19.839150 avrotize-1.0.3/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-04-07 09:39:19.839150 avrotize-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    19591 1970-01-01 00:00:00.000000 avrotize-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    22578 2024-04-08 14:03:36.861370 avrotize-1.1.1/README.md
+-rw-r--r--   0        0        0      924 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-08 14:03:42.313428 avrotize-1.1.1/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    12403 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotize.py
+-rw-r--r--   0        0        0    11455 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    13646 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    18100 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22185 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0     9514 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12889 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    91241 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15532 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    15752 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1019 2024-04-08 14:03:36.861370 avrotize-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    23245 1970-01-01 00:00:00.000000 avrotize-1.1.1/PKG-INFO
```

### Comparing `avrotize-1.0.3/README.md` & `avrotize-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 different schema formats, using [Apache Avro](https://avro.apache.org/) Schema
 as the integration schema model.
 
 You can use the tool to convert between Avro Schema and other schema formats
 like JSON Schema, XML Schema (XSD), Protocol Buffers (Protobuf), ASN.1, and
 database schema formats like Kusto Data Table Definition (KQL) and T-SQL Table
 Definition (SQL). That means you can also convert from JSON Schema to Protobuf
-going via Avro Schema.
+going via Avro Schema. 
+
+You can also generate C# and Java code from the Avro Schema documents with
+Avrotize. The difference to the native Avto tools is that Avrotize can emit
+data classes without Avro library dependencies and, optionally, with annotations
+for JSON serialization libraries like Jackson or System.Text.Json.
 
 The tool does not convert data (instances of schemas), only the data structure
 definitions.
 
 Mind that the primary objective of the tool is the conversion of schemas that
 describe data structures used in applications, databases, and message systems.
 While the project's internal tests do cover a lot of ground, it is nevertheless
@@ -122,14 +127,19 @@
 - [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avro schema to Protobuf 3 schema.
 - [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avro schema to JSON schema.
 - [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avro schema to XML schema.
 - [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avro schema to Kusto table definition.
 - [`avrotize a2tsql`](#convert-avro-schema-to-t-sql-table-definition) - Convert Avro schema to T-SQL table definition.
 - [`avrotize a2pq`](#convert-avro-schema-to-empty-parquet-file) - Convert Avro schema to empty Parquet file.
 
+Generate code from Avro Schema:
+
+- [`avrotize a2csharp`](#generate-c-code-from-avro-schema) - Generate C# code from Avro schema.
+- [`avrotize a2java`](#generate-java-code-from-avro-schema) - Generate Java code from Avro schema.
+
 ### Convert Proto schema to Avro schema
 
 ```bash
 avrotize p2a --proto <path_to_proto_file> --avsc <path_to_avro_schema_file>
 ```
 
 Parameters:
@@ -388,14 +398,68 @@
   single `record` type. If the Avro schema contains a top-level union, the
   `--record-type` option must be used to specify which record type to emit.
 - The fields of the record are mapped to columns in the Parquet file. Array and
   record fields are mapped to Parquet nested types. Avro type unions are mapped
   to structures, not to Parquet unions since those are not supported by the
   PyArrow library used here.
 
+### Generate C# code from Avro schema
+
+```bash
+avrotize a2csharp --avsc <path_to_avro_schema_file> --csharp <path_to_csharp_directory> [--avro-annotation] [--system-text-json-annotation] [--newtonsoft-json-annotation] [--pascal-properties]
+```
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--csharp`: The path to the C# directory to write the conversion result to.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the C# classes.
+- `--system-text-json-annotation`: (optional) If set, the tool will add System.Text.Json annotations to the C# classes.
+- `--newtonsoft-json-annotation`: (optional) If set, the tool will add Newtonsoft.Json annotations to the C# classes.
+- `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the C# classes.
+
+Conversion notes:
+- The tool generates C# classes that represent the Avro schema as data classes.
+- Using the `--system-text-json-annotation` or `--newtonsoft-json-annotation` option
+  will add annotations for the respective JSON serialization library to the generated
+  C# classes. Because the [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
+  preserves the JSON Schema structure in the Avro schema, the generated C# classes
+  can be used to serialize and deserialize data that is valid per the input JSON schema.
+- The classes are generated into a directory structure that reflects the Avro namespace
+  structure. The tool drops a minimal, default `.csproj` project file into the given
+  directory if none exists.
+
+
+### Generate Java code from Avro schema
+
+```bash
+avrotize a2java --avsc <path_to_avro_schema_file> --java <path_to_java_directory> [--package <java_package_name>] [--avro-annotation] [--jackson-annotation] [--pascal-properties]
+```
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--java`: The path to the Java directory to write the conversion result to.
+- `--package`: (optional) The Java package name to use in the generated Java classes.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the Java classes.
+- `--jackson-annotation`: (optional) If set, the tool will add Jackson annotations to the Java classes.
+- `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the Java classes.
+
+Conversion notes:
+
+- The tool generates Java classes that represent the Avro schema as data classes. 
+- Using the `--jackson-annotation` option will add annotations for the Jackson 
+  JSON serialization library to the generated Java classes. Because the 
+  [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
+  preserves the JSON Schema structure in the Avro schema, the generated Java classes
+  can be used to serialize and deserialize data that is valid per the input JSON schema.
+- The directory `/src/main/java` is created in the specified directory and the
+  generated Java classes are written to this directory. The tool drops a
+  minimal, default `pom.xml` Maven project file into the given directory if none
+  exists.
+
+
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
 
 Avrotize is released under the Apache License. See the LICENSE file for more details.
```

### Comparing `avrotize-1.0.3/avrotize/__init__.py` & `avrotize-1.1.1/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/asn1toavro.py` & `avrotize-1.1.1/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/avrotojsons.py` & `avrotize-1.1.1/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/avrotokusto.py` & `avrotize-1.1.1/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/avrotoparquet.py` & `avrotize-1.1.1/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/avrotoproto.py` & `avrotize-1.1.1/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/avrototsql.py` & `avrotize-1.1.1/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/avrotoxsd.py` & `avrotize-1.1.1/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/common.py` & `avrotize-1.1.1/avrotize/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -296,7 +296,29 @@
 
     # Filter out unique hashes to only return groups with more than one path
     for k in list(hash_groups.keys()):
         if len(hash_groups[k]) == 1:
             del hash_groups[k]
     return hash_groups
 
+def pascal(string):
+    """ Convert a string to PascalCase """
+    if '::' in string:
+        strings = string.split('::')
+        return strings[0] + '::' + '::'.join(pascal(s) for s in strings[1:])
+    if '.' in string:
+        strings = string.split('.')
+        return '.'.join(pascal(s) for s in strings)
+    if not string or len(string) == 0:
+        return string
+    words = []
+    if '_' in string:
+        # snake_case
+        words = re.split(r'_', string)
+    elif string[0].isupper():
+        # PascalCase
+        words = re.findall(r'[A-Z][a-z0-9_]*\.?', string)
+    else:
+        # camelCase
+        words = re.findall(r'[a-z0-9]+\.?|[A-Z][a-z0-9_]*\.?', string)
+    result = ''.join(word.capitalize() for word in words)
+    return result
```

### Comparing `avrotize-1.0.3/avrotize/dependency_resolver.py` & `avrotize-1.1.1/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/generic/generic.avsc` & `avrotize-1.1.1/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/jsonstoavro.py` & `avrotize-1.1.1/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/kconnect.json` & `avrotize-1.1.1/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/kstructtoavro.py` & `avrotize-1.1.1/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/proto2parser.py` & `avrotize-1.1.1/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/proto3parser.py` & `avrotize-1.1.1/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototoavro.py` & `avrotize-1.1.1/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototypes/any.avsc` & `avrotize-1.1.1/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototypes/api.avsc` & `avrotize-1.1.1/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototypes/duration.avsc` & `avrotize-1.1.1/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototypes/field_mask.avsc` & `avrotize-1.1.1/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototypes/struct.avsc` & `avrotize-1.1.1/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototypes/timestamp.avsc` & `avrotize-1.1.1/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototypes/type.avsc` & `avrotize-1.1.1/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/prototypes/wrappers.avsc` & `avrotize-1.1.1/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/avrotize/xsdtoavro.py` & `avrotize-1.1.1/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/pyproject.toml` & `avrotize-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.3/PKG-INFO` & `avrotize-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.0.3
+Version: 1.1.1
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,20 @@
 different schema formats, using [Apache Avro](https://avro.apache.org/) Schema
 as the integration schema model.
 
 You can use the tool to convert between Avro Schema and other schema formats
 like JSON Schema, XML Schema (XSD), Protocol Buffers (Protobuf), ASN.1, and
 database schema formats like Kusto Data Table Definition (KQL) and T-SQL Table
 Definition (SQL). That means you can also convert from JSON Schema to Protobuf
-going via Avro Schema.
+going via Avro Schema. 
+
+You can also generate C# and Java code from the Avro Schema documents with
+Avrotize. The difference to the native Avto tools is that Avrotize can emit
+data classes without Avro library dependencies and, optionally, with annotations
+for JSON serialization libraries like Jackson or System.Text.Json.
 
 The tool does not convert data (instances of schemas), only the data structure
 definitions.
 
 Mind that the primary objective of the tool is the conversion of schemas that
 describe data structures used in applications, databases, and message systems.
 While the project's internal tests do cover a lot of ground, it is nevertheless
@@ -141,14 +146,19 @@
 - [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avro schema to Protobuf 3 schema.
 - [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avro schema to JSON schema.
 - [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avro schema to XML schema.
 - [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avro schema to Kusto table definition.
 - [`avrotize a2tsql`](#convert-avro-schema-to-t-sql-table-definition) - Convert Avro schema to T-SQL table definition.
 - [`avrotize a2pq`](#convert-avro-schema-to-empty-parquet-file) - Convert Avro schema to empty Parquet file.
 
+Generate code from Avro Schema:
+
+- [`avrotize a2csharp`](#generate-c-code-from-avro-schema) - Generate C# code from Avro schema.
+- [`avrotize a2java`](#generate-java-code-from-avro-schema) - Generate Java code from Avro schema.
+
 ### Convert Proto schema to Avro schema
 
 ```bash
 avrotize p2a --proto <path_to_proto_file> --avsc <path_to_avro_schema_file>
 ```
 
 Parameters:
@@ -407,14 +417,68 @@
   single `record` type. If the Avro schema contains a top-level union, the
   `--record-type` option must be used to specify which record type to emit.
 - The fields of the record are mapped to columns in the Parquet file. Array and
   record fields are mapped to Parquet nested types. Avro type unions are mapped
   to structures, not to Parquet unions since those are not supported by the
   PyArrow library used here.
 
+### Generate C# code from Avro schema
+
+```bash
+avrotize a2csharp --avsc <path_to_avro_schema_file> --csharp <path_to_csharp_directory> [--avro-annotation] [--system-text-json-annotation] [--newtonsoft-json-annotation] [--pascal-properties]
+```
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--csharp`: The path to the C# directory to write the conversion result to.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the C# classes.
+- `--system-text-json-annotation`: (optional) If set, the tool will add System.Text.Json annotations to the C# classes.
+- `--newtonsoft-json-annotation`: (optional) If set, the tool will add Newtonsoft.Json annotations to the C# classes.
+- `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the C# classes.
+
+Conversion notes:
+- The tool generates C# classes that represent the Avro schema as data classes.
+- Using the `--system-text-json-annotation` or `--newtonsoft-json-annotation` option
+  will add annotations for the respective JSON serialization library to the generated
+  C# classes. Because the [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
+  preserves the JSON Schema structure in the Avro schema, the generated C# classes
+  can be used to serialize and deserialize data that is valid per the input JSON schema.
+- The classes are generated into a directory structure that reflects the Avro namespace
+  structure. The tool drops a minimal, default `.csproj` project file into the given
+  directory if none exists.
+
+
+### Generate Java code from Avro schema
+
+```bash
+avrotize a2java --avsc <path_to_avro_schema_file> --java <path_to_java_directory> [--package <java_package_name>] [--avro-annotation] [--jackson-annotation] [--pascal-properties]
+```
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--java`: The path to the Java directory to write the conversion result to.
+- `--package`: (optional) The Java package name to use in the generated Java classes.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the Java classes.
+- `--jackson-annotation`: (optional) If set, the tool will add Jackson annotations to the Java classes.
+- `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the Java classes.
+
+Conversion notes:
+
+- The tool generates Java classes that represent the Avro schema as data classes. 
+- Using the `--jackson-annotation` option will add annotations for the Jackson 
+  JSON serialization library to the generated Java classes. Because the 
+  [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
+  preserves the JSON Schema structure in the Avro schema, the generated Java classes
+  can be used to serialize and deserialize data that is valid per the input JSON schema.
+- The directory `/src/main/java` is created in the specified directory and the
+  generated Java classes are written to this directory. The tool drops a
+  minimal, default `pom.xml` Maven project file into the given directory if none
+  exists.
+
+
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
 
 Avrotize is released under the Apache License. See the LICENSE file for more details.
```

