# Comparing `tmp/omniply-0.3.tar.gz` & `tmp/omniply-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniply-0.3.tar", last modified: Sat Apr  6 12:19:43 2024, max compression
+gzip compressed data, was "omniply-0.3.1.tar", last modified: Mon Apr  8 10:10:00 2024, max compression
```

## Comparing `omniply-0.3.tar` & `omniply-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.529205 omniply-0.3/
--rw-r--r--   0 fleeb     (7343) is        (1040)     1067 2024-02-14 16:25:24.000000 omniply-0.3/LICENSE
--rw-r--r--   0 fleeb     (7343) is        (1040)      516 2024-04-06 12:19:43.529205 omniply-0.3/PKG-INFO
--rw-r--r--   0 fleeb     (7343) is        (1040)      216 2024-02-14 16:25:24.000000 omniply-0.3/README.md
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.525205 omniply-0.3/omniply/
--rw-r--r--   0 fleeb     (7343) is        (1040)       60 2024-04-06 12:17:07.000000 omniply-0.3/omniply/__init__.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.525205 omniply-0.3/omniply/_future/
--rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:25:24.000000 omniply-0.3/omniply/_future/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     2501 2024-02-14 16:25:24.000000 omniply-0.3/omniply/_future/common.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     4287 2024-02-14 16:25:24.000000 omniply-0.3/omniply/_future/specification.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3749 2024-02-14 16:25:24.000000 omniply-0.3/omniply/_future/wrappers.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.525205 omniply-0.3/omniply/apps/
--rw-r--r--   0 fleeb     (7343) is        (1040)      159 2024-03-27 17:40:13.000000 omniply-0.3/omniply/apps/__init__.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.529205 omniply-0.3/omniply/apps/iterative/
--rw-r--r--   0 fleeb     (7343) is        (1040)       25 2024-03-29 16:54:35.000000 omniply-0.3/omniply/apps/iterative/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1580 2024-03-29 17:08:38.000000 omniply-0.3/omniply/apps/iterative/abstract.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      671 2024-03-29 16:54:35.000000 omniply-0.3/omniply/apps/iterative/guru.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      188 2024-03-17 13:15:20.000000 omniply-0.3/omniply/apps/iterative/imports.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      723 2024-03-29 16:47:20.000000 omniply-0.3/omniply/apps/iterative/innovators.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1343 2024-03-29 16:54:35.000000 omniply-0.3/omniply/apps/iterative/moguls.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3654 2024-03-29 16:05:33.000000 omniply-0.3/omniply/apps/simple.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1360 2024-03-29 15:44:11.000000 omniply-0.3/omniply/apps/staging.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1384 2024-03-15 14:29:45.000000 omniply-0.3/omniply/apps/templating.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.529205 omniply-0.3/omniply/core/
--rw-r--r--   0 fleeb     (7343) is        (1040)      171 2024-03-14 13:44:31.000000 omniply-0.3/omniply/core/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     8643 2024-03-28 15:53:05.000000 omniply-0.3/omniply/core/abstract.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     2050 2024-02-14 16:25:24.000000 omniply-0.3/omniply/core/errors.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     6732 2024-03-24 15:18:18.000000 omniply-0.3/omniply/core/gadgets.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    11322 2024-03-24 16:04:01.000000 omniply-0.3/omniply/core/gaggles.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     8118 2024-03-24 14:49:06.000000 omniply-0.3/omniply/core/gangs.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     8762 2024-03-29 16:12:01.000000 omniply-0.3/omniply/core/genetics.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    10998 2024-03-24 14:47:29.000000 omniply-0.3/omniply/core/gigs.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1353 2024-02-14 16:25:24.000000 omniply-0.3/omniply/core/gizmos.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     5275 2024-03-28 17:28:50.000000 omniply-0.3/omniply/core/op.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     7135 2024-03-29 16:12:01.000000 omniply-0.3/omniply/core/tools.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    27493 2024-03-28 17:26:39.000000 omniply-0.3/omniply/core/unit_test.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.529205 omniply-0.3/omniply/spaces/
--rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:57:26.000000 omniply-0.3/omniply/spaces/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:58:04.000000 omniply-0.3/omniply/spaces/imports.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.525205 omniply-0.3/omniply.egg-info/
--rw-r--r--   0 fleeb     (7343) is        (1040)      516 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/PKG-INFO
--rw-r--r--   0 fleeb     (7343) is        (1040)      961 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/SOURCES.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)        1 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/dependency_links.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)       15 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/requires.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)        8 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/top_level.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)      428 2024-04-06 12:19:43.529205 omniply-0.3/setup.cfg
--rw-r--r--   0 fleeb     (7343) is        (1040)       38 2024-02-14 16:25:24.000000 omniply-0.3/setup.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1067 2024-02-14 16:25:24.000000 omniply-0.3.1/LICENSE
+-rw-r--r--   0 fleeb     (7343) is        (1040)      518 2024-04-08 10:10:00.592860 omniply-0.3.1/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)      216 2024-02-14 16:25:24.000000 omniply-0.3.1/README.md
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/
+-rw-r--r--   0 fleeb     (7343) is        (1040)       62 2024-04-08 10:09:14.000000 omniply-0.3.1/omniply/__init__.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/_future/
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/_future/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2501 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/_future/common.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4287 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/_future/specification.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3749 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/_future/wrappers.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/apps/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      225 2024-04-08 10:02:27.000000 omniply-0.3.1/omniply/apps/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8556 2024-04-08 10:08:53.000000 omniply-0.3.1/omniply/apps/decisions.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/apps/iterative/
+-rw-r--r--   0 fleeb     (7343) is        (1040)       25 2024-03-29 16:54:35.000000 omniply-0.3.1/omniply/apps/iterative/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1590 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/iterative/abstract.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      673 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/iterative/guru.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      189 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/iterative/imports.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      725 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/iterative/innovators.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1343 2024-03-29 16:54:35.000000 omniply-0.3.1/omniply/apps/iterative/moguls.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3633 2024-04-07 16:16:51.000000 omniply-0.3.1/omniply/apps/simple.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1362 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/staging.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1386 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/templating.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1884 2024-04-07 16:40:21.000000 omniply-0.3.1/omniply/apps/unit_test.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/core/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      172 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/core/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8828 2024-04-07 15:17:06.000000 omniply-0.3.1/omniply/core/abstract.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2050 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/core/errors.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6745 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/core/gadgets.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    11763 2024-04-07 15:55:23.000000 omniply-0.3.1/omniply/core/gaggles.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    11004 2024-04-07 15:24:29.000000 omniply-0.3.1/omniply/core/games.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8124 2024-04-07 15:24:29.000000 omniply-0.3.1/omniply/core/gates.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8770 2024-04-07 15:11:45.000000 omniply-0.3.1/omniply/core/genetics.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1353 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/core/gizmos.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5437 2024-04-07 15:24:29.000000 omniply-0.3.1/omniply/core/op.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     7138 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/core/tools.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    27492 2024-04-07 15:24:29.000000 omniply-0.3.1/omniply/core/unit_test.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/spaces/
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:57:26.000000 omniply-0.3.1/omniply/spaces/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:58:04.000000 omniply-0.3.1/omniply/spaces/imports.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply.egg-info/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      518 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1014 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/SOURCES.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        1 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/dependency_links.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)       15 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/requires.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        8 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/top_level.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)      428 2024-04-08 10:10:00.592860 omniply-0.3.1/setup.cfg
+-rw-r--r--   0 fleeb     (7343) is        (1040)       38 2024-02-14 16:25:24.000000 omniply-0.3.1/setup.py
```

### Comparing `omniply-0.3/LICENSE` & `omniply-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omniply-0.3/PKG-INFO` & `omniply-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniply
-Version: 0.3
+Version: 0.3.1
 Summary: "Omni-ply Versatile Data Management for Rapid AI Prototyping and Research"
 Author: Felix Leeb
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `omniply-0.3/omniply/_future/common.py` & `omniply-0.3.1/omniply/_future/common.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3/omniply/_future/specification.py` & `omniply-0.3.1/omniply/_future/specification.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3/omniply/_future/wrappers.py` & `omniply-0.3.1/omniply/_future/wrappers.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3/omniply/apps/iterative/abstract.py` & `omniply-0.3.1/omniply/apps/iterative/abstract.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,66 +6,66 @@
 	def gadgetry(self) -> Iterator[AbstractGadget]:
 		raise NotImplementedError
 
 
 
 class AbstractGod:
 	'''source that can generate a stream of contexts given a base (mogul)'''
-	def grant(self, base: AbstractGuru | Iterable[AbstractGadget] = None) -> Iterator[AbstractGig]:
+	def grant(self, base: AbstractGuru | Iterable[AbstractGadget] = None) -> Iterator[AbstractGame]:
 		raise NotImplementedError
 
 
 
 class AbstractEvaluator(AbstractGuru):
 	def evaluate(self, src: AbstractGod) -> Any:
 		for ctx in src.grant(self):
 			yield self.eval_step(ctx)
 
 
-	def eval_step(self, ctx: AbstractGig) -> AbstractGig:
+	def eval_step(self, ctx: AbstractGame) -> AbstractGame:
 		raise NotImplementedError
 
 
 
 class AbstractTrainer(AbstractEvaluator):
 	def fit(self, src: AbstractGod) -> Any:
 		for ctx in src.grant(self):
 			yield self.learn(ctx)
 
 
-	def learn(self, ctx: AbstractGig) -> AbstractGig:
+	def learn(self, ctx: AbstractGame) -> AbstractGame:
 		'''single optimization step'''
 		raise NotImplementedError
 
 
 
 class AbstractGenie(AbstractGuru, AbstractGod):
-	def grant(self, base: 'AbstractGenius' = None) -> Iterator[AbstractGig]:
-		'''emits gigs from goals'''
+	def grant(self, base: 'AbstractGenius' = None) -> Iterator[AbstractGame]:
+		'''emits games from goals'''
 		if isinstance(base, AbstractGenius):
 			for goal in base.grant(base):
 				raise NotImplementedError
 		return super().grant(base)
 
 
 
 class AbstractGenius(AbstractGenie):
-	def grant(self, base: AbstractGod = None) -> Iterator[AbstractGig]:
-		'''emits goals for a genie to transform into gigs'''
+	def grant(self, base: AbstractGod = None) -> Iterator[AbstractGame]:
+		'''emits goals for a genie to transform into games'''
 		raise NotImplementedError
 
 
 
 
 
 class GeniusBase(AbstractGenius):
 	_Goal = None
 
 
-	def grant(self, base: AbstractGuru | Iterator[AbstractGadget] = None) -> Iterator[AbstractGig]:
+	def grant(self, base: AbstractGuru | Iterator[AbstractGadget] = None) -> Iterator[AbstractGame]:
 		goal = self._Goal(base)
 		for progress in sprint:
 			yield progress
 			if progress.grab('stop', False):
 				break
```

### Comparing `omniply-0.3/omniply/apps/iterative/guru.py` & `omniply-0.3.1/omniply/apps/iterative/guru.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .imports import *
 
 from .abstract import AbstractGuru, AbstractGod
 
 
 
 class GodBase(AbstractGod):
-	_Gift: Type[AbstractGig] = Context
+	_Gift: Type[AbstractGame] = Context
 
 
 	def _guide_sparks(self):
 		raise NotImplementedError
 
 
-	def grant(self, base: AbstractGuru | Iterable[AbstractGadget] = None) -> Iterator[AbstractGig]:
+	def grant(self, base: AbstractGuru | Iterable[AbstractGadget] = None) -> Iterator[AbstractGame]:
 		for spark in self._guide_sparks():
 			ctx = self._Gift(spark) if spark is not None else self._Gift()
 			if isinstance(self, AbstractGadget):
 				ctx.include(self)
 			if base is not None:
 				ctx.extend(base.gadgetry() if isinstance(base, AbstractGuru) else base)
 			yield ctx
```

### Comparing `omniply-0.3/omniply/apps/iterative/innovators.py` & `omniply-0.3.1/omniply/apps/iterative/innovators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .imports import *
 
 from .abstract import AbstractGuru, AbstractInnovator
 
 
 
 class InnovatorBase(AbstractInnovator):
-	_Innovation: Type[AbstractGig] = Context
+	_Innovation: Type[AbstractGame] = Context
 
 
 	def _generate_sparks(self):
 		raise NotImplementedError
 
 
-	def innovate(self, base: AbstractGuru | Iterator[AbstractGadget] = None) -> Iterator[AbstractGig]:
+	def innovate(self, base: AbstractGuru | Iterator[AbstractGadget] = None) -> Iterator[AbstractGame]:
 		for spark in self._generate_sparks():
 			ctx = self._Innovation(spark) if spark is not None else self._Innovation()
 			if isinstance(self, AbstractGadget):
 				ctx.include(self)
 			if base is not None:
 				ctx.extend(base.resources() if isinstance(base, AbstractGuru) else base)
 			yield ctx
```

### Comparing `omniply-0.3/omniply/apps/iterative/moguls.py` & `omniply-0.3.1/omniply/apps/iterative/moguls.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3/omniply/apps/simple.py` & `omniply-0.3.1/omniply/apps/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Iterator, Callable, Optional
 from collections import UserDict
 from omnibelt import filter_duplicates
 
 # from collections import frozenset
 
-from ..core import AbstractGig
+from ..core import AbstractGame
 from ..core.gadgets import GadgetBase
 from ..core.genetics import GeneticGadget
 
 
 class DictGadget(GeneticGadget):
 	def __init__(self, *srcs: dict, **data):
 		super().__init__()
@@ -32,19 +32,18 @@
 	def gizmos(self) -> Iterator[str]:
 		yield from filter_duplicates(self.data.keys(), *map(lambda x: x.keys(), self._srcs))
 
 
 	def _genetic_information(self, gizmo: str):
 		info = super()._genetic_information(gizmo)
 		info['parents'] = []
-		info['siblings'] = []
 		return info
 
 
-	def grab_from(self, ctx: 'AbstractGig', gizmo: str) -> Any:
+	def grab_from(self, ctx: 'AbstractGame', gizmo: str) -> Any:
 		return self[gizmo]
 
 
 
 class Table(GeneticGadget):
 	_index_gizmo = 'index'
 	_index_attribute = None
@@ -82,15 +81,15 @@
 
 	@property
 	def number_of_rows(self) -> int:
 		if self.is_loaded:
 			return len(self.data[self.columns[0]])
 
 
-	def grab_from(self, ctx: 'AbstractGig', gizmo: str) -> Any:
+	def grab_from(self, ctx: 'AbstractGame', gizmo: str) -> Any:
 		self.load()
 		index = ctx.grab(self._index_gizmo) if self._index_attribute is None else getattr(ctx, self._index_attribute)
 		return self.data[gizmo][index]
 
 
 	def gizmos(self) -> Iterator[str]:
 		self.load()
```

### Comparing `omniply-0.3/omniply/apps/staging.py` & `omniply-0.3.1/omniply/apps/staging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 
-from ..core import AbstractGadget, AbstractGig, AbstractGaggle
+from ..core import AbstractGadget, AbstractGame, AbstractGaggle
 from ..core.gaggles import GaggleBase
 from ..core.gadgets import AbstractGenetic
 
 
 
 # class AbstractSpaced(AbstractGadget):
-# 	def infer_space(self, ctx: AbstractGig, gizmo: str):
+# 	def infer_space(self, ctx: AbstractGame, gizmo: str):
 # 		raise NotImplementedError
 
 
 
 class AbstractPlan:
 	pass
 
@@ -65,15 +65,15 @@
 			raise self._AlreadyStagedError(f'{self} is already staged.')
 		return super().stage(plan)
 
 
 
 class StagedGaggle(GaggleBase, Staged):
 	def _stage(self, plan: AbstractPlan):
-		for gadget in self._vendors():
+		for gadget in self._gadgets():
 			if isinstance(gadget, Staged):
 				gadget.stage(plan)
 		return super()._stage(plan)
```

### Comparing `omniply-0.3/omniply/apps/templating.py` & `omniply-0.3.1/omniply/apps/templating.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Optional
 from omnibelt import pformat, pformat_vars, pathfinder
 
-from ..core import AbstractGig
+from ..core import AbstractGame
 from ..core.gadgets import SingleGadgetBase
 
 
 
 class Template(SingleGadgetBase):
 	def __init__(self, template: str, gizmo: str = None, **kwargs):
 		super().__init__(gizmo=gizmo, **kwargs)
@@ -28,15 +28,15 @@
 		return list(pformat_vars(template))
 
 
 	def fill_in(self, reqs: dict[str, str] = None, **vals: str):
 		return pformat(self.template, reqs, **vals)
 
 
-	def _grab_from(self, ctx: Optional[AbstractGig]) -> Any:
+	def _grab_from(self, ctx: Optional[AbstractGame]) -> Any:
 		reqs = {key: ctx.grab_from(ctx, key) for key in self.keys}
 		return self.fill_in(reqs)
 
 
 
 class FileTemplate(Template):
 	_find_template_path = pathfinder(default_suffix='txt', must_exist=True, validate=lambda p: p.is_file())
```

### Comparing `omniply-0.3/omniply/core/abstract.py` & `omniply-0.3.1/omniply/core/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,23 @@
 		This method must be overridden by subclasses to provide the actual implementation.
 
 		Returns:
 			Iterator[str]: An iterator over the known products of this tool.
 		"""
 		raise NotImplementedError
 
-	def grab_from(self, ctx: 'AbstractGig', gizmo: str) -> Any:
+	def grab_from(self, ctx: 'AbstractGame', gizmo: str) -> Any:
 		"""
 		Transforms the given context `ctx` to produce the specified `gizmo`, or raises ToolFailedError.
 		The context can be expected to contain all the necessary input gizmos.
 
 		This method should be overridden by subclasses to provide the actual implementation.
 
 		Args:
-			ctx (Optional['AbstractGig']): The context from which to grab any necessary input gizmos.
+			ctx (Optional['AbstractGame']): The context from which to grab any necessary input gizmos.
 			gizmo (str): The gizmo that must be produced.
 
 		Returns:
 			Any: The specified output gizmo.
 
 		Raises:
 			ToolFailedError: If the gizmo cannot be grabbed (possibly because a necessary input gizmo is missing).
@@ -172,27 +172,27 @@
 
 		Returns:
 			Iterator[AbstractGadget]: An iterator over the known gadgets that can directly produce the given gizmo.
 		"""
 		raise NotImplementedError
 
 
-_unique_gig_default_value = object()
+_unique_game_default_value = object()
 
 
 
-class AbstractGig(AbstractGaggle):
+class AbstractGame(AbstractGaggle):
 	"""
-	Gigs are usually the top-level interface for users to use the inference engine of `omni-ply`. Gigs are a special
+	Games are usually the top-level interface for users to use the inference engine of `omni-ply`. Games are a special
 	kind of gaggle that takes ownership of a `grab_from()` call, rather than (usually silently) delegating to an
-	appropriate gadget to produce the specified gizmo. This also means gigs are responsible providing the current
+	appropriate gadget to produce the specified gizmo. This also means games are responsible providing the current
 	context for gadgets (which often includes caching existing gizmos).
 	"""
 
-	def grab(self, gizmo: str, default: Any = _unique_gig_default_value):
+	def grab(self, gizmo: str, default: Any = _unique_game_default_value):
 		"""
 		Convenience function for grab_from to match dict.get API. It returns the given gizmo from this gadget,
 		or raises ToolFailedError if the gizmo cannot be grabbed and no default value is provided.
 
 		Args:
 			gizmo (str): The gizmo to grab.
 			default (Any): The default value to return if the gizmo cannot be grabbed. If not specified,
@@ -203,25 +203,25 @@
 
 		Raises:
 			AbstractGadgetError: If the gizmo cannot be grabbed and no default value is provided.
 		"""
 		try:
 			return self.grab_from(None, gizmo)
 		except AbstractGadgetError:
-			if default is _unique_gig_default_value:
+			if default is _unique_game_default_value:
 				raise
 			return default
 
 
-class AbstractGang(AbstractGig):
+class AbstractGate(AbstractGame):
 	"""
-	Gangs are a special kind of gig that relabels gizmos. It behaves a bit like a local/internal scope
+	Gates are a special kind of game that relabels gizmos. It behaves a bit like a local/internal scope
 	for its sub-gadgets, and can default to the global/external scope if necessary.
 
-	This class must be typically subclassed to create a specific type of gang.
+	This class must be typically subclassed to create a specific type of gate.
 	"""
 
 	def gizmo_from(self, gizmo: str) -> str:
 		"""
 		Converts external gizmo names to internal gizmo names used by sub-gadgets.
 
 		This method must be overridden by subclasses to provide the actual implementation.
@@ -249,17 +249,22 @@
 		raise NotImplementedError
 
 
 
 ### exotic animals
 
 
+class AbstractGenerous(AbstractGame):
+	def gabel(self):
+		'''duplicates this game, all the tools should be included, but not the cache'''
+		raise NotImplementedError
+
 
 
-class AbstractConsistentGig(AbstractGig):
+class AbstractConsistentGame(AbstractGame):
 	def is_unchanged(self, gizmo: str):
 		raise NotImplementedError
 
 
 	def update_gadget_cache(self, gadget: AbstractGadget, cache: dict[str,Any] = None):
 		raise NotImplementedError
```

### Comparing `omniply-0.3/omniply/core/errors.py` & `omniply-0.3.1/omniply/core/errors.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3/omniply/core/gadgets.py` & `omniply-0.3.1/omniply/core/gadgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterator, Optional, Any, Iterable, Callable
 from omnibelt import extract_function_signature, extract_missing_args
 from omnibelt.crafts import AbstractSkill, NestableCraft
 
 from .errors import GadgetFailure, MissingGadget
-from .abstract import AbstractGadget, AbstractGaggle, AbstractGig
+from .abstract import AbstractGadget, AbstractGaggle, AbstractGame
 
 
 class GadgetBase(AbstractGadget):
 	"""
 	GadgetBase is a simple base class that adds two kinds of internal exceptions for gadgets to raise or catch as
 	needed.
 
@@ -45,33 +45,33 @@
 
 		Returns:
 			Iterator[str]: An iterator over the gizmo that this gadget grabs.
 		"""
 		yield self._gizmo
 
 
-	def _grab_from(self, ctx: AbstractGig):
+	def _grab_from(self, ctx: AbstractGame):
 		"""
 		Grabs the gizmo from the given context. This method is called by grab_from.
 
 		Args:
-			ctx (AbstractGig): The context from which to grab the gizmo.
+			ctx (AbstractGame): The context from which to grab the gizmo.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
 		raise NotImplementedError
 
 
-	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def grab_from(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		"""
 		Returns the given gizmo from this gadget, or raises MissingGadgetError if the gizmo cannot be grabbed.
 
 		Args:
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
+			ctx (Optional[AbstractGame]): The context from which to grab the gizmo.
 			gizmo (str): The gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 
 		Raises:
 			MissingGadgetError: If the wrong gizmo is requested.
@@ -87,15 +87,15 @@
 	The function should take a single argument, the context (gig), and return the output gizmo.
 
 	Attributes:
 		_gizmo (str): The gizmo that this gadget grabs.
 		_fn (Callable[[AbstractGig], Any]): The function that this gadget uses to grab the gizmo.
 	"""
 
-	def __init__(self, gizmo: str, fn: Callable[[AbstractGig], Any], **kwargs):
+	def __init__(self, gizmo: str, fn: Callable[[AbstractGame], Any], **kwargs):
 		"""
 		Initializes a new instance of the FunctionGadget class.
 
 		Args:
 			gizmo (str): The gizmo that this gadget produces.
 			fn (Callable[[AbstractGig], Any]): The function that this gadget uses to produce the gizmo.
 			**kwargs: Arbitrary keyword arguments for superclasses.
@@ -136,20 +136,20 @@
 
 		Returns:
 			Callable[[AbstractGig], Any]: The function that this gadget uses to grab the gizmo.
 		"""
 		return self._fn.__get__(instance, owner)
 
 
-	def _grab_from(self, ctx: AbstractGig) -> Any:
+	def _grab_from(self, ctx: AbstractGame) -> Any:
 		"""
 		Grabs the gizmo from the given context. This method is called by grab_from.
 
 		Args:
-			ctx (AbstractGig): The context from which to grab the gizmo.
+			ctx (AbstractGame): The context from which to grab the gizmo.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
 		return self._fn(ctx)
 
 
@@ -163,39 +163,39 @@
 	Attributes:
 		_gizmo (str): The gizmo that this gadget grabs.
 		_fn (Callable[tuple, Any]): The function that this gadget uses to grab the gizmo.
 	"""
 
 
 	@staticmethod
-	def _extract_gizmo_args(fn: Callable, ctx: AbstractGig, *, args: Optional[tuple] = None,
+	def _extract_gizmo_args(fn: Callable, ctx: AbstractGame, *, args: Optional[tuple] = None,
 							kwargs: Optional[dict[str, Any]] = None) -> tuple[list[Any], dict[str, Any]]:
 		"""
 		Extracts the arguments for the function that this gadget uses to grab the gizmo. Any arguments that are gizmos
 		are grabbed from the gig.
 
 		Args:
 			fn (Callable): The function that this gadget uses to produce the gizmo.
-			ctx (AbstractGig): The context from which to grab any arguments needed by fn.
+			ctx (AbstractGame): The context from which to grab any arguments needed by fn.
 			args (Optional[tuple]): The positional arguments for the function passed in manually.
 			kwargs (Optional[dict[str, Any]]): The keyword arguments for the function passed in manually.
 
 		Returns:
 			tuple[list[Any], dict[str, Any]]: A tuple containing a list of positional arguments and a dictionary
 			of keyword arguments.
 		"""
 		return extract_function_signature(fn, args=args, kwargs=kwargs, default_fn=ctx.grab)
 
 
-	def _grab_from(self, ctx: AbstractGig) -> Any:
+	def _grab_from(self, ctx: AbstractGame) -> Any:
 		"""
 		Grabs the gizmo from the given context. This method is called by grab_from.
 
 		Args:
-			ctx (AbstractGig): The context from which to grab the gizmo.
+			ctx (AbstractGame): The context from which to grab the gizmo.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
 		args, kwargs = self._extract_gizmo_args(self._fn, ctx)
 		return self._fn(*args, **kwargs)
 
@@ -204,15 +204,15 @@
 class FunctionGadget(SingleGadgetBase):
 	'''the function is expected to be MISO'''
 	def __init__(self, fn: Callable = None, **kwargs):
 		super().__init__(**kwargs)
 		self._fn = fn
 
 
-	def _grab_from(self, ctx: 'AbstractGig') -> Any:
+	def _grab_from(self, ctx: 'AbstractGame') -> Any:
 		return self._fn(ctx)
 
 
 	@property
 	def __call__(self):
 		return self._fn
```

### Comparing `omniply-0.3/omniply/core/gaggles.py` & `omniply-0.3.1/omniply/core/gaggles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Any, Iterator, TypeVar, Generic, Union, Callable, Iterable, Mapping, Sequence, Self
 from itertools import chain
 from collections import OrderedDict
 from omnibelt import filter_duplicates
 from omnibelt.crafts import InheritableCrafty
 
-from .abstract import AbstractGadget, AbstractGaggle, AbstractGig
+from .abstract import AbstractGadget, AbstractGaggle, AbstractGame
 from .errors import logger, GadgetFailure, MissingGadget, AssemblyError
 from .gadgets import GadgetBase, SingleGadgetBase, SingleFunctionGadget, AutoSingleFunctionGadget
 
 
 
 class GaggleBase(GadgetBase, AbstractGaggle):
 	"""
@@ -20,28 +20,28 @@
 
 	Attributes:
 		_gadgets_table (dict[str, list[AbstractGadget]]): A dictionary where keys are gadget names and values are lists
 		of subgadgets.
 	"""
 
 	_gadgets_table: dict[str, list[AbstractGadget]]
+	_gadgets_list: list[AbstractGadget]
 
-	def __init__(self, *args, gadgets_table: Optional[Mapping] = None, **kwargs):
+	def __init__(self, *args, **kwargs):
 		"""
 		Initializes a new instance of the GaggleBase class.
 
 		Args:
 			args: unused
 			gadgets_table (Optional[Mapping]): A dictionary of gadgets. If not provided, defauls to an empty dictionary.
 			kwargs: Arbitrary keyword arguments.
 		"""
-		if gadgets_table is None:
-			gadgets_table = {}
 		super().__init__(*args, **kwargs)
-		self._gadgets_table = gadgets_table
+		self._gadgets_table = {}
+		self._gadgets_list = []
 
 	def gizmos(self) -> Iterator[str]:
 		"""
 		Iterates over all known gizmos that this gaggle can produce in order of oldest to newest.
 		"""
 		yield from self._gadgets_table.keys()
 
@@ -77,46 +77,56 @@
 		Args:
 			gizmo (Optional[str]): The name of the gizmo to check. If not provided, all gadgets are returned.
 
 		Returns:
 			Iterator[AbstractGadget]: An iterator over the gadgets that can produce the given gizmo.
 		"""
 		if gizmo is None:
-			for gadget in chain.from_iterable(map(reversed, self._gadgets_table.values())):
-				if isinstance(gadget, AbstractGaggle):
-					yield from gadget.vendors(gizmo)
-				else:
-					yield gadget
+			yield from reversed(self._gadgets_list)
 		else:
 			if gizmo not in self._gadgets_table:
 				raise self._MissingGadgetError(gizmo)
-			for gadget in reversed(self._gadgets_table[gizmo]):
-				if isinstance(gadget, AbstractGaggle):
-					yield from gadget.vendors(gizmo)
-				else:
-					yield gadget
+			yield from reversed(self._gadgets_table[gizmo])
+
+
+	def _gadgets(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
+		"""
+		Private method that returns all known subgadgets that can produce the given gizmo.
+
+		Args:
+			gizmo (Optional[str]): The name of the gizmo to check. If not provided, all gadgets are returned.
+
+		Returns:
+			Iterator[AbstractGadget]: An iterator over the gadgets that can produce the given gizmo.
+		"""
+		for vendor in self._vendors(gizmo):
+			if isinstance(vendor, AbstractGaggle):
+				yield from vendor.gadgets(gizmo)
+			else:
+				yield vendor
+
 
 	_AssemblyFailedError = AssemblyError
-	def grab_from(self, ctx: AbstractGig, gizmo: str) -> Any:
+	def grab_from(self, ctx: AbstractGame, gizmo: str) -> Any:
 		"""
 		Tries to grab a gizmo using the subgadgets given the context.
 
 		Args:
-			ctx (AbstractGig): The context with which to grab the gizmo.
+			ctx (AbstractGame): The context with which to grab the gizmo.
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 
 		Raises:
 			AssemblyFailedError: If all subgadgets fail to produce the gizmo.
 			MissingGadgetError: If no gadget can produce the gizmo.
 		"""
 		failures = OrderedDict()
-		for gadget in self._vendors(gizmo):
+		for gadget in self._gadgets(gizmo):
 			try:
 				return gadget.grab_from(ctx, gizmo)
 			except self._GadgetFailure as e:
 				failures[e] = gadget
 			except:
 				logger.debug(f'{gadget!r} failed while trying to produce {gizmo!r}')
 				raise
@@ -186,31 +196,31 @@
 		Args:
 			args: unused, passed to super.
 			kwargs: unused, passed to super.
 		"""
 		super().__init__(*args, **kwargs)
 		self._grabber_stack = {}
 
-	def grab_from(self, ctx: 'AbstractGig', gizmo: str) -> Any:
+	def grab_from(self, ctx: 'AbstractGame', gizmo: str) -> Any:
 		"""
 		Tries to grab a gizmo from the context using the gadgets in the _grabber_stack dictionary.
 
 		Args:
-			ctx (AbstractGig): The context with which to grab the gizmo.
+			ctx (AbstractGame): The context with which to grab the gizmo.
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 
 		Raises:
 			AssemblyFailedError: If all gadgets fail to produce the gizmo.
 			MissingGadgetError: If no gadget can produce the gizmo.
 		"""
 		failures = OrderedDict()
-		itr = self._grabber_stack.setdefault(gizmo, self._vendors(gizmo))
+		itr = self._grabber_stack.setdefault(gizmo, self._gadgets(gizmo))
 		for gadget in itr:
 			try:
 				out = gadget.grab_from(ctx, gizmo)
 			except self._GadgetFailure as e:
 				failures[e] = gadget
 			except:
 				logger.debug(f'{gadget!r} failed while trying to produce {gizmo!r}')
@@ -250,14 +260,15 @@
 
 		Args:
 			gadgets (Iterable[AbstractGadget]): The gadgets to be added.
 
 		Returns:
 			Self: this gaggle.
 		"""
+		self._gadgets_list.extend(reversed(gadgets))
 		new = {}
 		for gadget in gadgets:
 			for gizmo in gadget.gizmos():
 				new.setdefault(gizmo, []).append(gadget)
 		for gizmo, gadgets in new.items():
 			if gizmo in self._gadgets_table:
 				for gadget in gadgets:
@@ -276,14 +287,16 @@
 		Returns:
 			Self: this gaggle.
 		"""
 		for gadget in gadgets:
 			for gizmo in gadget.gizmos():
 				if gizmo in self._gadgets_table and gadget in self._gadgets_table[gizmo]:
 					self._gadgets_table[gizmo].remove(gadget)
+			if gadget in self._gadget_list:
+				self._gadgets_list.remove(gadget)
 		return self
 
 class CraftyGaggle(GaggleBase, InheritableCrafty):
 	"""
 	The CraftyGaggle class is a mix-in for custom gaggles to handle crafts such as `tool`.
 
 	Note that in order to procuess and add all found crafts, a subclass must call `_process_crafts()`, which is not
@@ -294,27 +307,28 @@
 		"""
 		Identifies all crafts contained in the class (including super classes) that are gadgets and adds those as
 		subgadgets, in the order in which they are defined.
 
 		Note that, in order to be processed correctly, the crafts should produce skills which are instances of
 		`AbstractGadget`.
 		"""
-		# group by where the craft is defined
+		# gate by where the craft is defined
 		history = OrderedDict() # src<N-O> : craft<N-O>
 		for src, key, craft in self._emit_all_craft_items(): # craft<N-O>
 			history.setdefault(src, []).append(craft)
 
 		# convert crafts to skills and add in O-N (N-O) order to table
 		for crafts in reversed(history.values()): # O-N
 			gizmos = {}
 			for craft in reversed(crafts): # N-O (in order of precedence)
 				skill = craft.as_skill(self) # TODO: convert as_skill to a generator to enable multiple skills per craft
 				if isinstance(skill, AbstractGadget):
 					for gizmo in skill.gizmos():
 						gizmos.setdefault(gizmo, []).append(skill)
+					self._gadgets_list.append(skill) # O-N (in order of appearance)
 				else:
 					self._process_auxiliary_skill(skill)
 			for gizmo, skills in gizmos.items():
 				self._gadgets_table.setdefault(gizmo, []).extend(reversed(skills)) # O-N (in order of appearance)
 
 
 	def _process_auxiliary_skill(self, skill):
```

### Comparing `omniply-0.3/omniply/core/gangs.py` & `omniply-0.3.1/omniply/core/gates.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from typing import Any, Optional, Iterator
 from collections import UserDict
 from omnibelt import filter_duplicates
 
-from .abstract import AbstractGang, AbstractGig
+from .abstract import AbstractGate, AbstractGame
 from .errors import GadgetFailure, ApplicationAmbiguityError
 from .gaggles import GaggleBase, MultiGadgetBase
-from .gigs import GigBase, GroupCache
+from .games import GameBase, GatedCache
 
 
-class GroupBase(MultiGadgetBase, GaggleBase, AbstractGang):
+class GateBase(MultiGadgetBase, GaggleBase, AbstractGate):
 	"""
-	The GroupBase class is a subclass of GaggleBase and AbstractGroup. It provides methods to handle gizmo grabbing and packaging.
+	The GateBase class is a subclass of GaggleBase and AbstractGate. It provides methods to handle gizmo grabbing and packaging.
 
 	Attributes:
-		_current_context (Optional[AbstractGig]): The current context of the group.
+		_current_context (Optional[AbstractGame]): The current context of the gate.
 	"""
 
-	_current_context: Optional[AbstractGig]
+	_current_context: Optional[AbstractGame]
 
 	def __init__(self, *args, gap: Optional[dict[str, str]] = None, **kwargs):
 		"""
-		Initializes a new instance of the GroupBase class.
+		Initializes a new instance of the GateBase class.
 
 		Args:
 			args: Variable length argument list.
 			gap (Optional[dict[str, str]]): A dictionary of gizmo mappings. If not provided, an empty dictionary will be used.
 			kwargs: Arbitrary keyword arguments.
 		"""
 		if gap is None:
 			gap = {}
 		super().__init__(*args, **kwargs)
 		self._raw_gap = gap # internal gizmos -> external gizmos
 		self._raw_reverse_gap = None
-		self._gig_stack = []
+		self._game_stack = []
 
 	def _gizmos(self) -> Iterator[str]:
 		"""
 		Lists gizmos produced by self using internal names.
 
 		Returns:
 			Iterator[str]: An iterator over the gizmos.
@@ -139,121 +139,121 @@
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
 		return super().grab_from(self, gizmo)
 
-	def grab_from(self, ctx: AbstractGig, gizmo: str) -> Any:
+	def grab_from(self, ctx: AbstractGame, gizmo: str) -> Any:
 		"""
 		Tries to grab a gizmo from the context.
 
 		Args:
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
+			ctx (Optional[AbstractGame]): The context from which to grab the gizmo.
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
 		if ctx is not None and ctx is not self:
-			self._gig_stack.append(ctx)
+			self._game_stack.append(ctx)
 			gizmo = self.gizmo_from(gizmo)  # convert to internal gizmo
 
 		try:
 			out = self._grab(gizmo)
 		except self._GadgetFailure:
-			if len(self._gig_stack) == 0 or ctx is self._gig_stack[-1]:
+			if len(self._game_stack) == 0 or ctx is self._game_stack[-1]:
 				raise
 			# default to parent/s
-			out = self._gig_stack[-1].grab(self.gizmo_to(gizmo))
+			out = self._game_stack[-1].grab(self.gizmo_to(gizmo))
 
-		if len(self._gig_stack) and ctx is self._gig_stack[-1]:
-			self._gig_stack.pop()
+		if len(self._game_stack) and ctx is self._game_stack[-1]:
+			self._game_stack.pop()
 
 		return out
 
-	# def _grab_from_fallback(self, error: Exception, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	# def _grab_from_fallback(self, error: Exception, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 	# 	assert ctx is self, f'{ctx} != {self}'
-	# 	if len(self._gig_stack):
-	# 		return super()._grab_from_fallback(error, self._gig_stack[-1], self.gizmo_to(gizmo))
+	# 	if len(self._game_stack):
+	# 		return super()._grab_from_fallback(error, self._game_stack[-1], self.gizmo_to(gizmo))
 	# 	raise error from error
 	#
 	#
-	# def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	# def grab_from(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 	# 	if ctx is not None and ctx is not self:
-	# 		self._gig_stack.append(ctx)
+	# 		self._game_stack.append(ctx)
 	# 		gizmo = self.gizmo_from(gizmo) # convert to internal gizmo
 	# 	out = super().grab_from(self, gizmo)
-	# 	if len(self._gig_stack) and ctx is self._gig_stack[-1]:
-	# 		self._gig_stack.pop()
+	# 	if len(self._game_stack) and ctx is self._game_stack[-1]:
+	# 		self._game_stack.pop()
 	# 	return out
 
 
-class CachableGroup(GroupBase):
+class CachableGate(GateBase):
 	"""
-	The CachableGroup class is a subclass of GroupBase. It provides methods to handle gizmo grabbing with cache support.
+	The CachableGate class is a subclass of GateBase. It provides methods to handle gizmo grabbing with cache support.
 
 	Attributes:
-		_GroupCacheMiss (KeyError): The exception to be raised when a cache miss occurs.
+		_GateCacheMiss (KeyError): The exception to be raised when a cache miss occurs.
 	"""
 
-	_GroupCacheMiss = KeyError
+	_GateCacheMiss = KeyError
 
 	def _grab(self, gizmo: str) -> Any:
 		"""
-		Tries to grab a gizmo from the group. If the gizmo is not found in the group's cache, it checks the cache using
-		the external gizmo name. If it still can't be found in any cache, it grabs it from the group's gadgets.
+		Tries to grab a gizmo from the gate. If the gizmo is not found in the gate's cache, it checks the cache using
+		the external gizmo name. If it still can't be found in any cache, it grabs it from the gate's gadgets.
 
 		Args:
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
-		if len(self._gig_stack):
+		if len(self._game_stack):
 			# check cache (if one exists)
-			for parent in reversed(self._gig_stack):
-				if isinstance(parent, GroupCache):
+			for parent in reversed(self._game_stack):
+				if isinstance(parent, GatedCache):
 					try:
-						return parent.check_group_cache(self, gizmo)
-					except self._GroupCacheMiss:
+						return parent.check_gate_cache(self, gizmo)
+					except self._GateCacheMiss:
 						pass
 
 			# if it can't be found in my cache, check the cache using the external gizmo name
 			ext = self.gizmo_to(gizmo)
-			for parent in reversed(self._gig_stack):
-				if isinstance(parent, GroupCache) and parent.is_cached(ext):
+			for parent in reversed(self._game_stack):
+				if isinstance(parent, GatedCache) and parent.is_cached(ext):
 					return parent.grab(ext)
 
 		# if it can't be found in any cache, grab it from my gadgets
 		out = super()._grab(gizmo)
 
 		# update my cache
-		if len(self._gig_stack):
-			for parent in reversed(self._gig_stack):
-				if isinstance(parent, GroupCache):
-					parent.update_group_cache(self, gizmo, out)
+		if len(self._game_stack):
+			for parent in reversed(self._game_stack):
+				if isinstance(parent, GatedCache):
+					parent.update_gate_cache(self, gizmo, out)
 					break
 
 		return out
 
 
-class SelectiveGroup(GroupBase):
+class SelectiveGate(GateBase):
 	"""
-	The SelectiveGroup class is a subclass of GroupBase. It provides methods to handle selective gizmo mapping.
+	The SelectiveGate class is a subclass of GateBase. It provides methods to handle selective gizmo mapping.
 
 	Args:
 		args: Variable length argument list.
 		gap (dict[str, str] | list[str] | None): A dictionary or list of gizmo mappings. If not provided, an empty dictionary will be used.
 		kwargs: Arbitrary keyword arguments.
 	"""
 
 	def __init__(self, *args, gap: dict[str, str] | list[str] | None = None, **kwargs):
 		"""
-		Initializes a new instance of the SelectiveGroup class.
+		Initializes a new instance of the SelectiveGate class.
 
 		If the gap argument is a list, it is converted to a dictionary with the same keys and values.
 		If the gap argument is a dictionary, it is processed to ensure that all values are not None.
 
 		Args:
 			args: Variable length argument list.
 			gap (dict[str, str] | list[str] | None): A dictionary or list of gizmo mappings. If not provided, an empty dictionary will be used.
```

### Comparing `omniply-0.3/omniply/core/genetics.py` & `omniply-0.3.1/omniply/core/genetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterator, Callable, Optional, Any, Iterable
 import inspect
 from functools import cache, cached_property
 from omnibelt import extract_missing_args
 from omnibelt.crafts import NestableCraft, AbstractCrafty
 
 from .errors import GrabError
-from .abstract import AbstractConsistentGig, AbstractGig, AbstractGadget, AbstractGaggle
+from .abstract import AbstractConsistentGame, AbstractGame, AbstractGadget, AbstractGaggle
 from .gadgets import FunctionGadget, GadgetBase
 from .gaggles import GaggleBase
 
 
 # from .gaggles import CraftyGaggle
 # from .tools import SkillBase, CraftBase
 
@@ -127,15 +127,15 @@
 class GeneticGadget(GeneticBase, GadgetBase):
 	pass
 
 
 
 class GeneticGaggle(GaggleBase, AbstractGenetic):
 	def genes(self, gizmo: str) -> AbstractGene:
-		for vendor in self._vendors(gizmo):
+		for vendor in self._gadgets(gizmo):
 			if isinstance(vendor, AbstractGenetic):
 				yield from vendor.genes(gizmo)
 
 
 
 class AutoFunctionGadget(FunctionGadget, AbstractGenetic):
 	def __init__(self, fn: Callable = None, gizmo: str = None, arg_map: dict[str, str] = None, **kwargs):
@@ -152,23 +152,23 @@
 		return extract_missing_args(fn, args=args, kwargs=kwargs, skip_first=isinstance(fn, classmethod))
 
 	_Gene = Gene
 	def genes(self, gizmo: str) -> Iterator[AbstractGene]:
 		parents = [self._arg_map.get(param.name, param.name) for param in self._extract_missing_genes()]
 		yield self._Gene(gizmo, self, parents=tuple(parents), endpoint=self._fn)
 
-	def _find_missing_gene(self, ctx: 'AbstractGig', param: inspect.Parameter) -> dict[str, Any]:
+	def _find_missing_gene(self, ctx: 'AbstractGame', param: inspect.Parameter) -> dict[str, Any]:
 		try:
 			return ctx.grab(self._arg_map.get(param.name, param.name))
 		except GrabError:
 			if param.default == param.empty:
 				raise
 			return param.default
 
-	def _grab_from(self, ctx: 'AbstractGig') -> Any:
+	def _grab_from(self, ctx: 'AbstractGame') -> Any:
 		# conditions = {param.name: self._find_missing_gene(ctx, param) for param in self._extract_missing_genes()}
 		conditions = {}
 		genes = self._extract_missing_genes()
 		for param in genes:
 			conditions[param.name] = self._find_missing_gene(ctx, param)
 		return self._fn(**conditions)
 
@@ -191,17 +191,17 @@
 
 	# @cache # TODO: does this matter for performance?
 	def _multi_output_order(self, gizmo: str = None):
 		if isinstance(self._gizmo, tuple):
 			return self._gizmo
 
 
-	def _grab_from_multi_output(self, ctx: Optional[AbstractGig], gizmo: str) -> dict[str, Any]:
-		if not isinstance(ctx, AbstractConsistentGig):
-			raise TypeError(f'Cannot use MIMOFunctionGadget with non-consistent gig')
+	def _grab_from_multi_output(self, ctx: Optional[AbstractGame], gizmo: str) -> dict[str, Any]:
+		if not isinstance(ctx, AbstractConsistentGame):
+			raise TypeError(f'Cannot use MIMOFunctionGadget with non-consistent game')
 
 		reqs = list(next(self.genes(gizmo)).parents)
 
 		if all(ctx.is_unchanged(gene) for gene in reqs):
 			cache = ctx.check_gadget_cache(self)
 			if gizmo in cache:
 				return cache[gizmo]
@@ -219,15 +219,15 @@
 		assert all(g in out for g in order), (f'Expected MIMO function to return dict with keys '
 													f'{order}, got {out.keys()}')
 
 		ctx.update_gadget_cache(self, out)
 		return out[gizmo]
 
 
-	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def grab_from(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		if self._multi_output_order(gizmo) is None:
 			return super().grab_from(ctx, gizmo)
 		return self._grab_from_multi_output(ctx, gizmo)
 
 
 	def gizmos(self) -> Iterator[str]:
 		if self._multi_output_order() is None:
```

### Comparing `omniply-0.3/omniply/core/gigs.py` & `omniply-0.3.1/omniply/core/games.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from typing import Any, Optional, Iterator, Self, Iterable
 from collections import UserDict
 from omnibelt import filter_duplicates
 
-from .abstract import (AbstractGadget, AbstractGaggle, AbstractGig, AbstractGang, AbstractGadgetError,
-					   AbstractConsistentGig)
+from .abstract import (AbstractGadget, AbstractGaggle, AbstractGame, AbstractGate, AbstractGadgetError,
+					   AbstractConsistentGame)
 from .errors import GadgetFailure, MissingGadget, AssemblyError, GrabError
 from .gadgets import GadgetBase
-from .gaggles import MutableGaggle, MultiGadgetBase
+from .gaggles import GaggleBase, MutableGaggle, MultiGadgetBase
 
 
-class GigBase(MultiGadgetBase, GadgetBase, AbstractGig):
+class GameBase(MultiGadgetBase, GadgetBase, AbstractGame):
 	"""
-	The GigBase class is a subclass of GadgetBase and AbstractGig. It provides methods to handle gizmo grabbing and packaging.
+	The GameBase class is a subclass of GadgetBase and AbstractGame. It provides methods to handle gizmo grabbing and packaging.
 
 	Attributes:
 		_GrabError (Exception): The exception to be raised when a grab operation fails.
 	"""
 
 	_GrabError = GrabError
 
-	def _grab_from_fallback(self, error: Exception, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def _grab_from_fallback(self, error: Exception, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		"""
 		Handles a GadgetFailure when trying to grab a gizmo from the context.
 
 		Args:
 			error (Exception): The exception that occurred during the grab operation.
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
+			ctx (Optional[AbstractGame]): The context from which to grab the gizmo.
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The result of the fallback operation.
 
 		Raises:
 			_GrabError: If the error is a GrabError or if the context is None or self.
@@ -50,20 +50,20 @@
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
 		return super().grab_from(self, gizmo)
 
-	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def grab_from(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		"""
 		Tries to grab a gizmo from the context.
 
 		Args:
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
+			ctx (Optional[AbstractGame]): The context from which to grab the gizmo.
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
 		try:
 			out = self._grab(gizmo)
@@ -81,17 +81,17 @@
 
 		Returns:
 			Any: The packaged value.
 		"""
 		return val
 
 
-class CacheGig(GigBase, UserDict):
+class CacheGame(GameBase, UserDict):
 	"""
-	The CacheGig class is a subclass of GigBase and UserDict. It provides methods to handle gizmo caching.
+	The CacheGame class is a subclass of GameBase and UserDict. It provides methods to handle gizmo caching.
 
 	Attributes:
 		_gizmo_type (Optional[type]): The type of the gizmo. Defaults to None.
 	"""
 
 	_gizmo_type = None
 
@@ -116,18 +116,18 @@
 			val (Any): The value of the gizmo to add.
 		"""
 		self.data[gizmo] = val
 		return self
 
 	def __repr__(self):
 		"""
-		Returns a string representation of the CacheGig instance.
+		Returns a string representation of the CacheGame instance.
 
 		Returns:
-			str: A string representation of the CacheGig instance.
+			str: A string representation of the CacheGame instance.
 		"""
 		gizmos = [(gizmo if self.is_cached(gizmo) else '{' + str(gizmo) + '}') for gizmo in self.gizmos()]
 		return f'{self.__class__.__name__}({", ".join(gizmos)})'
 
 	def gizmos(self) -> Iterator[str]:
 		"""
 		Lists gizmos produced by self.
@@ -162,139 +162,140 @@
 	def clear_cache(self) -> Self:
 		"""
 		Clears the cache.
 		"""
 		self.data.clear()
 		return self
 
-	def _cache_miss(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def _cache_miss(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		"""
 		Handles a cache miss.
 
 		Args:
 			gizmo (str): The name of the gizmo that was not found in the cache.
 
 		Raises:
 			AssemblyError: Always.
 		"""
 		return super().grab_from(ctx, gizmo)
 
-	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def grab_from(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		"""
 		Tries to grab a gizmo from the context.
 
 		Args:
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
+			ctx (Optional[AbstractGame]): The context from which to grab the gizmo.
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 		"""
 		if gizmo in self.data:
 			return self.data[gizmo]
 		val = self._cache_miss(ctx, gizmo)
 		self[gizmo] = val  # cache packaged val
 		return val
 
 
-class GroupCache(CacheGig):
+
+class GatedCache(CacheGame):
 	"""
-	The GroupCache class is a subclass of CacheGig. It provides methods to handle gizmo caching with group support.
+	The GatedCache class is a subclass of CacheGame. It provides methods to handle gizmo caching with support for gates.
 
 	Attributes:
-		_group_cache (dict): A dictionary to store group caches.
+		_gate_cache (dict): A dictionary to store gate caches.
 	"""
 
-	def __init__(self, *args, group_cache=None, **kwargs):
+	def __init__(self, *args, gate_cache=None, **kwargs):
 		"""
-		Initializes a new instance of the GroupCache class.
+		Initializes a new instance of the GateCache class.
 
 		Args:
 			args: Variable length argument list.
-			group_cache (Optional[dict]): A dictionary of group caches. If not provided, an empty dictionary will be used.
+			gate_cache (Optional[dict]): A dictionary of gate caches. If not provided, an empty dictionary will be used.
 			kwargs: Arbitrary keyword arguments.
 		"""
-		if group_cache is None:
-			group_cache = {}
+		if gate_cache is None:
+			gate_cache = {}
 		super().__init__(*args, **kwargs)
-		self._group_cache = group_cache
+		self._gate_cache = gate_cache
 
 	def is_cached(self, gizmo: str) -> bool:
 		"""
-		Checks if a gizmo is cached in either the main cache or any of the group caches.
+		Checks if a gizmo is cached in either the main cache or any of the gate caches.
 
 		Args:
 			gizmo (str): The name of the gizmo to check.
 
 		Returns:
 			bool: True if the gizmo is cached, False otherwise.
 		"""
 		if super().is_cached(gizmo):
 			return True
-		for group, cache in self._group_cache.items():
+		for gate, cache in self._gate_cache.items():
 			for key in cache:
-				if group.gizmo_to(key) == gizmo:
+				if gate.gizmo_to(key) == gizmo:
 					return True
 		return False
 
 	def cached(self) -> Iterator[str]:
 		"""
-		Lists the cached gizmos in both the main cache and the group caches.
+		Lists the cached gizmos in both the main cache and the gate caches.
 
 		Returns:
 			Iterator[str]: An iterator over the cached gizmos.
 		"""
-		def _group_cached():
-			for group, cache in self._group_cache.items():
+		def _gate_cached():
+			for gate, cache in self._gate_cache.items():
 				for key in cache:
-					yield group.gizmo_to(key)
-		yield from filter_duplicates(super().cached(), _group_cached())
+					yield gate.gizmo_to(key)
+		yield from filter_duplicates(super().cached(), _gate_cached())
 
-	def check_group_cache(self, group: AbstractGang, gizmo: str):
+	def check_gate_cache(self, gate: AbstractGate, gizmo: str):
 		"""
-		Checks a group cache for a gizmo.
+		Checks a gate cache for a gizmo.
 
 		Args:
-			group (AbstractGroup): The group to check.
+			gate (AbstractGate): The gate to check.
 			gizmo (str): The name of the gizmo to check.
 
 		Returns:
-			Any: The cached value of the gizmo in the group cache.
+			Any: The cached value of the gizmo in the gate cache.
 		"""
-		return self._group_cache[group][gizmo]
+		return self._gate_cache[gate][gizmo]
 
-	def update_group_cache(self, group: AbstractGang, gizmo: str, val: Any):
+	def update_gate_cache(self, gate: AbstractGate, gizmo: str, val: Any):
 		"""
-		Updates a group cache with a gizmo and its value.
+		Updates a gate cache with a gizmo and its value.
 
 		Args:
-			group (AbstractGroup): The group to update.
+			gate (AbstractGate): The gate to update.
 			gizmo (str): The name of the gizmo to update.
 			val (Any): The value of the gizmo to update.
 		"""
 		if self._gizmo_type is not None:
 			gizmo = self._gizmo_type(gizmo)
-		self._group_cache.setdefault(group, {})[gizmo] = val
+		self._gate_cache.setdefault(gate, {})[gizmo] = val
 
-	def clear_cache(self, *, clear_group_caches=True, **kwargs) -> None:
+	def clear_cache(self, *, clear_gate_caches=True, **kwargs) -> None:
 		"""
-		Clears the cache and optionally the group caches.
+		Clears the cache and optionally the gate caches.
 
 		Args:
-			clear_group_caches (bool): Whether to clear the group caches. Defaults to True.
+			clear_gate_caches (bool): Whether to clear the gate caches. Defaults to True.
 		"""
 		super().clear_cache(**kwargs)
-		if clear_group_caches:
-			self._group_cache.clear()
+		if clear_gate_caches:
+			self._gate_cache.clear()
 
 
 
-class TraceGig(CacheGig):
+class TraceGame(CacheGame):
 	"""
-	The TraceGig class is a subclass of CacheGig. It provides methods to handle gizmo caching with trace support.
+	The TraceGame class is a subclass of CacheGame. It provides methods to handle gizmo caching with trace support.
 	"""
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self._history = {} # gizmo -> list of gizmos that were created as a result
 		self._products = {} # gizmo -> list of gizmos that used it
 		self._partial_grabs = []
 
@@ -310,34 +311,34 @@
 		'''remove any cached gizmo that depends on the given gizmo'''
 		self.data.pop(gizmo, None)
 		for dep in self._products.pop(gizmo, []):
 			# self.data.pop(dep, None)
 			self.purge(dep)
 		return self
 
-	def _cache_miss(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def _cache_miss(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		self._partial_grabs.append(gizmo)
 		try:
 			val = super()._cache_miss(ctx, gizmo)
 		finally:
 			self._partial_grabs.pop()
 
 		if len(self._partial_grabs):
 			self._history.setdefault(self._partial_grabs[-1], set()).add(gizmo)
 		return val
 
-	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def grab_from(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		val = super().grab_from(ctx, gizmo)
 		if len(self._partial_grabs):
 			self._products.setdefault(gizmo, set()).add(self._partial_grabs[-1])
 		return val
 
 
 
-class RollingGig(TraceGig, MutableGaggle):
+class RollingGame(TraceGame, MutableGaggle):
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self._rolling_stock = {} # gizmo -> list of gadgets that were included during the gizmos creation
 
 
 	def rollback(self, gizmo: str):
 		'''remove any cached gizmo that depends on the given gizmo'''
@@ -357,15 +358,15 @@
 			for gadget in gadgets:
 				if gadget in known:
 					known.remove(gadget)
 		return super().exclude(*gadgets)
 
 
 
-class ConsistentGig(TraceGig, AbstractConsistentGig):
+class ConsistentGame(TraceGame, AbstractConsistentGame):
 	'''can handle gadgets with multiple outputs (provided those gadgets are deterministic wrt their inputs)'''
 
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self._gadget_precomputes: dict[AbstractGadget,dict[str,Any]] = {} # gadget -> outputs that were already computed (only relevant for gadgets with multiple outputs)
 
 	def clear_cache(self, *, clear_gadget_cache: bool = True, **kwargs) -> None:
```

### Comparing `omniply-0.3/omniply/core/gizmos.py` & `omniply-0.3.1/omniply/core/gizmos.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3/omniply/core/op.py` & `omniply-0.3.1/omniply/core/op.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable, Callable
-from .abstract import AbstractGadget, AbstractGaggle, AbstractGig, AbstractGang
+from .abstract import AbstractGadget, AbstractGaggle, AbstractGame, AbstractGate, AbstractGenerous
 from .errors import GadgetFailure, MissingGadget
 from .tools import ToolCraftBase, AutoToolCraft, MIMOToolDecorator, AutoToolDecorator
 from .gizmos import DashGizmo
 from .gaggles import MutableGaggle, LoopyGaggle, CraftyGaggle
-from .gigs import CacheGig, GroupCache, TraceGig, RollingGig, ConsistentGig
-from .gangs import GroupBase, CachableGroup, SelectiveGroup
+from .games import CacheGame, GatedCache, TraceGame, RollingGame, ConsistentGame
+from .gates import GateBase, CachableGate, SelectiveGate
 from .genetics import GeneticGaggle
 
 
 
 class tool(AutoToolDecorator):
 	"""
 	The tool class is a subclass of AutoToolDecorator. It provides a convenient way to create tool instances
@@ -59,17 +59,18 @@
 			args: Variable length argument list.
 			kwargs: Arbitrary keyword arguments.
 		"""
 		super().__init__(*args, **kwargs)
 		self._process_crafts()
 
 
-class Context(GroupCache, ConsistentGig, RollingGig, LoopyGaggle, MutableGaggle, GeneticGaggle, AbstractGig):
+class Context(GatedCache, ConsistentGame, RollingGame, LoopyGaggle, MutableGaggle, GeneticGaggle,
+			  AbstractGenerous, AbstractGame):
 	"""
-	The Context class is a subclass of GroupCache, LoopyGaggle, MutableGaggle, and AbstractGig. It provides methods to handle
+	The Context class is a subclass of GateCache, LoopyGaggle, MutableGaggle, and AbstractGame. It provides methods to handle
 	gadgets in a context.
 
 	Methods:
 		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Context class.
 		__getitem__(self, item): Returns the grabbed item from the context.
 	"""
 
@@ -84,30 +85,36 @@
 		Args:
 			gadgets (AbstractGadget): The gadgets to be included in the context.
 			kwargs: Arbitrary keyword arguments.
 		"""
 		super().__init__(**kwargs)
 		self.include(*gadgets)
 
+
+	def gabel(self):
+		'''effectively a shallow copy, excluding the cache'''
+		return self.__class__(*self._vendors())
+
+
 	def __getitem__(self, item):
 		"""
 		Returns the grabbed item from the context.
 
 		Args:
 			item: The item to be grabbed from the context.
 
 		Returns:
 			Any: The grabbed item from the context.
 		"""
 		return self.grab(item)
 
 
-class Scope(CachableGroup, LoopyGaggle, MutableGaggle, AbstractGang):
+class Scope(CachableGate, LoopyGaggle, MutableGaggle, AbstractGate):
 	"""
-	The Scope class is a subclass of CachableGroup, LoopyGaggle, MutableGaggle, and AbstractGang. It provides methods
+	The Scope class is a subclass of CachableGate, LoopyGaggle, MutableGaggle, and AbstractGate. It provides methods
 	to handle gadgets in a scope.
 
 	Methods:
 		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Scope class.
 	"""
 
 	def __init__(self, *gadgets: AbstractGadget, **kwargs):
@@ -131,17 +138,17 @@
 			item: The item to be grabbed from the context.
 
 		Returns:
 			Any: The grabbed item from the context.
 		"""
 		return self.grab(item)
 
-class Selection(SelectiveGroup, Scope):
+class Selection(SelectiveGate, Scope):
 	"""
-	The Selection class is a subclass of SelectiveGroup and Scope. It provides methods to handle selective gizmo mapping
+	The Selection class is a subclass of SelectiveGate and Scope. It provides methods to handle selective gizmo mapping
 	within a scope.
 
 	Methods:
 		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Selection class.
 	"""
 
 	def __init__(self, *gadgets: AbstractGadget, **kwargs):
```

### Comparing `omniply-0.3/omniply/core/tools.py` & `omniply-0.3.1/omniply/core/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Iterator, Optional, Any, Iterable, Callable
 from omnibelt.crafts import AbstractSkill, AbstractCraft, AbstractCrafty, NestableCraft
 
-from .abstract import AbstractGadget, AbstractGaggle, AbstractGig
+from .abstract import AbstractGadget, AbstractGaggle, AbstractGame
 from .gadgets import GadgetBase, FunctionGadget
 from .genetics import AutoMIMOFunctionGadget, MIMOGadgetBase, Parentable, AbstractGenetic, Gene, ParentedSkill
 
 
 
 class SkillBase(AbstractSkill):
 	def __init__(self, *, unbound_fn: Callable, base: Optional[AbstractCraft] = None, **kwargs):
@@ -145,20 +145,20 @@
 			gizmo (str): The name of the gizmo to check.
 
 		Returns:
 			bool: True if the gizmo can be grabbed, False otherwise.
 		"""
 		return gizmo == self._gizmo
 
-	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	def grab_from(self, ctx: Optional[AbstractGame], gizmo: str) -> Any:
 		"""
 		Tries to grab a gizmo from the context.
 
 		Args:
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
+			ctx (Optional[AbstractGame]): The context from which to grab the gizmo.
 			gizmo (str): The name of the gizmo to grab.
 
 		Returns:
 			Any: The grabbed gizmo.
 
 		Raises:
 			_GadgetFailed: If the gizmo cannot be grabbed.
```

### Comparing `omniply-0.3/omniply/core/unit_test.py` & `omniply-0.3.1/omniply/core/unit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,15 @@
 	# Asserts that the context correctly maps 'x' to 'y'.
 	assert list(ctx.gizmos()) == ['x', 'y']
 
 	# Asserts that the context correctly maps 'y' to 2.
 	assert ctx['y'] == 2
 
 
-def test_group_cache():
+def test_gate_cache():
 	"""
 	This function tests the functionality of the 'tool' decorator, the 'Context' class, the 'Scope' class, and the '_Kit1' instance.
 
 	The 'tool' decorator is used to define two functions, 'f' and 'g', with 'a' and 'x' as their respective gizmos.
 	The 'Context' class is used to create a context with the functions 'f' and 'g'.
 	The 'Scope' class is used to create a scope with the functions 'f' and 'g' and a gizmo mapping from 'a' to 'b'.
 	The 'clear_cache' method is then used to clear the context's cache.
```

### Comparing `omniply-0.3/omniply.egg-info/PKG-INFO` & `omniply-0.3.1/omniply.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniply
-Version: 0.3
+Version: 0.3.1
 Summary: "Omni-ply Versatile Data Management for Rapid AI Prototyping and Research"
 Author: Felix Leeb
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `omniply-0.3/omniply.egg-info/SOURCES.txt` & `omniply-0.3.1/omniply.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 omniply.egg-info/requires.txt
 omniply.egg-info/top_level.txt
 omniply/_future/__init__.py
 omniply/_future/common.py
 omniply/_future/specification.py
 omniply/_future/wrappers.py
 omniply/apps/__init__.py
+omniply/apps/decisions.py
 omniply/apps/simple.py
 omniply/apps/staging.py
 omniply/apps/templating.py
+omniply/apps/unit_test.py
 omniply/apps/iterative/__init__.py
 omniply/apps/iterative/abstract.py
 omniply/apps/iterative/guru.py
 omniply/apps/iterative/imports.py
 omniply/apps/iterative/innovators.py
 omniply/apps/iterative/moguls.py
 omniply/core/__init__.py
 omniply/core/abstract.py
 omniply/core/errors.py
 omniply/core/gadgets.py
 omniply/core/gaggles.py
-omniply/core/gangs.py
+omniply/core/games.py
+omniply/core/gates.py
 omniply/core/genetics.py
-omniply/core/gigs.py
 omniply/core/gizmos.py
 omniply/core/op.py
 omniply/core/tools.py
 omniply/core/unit_test.py
 omniply/spaces/__init__.py
 omniply/spaces/imports.py
```

