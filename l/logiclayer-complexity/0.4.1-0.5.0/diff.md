# Comparing `tmp/logiclayer_complexity-0.4.1.tar.gz` & `tmp/logiclayer_complexity-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logiclayer_complexity-0.4.1.tar", max compression
+gzip compressed data, was "logiclayer_complexity-0.5.0.tar", max compression
```

## Comparing `logiclayer_complexity-0.4.1.tar` & `logiclayer_complexity-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1093 2022-08-10 00:34:08.071136 logiclayer_complexity-0.4.1/LICENSE
--rw-r--r--   0        0        0      225 2023-03-24 16:22:43.492174 logiclayer_complexity-0.4.1/logiclayer_complexity/__init__.py
--rw-r--r--   0        0        0      201 2023-09-29 19:47:39.062338 logiclayer_complexity-0.4.1/logiclayer_complexity/__version__.py
--rw-r--r--   0        0        0     3136 2024-02-12 21:27:27.164005 logiclayer_complexity-0.4.1/logiclayer_complexity/common.py
--rw-r--r--   0        0        0      184 2023-12-07 21:31:37.974492 logiclayer_complexity-0.4.1/logiclayer_complexity/complexity/__init__.py
--rw-r--r--   0        0        0     3409 2024-02-09 22:30:54.554079 logiclayer_complexity-0.4.1/logiclayer_complexity/complexity/dependencies.py
--rw-r--r--   0        0        0     5552 2024-02-02 20:00:19.587245 logiclayer_complexity-0.4.1/logiclayer_complexity/complexity/structs.py
--rw-r--r--   0        0        0     4691 2024-02-09 00:04:22.385847 logiclayer_complexity-0.4.1/logiclayer_complexity/dependencies.py
--rw-r--r--   0        0        0    13737 2024-02-12 21:01:23.691388 logiclayer_complexity-0.4.1/logiclayer_complexity/module.py
--rw-r--r--   0        0        0     2912 2024-02-09 22:30:54.588648 logiclayer_complexity-0.4.1/logiclayer_complexity/opportunity_gain.py
--rw-r--r--   0        0        0     4520 2024-02-12 20:17:13.863911 logiclayer_complexity-0.4.1/logiclayer_complexity/peii.py
--rw-r--r--   0        0        0     4257 2024-02-12 20:17:52.249890 logiclayer_complexity-0.4.1/logiclayer_complexity/pgi.py
--rw-r--r--   0        0        0      134 2023-12-07 21:02:11.815737 logiclayer_complexity-0.4.1/logiclayer_complexity/rca/__init__.py
--rw-r--r--   0        0        0     6425 2024-02-09 19:43:15.189094 logiclayer_complexity-0.4.1/logiclayer_complexity/rca/dependencies.py
--rw-r--r--   0        0        0     6103 2024-02-09 00:01:19.725946 logiclayer_complexity-0.4.1/logiclayer_complexity/rca/structs.py
--rw-r--r--   0        0        0      359 2024-02-02 19:36:49.968808 logiclayer_complexity-0.4.1/logiclayer_complexity/relatedness/__init__.py
--rw-r--r--   0        0        0     2705 2024-02-09 22:30:54.589330 logiclayer_complexity-0.4.1/logiclayer_complexity/relatedness/dependencies.py
--rw-r--r--   0        0        0     4124 2024-02-02 21:19:27.228036 logiclayer_complexity-0.4.1/logiclayer_complexity/relatedness/structs.py
--rw-r--r--   0        0        0     2435 2024-01-31 15:18:46.516787 logiclayer_complexity-0.4.1/logiclayer_complexity/wdi.py
--rw-r--r--   0        0        0     1658 2022-08-10 00:46:00.273578 logiclayer_complexity-0.4.1/PACKAGE.md
--rw-r--r--   0        0        0     1014 2024-02-12 21:33:30.499853 logiclayer_complexity-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 logiclayer_complexity-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2022-08-10 00:34:08.071136 logiclayer_complexity-0.5.0/LICENSE
+-rw-r--r--   0        0        0      292 2024-04-08 21:02:29.621542 logiclayer_complexity-0.5.0/logiclayer_complexity/__init__.py
+-rw-r--r--   0        0        0     1686 2024-04-08 19:52:31.149383 logiclayer_complexity-0.5.0/logiclayer_complexity/common.py
+-rw-r--r--   0        0        0      184 2023-12-07 21:31:37.974492 logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/__init__.py
+-rw-r--r--   0        0        0     3409 2024-02-09 22:30:54.554079 logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/dependencies.py
+-rw-r--r--   0        0        0     5576 2024-04-08 20:57:25.893205 logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/structs.py
+-rw-r--r--   0        0        0     4721 2024-02-27 19:14:50.359214 logiclayer_complexity-0.5.0/logiclayer_complexity/dependencies.py
+-rw-r--r--   0        0        0    15938 2024-04-08 20:30:18.639653 logiclayer_complexity-0.5.0/logiclayer_complexity/module.py
+-rw-r--r--   0        0        0     2912 2024-02-09 22:30:54.588648 logiclayer_complexity-0.5.0/logiclayer_complexity/opportunity_gain.py
+-rw-r--r--   0        0        0      279 2024-04-03 16:43:40.886690 logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/__init__.py
+-rw-r--r--   0        0        0     4565 2024-04-08 18:59:34.649911 logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/peii.py
+-rw-r--r--   0        0        0     4302 2024-04-08 18:59:50.506445 logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/pgi.py
+-rw-r--r--   0        0        0      134 2023-12-07 21:02:11.815737 logiclayer_complexity-0.5.0/logiclayer_complexity/rca/__init__.py
+-rw-r--r--   0        0        0     6425 2024-02-09 19:43:15.189094 logiclayer_complexity-0.5.0/logiclayer_complexity/rca/dependencies.py
+-rw-r--r--   0        0        0     6105 2024-03-25 19:51:09.834805 logiclayer_complexity-0.5.0/logiclayer_complexity/rca/structs.py
+-rw-r--r--   0        0        0      359 2024-02-02 19:36:49.968808 logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/__init__.py
+-rw-r--r--   0        0        0     2705 2024-02-09 22:30:54.589330 logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/dependencies.py
+-rw-r--r--   0        0        0     4124 2024-02-02 21:19:27.228036 logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/structs.py
+-rw-r--r--   0        0        0     3040 2024-04-08 19:17:16.727139 logiclayer_complexity-0.5.0/logiclayer_complexity/response.py
+-rw-r--r--   0        0        0     2660 2024-04-08 19:17:07.621358 logiclayer_complexity-0.5.0/logiclayer_complexity/wdi.py
+-rw-r--r--   0        0        0     1658 2022-08-10 00:46:00.273578 logiclayer_complexity-0.5.0/PACKAGE.md
+-rw-r--r--   0        0        0     1078 2024-04-08 21:02:20.533797 logiclayer_complexity-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 logiclayer_complexity-0.5.0/PKG-INFO
```

### Comparing `logiclayer_complexity-0.4.1/LICENSE` & `logiclayer_complexity-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/complexity/dependencies.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/dependencies.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/complexity/structs.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         cmplx = self._calculate(rca, kind)
 
         df_cmplx = cmplx.reset_index(name=name)
 
         col_id: str = df_pivot.index.name if kind == "ECI" else df_pivot.columns.name
         if col_id.endswith(" ID") and col_id[:-3] in df.columns:
             col = col_id[:-3]
-            df_index = df[[col_id, col]].set_index(col_id)
+            df_index = df.loc[:, [col_id, col]].set_index(col_id)
             dict_index = df_index[col].to_dict()
             df_cmplx.insert(0, col, df_cmplx[col_id].map(dict_index))
 
         if sort_ascending is not None:
             df_cmplx.sort_values(by=name, ascending=sort_ascending, inplace=True)
 
         if sort_ascending is not None or self.rank:
@@ -122,15 +122,15 @@
         eci, pci = ec.complexity(ec.rca(tbl))
         df_pci = pd.DataFrame(pci).rename(columns={0: complexity_measure}).reset_index()
         df_pci = df_pci.merge(df_copy, on=activity_id)
 
         results = (
             df_pci[df_pci[rca_measure] >= 1]
             .groupby([complexity_dd_id])
-            .mean()
+            .mean(numeric_only=True)
             .reset_index()
         )
         results = results[[complexity_dd_id] + [complexity_measure]]
 
         return results
 
     def calculate(
```

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/dependencies.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from fastapi import HTTPException, Query
 from typing_extensions import Annotated
 
-from logiclayer_complexity.common import split_dict
+from logiclayer_complexity.common import VALID_COMPARISONS, split_dict
 
 
 def parse_alias(
     aliases: Annotated[
         List[str],
         Query(
             alias="alias",
@@ -102,27 +102,27 @@
 def parse_threshold_singleton(params: str):
     """Parses a threshold singleton from a string."""
     if ":" in params:
         comparison, value = params.split(":", maxsplit=1)
     else:
         comparison, value = "gte", params
 
-    if comparison not in ("lt", "lte", "gt", "gte", "eq", "neq"):
+    if comparison not in VALID_COMPARISONS:
         raise HTTPException(
             400,
-            f"Malformed 'threshold' parameter, '{comparison}' is not a valid "
-            "comparison identifier",
-        ) from None
+            f"Malformed 'threshold' parameter, '{comparison}' is not a valid comparison keyword. "
+            f"Accepted values are: {', '.join(VALID_COMPARISONS)}",
+        )
 
     try:
-        value = int(value)
+        value = float(value)
     except ValueError:
         raise HTTPException(
             400, f"Malformed 'threshold' parameter, '{value}' must be numeric"
-        ) from None
+        )
 
     return comparison, value
 
 
 def parse_threshold(
     threshold: Annotated[
         List[str],
@@ -137,13 +137,13 @@
     """Threshold dependency.
 
     Parses the threshold parameter into a dict of {Level: (Comparison, Value)}.
 
     The parameter is a list of strings, but each item is split by comma anyway
     to ensure compatibility with URLSearchParams of both formats:
     - `threshold[]=level1:gte:10&threshold[]=level2:lt:20`
-    - `threshold=level1:gte:10,level2:lt:20`
+    - `threshold=level1:gte:10;level2:lt:20`
     """
     return {
         level: parse_threshold_singleton(params)
-        for level, params in split_dict(threshold, ",")
+        for level, params in split_dict(threshold, ";")
     }
```

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/module.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/module.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,388 +1,416 @@
 """Economic Complexity adapter for use in LogicLayer.
 
 Contains a module to enable endpoints which return economic complexity
 calculations, using a Tesseract OLAP server as data source.
 """
 
-import asyncio
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, List, Mapping, Optional, Tuple
 
+import logiclayer as ll
 import pandas as pd
-from fastapi import Depends, Header, HTTPException, Request
-from fastapi.responses import RedirectResponse
-from logiclayer import LogicLayerModule, route
-from tesseract_olap import DataRequest, OlapServer
-from tesseract_olap.backend.exceptions import BackendError
-from tesseract_olap.query.exceptions import QueryError
+import polars as pl
+from fastapi import Depends, Header, HTTPException, Request, status
+from fastapi.responses import JSONResponse, RedirectResponse
+from tesseract_olap import DataRequest, OlapServer, PublicCube, PublicSchema
+from tesseract_olap.backend import Session
+from tesseract_olap.exceptions import QueryError, TesseractError
 from typing_extensions import Annotated
 
-from .__version__ import __title__, __version__
-from .common import ResponseFormat
+from . import __title__, __version__
 from .complexity import (
     ComplexityParameters,
     ComplexitySubnationalParameters,
     prepare_complexity_params,
     prepare_complexity_subnational_params,
 )
 from .dependencies import parse_alias, parse_filter
 from .opportunity_gain import OpportunityGainParameters, prepare_opportunity_gain_params
-from .peii import PEIIParameters, prepare_peii_params
-from .pgi import PGIParameters, prepare_pgi_params
+from .pmi import (
+    PEIIParameters,
+    PGIParameters,
+    prepare_peii_params,
+    prepare_pgi_params,
+)
 from .rca import (
     RcaParameters,
     RcaSubnationalParameters,
     prepare_rca_params,
     prepare_subnatrca_params,
 )
 from .relatedness import (
     RelatednessParameters,
     RelatednessSubnationalParameters,
     prepare_relatedness_params,
     prepare_relatedness_subnational_params,
 )
+from .response import ComplexityStatus, ResponseFormat
 from .wdi import WdiParameters, WdiReference, WdiReferenceSchema, parse_wdi
 
 
-class EconomicComplexityModule(LogicLayerModule):
+class EconomicComplexityModule(ll.LogicLayerModule):
     """Economic Complexity calculations module class for LogicLayer."""
 
-    server: "OlapServer"
+    olap: "OlapServer"
     wdi: Optional["WdiReference"]
 
     def __init__(
         self,
-        server: "OlapServer",
+        olap: "OlapServer",
         wdi: Optional["WdiReferenceSchema"] = None,
+        **kwargs,
     ):
         """Setups the server for this instance."""
         super().__init__()
 
-        if server is None:
+        if olap is None:
             raise ValueError(
                 "EconomicComplexityModule requires a tesseract_olap.OlapServer instance"
             )
 
-        self.server = server
+        self.debug = kwargs.get("debug", False)
+        self.olap = olap
         self.wdi = None if wdi is None else WdiReference(**wdi)
 
-    async def fetch_data(self, query: DataRequest):
+    def apply_threshold(
+        self,
+        session: Session,
+        df: pl.DataFrame,
+        *,
+        rca: RcaParameters,
+        wdi: List[WdiParameters] = [],
+    ) -> pd.DataFrame:
+        threshold_expr = [
+            *_yield_threshold_expr(df, rca.measure, rca.threshold),
+            *self._yield_wdi_threshold_expr(session, wdi),
+        ]
+        if len(threshold_expr) > 0:
+            df = df.filter(threshold_expr)
+        return df.to_pandas()
+
+    def _yield_wdi_threshold_expr(self, session: Session, params: List[WdiParameters]):
+        if not self.wdi or len(params) == 0:
+            return None
+
+        for item in params:
+            request = self.wdi.build_request(item)
+            data = self.fetch_data(session, request)
+            location = f"{self.wdi.get_level(item.location)} ID"
+            yield pl.col(location).is_in(data[location])
+
+    def fetch_data(self, session: Session, request: DataRequest):
         """Retrieves the data from the backend, and handles related errors."""
-        try:
-            res = await self.server.execute(query)
-        except QueryError as exc:
-            raise HTTPException(status_code=400, detail=exc.message) from None
-        except BackendError as exc:
-            raise HTTPException(status_code=500, detail=exc.message) from None
-
-        return pd.DataFrame([item async for item in res])
-
-    async def apply_wdi_threshold(
-        self,
-        df: pd.DataFrame,
-        wdi_params: WdiParameters,
-        location: str,
-    ):
-        if self.wdi is None:
-            raise HTTPException(500, "WDI reference is not configured")
-
-        wdi_location = self.wdi.level_mapper.get(location, location)
-        wdi_query = self.wdi.build_query(wdi_params, wdi_location)
-        wdi_data = await self.fetch_data(wdi_query)
-        wdi_members = wdi_data[f"{wdi_location} ID"].to_list()
-
-        # WDI works the same as threshold, but using remote data
-        data_to_drop = df.loc[~df[f"{location} ID"].isin(wdi_members)]
-        df.drop(data_to_drop.index, inplace=True)
-
-        del wdi_data, data_to_drop
-
-    @route("GET", "/")
-    def route_root(self):
-        return {
-            "module": __title__,
-            "version": __version__,
-            "wdi": "disabled" if self.wdi is None else "enabled",
-        }
+        query = self.olap.build_query(request)
+        result = session.fetch_dataframe(query)
+        return result.data
+
+    @ll.route("GET", "/")
+    def route_status(self) -> ComplexityStatus:
+        return ComplexityStatus(
+            module=__title__,
+            version=__version__,
+            debug=False,
+            extras={
+                "wdi": "disabled" if self.wdi is None else "enabled",
+            },
+        )
+
+    @ll.route("GET", "/cubes")
+    def route_schema(self, locale: Optional[str] = None) -> PublicSchema:
+        roles = []
+        locale = self.olap.schema.default_locale if locale is None else locale
+        return PublicSchema.from_entity(self.olap.schema, locale=locale, roles=roles)
+
+    @ll.route("GET", "/cubes/{cube_name}")
+    def route_schema_cube(self, cube_name: str, locale: Optional[str] = None):
+        roles = []
+        cube = self.olap.schema.get_cube(cube_name)
+        if not cube.is_authorized(roles):
+            raise HTTPException(
+                status.HTTP_403_FORBIDDEN,
+                "You don't have authorization to access this cube. "
+                "Check your credentials and try again.",
+            )
+        locale = self.olap.schema.default_locale if locale is None else locale
+        return PublicCube.from_entity(cube, locale=locale)
 
-    @route("GET", "/rca.{extension}")
-    async def route_rca(
+    @ll.route("GET", "/rca.{extension}")
+    def route_rca(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: RcaParameters = Depends(prepare_rca_params),
         wdi: List[WdiParameters] = Depends(parse_wdi),
     ):
         """RCA calculation endpoint."""
-        df = await self.fetch_data(params.request)
-
-        params.apply_threshold(df)
-        for item in wdi:
-            await self.apply_wdi_threshold(df, item, params.location)
+        with self.olap.session() as session:
+            df = self.fetch_data(session, params.request)
+            df = self.apply_threshold(session, df, rca=params, wdi=wdi)
 
         df_rca = params.calculate(df)
 
-        apply_filters(df_rca, filters)
-        apply_aliases(df_rca, aliases)
+        return extension.serialize(df_rca, aliases, filters)
 
-        return extension.serialize(df_rca)
-
-    @route("GET", "/eci.{extension}")
-    async def route_eci(
+    @ll.route("GET", "/eci.{extension}")
+    def route_eci(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: ComplexityParameters = Depends(prepare_complexity_params),
         wdi: List[WdiParameters] = Depends(parse_wdi),
     ):
         """ECI calculation endpoint."""
-        df = await self.fetch_data(params.request)
-
-        params.rca_params.apply_threshold(df)
-        for item in wdi:
-            await self.apply_wdi_threshold(df, item, params.rca_params.location)
+        with self.olap.session() as session:
+            df = self.fetch_data(session, params.request)
+            df = self.apply_threshold(session, df, rca=params.rca_params, wdi=wdi)
 
         df_eci = params.calculate(df, "ECI")
 
-        apply_filters(df_eci, filters)
-        apply_aliases(df_eci, aliases)
+        return extension.serialize(df_eci, aliases, filters)
 
-        return extension.serialize(df_eci)
-
-    @route("GET", "/pci.{extension}")
-    async def route_pci(
+    @ll.route("GET", "/pci.{extension}")
+    def route_pci(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: ComplexityParameters = Depends(prepare_complexity_params),
         wdi: List[WdiParameters] = Depends(parse_wdi),
     ):
         """PCI calculation endpoint."""
-        df = await self.fetch_data(params.request)
-
-        params.rca_params.apply_threshold(df)
-        for item in wdi:
-            await self.apply_wdi_threshold(df, item, params.rca_params.location)
+        with self.olap.session() as session:
+            df = self.fetch_data(session, params.request)
+            df = self.apply_threshold(session, df, rca=params.rca_params, wdi=wdi)
 
         df_pci = params.calculate(df, "PCI")
 
-        apply_filters(df_pci, filters)
-        apply_aliases(df_pci, aliases)
-
-        return extension.serialize(df_pci)
+        return extension.serialize(df_pci, aliases, filters)
 
-    @route("GET", "/relatedness.{extension}")
-    async def route_relatedness(
+    @ll.route("GET", "/relatedness.{extension}")
+    def route_relatedness(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: RelatednessParameters = Depends(prepare_relatedness_params),
     ):
         """Relatedness calculation endpoint."""
-        df = await self.fetch_data(params.request)
-
-        params.rca_params.apply_threshold(df)
+        with self.olap.session() as session:
+            df = self.fetch_data(session, params.request)
+            df = self.apply_threshold(session, df, rca=params.rca_params)
 
         df_reltd = params.calculate(df)
 
-        apply_filters(df_reltd, filters)
-        apply_aliases(df_reltd, aliases)
-
-        return extension.serialize(df_reltd)
+        return extension.serialize(df_reltd, aliases, filters)
 
-    @route("GET", "/opportunity_gain.{extension}")
-    async def route_opportunity_gain(
+    @ll.route("GET", "/opportunity_gain.{extension}")
+    def route_opportunity_gain(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: OpportunityGainParameters = Depends(prepare_opportunity_gain_params),
     ):
         """Opportunity Gain calculation endpoint."""
-        df = await self.fetch_data(params.request)
-
-        params.rca_params.apply_threshold(df)
+        with self.olap.session() as session:
+            df = self.fetch_data(session, params.request)
+            df = self.apply_threshold(session, df, rca=params.rca_params)
 
         df_opgain = params.calculate(df)
 
-        apply_filters(df_opgain, filters)
-        apply_aliases(df_opgain, aliases)
-
-        return extension.serialize(df_opgain)
+        return extension.serialize(df_opgain, aliases, filters)
 
-    @route("GET", "/pgi.{extension}")
-    async def route_pgi(
+    @ll.route("GET", "/pgi.{extension}")
+    def route_pgi(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: PGIParameters = Depends(prepare_pgi_params),
     ):
         """PGI calculation endpoint."""
-        df, df_gini = await asyncio.gather(
-            self.fetch_data(params.rca_params.request),
-            self.fetch_data(params.request),
-        )
-
-        params.rca_params.apply_threshold(df)
+        with self.olap.session() as session:
+            df = self.fetch_data(session, params.rca_params.request)
+            df = self.apply_threshold(session, df, rca=params.rca_params)
+            df_gini = self.fetch_data(session, params.request).to_pandas()
 
         df_pgi = params.calculate(df, df_gini)
 
-        apply_filters(df_pgi, filters)
-        apply_aliases(df_pgi, aliases)
+        return extension.serialize(df_pgi, aliases, filters)
 
-        return extension.serialize(df_pgi)
-
-    @route("GET", "/peii.{extension}")
-    async def route_peii(
+    @ll.route("GET", "/peii.{extension}")
+    def route_peii(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: PEIIParameters = Depends(prepare_peii_params),
     ):
         """PEII calculation endpoint."""
-        df, df_emissions = await asyncio.gather(
-            self.fetch_data(params.rca_params.request),
-            self.fetch_data(params.request),
-        )
-
-        params.rca_params.apply_threshold(df)
+        with self.olap.session() as session:
+            df = self.fetch_data(session, params.rca_params.request)
+            df = self.apply_threshold(session, df, rca=params.rca_params)
+            df_emissions = self.fetch_data(session, params.request).to_pandas()
 
         df_peii = params.calculate(df, df_emissions)
 
-        apply_filters(df_peii, filters)
-        apply_aliases(df_peii, aliases)
+        return extension.serialize(df_peii, aliases, filters)
 
-        return extension.serialize(df_peii)
-
-    @route("GET", "/rca_subnational.{extension}")
-    async def route_rca_subnational(
+    @ll.route("GET", "/rca_subnational.{extension}")
+    def route_rca_subnational(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: RcaSubnationalParameters = Depends(prepare_subnatrca_params),
     ):
-        df_subnat, df_global = await asyncio.gather(
-            self.fetch_data(params.subnat_params.request),
-            self.fetch_data(params.global_params.request),
-        )
+        with self.olap.session() as session:
+            df_subnat = self.fetch_data(
+                session, params.subnat_params.request
+            ).to_pandas()
+            df_global = self.fetch_data(
+                session, params.global_params.request
+            ).to_pandas()
 
         df_rca = params.calculate(df_subnat, df_global)
 
-        apply_filters(df_rca, filters)
-        apply_aliases(df_rca, aliases)
+        return extension.serialize(df_rca, aliases, filters)
 
-        return extension.serialize(df_rca)
-
-    @route("GET", "/eci_subnational.{extension}")
-    async def route_eci_subnational(
+    @ll.route("GET", "/eci_subnational.{extension}")
+    def route_eci_subnational(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: ComplexitySubnationalParameters = Depends(
             prepare_complexity_subnational_params
         ),
     ):
         """ECI calculation endpoint."""
-        df_subnat, df_global = await asyncio.gather(
-            self.fetch_data(params.rca_params.subnat_params.request),
-            self.fetch_data(params.rca_params.global_params.request),
-        )
+        with self.olap.session() as session:
+            df_subnat = self.fetch_data(
+                session, params.rca_params.subnat_params.request
+            ).to_pandas()
+            df_global = self.fetch_data(
+                session, params.rca_params.global_params.request
+            ).to_pandas()
 
         df_eci = params.calculate(df_subnat, df_global, "ECI")
 
-        apply_filters(df_eci, filters)
-        apply_aliases(df_eci, aliases)
+        return extension.serialize(df_eci, aliases, filters)
 
-        return extension.serialize(df_eci)
-
-    @route("GET", "/pci_subnational.{extension}")
-    async def route_pci_subnational(
+    @ll.route("GET", "/pci_subnational.{extension}")
+    def route_pci_subnational(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: ComplexitySubnationalParameters = Depends(
             prepare_complexity_subnational_params
         ),
     ):
         """PCI calculation endpoint."""
-        df_subnat, df_global = await asyncio.gather(
-            self.fetch_data(params.rca_params.subnat_params.request),
-            self.fetch_data(params.rca_params.global_params.request),
-        )
+        with self.olap.session() as session:
+            df_subnat = self.fetch_data(
+                session, params.rca_params.subnat_params.request
+            ).to_pandas()
+            df_global = self.fetch_data(
+                session, params.rca_params.global_params.request
+            ).to_pandas()
 
         df_pci = params.calculate(df_subnat, df_global, "PCI")
 
-        apply_filters(df_pci, filters)
-        apply_aliases(df_pci, aliases)
+        return extension.serialize(df_pci, aliases, filters)
 
-        return extension.serialize(df_pci)
-
-    @route("GET", "/relatedness_subnational.{extension}")
-    async def route_relatedness_subnational(
+    @ll.route("GET", "/relatedness_subnational.{extension}")
+    def route_relatedness_subnational(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: RelatednessSubnationalParameters = Depends(
             prepare_relatedness_subnational_params
         ),
     ):
         """Relatedness calculation endpoint."""
-        df_subnat, df_global = await asyncio.gather(
-            self.fetch_data(params.rca_params.subnat_params.request),
-            self.fetch_data(params.rca_params.global_params.request),
-        )
+        with self.olap.session() as session:
+            df_subnat = self.fetch_data(
+                session, params.rca_params.subnat_params.request
+            ).to_pandas()
+            df_global = self.fetch_data(
+                session, params.rca_params.global_params.request
+            ).to_pandas()
 
         df_reltd = params.calculate(df_subnat, df_global)
 
-        apply_filters(df_reltd, filters)
-        apply_aliases(df_reltd, aliases)
-
-        return extension.serialize(df_reltd)
+        return extension.serialize(df_reltd, aliases, filters)
 
-    @route("GET", "/{endpoint}", response_class=RedirectResponse)
+    @ll.route("GET", "/{endpoint}", response_class=RedirectResponse)
     def route_redirect(
         self,
         request: Request,
         endpoint: str,
         accept: Annotated[Optional[str], Header()] = None,
     ):
-        # TODO: check the endpoint exists; requires update in LogicLayerModule
+        if not any(path.startswith("/" + endpoint + ".") for path in self.route_paths):
+            raise HTTPException(404, "Not found")
+
         if accept is None or accept.startswith("*/*") or "text/csv" in accept:
-            fmt = ResponseFormat.csv
+            extension = ResponseFormat.csv
         elif "application/x-jsonarray" in accept:
-            fmt = ResponseFormat.jsonarrays
+            extension = ResponseFormat.jsonarrays
         elif "application/x-jsonrecords" in accept:
-            fmt = ResponseFormat.jsonrecords
+            extension = ResponseFormat.jsonrecords
         elif "text/tab-separated-values" in accept:
-            fmt = ResponseFormat.tsv
+            extension = ResponseFormat.tsv
         else:
-            raise HTTPException(
-                status_code=406,
-                detail=f"Requested invalid format: '{accept}'. Prefer an explicit format using a path with a filetype extension.",
-            )
+            message = f"Requested invalid format: '{accept}'. Prefer an explicit format using a path with a filetype extension."
+            raise HTTPException(status_code=406, detail=message)
 
         url = request.url
         path, endpoint = url.path.rsplit("/", maxsplit=1)
-        return f"{path}/{endpoint}.{fmt}?{url.query}"
-
+        return f"{path}/{endpoint}.{extension}?{url.query}"
 
-def apply_filters(df: pd.DataFrame, filters: Dict[str, Tuple[str, ...]]):
-    # filter which members will be sent in the response
-    for key, values in filters.items():
-        column_id = f"{key} ID"
-        dropping = df.loc[~df[column_id].isin(values)].index
-        df.drop(dropping, inplace=True)
-        del dropping
+    @ll.exception_handler(TesseractError)
+    def exc_tesseracterror(self, request: Request, exc: TesseractError):
+        if self.debug or isinstance(exc, QueryError):
+            content = {"error": True, "type": type(exc).__name__, "detail": exc.message}
+        else:
+            content = {"error": True, "detail": "Backend error"}
+        return JSONResponse(content, status_code=exc.code)
 
 
-def apply_aliases(df: pd.DataFrame, aliases: Dict[str, str]):
-    df.rename(columns=aliases, inplace=True)
+def condition_expr(measure: str, operator: str, value: float):
+    if operator == "lt":
+        return pl.col(measure) < value
+    elif operator == "lte":
+        return pl.col(measure) <= value
+    elif operator == "gt":
+        return pl.col(measure) > value
+    elif operator == "gte":
+        return pl.col(measure) >= value
+    elif operator == "eq":
+        return pl.col(measure) == value
+    else:
+        return pl.col(measure) != value
+
+
+def _yield_threshold_expr(
+    df: pl.DataFrame, measure: str, threshold: Mapping[str, Tuple[str, float]]
+):
+    for level, (operator, value) in threshold.items():
+        column = f"{level} ID"
+        # Group rows by `column` and get the sum of `measure`, then
+        # apply threshold condition and get `column` of rows that comply
+        keepids = (
+            df.lazy()
+            .select(column, measure)
+            .group_by(column)
+            .agg(pl.col(measure).sum())
+            .filter(condition_expr(measure, operator, value))
+            .select(column)
+            .collect()
+        )
+        # Yield Expr for this threshold instruction
+        yield pl.col(column).is_in(keepids[column])
```

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/opportunity_gain.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/opportunity_gain.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/peii.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/peii.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import economic_complexity as ec
 import pandas as pd
 from fastapi import Depends, Query
 from tesseract_olap import DataRequest, DataRequestParams
 from typing_extensions import Annotated
 
-from .rca import RcaParameters, prepare_rca_params
+from ..rca import RcaParameters, prepare_rca_params
 
 
 @dataclass
 class PEIIParameters:
     rca_params: RcaParameters
     emissions_cube: str
     emissions_measure: str
@@ -60,17 +60,18 @@
 
         rca = self.rca_params._calculate(df_pivot)
         peii = self._calculate(df_pivot, rca, emissions)
 
         # restore columns labels if needed
         if self.rca_params.activity_id in df.columns:
             activity_id = self.rca_params.activity_id
-            df_labels = df[[activity_id, self.rca_params.activity]]
+            df_labels = df.loc[:, [activity_id, self.rca_params.activity]]
             df_labels.drop_duplicates(subset=activity_id, inplace=True)
-            labels = df_labels.set_index(activity_id)[self.rca_params.activity]
+            df_labels.set_index(activity_id, inplace=True)
+            labels = df_labels[self.rca_params.activity]
 
             ds = pd.concat([labels, peii], axis=1).reset_index()
         else:
             ds = peii.reset_index()
 
         if sort_ascending is not None:
             ds.sort_values(by=name, ascending=sort_ascending, inplace=True)
```

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/pgi.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/pgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import economic_complexity as ec
 import pandas as pd
 from fastapi import Depends, Query
 from tesseract_olap import DataRequest, DataRequestParams
 from typing_extensions import Annotated
 
-from .rca import RcaParameters, prepare_rca_params
+from ..rca import RcaParameters, prepare_rca_params
 
 
 @dataclass
 class PGIParameters:
     rca_params: RcaParameters
     gini_cube: str
     gini_location: str
@@ -55,17 +55,18 @@
         df_pivot = self.rca_params.pivot(df)
 
         rca = self.rca_params._calculate(df_pivot)
         pgi = self._calculate(df_pivot, rca, gini)
 
         if self.rca_params.activity_id in df.columns:
             activity_id = self.rca_params.activity_id
-            df_labels = df[[activity_id, self.rca_params.activity]]
+            df_labels = df.loc[:, [activity_id, self.rca_params.activity]]
             df_labels.drop_duplicates(subset=activity_id, inplace=True)
-            labels = df_labels.set_index(activity_id)[self.rca_params.activity]
+            df_labels.set_index(activity_id, inplace=True)
+            labels = df_labels[self.rca_params.activity]
 
             ds = pd.concat([labels, pgi], axis=1).reset_index()
         else:
             ds = pgi.reset_index()
 
         if sort_ascending is not None:
             ds.sort_values(by=name, ascending=sort_ascending, inplace=True)
```

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/rca/dependencies.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/rca/dependencies.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/rca/structs.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/rca/structs.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     cube: str
     activity: str
     location: str
     measure: str
     cuts: Mapping[str, Tuple[str, ...]] = field(default_factory=dict)
     locale: Optional[str] = None
     parents: bool = False
-    threshold: Mapping[str, Tuple[str, int]] = field(default_factory=dict)
+    threshold: Mapping[str, Tuple[str, float]] = field(default_factory=dict)
 
     @property
     def activity_id(self):
         return self.activity + " ID"
 
     @property
     def location_id(self):
```

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/relatedness/dependencies.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/dependencies.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/relatedness/structs.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/structs.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.4.1/logiclayer_complexity/wdi.py` & `logiclayer_complexity-0.5.0/logiclayer_complexity/wdi.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,49 +4,56 @@
 from fastapi import HTTPException, Query
 from tesseract_olap import DataRequest
 from typing_extensions import Annotated, Required, TypedDict
 
 
 @dataclass
 class WdiParameters:
-    indicator: str
     year: List[int]
+    indicator: str
     comparison: str
     value: int
+    location: str
 
 
 class WdiReferenceSchema(TypedDict, total=False):
     cube: Required[str]
     measure: str
     level_mapper: Dict[str, str]
 
 
 @dataclass
 class WdiReference:
     cube: str
     measure: str = field(default="Measure")
     level_mapper: Dict[str, str] = field(default_factory=dict)
 
-    def build_query(self, params: WdiParameters, location: str):
+    def build_request(self, params: WdiParameters):
+        location = self.level_mapper.get(params.location, params.location)
+
         return DataRequest.new(
             self.cube,
             {
                 "drilldowns": [location],
                 "measures": [self.measure],
                 "cuts_include": {
                     "Indicator": [params.indicator],
                     "Year": [str(item) for item in params.year],
                 },
                 "filters": {self.measure: ((params.comparison, params.value),)},
                 "sorting": (self.measure, "desc"),
             },
         )
 
+    def get_level(self, name: str):
+        return self.level_mapper.get(name, name)
+
 
 def parse_wdi(
+    location: str,
     wdi: Annotated[
         List[str],
         Query(
             description="Applies an additional threshold over the data, using a parameter from the World Bank's WDI database."
         ),
     ] = [],
 ) -> List[WdiParameters]:
@@ -69,14 +76,15 @@
 
         if not value.isnumeric():
             raise HTTPException(
                 400, f"Malformed 'wdi' parameter, '{value}' must be numeric"
             )
 
         return WdiParameters(
-            indicator=indicator,
             year=[int(item) for item in year.split(",")],
+            indicator=indicator,
             comparison=comparison,
             value=int(value),
+            location=location,
         )
 
     return [parse_singleton(param) for token in wdi for param in token.split(",")]
```

### Comparing `logiclayer_complexity-0.4.1/PACKAGE.md` & `logiclayer_complexity-0.5.0/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.4.1/pyproject.toml` & `logiclayer_complexity-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "logiclayer-complexity"
-version = "0.4.1"
+version = "0.5.0"
 description = "LogicLayer module to enable Economic Complexity calculations, using data from a tesseract-olap server."
 authors = [
   "Francisco Abarzua <francisco@datawheel.us>",
   "Jelmy Hermosilla <jelmy@datawheel.us>",
   "Samuel Osorio <samuel@datawheel.us>",
   "Nicolás Netz <nicolas.netz@datawheel.us>",
 ]
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/logiclayer-complexity"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 economic-complexity = "^0.2.1"
-logiclayer = "^0.2.0"
+logiclayer = "^0.3.0"
+orjson = "^3.8.0"
 pandas = ">=1.5.0"
-tesseract-olap = ">=0.8.0"
+polars = "^0.20.0"
+pyarrow = "^15.0.0"
+tesseract-olap = ">=0.9.2"
 
 [tool.poetry.group.dev.dependencies]
+granian = {extras = ["reload"], version = "^1.2.0"}
 ipykernel = "^6.0.0"
 pandas = "^1.5.3"
 pyinstrument = "^4.6.1"
 pytest = "^7.2.0"
-pytest-asyncio = "^0.20.0"
-ruff = "^0.1.7"
+ruff = "^0.3.4"
 snakeviz = "^2.2.0"
-tesseract-olap = {version = "^0.8.0", extras = ["clickhouse"]}
-uvicorn = "^0.22.0"
+tesseract-olap = {version = "^0.9.2", extras = ["clickhouse"]}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `logiclayer_complexity-0.4.1/PKG-INFO` & `logiclayer_complexity-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: logiclayer-complexity
-Version: 0.4.1
+Version: 0.5.0
 Summary: LogicLayer module to enable Economic Complexity calculations, using data from a tesseract-olap server.
 Home-page: https://github.com/Datawheel/logiclayer-complexity
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: economic-complexity (>=0.2.1,<0.3.0)
-Requires-Dist: logiclayer (>=0.2.0,<0.3.0)
+Requires-Dist: logiclayer (>=0.3.0,<0.4.0)
+Requires-Dist: orjson (>=3.8.0,<4.0.0)
 Requires-Dist: pandas (>=1.5.0)
-Requires-Dist: tesseract-olap (>=0.8.0)
+Requires-Dist: polars (>=0.20.0,<0.21.0)
+Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
+Requires-Dist: tesseract-olap (>=0.9.2)
 Project-URL: Repository, https://github.com/Datawheel/logiclayer-complexity
 Description-Content-Type: text/markdown
 
 <p>
 <a href="https://github.com/Datawheel/logiclayer-complexity/releases"><img src="https://flat.badgen.net/github/release/Datawheel/logiclayer-complexity" /></a>
 <a href="https://github.com/Datawheel/logiclayer-complexity/blob/master/LICENSE"><img src="https://flat.badgen.net/github/license/Datawheel/logiclayer-complexity" /></a>
 <a href="https://github.com/Datawheel/logiclayer-complexity/"><img src="https://flat.badgen.net/github/checks/Datawheel/logiclayer-complexity" /></a>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: logiclayer-complexity Version: 0.4.1 Summary:
+Metadata-Version: 2.1 Name: logiclayer-complexity Version: 0.5.0 Summary:
 LogicLayer module to enable Economic Complexity calculations, using data from a
 tesseract-olap server. Home-page: https://github.com/Datawheel/logiclayer-
 complexity License: MIT Author: Francisco Abarzua Author-email:
 francisco@datawheel.us Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: economic-complexity (>=0.2.1,<0.3.0)
-Requires-Dist: logiclayer (>=0.2.0,<0.3.0) Requires-Dist: pandas (>=1.5.0)
-Requires-Dist: tesseract-olap (>=0.8.0) Project-URL: Repository, https://
-github.com/Datawheel/logiclayer-complexity Description-Content-Type: text/
-markdown
+Requires-Dist: logiclayer (>=0.3.0,<0.4.0) Requires-Dist: orjson
+(>=3.8.0,<4.0.0) Requires-Dist: pandas (>=1.5.0) Requires-Dist: polars
+(>=0.20.0,<0.21.0) Requires-Dist: pyarrow (>=15.0.0,<16.0.0) Requires-Dist:
+tesseract-olap (>=0.9.2) Project-URL: Repository, https://github.com/Datawheel/
+logiclayer-complexity Description-Content-Type: text/markdown
 _[_h_t_t_p_s_:_/_/_f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_D_a_t_a_w_h_e_e_l_/_l_o_g_i_c_l_a_y_e_r_-_c_o_m_p_l_e_x_i_t_y_]_[_h_t_t_p_s_:
 _/_/_f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_D_a_t_a_w_h_e_e_l_/_l_o_g_i_c_l_a_y_e_r_-_c_o_m_p_l_e_x_i_t_y_]_[_h_t_t_p_s_:_/_/
 _f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_c_h_e_c_k_s_/_D_a_t_a_w_h_e_e_l_/_l_o_g_i_c_l_a_y_e_r_-_c_o_m_p_l_e_x_i_t_y_]_[_h_t_t_p_s_:_/_/
 _f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_D_a_t_a_w_h_e_e_l_/_l_o_g_i_c_l_a_y_e_r_-_c_o_m_p_l_e_x_i_t_y_]
 ## Getting started This module must be used with LogicLayer. An instance of
 `OlapServer` from the `tesseract_olap` package is also required to retrieve the
 data. ```python # app.py from logiclayer import LogicLayer from
```

