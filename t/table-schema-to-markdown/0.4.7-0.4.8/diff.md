# Comparing `tmp/table_schema_to_markdown-0.4.7-py3-none-any.whl.zip` & `tmp/table_schema_to_markdown-0.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8303 bytes, number of entries: 7
--rw-r--r--  2.0 unx    12982 b- defN 24-Mar-20 10:40 table_schema_to_markdown/__init__.py
--rwxr-xr-x  2.0 unx     1056 b- defN 24-Mar-20 10:41 table_schema_to_markdown-0.4.7.data/scripts/table-schema-to-md
--rw-r--r--  2.0 unx     1072 b- defN 24-Mar-20 10:41 table_schema_to_markdown-0.4.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     5402 b- defN 24-Mar-20 10:41 table_schema_to_markdown-0.4.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-20 10:41 table_schema_to_markdown-0.4.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 24-Mar-20 10:41 table_schema_to_markdown-0.4.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      684 b- defN 24-Mar-20 10:41 table_schema_to_markdown-0.4.7.dist-info/RECORD
-7 files, 21313 bytes uncompressed, 7065 bytes compressed:  66.9%
+Zip file size: 8523 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    13802 b- defN 24-Apr-08 09:36 table_schema_to_markdown/__init__.py
+-rwxr-xr-x  2.0 unx     1056 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.data/scripts/table-schema-to-md
+-rw-r--r--  2.0 unx     1072 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5402 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/WHEEL
+-rwxr--r--  2.0 unx       25 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      684 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/RECORD
+7 files, 22133 bytes uncompressed, 7285 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: table_schema_to_markdown/__init__.py
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.7.data/scripts/table-schema-to-md
+Filename: table_schema_to_markdown-0.4.8.data/scripts/table-schema-to-md
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.7.dist-info/LICENSE
+Filename: table_schema_to_markdown-0.4.8.dist-info/LICENSE
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.7.dist-info/METADATA
+Filename: table_schema_to_markdown-0.4.8.dist-info/METADATA
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.7.dist-info/WHEEL
+Filename: table_schema_to_markdown-0.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.7.dist-info/top_level.txt
+Filename: table_schema_to_markdown-0.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.7.dist-info/RECORD
+Filename: table_schema_to_markdown-0.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## table_schema_to_markdown/__init__.py

```diff
@@ -64,79 +64,79 @@
         ("trueValues", "Valeurs considérées comme vraies"),
         ("falseValues", "Valeurs considérées comme fausses"),
     ]
 )
 
 CONSTRAINTS_MAP = OrderedDict(
     [
-        ("minLength", lambda v: "Taille minimale : {}".format(v)),
-        ("maxLength", lambda v: "Taille maximale : {}".format(v)),
-        ("minimum", lambda v: "Valeur minimale : {}".format(v)),
-        ("maximum", lambda v: "Valeur maximale : {}".format(v)),
-        ("pattern", lambda v: "Motif : `{}`".format(v)),
-        ("enum", lambda v: "Valeurs autorisées : {}".format(", ".join(v))),
+        ("minLength", lambda v: f"Taille minimale : {v}"),
+        ("maxLength", lambda v: f"Taille maximale : {v}"),
+        ("minimum", lambda v: f"Valeur minimale : {v}"),
+        ("maximum", lambda v: f"Valeur maximale : {v}"),
+        ("pattern", lambda v: f"Motif : `{v}`"),
+        ("enum", lambda v: f"Valeurs autorisées : {', '.join(v)}"),
     ]
 )
 
 
 def format_format(format_val):
     """ Return markdown format information """
-    return "- `{}` {}\n".format(format_val, FORMAT_MAP.get(format_val, ""))
+    return f"- `{format_val}` {FORMAT_MAP.get(format_val, '')}\n"
 
 
 def format_type_specific_info(col_content):
     """ Formats and return info relative to type """
     buff = io.StringIO()
     for prop in TYPE_SPECIFIC_MAP:
         if prop in col_content:
-            buff.write("{} : {}".format(TYPE_SPECIFIC_MAP[prop], col_content[prop]))
+            buff.write(f"{TYPE_SPECIFIC_MAP[prop]} : {col_content[prop]}")
 
     if "bareNumber" in col_content and col_content["bareNumber"] == "false":
         buff.write(
-            "Le nombre peut contenir des caractères supplémentaires (« € », « % » ...)"
+            "Le nombre peut contenir des caractères "
+            "supplémentaires (« € », « % » ...)"
         )
     ret = buff.getvalue()
     buff.close()
     return ret
 
 
 def format_type(col_content):
     buff = io.StringIO()
     # Type
     type_ = col_content.get("type")
     format_ = col_content.get("format")
 
     if type_:
-        type_val = TYPE_MAP.get(type_, "??{}??".format(type_))
+        type_val = TYPE_MAP.get(type_, f"??{type_}??")
         buff.write(
             "{}{}|".format(
                 type_val,
                 ""
                 if format_ in ["default", None]
                 else " (format `{}`)".format(format_),
             )
         )
         # Type specific properties
         buff.write(format_type_specific_info(col_content))
 
     # RDFType
     rdf_type = col_content.get("rdfType")
     if rdf_type:
-        buff.write("{}|".format(rdf_type))
+        buff.write(f"{rdf_type}|")
 
     ret = buff.getvalue()
     buff.close()
     return ret
 
 
 def format_example(col_content):
     example = col_content.get(EXAMPLE)
     if example:
-        return "{}|".format(example)
-
+        return f"{example}|"
     return "|"
 
 
 def format_constraints(col_content):
     """ Converts type and constraints information into Markdown """
     buff = io.StringIO()
 
@@ -145,225 +145,288 @@
         required = None
         if constraints.get("required"):
             required = "Valeur obligatoire"
         elif not constraints.get("required", True):
             required = "Valeur optionnelle"
         constraint_str_list = list(
             filter(
-                None, [required, "Valeur unique" if constraints.get("unique") else None]
+                None,
+                [
+                    required,
+                    "Valeur unique" if constraints.get("unique") else None
+                ]
             )
         )
 
         # minLength, maxLength, minimum, maximum, pattern, enum
         for prop in [prop for prop in CONSTRAINTS_MAP if prop in constraints]:
-            constraint_str_list.append(CONSTRAINTS_MAP[prop](constraints[prop]))
+            constraint_str_list.append(
+                CONSTRAINTS_MAP[prop](constraints[prop])
+            )
 
         buff.write(", ".join(constraint_str_list))
 
     ret = buff.getvalue()
     buff.close()
     return ret
 
 
 def format_property(name, value):
     if name == CREATED:
         return datetime.strptime(value, "%Y-%m-%d").strftime("%d/%m/%Y")
     if name == MISSING_VALUES:
         if value == [""]:
             return ""
-        return ", ".join(map(lambda v: '`"{}"`'.format(v), value))
+        return ", ".join(map(lambda v: f'`"{v}"`', value))
     if name == PRIMARY_KEY:
         return ", ".join(value) if isinstance(value, list) else value
     return value
 
 
 def format_name(field_json):
     buff = io.StringIO()
 
     field_name = field_json.get("name")
     buff.write(
-        "|{}".format("{}".format(field_name) if field_name else "Erreur : nom manquant")
+        f"|{field_name if field_name else 'Erreur : nom manquant'}"
     )
 
     title = field_json.get("title")
     if title:
-        buff.write(" ({})".format(title))
+        buff.write(f" ({title})")
 
     buff.write("|")
 
     ret = buff.getvalue()
     buff.close()
     return ret
 
 
-def convert_source(source, out_fd,style='table'):
+def convert_source(source, out_fd, style='table'):
     log.info("Loading schema from %r", source)
     with open(source, encoding="utf-8") as f:
         schema = json.load(f)
-
-    convert_json(schema, out_fd,style)
+    convert_json(schema, out_fd, style)
 
 
-def write_property(schema_json, property_name, out_fd, prefix="", suffix="\n\n"):
+def write_property(
+    schema_json,
+    property_name,
+    out_fd,
+    prefix="",
+    suffix="\n\n"
+):
     if property_name in schema_json:
-        property_value = format_property(property_name, schema_json[property_name])
+        property_value = format_property(
+            property_name,
+            schema_json[property_name]
+        )
         if property_value != "":
             out_fd.write(prefix + property_value + suffix)
 
 
-def convert_json(schema_json, out_fd,style):
+def make_link_suitable(field_name):
+    # replacing dots and underscores with dashes to make the inner links work
+    return field_name.lower().replace('.', '-').replace('_', '-')
+
+
+def convert_json(schema_json, out_fd, style):
     """ Converts table schema data to markdown """
 
     # Header
     if NAME in schema_json:
         write_property(schema_json, NAME, out_fd, "## ")
         write_property(schema_json, TITLE, out_fd)
     else:
         write_property(schema_json, TITLE, out_fd, "## ")
     write_property(schema_json, DESCRIPTION, out_fd)
 
     for property_name in SCHEMA_PROP_MAP.keys():
         prefix = "- {} : ".format(SCHEMA_PROP_MAP[property_name])
         write_property(schema_json, property_name, out_fd, prefix, "\n")
 
-    write_property(schema_json, MISSING_VALUES, out_fd, "- Valeurs manquantes : ", "\n")
-    write_property(schema_json, PRIMARY_KEY, out_fd, "- Clé primaire : `", "`\n")
+    write_property(
+        schema_json,
+        MISSING_VALUES,
+        out_fd,
+        "- Valeurs manquantes : ",
+        "\n"
+    )
+    write_property(
+        schema_json,
+        PRIMARY_KEY,
+        out_fd,
+        "- Clé primaire : `",
+        "`\n"
+    )
 
-    # Foreign keys constraint is more complex than a list of strings, more work required.
+    # Foreign keys constraint is more complex
+    # than a list of strings, more work required.
 
     out_fd.write("\n")
 
     fields = schema_json.get("fields")
 
     if fields:
         out_fd.write("### Modèle de données\n\n")
-        if(style == 'table'):
+        if style == 'table':
             # GitHub Flavored Markdown table header
             headers = ["Nom", "Type", "Description", "Exemple", "Propriétés"]
             out_fd.write("|" + "|".join(headers) + "|\n")
             out_fd.write("|" + "|".join("-" * len(headers)) + "|\n")
             for field in fields:
                 convert_field(field, out_fd)
 
-        elif(style == 'page'):
+        elif style == 'page':
 
             out_fd.write("\n##### Liste des propriétés")
             out_fd.write("\n\n| Propriété | Type | Obligatoire |")
             out_fd.write("\n| -- | -- | -- |")
-            
+
             for field in fields:
                 field_name = field.get("name")
                 field_title = field.get("title")
-                if(field_title is not None):
-                    strUrl = "["+field_name+"](#"+field_title.lower().replace(" ","-")+"---propriété-"+field_name.lower()+")"
+                if field_title is not None:
+                    strUrl = (
+                        f"[{field_name}]"
+                        f"(#{field_title.lower().replace(' ', '-')}"
+                        f"---propriete-{make_link_suitable(field_name)})"
+                    )
                 else:
-                    strUrl = "["+field_name+"](#propriété-"+field_name.lower()+")"
+                    strUrl = (
+                        f"[{field_name}]"
+                        f"(#propriete-{make_link_suitable(field_name)})"
+                    )
 
                 field_type = field.get("type")
-                field_format = field.get("format")   
-                field_constraints = field.get("constraints")   
+                field_format = field.get("format")
+                field_constraints = field.get("constraints")
                 strFormat = ""
                 if field_format is not None:
-                    strFormat = "(format `"+field.get("format")+"`)"
+                    strFormat = f"(format `{field.get('format')}`)"
 
                 field_title = field.get("title")
                 listenums = []
                 intervals = ""
                 sizes = ""
                 pattern = ""
 
-                if field_constraints:
-                    required = None
-                    if field_constraints.get("required"):
-                        required = "Oui"
-                    elif not field_constraints.get("required", True):
-                        required = "Non"
+                if field_constraints and field_constraints.get("required"):
+                    required = "Oui"
                 else:
                     required = "Non"
-                
-                out_fd.write("\n| {} | {} {} | {} |".format(strUrl,TYPE_MAP[field_type],strFormat,required))
-                    
+
+                out_fd.write(
+                    f"\n| {strUrl} | {TYPE_MAP[field_type]} "
+                    f"{strFormat} | {required} |"
+                )
+
             out_fd.write("\n")
 
             for field in fields:
                 field_name = field.get("name")
                 field_description = field.get("description")
                 field_type = field.get("type")
-                field_example = field.get("example")               
-                field_constraints = field.get("constraints")   
+                field_example = field.get("example")
+                field_constraints = field.get("constraints")
                 field_format = field.get("format")
                 field_title = field.get("title")
                 listenums = []
                 intervals = ""
                 sizes = ""
                 pattern = ""
 
                 required = None
                 if field_constraints:
                     if field_constraints.get("required"):
                         required = "Valeur obligatoire"
-                    elif not field_constraints.get("required", True):
+                    else:
                         required = "Valeur optionnelle"
-                    
-                    if "minLength" in field_constraints:
-                        if(field_constraints["minLength"] != None):
-                            sizes = "Plus de "+str(field_constraints["minLength"])+" caractères"
-                        
-                    if "maxLength" in field_constraints:
-                        if(sizes != ""):
-                            sizes = "Entre "+sizes.replace("Plus de ","").replace(" caractères","")+" et "+str(field_constraints['maxLength'])+" caractères"
+
+                    if field_constraints.get("minLength"):
+                        sizes = (
+                            f"Plus de {field_constraints['minLength']} "
+                            "caractères"
+                        )
+
+                    if field_constraints.get("maxLength"):
+                        if sizes:
+                            sizes = (
+                                f"Entre {field_constraints['minLength']} "
+                                f"et {field_constraints['maxLength']} "
+                                "caractères"
+                            )
                         else:
-                            sizes = "Moins de "+str(field_constraints['maxLength'])+" caractères"        
-                    
-                    if "minimum" in field_constraints:
-                        if(field_constraints["minimum"] != None):
-                            intervals = "Valeur supérieur à "+str(field_constraints["minimum"])
-                        
-                    if "maximum" in field_constraints:
-                        if(intervals != ""):
-                            intervals = "Valeur entre "+intervals.replace("Valeur supérieur à ","")+" et "+str(field_constraints['maximum'])
+                            sizes = (
+                                f"Moins de {field_constraints['maxLength']} "
+                                "caractères"
+                            )
+
+                    if field_constraints.get("minimum"):
+                        intervals = (
+                            "Valeur supérieure à "
+                            f"{field_constraints['minimum']}"
+                        )
+
+                    if field_constraints.get("maximum"):
+                        if intervals:
+                            intervals = (
+                                f"Valeur entre {field_constraints['minimum']}"
+                                f" et {field_constraints['maximum']}"
+                            )
                         else:
-                            intervals = "Valeur inférieur à : "+str(field_constraints['maximum'])
-                            
-                    if "pattern" in field_constraints:
+                            intervals = (
+                                "Valeur inférieure à : "
+                                f"{field_constraints['maximum']}"
+                            )
+
+                    if field_constraints.get("pattern"):
                         pattern = str(field_constraints['pattern'])
 
-                    if "enum" in field_constraints:
+                    if field_constraints.get("enum"):
                         listenums = field_constraints["enum"]
 
-
                 out_fd.write("\n#### ")
-                if(field_title is not None):
-                    out_fd.write("{} - ".format(field_title))
-                out_fd.write("Propriété `{}`".format(field_name))
-                out_fd.write("\n\n> *Description : {}<br/>Ex : {}*".format(field_description, field_example))
-                if(required is not None):
-                    out_fd.write("\n- {}".format(required))
+                if field_title is not None:
+                    out_fd.write(f"{field_title} - ")
+                out_fd.write(f"Propriété `{field_name}`")
+                out_fd.write(f"\n\n> *Description : {field_description}*")
+                if field_example:
+                    out_fd.write(f"<br/>*Exemple : {field_example}*")
+                if required is not None:
+                    out_fd.write(f"\n- {required}")
                 else:
                     out_fd.write("\n- Valeur optionnelle")
-                out_fd.write("\n- Type : {}".format(TYPE_MAP[field_type]))
+                out_fd.write(f"\n- Type : {TYPE_MAP[field_type]}")
                 if field_format is not None:
-                    out_fd.write(" (format `{}`)".format(field_format))
-                if(len(listenums) > 0):
+                    out_fd.write(f" (format `{field_format}`)")
+                if len(listenums) > 0:
                     out_fd.write("\n- Valeurs autorisées : ")
                     for enum in listenums:
-                        out_fd.write("\n    - {}".format(enum))
-                if(intervals != ""):
-                    out_fd.write("\n- {}".format(intervals))
-                if(sizes != ""):
-                    out_fd.write("\n- {}".format(sizes))
-                if(pattern != ""):
-                    out_fd.write("\n- Motif : `{}`".format(pattern))
+                        # to prevent weird display due
+                        # to markdown quoting mechanism
+                        out_fd.write(
+                            "\n    - {}".format(
+                                enum if not enum.startswith(">")
+                                else "\\" + enum
+                            )
+                        )
+                if intervals != "":
+                    out_fd.write(f"\n- {intervals}")
+                if sizes != "":
+                    out_fd.write(f"\n- {sizes}")
+                if pattern != "":
+                    out_fd.write(f"\n- Motif : `{pattern}`")
                 out_fd.write("\n")
-              
+
 
 def format_description(field_json):
     description = field_json.get("description")
     if description:
-        return "{}|".format(description)
+        return f"{description}|"
     return ""
 
 
 def convert_field(field_json, out_fd):
     """ Convert JSON content describing a column to Markdown"""
 
     out_fd.write(format_name(field_json))
```

## Comparing `table_schema_to_markdown-0.4.7.data/scripts/table-schema-to-md` & `table_schema_to_markdown-0.4.8.data/scripts/table-schema-to-md`

 * *Files identical despite different names*

## Comparing `table_schema_to_markdown-0.4.7.dist-info/LICENSE` & `table_schema_to_markdown-0.4.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `table_schema_to_markdown-0.4.7.dist-info/METADATA` & `table_schema_to_markdown-0.4.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: table-schema-to-markdown
-Version: 0.4.7
+Version: 0.4.8
 Summary: Generate Markdown documentation from a table schema file from Frictionless Data
 Home-page: https://github.com/geoffreyaldebert/table-schema-to-markdown
 Author: Antoine Augusti, Geoffrey Aldebert
 Author-email: hi@antoine-augusti.fr, geoffrey.aldebert@data.gouv.fr
 License: MIT
 Keywords: frictionlessdata,documentation,tableschema,table-schema,frictionless data,open data,json schema,json table schema,data package,tabular data package
 Platform: UNKNOWN
```

## Comparing `table_schema_to_markdown-0.4.7.dist-info/RECORD` & `table_schema_to_markdown-0.4.8.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-table_schema_to_markdown/__init__.py,sha256=Cm6xjOYhkBIahmU4VOvCNy-UPilwxw53EVJXOxm5k9c,12982
-table_schema_to_markdown-0.4.7.data/scripts/table-schema-to-md,sha256=c2IgvuLFUBBrwY8LxvO9GrADX6ZIT5-_SVW8-0iErwU,1056
-table_schema_to_markdown-0.4.7.dist-info/LICENSE,sha256=qV08noOLMZNHkulCB6KzZKm-aPGZjbP-sYJqmz2dUeM,1072
-table_schema_to_markdown-0.4.7.dist-info/METADATA,sha256=fXUvuyQGi7mNMDeGkbT-7cGTWHVydvFxD6tGPoY1hH8,5402
-table_schema_to_markdown-0.4.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-table_schema_to_markdown-0.4.7.dist-info/top_level.txt,sha256=jsrAX2CW2-lFIx28kPUYPlwep72sLHxmjd13pvAHS-c,25
-table_schema_to_markdown-0.4.7.dist-info/RECORD,,
+table_schema_to_markdown/__init__.py,sha256=Qq0avn1hX81N6zInMdpqScm4Ncr2-uaSBGsz_EryjX4,13802
+table_schema_to_markdown-0.4.8.data/scripts/table-schema-to-md,sha256=c2IgvuLFUBBrwY8LxvO9GrADX6ZIT5-_SVW8-0iErwU,1056
+table_schema_to_markdown-0.4.8.dist-info/LICENSE,sha256=qV08noOLMZNHkulCB6KzZKm-aPGZjbP-sYJqmz2dUeM,1072
+table_schema_to_markdown-0.4.8.dist-info/METADATA,sha256=x2zeKQKdOrpep7yAra_k3cbq5rUUvlMmczmgqQlDBcU,5402
+table_schema_to_markdown-0.4.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+table_schema_to_markdown-0.4.8.dist-info/top_level.txt,sha256=jsrAX2CW2-lFIx28kPUYPlwep72sLHxmjd13pvAHS-c,25
+table_schema_to_markdown-0.4.8.dist-info/RECORD,,
```

