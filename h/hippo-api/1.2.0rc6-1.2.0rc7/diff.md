# Comparing `tmp/hippo_api-1.2.0rc6-py3-none-any.whl.zip` & `tmp/hippo_api-1.2.0rc7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 31340 bytes, number of entries: 20
+Zip file size: 31611 bytes, number of entries: 20
 -rw-r--r--  2.0 unx       78 b- defN 23-Aug-22 09:32 transwarp_embedding_hub/__init__.py
 -rw-r--r--  2.0 unx     2858 b- defN 23-Sep-01 03:36 transwarp_embedding_hub/azure.py
 -rw-r--r--  2.0 unx      846 b- defN 23-Sep-01 03:36 transwarp_embedding_hub/base_embedding.py
 -rw-r--r--  2.0 unx      355 b- defN 23-Aug-22 09:32 transwarp_embedding_hub/config.yaml
 -rw-r--r--  2.0 unx      703 b- defN 23-Sep-01 03:33 transwarp_embedding_hub/embedding_hub.py
 -rw-r--r--  2.0 unx     2389 b- defN 23-Sep-01 03:33 transwarp_embedding_hub/openai.py
 -rw-r--r--  2.0 unx     4608 b- defN 23-Sep-01 03:33 transwarp_embedding_hub/pulse.py
 -rw-r--r--  2.0 unx     4552 b- defN 23-Aug-22 09:32 transwarp_embedding_hub/text_segmentation.py
 -rw-r--r--  2.0 unx       78 b- defN 23-Aug-22 09:32 transwarp_hippo_api/__init__.py
--rw-r--r--  2.0 unx     2625 b- defN 24-Mar-14 09:49 transwarp_hippo_api/conn_mgr.py
--rw-r--r--  2.0 unx    99327 b- defN 24-Mar-26 07:44 transwarp_hippo_api/hippo_client.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Apr-08 06:04 transwarp_hippo_api/conn_mgr.py
+-rw-r--r--  2.0 unx   101690 b- defN 24-Apr-08 06:08 transwarp_hippo_api/hippo_client.py
 -rw-r--r--  2.0 unx     1555 b- defN 24-Mar-01 10:41 transwarp_hippo_api/hippo_type.py
 -rw-r--r--  2.0 unx      577 b- defN 23-Nov-22 08:20 transwarp_hippo_api/private_embedding.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-22 09:32 transwarp_hippo_langchain/__init__.py
 -rw-r--r--  2.0 unx     1223 b- defN 23-Sep-01 03:37 transwarp_hippo_langchain/embedding_hub_langchain.py
 -rw-r--r--  2.0 unx    23069 b- defN 23-Oct-13 02:58 transwarp_hippo_langchain/hippo_langchain.py
--rw-r--r--  2.0 unx      129 b- defN 24-Mar-26 07:44 hippo_api-1.2.0rc6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 07:44 hippo_api-1.2.0rc6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 24-Mar-26 07:44 hippo_api-1.2.0rc6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1815 b- defN 24-Mar-26 07:44 hippo_api-1.2.0rc6.dist-info/RECORD
-20 files, 146925 bytes uncompressed, 28312 bytes compressed:  80.7%
+-rw-r--r--  2.0 unx      129 b- defN 24-Apr-08 06:13 hippo_api-1.2.0rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 06:13 hippo_api-1.2.0rc7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-Apr-08 06:13 hippo_api-1.2.0rc7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1816 b- defN 24-Apr-08 06:13 hippo_api-1.2.0rc7.dist-info/RECORD
+20 files, 149288 bytes uncompressed, 28583 bytes compressed:  80.9%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: transwarp_hippo_langchain/embedding_hub_langchain.py
 Comment: 
 
 Filename: transwarp_hippo_langchain/hippo_langchain.py
 Comment: 
 
-Filename: hippo_api-1.2.0rc6.dist-info/METADATA
+Filename: hippo_api-1.2.0rc7.dist-info/METADATA
 Comment: 
 
-Filename: hippo_api-1.2.0rc6.dist-info/WHEEL
+Filename: hippo_api-1.2.0rc7.dist-info/WHEEL
 Comment: 
 
-Filename: hippo_api-1.2.0rc6.dist-info/top_level.txt
+Filename: hippo_api-1.2.0rc7.dist-info/top_level.txt
 Comment: 
 
-Filename: hippo_api-1.2.0rc6.dist-info/RECORD
+Filename: hippo_api-1.2.0rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## transwarp_hippo_api/conn_mgr.py

```diff
@@ -72,15 +72,15 @@
             for u in view:
                 if u in self.conns and self.conns[u] == ConnState.ACTIVE or self.conns[u] == ConnState.NO_CHECK_YET:
                     ret.append(u)
         if len(ret) > 0:
             random.shuffle(ret)
             return ret[0]
         else:
-            raise ValueError(f"no available host port from {view}.")
+            raise ValueError(f"Can not connect with hippo {view}.")
 
 
 globalConnManager = ConnManager()
 
 if __name__ == "__main__":
     test_cm = ConnManager(2)
     test_cm.add_conn("http://tw-node45:9500")
```

## transwarp_hippo_api/hippo_client.py

```diff
@@ -95,15 +95,15 @@
     @staticmethod
     def handle_json_resp(resp: Response) -> dict:
         if resp.status_code == 200:
             s = resp.content
             return json.loads(s)
         else:
             js = resp.json()
-            r = "error from restful_api:" + js["error"]["reason"]
+            r = "Error message from hippo server:" + js["error"]["reason"]
             raise ValueError(r)
 
 
 ''' Define the HippoTableMeta data class for storing table metadata information '''
 
 
 @dataclass
@@ -465,15 +465,14 @@
             "index_name": index_name,
             "wait_for_completion": wait_for_completion,
             "timeout": timeout,
         }
 
         js = json.dumps(req)
         js = json.loads(js)
-        print(js)
 
         if wait_for_completion:
             resp = self.hippo_conn.post(
                 f"/{self.tbl_name}/_activate_embedding_index?database_name={self.tbl_meta.db_name}&pretty",
                 js_data=js)
             r = HippoConn.handle_json_resp(resp)
             st = r.get("job_status")
@@ -915,36 +914,35 @@
               search_field: str,
               vectors,
               output_fields: list[str],
               topk: int,
               metric_type: str = 'l2',
               dsl: str = None,
               round_decimal: int = None,
-              only_explain = None,
-              with_profile = None,
+              only_explain=None,
+              with_profile=None,
               **params,
               ) -> list[HippoResult]:
-
         """
-                Query the table according to the specified query parameters and return the result.
+                        Query the table according to the specified query parameters and return the result.
 
-                Args:
-                    search_field: The name of the search field.
-                    vectors: The list of vectors for search.
-                    output_fields: The list of output fields.
-                    topk: The maximum number of results to return.
-                    metric_type: The type of metric, default is 'l2'.
-                    dsl: The specified Domain Specific Language (optional).
-                    round_decimal: decimal places to retain after scores defalut 2
-                    only_explain: Whether to only execute explain defalut false
-                    **params: Other query parameters.
-
-                Returns:
-                    Returns a list containing the query result.
-        """
+                        Args:
+                            search_field: The name of the search field.
+                            vectors: The list of vectors for search.
+                            output_fields: The list of output fields.
+                            topk: The maximum number of results to return.
+                            metric_type: The type of metric, default is 'l2'.
+                            dsl: The specified Domain Specific Language (optional).
+                            round_decimal: decimal places to retain after scores defalut 2
+                            only_explain: Whether to only execute explain defalut false
+                            **params: Other query parameters.
+
+                        Returns:
+                            Returns a list containing the query result.
+                """
 
         flag = ""
         for schema in self.schema:
             if (schema.name == search_field):
                 flag = schema.data_type.value
 
         point = False
@@ -957,40 +955,39 @@
             if with_profile is None:
                 with_profile = False
         else:
             round_decimal = 2
             only_explain = False
             with_profile = False
 
-
         if flag == HippoType.BINARY_VECTOR.value:
             req = {
                 "output_fields": output_fields,
                 "search_params": {
                     "anns_field": search_field,
                     "topk": topk,
                     "params": params,
                 },
                 "binary_vectors": vectors,
                 "round_decimal": round_decimal,
                 "only_explain": only_explain,
-                "with_profile" : with_profile
+                "with_profile": with_profile
             }
         elif flag == HippoType.SPARSE_FLOAT_VECTOR.value:
             req = {
                 "output_fields": output_fields,
                 "search_params": {
                     "anns_field": search_field,
                     "topk": topk,
                     "params": params
                 },
                 "sparse_vectors": vectors,
                 "round_decimal": round_decimal,
                 "only_explain": only_explain,
-                "with_profile" : with_profile
+                "with_profile": with_profile
             }
         elif flag == HippoType.FLOAT_VECTOR.value:
             if point:
                 req = {
                     "output_fields": output_fields,
                     "search_params": {
                         "anns_field": search_field,
@@ -1006,15 +1003,15 @@
                         "anns_field": search_field,
                         "topk": topk,
                         "params": params,
                     },
                     "vectors": vectors,
                     "round_decimal": round_decimal,
                     "only_explain": only_explain,
-                    "with_profile" : with_profile
+                    "with_profile": with_profile
                 }
         else:
             req = {
                 "output_fields": output_fields,
                 "search_params": {
                     "anns_field": search_field,
                     "topk": topk,
@@ -1066,16 +1063,15 @@
                     this_query_ret_result[field_name] = field_values
                     this_query_ret_result[field_name + "%scores"] = scores
 
                 total_result[query_id] = this_query_ret_result
         except BaseException as e:
             raise ValueError(f"error during process result, exception -> is {e}. \nreturn json is {resp.json()}")
         return total_result
-    
-        
+
     def add_columns(self, fields: list[HippoField]):
         """
                 Add new columns to the current table.
 
                 Args:
                     fields (list[HippoField]): A list of HippoField objects representing the columns to be added.
 
@@ -1146,14 +1142,63 @@
         resp = self.hippo_conn.post(f"/{self.tbl_name}/_rename_columns?database_name={self.tbl_meta.db_name}&pretty", js_data=js)
         r = HippoConn.handle_json_resp(resp)
         if r.get("acknowledged"):
             return True
         else:
             raise ValueError(r)
         
+    def add_partitions(self, partitions: dict):
+        """
+                Add partitions to the current table.
+
+                Args:
+                    partitions (dict): A dictionary representing the partitions to be added.
+                                    The dictionary should follow the format {"partitions": [{"name": "partition_name", ...}, ...]}.
+
+                Returns:
+                    bool: True if the addition of partitions is successful.
+
+                Raises:
+                    ValueError: If the addition process is not acknowledged, a ValueError exception is raised.
+        """
+        data = partitions
+        js = json.dumps(data, cls=HippoTypesEncoder)
+        js = json.loads(js)
+        resp = self.hippo_conn.put(f"/{self.tbl_name}/_partitions?database_name={self.tbl_meta.db_name}&pretty", js_data=js)
+        r = HippoConn.handle_json_resp(resp)
+        if r.get("acknowledged"):
+            return True
+        else:
+            raise ValueError(r)
+        
+    def delete_partitions(self, partition_names: list):
+        """
+                Delete specified partitions from the current table.
+
+                Args:
+                    partition_names (list): A list of partition names to be deleted.
+
+                Returns:
+                    bool: True if the deletion of partitions is successful.
+
+                Raises:
+                    ValueError: If the deletion process is not acknowledged, a ValueError exception is raised.
+        """
+        
+        data = {}
+        data["partition_names"] = partition_names
+        js = json.dumps(data, cls=HippoTypesEncoder)
+        js = json.loads(js)
+        resp = self.hippo_conn.delete(f"/{self.tbl_name}/_partitions?database_name={self.tbl_meta.db_name}&pretty", js_data=js)
+        r = HippoConn.handle_json_resp(resp)
+        if r.get("acknowledged"):
+            return True
+        else:
+            raise ValueError(r)
+    
 # Define a function to handle type strings, returning the corresponding HippoType enumeration value or None
 def _handle_type_str(type_str: str) -> Optional[HippoType]:
     lower_type_name = type_str.lower()
     for m in HippoType.__members__.values():
         if m.value == lower_type_name:
             return m
     for k, v in HippoTypeAliases.items():
@@ -1840,26 +1885,32 @@
     # Creates a new table in a specified database.
     def create_table(self,
                      name: str,
                      fields: list[HippoField],
                      auto_id: bool = False,
                      database_name: str = "default",
                      number_of_shards: int = 1,
-                     number_of_replicas: int = 1) -> Optional[HippoTable]:
+                     number_of_replicas: int = 1,
+                     partition_schema: dict = None
+                     ) -> Optional[HippoTable]:
 
         """
                 Creates a new table in a specified database.
 
                 Parameters:
-                    name: The table name.
-                    fields: A list of HippoField objects, each representing a field.
-                    auto_id: Whether to set an auto-incrementing primary key.
-                    database_name: The database name, default is "default".
-                    number_of_shards: The number of shards, default is 1.
-                    number_of_replicas: The number of replicas, default is 1.
+                    schema:
+                        name: The table name.
+                        fields: A list of HippoField objects, each representing a field.
+                        auto_id: Whether to set an auto-incrementing primary key.
+                        database_name: The database name, default is "default".
+                    settings:
+                        number_of_shards: The number of shards, default is 1.
+                        number_of_replicas: The number of replicas, default is 1.
+                    partition_shcema:
+                        A dict of partition info
 
                 Returns:
                     If creation is successful, return a HippoTable object. Otherwise, throw a ValueError exception.
         """
         fields_for_req = [asdict(f) for f in fields]
 
         data = {
@@ -1868,19 +1919,23 @@
                 'number_of_replicas': number_of_replicas,
             },
             'schema': {
                 'auto_id': auto_id,
                 'fields': fields_for_req,
             }
         }
+        if partition_schema != None:
+            data['partition_schema'] = partition_schema
+        
 
         js = json.dumps(data, cls=HippoTypesEncoder)
         js = json.loads(js)
 
         resp = self.hippo_conn.put(f"/{name}?database_name={database_name}&pretty", js_data=js)
+
         r = HippoConn.handle_json_resp(resp)
         if resp.status_code == 200 and r.get("acknowledged") is True:
             meta = HippoTableMeta(tbl_name=name, auto_id=auto_id, schema=fields, n_replicas=number_of_replicas,
                                   n_shards=number_of_shards, db_name=database_name)
             return HippoTable(hippo_conn=self.hippo_conn, tbl_meta=meta)
         else:
             raise ValueError(resp.content)
@@ -2549,8 +2604,8 @@
                 return True
             elif st is None or st != HippoJobStatus.HIPPO_JOB_INVALID.value:
                 error_info = None
                 try:
                     error_info = r.get("errors")
                 except:
                     pass
-                raise ValueError(f"build index return status: {st}, error info: {error_info}")
+                raise ValueError(f"build index return status: {st}, error info: {error_info}")
```

## Comparing `hippo_api-1.2.0rc6.dist-info/RECORD` & `hippo_api-1.2.0rc7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 transwarp_embedding_hub/base_embedding.py,sha256=fV_7_awiGCnQWDMxJHUCDMoeUh_FX0S5RoiQAvtf0kY,846
 transwarp_embedding_hub/config.yaml,sha256=gUZ-_X-_RM2ScrDT-zLd4buwvQYJGzzMWtGkHQMN6cY,355
 transwarp_embedding_hub/embedding_hub.py,sha256=Us3EzCtrQ8kt31hC4o66JRVnhKosyPrlmMzKlvvVdCI,703
 transwarp_embedding_hub/openai.py,sha256=mYHjMSdg1PWnEOBsiwfoz_vkirmRSvPlUVSgmnd-8zw,2389
 transwarp_embedding_hub/pulse.py,sha256=o5El2p8FhaD52wsDzEqAxx0izqz07Bam73iy9IlWnEM,4608
 transwarp_embedding_hub/text_segmentation.py,sha256=kOjMLdAa_NHqXJl5VHNe1ywmIt1hV3u3bYf5vaH8bEA,4552
 transwarp_hippo_api/__init__.py,sha256=5HW4WI56IwE4O7nM7iQ7Bx0YceMppe6H5vYKagA3GDI,78
-transwarp_hippo_api/conn_mgr.py,sha256=ZoQHgyTtmryUXMKfv8jg3qgZtb2aU-6t1vb0raX51Z8,2625
-transwarp_hippo_api/hippo_client.py,sha256=p2IrhKd8UNvUeb6A3ZDhAyeUse4SjquP_bR5PcGIsaY,99327
+transwarp_hippo_api/conn_mgr.py,sha256=aorA355Q-OjmJ4DM_uvNb0XgDeEIbuatmvUGlrw49II,2624
+transwarp_hippo_api/hippo_client.py,sha256=Sc9HEpwy-J2mru01ML8bMH63vT9m9MaJWoKSBJp8mDE,101690
 transwarp_hippo_api/hippo_type.py,sha256=wjl-g8kJghHY6CUfSJ9bWhVhkyLH8aYMgOE6uevpqXY,1555
 transwarp_hippo_api/private_embedding.py,sha256=Chw8l9mQdV5SEg2quSyU_f8Z7DiwY30UPs4Vsad4xk8,577
 transwarp_hippo_langchain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 transwarp_hippo_langchain/embedding_hub_langchain.py,sha256=aqojyVU_lWdxUMge8L8xHeGySwgmuK0nJYDR6fmvkMk,1223
 transwarp_hippo_langchain/hippo_langchain.py,sha256=TNiyPZVRgJ7iRFaMc0X_wOwfHmyEw_PcIkGb-MtnuYg,23069
-hippo_api-1.2.0rc6.dist-info/METADATA,sha256=O7kfGdj77u97RZeJkeEcVziJIdOxZrGxAYZ0tCKRZgg,129
-hippo_api-1.2.0rc6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-hippo_api-1.2.0rc6.dist-info/top_level.txt,sha256=Xqsbi0Wu1Ti7R7-MeVmJ_k4xOx4mU4FfOmi4e9hgea4,46
-hippo_api-1.2.0rc6.dist-info/RECORD,,
+hippo_api-1.2.0rc7.dist-info/METADATA,sha256=xn3TzGNRw62ryOg6Ht-sZ8hw2JLC-SLZQufZD_I6JRs,129
+hippo_api-1.2.0rc7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+hippo_api-1.2.0rc7.dist-info/top_level.txt,sha256=Xqsbi0Wu1Ti7R7-MeVmJ_k4xOx4mU4FfOmi4e9hgea4,46
+hippo_api-1.2.0rc7.dist-info/RECORD,,
```

