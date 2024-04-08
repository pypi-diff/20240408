# Comparing `tmp/pydantic2_resolve-2.0.0.tar.gz` & `tmp/pydantic2_resolve-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic2_resolve-2.0.0.tar", max compression
+gzip compressed data, was "pydantic2_resolve-2.1.0.tar", max compression
```

## Comparing `pydantic2_resolve-2.0.0.tar` & `pydantic2_resolve-2.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-11-01 02:38:24.970361 pydantic2_resolve-2.0.0/LICENSE
--rw-r--r--   0        0        0     7683 2024-02-29 13:58:11.424300 pydantic2_resolve-2.0.0/README.md
--rw-r--r--   0        0        0      629 2024-02-29 13:58:11.435795 pydantic2_resolve-2.0.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      362 2024-02-29 13:58:11.435929 pydantic2_resolve-2.0.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     4239 2024-02-29 13:58:11.436082 pydantic2_resolve-2.0.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      280 2024-02-29 13:58:11.436236 pydantic2_resolve-2.0.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0    11242 2024-02-29 13:58:11.436452 pydantic2_resolve-2.0.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0    13279 2024-02-29 13:58:11.436756 pydantic2_resolve-2.0.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      766 2024-02-29 13:58:11.437011 pydantic2_resolve-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     8515 1970-01-01 00:00:00.000000 pydantic2_resolve-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-11-01 02:38:24.970361 pydantic2_resolve-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3914 2024-04-08 13:13:13.052286 pydantic2_resolve-2.1.0/README.md
+-rw-r--r--   0        0        0      815 2024-04-08 12:50:08.904200 pydantic2_resolve-2.1.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      425 2024-04-08 12:50:08.904487 pydantic2_resolve-2.1.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0    14051 2024-04-08 12:50:08.904882 pydantic2_resolve-2.1.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      280 2024-02-29 13:58:11.436236 pydantic2_resolve-2.1.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     9366 2024-04-08 12:51:17.738611 pydantic2_resolve-2.1.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0    13455 2024-04-08 12:55:52.837311 pydantic2_resolve-2.1.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      826 2024-04-08 13:14:11.402036 pydantic2_resolve-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 pydantic2_resolve-2.1.0/PKG-INFO
```

### Comparing `pydantic2_resolve-2.0.0/LICENSE` & `pydantic2_resolve-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic2_resolve-2.0.0/pydantic_resolve/__init__.py` & `pydantic2_resolve-2.1.0/pydantic_resolve/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 from .exceptions import (
     ResolverTargetAttrNotFound,
     DataloaderDependCantBeResolved,
     LoaderFieldNotProvidedError,
-    MissingAnnotationError)
-from .resolver import Resolver, LoaderDepend
-from .util import build_list, build_object, mapper, ensure_subset, output, copy_dataloader_kls, model_config
+    MissingAnnotationError,
+    GlobalLoaderFieldOverlappedError)
+from .resolver import Resolver 
+from .core import LoaderDepend, Collector, ICollector
+from .util import (
+    build_list,
+    build_object,
+    mapper,
+    ensure_subset,
+    output,
+    model_config,
+    copy_dataloader_kls)
 
 __all__ = [
     'Resolver',
     'LoaderDepend',
+    'Collector',
+    'ICollector',
     'ResolverTargetAttrNotFound',
     'DataloaderDependCantBeResolved',
     'LoaderFieldNotProvidedError',
     'MissingAnnotationError',
+    'GlobalLoaderFieldOverlappedError',
+
     'build_list',
     'build_object',
     'mapper',
     'ensure_subset',
     'output',
     'model_config',
     'copy_dataloader_kls'
```

### Comparing `pydantic2_resolve-2.0.0/pydantic_resolve/util.py` & `pydantic2_resolve-2.1.0/pydantic_resolve/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,24 @@
     anno = cls.__dict__.get('__annotations__') or {}
     return anno.keys()
 
 
 T = TypeVar("T")
 V = TypeVar("V")
 
+def safe_issubclass(kls, classinfo):
+    try:
+        return issubclass(kls, classinfo)
+    except TypeError:
+        return False
+
 def merge_dicts(a: Dict[str, Any], b: Dict[str, Any]):
     overlap = set(a.keys()) & set(b.keys())
     if overlap:
-        raise GlobalLoaderFieldOverlappedError(f'loader_filters and global_loader_filter have duplicated key(s): {",".join(overlap)}')
+        raise GlobalLoaderFieldOverlappedError(f'loader_params and global_loader_param have duplicated key(s): {",".join(overlap)}')
     else:
         return {**a, **b}
 
 def build_object(items: Sequence[T], keys: List[V], get_pk: Callable[[T], V]) -> Iterator[Optional[T]]:
     """
     helper function to build return object data required by aiodataloader
     """
@@ -64,32 +70,32 @@
     # 1. get required fields
     for fname, field in kls.model_fields.items():
         if field.is_required():
             required_fields.append(fname)
 
     # 2. get resolve_ and post_ target fields
     for f in dir(kls):
-        if f.startswith(const.PREFIX):
+        if f.startswith(const.RESOLVE_PREFIX):
             if isfunction(getattr(kls, f)):
-                required_fields.append(f.replace(const.PREFIX, ''))
+                required_fields.append(f.replace(const.RESOLVE_PREFIX, ''))
 
         if f.startswith(const.POST_PREFIX):
             if isfunction(getattr(kls, f)):
                 required_fields.append(f.replace(const.POST_PREFIX, ''))
     
     return required_fields
 
 
 def output(kls):
     """
     set required as True for all fields
     make typescript code gen result friendly to use
     """
 
-    if issubclass(kls, BaseModel):
+    if safe_issubclass(kls, BaseModel):
 
         def build():
             def schema_extra(schema: Dict[str, Any], model) -> None:
                 fnames = get_required_fields(model)
                 schema['required'] = fnames
             return schema_extra
 
@@ -105,15 +111,15 @@
     model_config now is just a simple decorator to remove fields (with exclude=True) from schema.properties
     and set schema.required for better schema description. 
     (same like `output` decorator, you can replace output with model_config)
 
     it keeps the form of model_config(params) in order to extend new features in future
     """
     def wrapper(kls):
-        if issubclass(kls, BaseModel):
+        if safe_issubclass(kls, BaseModel):
             def build():
                 def _schema_extra(schema: Dict[str, Any], model) -> None:
                     # 1. collect exclude fields and then hide in both schema and dump (default action)
                     excluded_fields = [k for k, v in kls.model_fields.items() if v.exclude == True]
                     props = {}
 
                     # config schema properties
@@ -182,15 +188,15 @@
 
 def _get_mapping_rule(target, source) -> Optional[Callable]:
     # do noting
     if isinstance(source, target):
         return None
 
     # pydantic
-    if issubclass(target, BaseModel):
+    if safe_issubclass(target, BaseModel):
         if target.model_config.get('from_attributes'):
             if isinstance(source, dict):
                 raise AttributeError(f"{type(source)} -> {target.__name__}: pydantic from_orm can't handle dict object")
             else:
                 return lambda t, s: t.model_validate(s)
 
         if isinstance(source, dict):
@@ -225,16 +231,16 @@
 
 def ensure_subset(base):
     """
     used with pydantic class to make sure a class's field is 
     subset of target class
     """
     def wrap(kls):
-        assert issubclass(base, BaseModel), 'base should be pydantic class'
-        assert issubclass(kls, BaseModel), 'class should be pydantic class'
+        assert safe_issubclass(base, BaseModel), 'base should be pydantic class'
+        assert safe_issubclass(kls, BaseModel), 'class should be pydantic class'
 
         @functools.wraps(kls)
         def inner():
             for k, field in kls.model_fields.items():
                 if field.is_required():
                     base_field = base.model_fields.get(k)
                     if not base_field:
@@ -266,15 +272,15 @@
             kls.__annotations__ = anno
             setattr(kls, const.DATACLASS_FORWARD_REF_UPDATED, True)
 
             for _, v in kls.__annotations__.items():
                 shelled_type = shelling_type(v)
                 update_forward_refs(shelled_type)
 
-    if issubclass(kls, BaseModel):
+    if safe_issubclass(kls, BaseModel):
         update_pydantic_forward_refs(kls)
 
     if is_dataclass(kls):
         update_dataclass_forward_refs(kls)
 
 
 class TypeAdapterManager:
```

### Comparing `pydantic2_resolve-2.0.0/pyproject.toml` & `pydantic2_resolve-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic2-resolve"
-version = "2.0.0"
+version = "2.1.0"
 description = "create nested data structure easily"
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic2_resolve"
 keywords = ["pydantic2", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
@@ -24,7 +24,12 @@
 pytest-asyncio = "^0.21.0"
 fastapi = "^0.100.0"
 uvicorn = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+]
```

