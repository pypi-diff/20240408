# Comparing `tmp/haskellian-either-0.1.4.tar.gz` & `tmp/haskellian-either-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-either-0.1.4.tar", last modified: Fri Apr  5 16:49:54 2024, max compression
+gzip compressed data, was "haskellian-either-0.1.5.tar", last modified: Mon Apr  8 10:51:53 2024, max compression
```

## Comparing `haskellian-either-0.1.4.tar` & `haskellian-either-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 16:49:54.851544 haskellian-either-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-05 16:49:54.851544 haskellian-either-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-05 16:49:52.000000 haskellian-either-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-05 16:49:54.851544 haskellian-either-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 16:49:54.851544 haskellian-either-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 16:49:54.851544 haskellian-either-0.1.4/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 16:49:54.851544 haskellian-either-0.1.4/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      225 2024-04-05 16:47:08.000000 haskellian-either-0.1.4/src/haskellian/either/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 16:49:54.851544 haskellian-either-0.1.4/src/haskellian/either/extras/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-05 16:46:47.000000 haskellian-either-0.1.4/src/haskellian/either/extras/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-05 16:46:28.000000 haskellian-either-0.1.4/src/haskellian/either/extras/pydantic.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1061 2024-04-05 16:45:19.000000 haskellian-either-0.1.4/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2121 2024-04-05 06:25:01.000000 haskellian-either-0.1.4/src/haskellian/either/type.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 16:49:54.851544 haskellian-either-0.1.4/src/haskellian_either.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-05 16:49:54.000000 haskellian-either-0.1.4/src/haskellian_either.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      425 2024-04-05 16:49:54.000000 haskellian-either-0.1.4/src/haskellian_either.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-05 16:49:54.000000 haskellian-either-0.1.4/src/haskellian_either.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-05 16:49:54.000000 haskellian-either-0.1.4/src/haskellian_either.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-05 16:49:54.000000 haskellian-either-0.1.4/src/haskellian_either.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-08 10:51:50.000000 haskellian-either-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.309388 haskellian-either-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.309388 haskellian-either-0.1.5/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-04-05 17:36:56.000000 haskellian-either-0.1.5/src/haskellian/either/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/src/haskellian/either/extras/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-05 16:46:47.000000 haskellian-either-0.1.5/src/haskellian/either/extras/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-05 16:46:28.000000 haskellian-either-0.1.5/src/haskellian/either/extras/pydantic.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1228 2024-04-08 10:51:36.000000 haskellian-either-0.1.5/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      294 2024-04-08 10:48:52.000000 haskellian-either-0.1.5/src/haskellian/either/narrowing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1942 2024-04-08 10:51:32.000000 haskellian-either-0.1.5/src/haskellian/either/type.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/src/haskellian_either.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/top_level.txt
```

### Comparing `haskellian-either-0.1.4/pyproject.toml` & `haskellian-either-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian-either"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple Either type"
 dependencies = []
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
```

### Comparing `haskellian-either-0.1.4/src/haskellian/either/funcs.py` & `haskellian-either-0.1.5/src/haskellian/either/funcs.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def safe(func: Callable[[], R], Exc: type[Err] = Exception) -> 'Either[Err, R]':
     try:
       return Right(func())
     except Exc as e:
       return Left(e)
     
 def maybe(x: R | None) -> 'Either[None, R]':
-  return Left() if x is None else Right(x)
+  return Left(None) if x is None else Right(x)
     
 def sequence(eithers: Iterable[Either[L, R]]) -> Either[list[L], list[R]]:
   """List of lefts if any (thus with length in `[1, len(eithers)]`), otherwise list of all rights (with length `len(eithers)`)"""
   lefts: list[L] = []
   rights: list[R] = []
   for x in eithers:
     x.match(lefts.append, rights.append)
@@ -29,7 +29,15 @@
         yield value
 
 def filter_lefts(eithers: Iterable[Either[L, R]]) -> Iterable[L]:
   for e in eithers:
     match e:
       case Left(err):
         yield err
+
+def take_while(eithers: Iterable[Either[L, R]]) -> Iterable[R]:
+  for e in eithers:
+    match e:
+      case Right(x):
+        yield x
+      case _:
+        return
```

### Comparing `haskellian-either-0.1.4/src/haskellian/either/type.py` & `haskellian-either-0.1.5/src/haskellian/either/type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,70 @@
-from typing import Generic, TypeVar, Literal, Callable
-from abc import ABC
+from typing import Generic, TypeVar, Literal, Callable, Any, TypeGuard
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 A = TypeVar('A')
 L = TypeVar('L', covariant=True)
 R = TypeVar('R', covariant=True)
 L2 = TypeVar('L2')
 R2 = TypeVar('R2')
 
 @dataclass(eq=False)
 class IsLeft(BaseException, Generic[L]):
   value: L
 
-@dataclass
-class Either(ABC, Generic[L, R]):
-  value: L | R
-  tag: Literal['left', 'right']
+class EitherBase(ABC, Generic[L, R]):
 
+  @abstractmethod
   def match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
     """Unwrap an `Either` by matching both branches"""
-    match self:
-      case Left(err):
-        return on_left(err)
-      case Right(value):
-        return on_right(value)
-      
-  def match_(self, on_left: Callable[[], A], on_right: Callable[[], A]) -> A:
-    """Like `match`, but handlers don't get the wrapped value"""
-    return self.match(lambda _: on_left(), lambda _: on_right())
-  
-  def tap(self, on_left: Callable[[L], None] = lambda _: None, on_right: Callable[[R], None] = lambda _: None) -> 'Either[L, R]':
-    """Execute `on_left`/`on_right` but return the either as is"""
-    match self:
-      case Left(err):
-        on_left(err)
-      case Right(value):
-        on_right(value)
-    return self
-  
+
+  @abstractmethod
+  def unsafe(self) -> R:
+    """Unwraps the value or throws an `IsLeft` exception
+    
+    (`IsLeft.value` will contain the wrapped value)"""
+    
+
+  def bind(self, f: 'Callable[[R], Either[L, R2]]') -> 'Either[L, R2]':
+    return self.match(lambda x: Left(x), f)
+
+  def fmap(self, f: Callable[[R], R2]) -> 'Either[L, R2]':
+    return self.match(lambda x: Left(x), lambda x: Right(f(x)))
+
   def mapl(self, f: Callable[[L], L2]) -> 'Either[L2, R]':
     """Map the left branch"""
     return self.match(lambda x: Left(f(x)), lambda x: Right(x))
-  
-  def fmap(self, f: Callable[[R], R2]) -> 'Either[L, R2]':
-    return self.match(lambda x: Left(x), lambda x: Right(f(x)))
-  
+
   __or__ = fmap
   """Alias of `fmap`"""
-      
-  def bind(self, f: 'Callable[[R], Either[L2, R2]]') -> 'Either[L|L2, R2]':
-    return self.match(lambda x: Left(x), f)
   
   __and__ = bind
   """Alias of `bind`"""
-
-  def unsafe(self) -> R:
-    """Unwraps the value or throws an `IsLeft` exception
-    
-    (`IsLeft.value` will contain the wrapped value)"""
-    match self:
-      case Left(err):
-        raise IsLeft(err)
-      case Right(value):
-        return value
-
+  
+  def match_(self, on_left: Callable[[], A], on_right: Callable[[], A]) -> A:
+    """Like `match`, but handlers don't get the wrapped value"""
+    return self.match(lambda _: on_left(), lambda _: on_right())
+  
 @dataclass
-class Left(Either[L, R]):
-  value: L = None
+class Left(EitherBase[L, Any], Generic[L]):
+  value: L
   tag: Literal['left'] = 'left'
 
+  def match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
+    return on_left(self.value)
+  
+  def unsafe(self):
+    raise IsLeft(self.value)
+
 @dataclass
-class Right(Either[L, R]):
-  value: R = None
-  tag: Literal['right'] = 'right'
+class Right(EitherBase[Any, R], Generic[R]):
+  value: R
+  tag: Literal['right'] = 'right'
+
+  def match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
+    return on_right(self.value)
+  
+  def unsafe(self) -> R:
+    return self.value
+
+Either = Left[L] | Right[R]
```

