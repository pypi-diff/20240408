# Comparing `tmp/zephony-1.7.1.tar.gz` & `tmp/zephony-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephony-1.7.1.tar", last modified: Thu Apr  4 23:08:07 2024, max compression
+gzip compressed data, was "zephony-1.9.tar", last modified: Mon Apr  8 20:10:30 2024, max compression
```

## Comparing `zephony-1.7.1.tar` & `zephony-1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:08:07.940306 zephony-1.7.1/
--rw-r--r--   0 root         (0) root         (0)      276 2024-04-04 23:08:07.940306 zephony-1.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      290 2024-04-04 23:07:50.000000 zephony-1.7.1/README.md
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-04 23:08:07.940306 zephony-1.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      408 2024-04-04 23:07:50.000000 zephony-1.7.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:08:07.936306 zephony-1.7.1/zephony/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3323 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/decorators.py
--rw-r--r--   0 root         (0) root         (0)     4145 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18046 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:08:07.936306 zephony-1.7.1/zephony/models/
--rw-r--r--   0 root         (0) root         (0)    46626 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7377 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:08:07.940306 zephony-1.7.1/zephony.egg-info/
--rw-r--r--   0 root         (0) root         (0)      276 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:10:30.746260 zephony-1.9/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-08 20:10:30.746260 zephony-1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      290 2024-04-08 20:10:13.000000 zephony-1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-08 20:10:30.750260 zephony-1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-08 20:10:13.000000 zephony-1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:10:30.746260 zephony-1.9/zephony/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 20:10:13.000000 zephony-1.9/zephony/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2024-04-08 20:10:13.000000 zephony-1.9/zephony/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2024-04-08 20:10:13.000000 zephony-1.9/zephony/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18046 2024-04-08 20:10:13.000000 zephony-1.9/zephony/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:10:30.746260 zephony-1.9/zephony/models/
+-rw-r--r--   0 root         (0) root         (0)    48370 2024-04-08 20:10:13.000000 zephony-1.9/zephony/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7377 2024-04-08 20:10:13.000000 zephony-1.9/zephony/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:10:30.746260 zephony-1.9/zephony.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-08 20:10:30.000000 zephony-1.9/zephony.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-08 20:10:30.000000 zephony-1.9/zephony.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 20:10:30.000000 zephony-1.9/zephony.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-08 20:10:30.000000 zephony-1.9/zephony.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 20:10:30.000000 zephony-1.9/zephony.egg-info/top_level.txt
```

### Comparing `zephony-1.7.1/zephony/decorators.py` & `zephony-1.9/zephony/decorators.py`

 * *Files identical despite different names*

### Comparing `zephony-1.7.1/zephony/exceptions.py` & `zephony-1.9/zephony/exceptions.py`

 * *Files identical despite different names*

### Comparing `zephony-1.7.1/zephony/helpers.py` & `zephony-1.9/zephony/helpers.py`

 * *Files identical despite different names*

### Comparing `zephony-1.7.1/zephony/models/__init__.py` & `zephony-1.9/zephony/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,14 +566,38 @@
                     ])
                 )
             else:
                 logger.warn(f'Invalid column type : {filter_["key"]}')
 
         return q
 
+    @classmethod
+    def apply_q_string_filter_to_query(cls, q, q_string):
+        if not q_string:
+            return q
+
+        # 0. Generate the wildcard q_string
+        q_wildcard_string = '%'
+        for character in q_string:
+            q_wildcard_string += character + '%'
+
+        # 1. Get all searchable fields of the model
+        fields = []
+        for searchable_field_string in cls.searchable_fields:
+            fields.append(getattr(cls, searchable_field_string))
+
+        # 2. Loop through them and apply the search filter
+        q = q.filter(
+            or_(
+                *[field.ilike(q_wildcard_string) for field in fields]
+            )
+        )
+
+        return q
+
     # NOTE: Doesn't do any joins
     @classmethod
     def get_one(cls, id_or_token, with_organization=True):
         """
         Returns the object from the database based on whether the
         filter is the id or the token. Returns None if the object
         is not found.
@@ -939,20 +963,22 @@
 
         db.session.flush()
 
         return self
 
     @staticmethod
     def convert_filters_to_ands_and_ors(join, model_string_alias_map):
-        # Returns something like this:
-        #
-        # and_(
-        #     or_(a==b, c==d),
-        #     or_(e==f, g==h),
-        # )
+        """
+        Returns something like this:
+       
+        and_(
+            or_(a==b, c==d),
+            or_(e==f, g==h),
+        )
+        """
 
         ors_list = []
         # if 'filters' is present in join
         for key in join.get('filters', {}).keys():
             model_string, property_string = key.split('.')
             Model = model_string_alias_map[model_string]
 
@@ -969,19 +995,20 @@
     @classmethod
     def filter(
         cls,
         filters={},
         joins=[],
         bridge_joins=[],
         list_joins=[],
-        order_by='id_',
+        order_by='name',
         reverse_order=False,
         pagination={},
         get_details=True,
         first_item=False,
+        params={},
     ):
         """
         sub_query is used to solve the pagination problem when doing
         left joins. (We're currently using that structure for all queries
         even when a join is not required - might have to fix it later if we
         notice any performance issue).
 
@@ -995,20 +1022,14 @@
         # Filters related
         if 'is_deleted' not in filters:
             filters['is_deleted'] = False
 
         # q = q.filter_by(**filters)
         sub_query = sub_query.filter_by(**filters)
 
-        # Order by related
-        order_by_field = getattr(cls, order_by)
-        if reverse_order:
-            order_by_field = desc(order_by_field)
-        sub_query = sub_query.order_by(order_by_field)
-
         if first_item:
             sub_query = sub_query.limit(1)
         else:
             # Get paginated_query
             (sub_query, page, page_size) = cls.add_pagination_to_query(
                 q=sub_query,
                 params={
@@ -1017,14 +1038,38 @@
                 },
             )
 
         sub_query = sub_query.subquery('parent_subquery')
         parent_alias = aliased(cls, sub_query)
 
         q = db.session.query(cls).join(sub_query, cls.id_==sub_query.c.id_)
+        
+        # Apply filters to the actual query (from params)
+        if hasattr(cls, 'filterable_fields'):
+            filterable_fields = cls.filterable_fields
+        else:
+            filterable_fields = []
+        filterable_fields_map = {}
+        for filterable_field in filterable_fields:
+            filterable_fields_map[filterable_field] = getattr(cls, filterable_field)
+
+        q = cls.add_filters_to_query(q, params, filterable_fields_map)
+        
+        # Apply q_string filter to the query (from params)
+        # TODO: Check if this requires protection from sql injection
+        # or needs removal of any special character before passing down
+        if 'q' in params:
+            q = cls.apply_q_string_filter_to_query(q, params['q'])
+
+        # Order by related
+        order_by_field = getattr(cls, order_by)
+        if reverse_order:
+            ic('Reverse ordering..')
+            order_by_field = desc(order_by_field)
+        q = q.order_by(order_by_field)
 
         # NX1 joins (aka. normal joins)
         for i, join in enumerate(joins):
             # This alias is required so that if there are multiple columns
             # being joined to the same table, SQLAlchemy knows which column
             # join is which.
             # 
@@ -1122,14 +1167,17 @@
                 )
                 .add_entity(join['secondary_model'])
             )
 
         # Fetch the results
         results = q.all()
 
+        for r in results:
+            print(r)
+
         if not get_details:
             return results
 
         # Final list
         objects_details = []
 
         # To avoid row duplicates due to 1xN or NxN relationship
@@ -1266,16 +1314,21 @@
                     details[join[2]] = None
 
         for primary_id, details in primary_objects_map.items():
             objects_details.append(details)
 
         # If the `with_summary` param is set, return the data with the
         # pagination details
-        if pagination.get('with_summary'):
-            return (objects_details, count)
+        if pagination.get('with_summary') and pagination.get('page'):
+            return cls.return_with_summary(
+                objects_details,
+                page,
+                page_size,
+                cls.query.filter(cls.is_deleted==False).count(),
+            )
 
         if first_item:
             if len(objects_details) == 0:
                 return None
             return objects_details[0]
 
         return objects_details
```

### Comparing `zephony-1.7.1/zephony/validators.py` & `zephony-1.9/zephony/validators.py`

 * *Files identical despite different names*

