# Comparing `tmp/openapi_service_client-0.0.2.tar.gz` & `tmp/openapi_service_client-0.0.3.tar.gz`

## Comparing `openapi_service_client-0.0.2.tar` & `openapi_service_client-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/__init__.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/auth_factory.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/client.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/config/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/config/auth_strategy.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/config/configuration.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/http_client/__init__.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/http_client/client.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/request_builder/__init__.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/request_builder/builder.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/spec/__init__.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/spec/open_api_spec.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/spec/operation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/__init__.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client.py
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_auth.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_complex_request_body.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_edge_cases.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_error_handling.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_live.py
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/github_compare.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_edge_cases.yml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_error_handling.yml
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_greeting_service.yml
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_order_service.json
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_order_service.yml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/serper.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/LICENSE
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/README.md
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/__init__.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/client.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/client_configuration.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/config/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/config/auth_strategy.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/config/configuration.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/http_client/__init__.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/http_client/client.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/request_builder/__init__.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/request_builder/builder.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/spec/__init__.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/spec/open_api_spec.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/src/openapi_service_client/spec/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/client/__init__.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/client/test_client.py
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/client/test_client_auth.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/client/test_client_complex_request_body.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/client/test_client_edge_cases.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/client/test_client_error_handling.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/client/test_client_live.py
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/test_files/github_compare.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/test_files/openapi_edge_cases.yml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/test_files/openapi_error_handling.yml
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/test_files/openapi_greeting_service.yml
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/test_files/openapi_order_service.json
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/test_files/openapi_order_service.yml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/tests/test_files/serper.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/README.md
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 openapi_service_client-0.0.3/PKG-INFO
```

### Comparing `openapi_service_client-0.0.2/.github/workflows/tests.yml` & `openapi_service_client-0.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/src/openapi_service_client/client.py` & `openapi_service_client-0.0.3/tests/client/test_client_complex_request_body.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,80 @@
 import json
-import os
-from pathlib import Path
-from typing import Any, Dict, Optional, Union
-
-from openapi_service_client.auth_factory import AuthenticationFactoryRegistry
-from openapi_service_client.config import AuthenticationStrategy
-from openapi_service_client.http_client import (
-    VALID_HTTP_METHODS,
-    AbstractHttpClient,
-    RequestsHttpClient,
-)
-from openapi_service_client.request_builder import RequestBuilder
-from openapi_service_client.spec import OpenAPISpecification, Operation
-
-
-class OpenAPIServiceClient:
-    def __init__(
-        self,
-        openapi_spec: Union[str, Dict[str, Any]],
-        http_client: Optional[AbstractHttpClient] = None,
-        auth_config: Optional[Union[str, Dict[str, Any], AuthenticationStrategy]] = None,
-    ):
-        if isinstance(openapi_spec, (str, Path)) and os.path.isfile(openapi_spec):
-            self.openapi_spec = OpenAPISpecification.from_file(openapi_spec)
-        elif isinstance(openapi_spec, dict):
-            self.openapi_spec = OpenAPISpecification.from_dict(openapi_spec)
-        else:
-            raise ValueError("Invalid OpenAPI specification format. Expected file path or dictionary.")
-
-        self.http_client = http_client or RequestsHttpClient()
-
-        auth_factory_registry = AuthenticationFactoryRegistry.get_instance().get_factory()
-        created_auth_config = auth_factory_registry.create_authentication(self.openapi_spec, auth_config)
-        self.request_builder = RequestBuilder(self.openapi_spec, self.http_client, auth_config=created_auth_config)
-
-    def get_operations(self) -> Dict[str, Dict[str, Operation]]:
-        operations: Dict[str, Dict[str, Operation]] = {}
-        for path, path_item in self.openapi_spec.get_paths().items():
-            operations[path] = {}
-            for method, operation in path_item.items():
-                if method in VALID_HTTP_METHODS:
-                    operations[path][method] = operation
-        return operations
-
-    def invoke(self, openai_fc_payload: Dict[str, Any]) -> Any:
-        op_id: str = openai_fc_payload.get("function", {}).get("name", "")
-        if not op_id:
-            raise OpenAPIClientError(
-                "Function name not provided in the function calling payload.",
-                openai_fc_payload,
-            )
+from typing import List
+
+import pytest
+from fastapi import FastAPI
+from fastapi.responses import JSONResponse
+from pydantic import BaseModel
+
+from openapi_service_client import OpenAPIServiceClient
+from openapi_service_client.client_configuration import DefaultOpenAPIServiceClientConfiguration
+from tests.conftest import FastAPITestClient
+
+
+class Customer(BaseModel):
+    name: str
+    email: str
+
+
+class OrderItem(BaseModel):
+    product: str
+    quantity: int
+
 
-        args_str = openai_fc_payload.get("function", {}).get("arguments", "")
-        operation = self.openapi_spec.find_operation_by_id(op_id)
-        request = self.request_builder.build_request(operation, **json.loads(args_str))
-        return self.http_client.send_request(request)
+class Order(BaseModel):
+    customer: Customer
+    items: List[OrderItem]
 
 
-class OpenAPIClientError(Exception):
-    pass
+class OrderResponse(BaseModel):
+    orderId: str  # noqa: N815
+    status: str
+    totalAmount: float  # noqa: N815
+
+
+def create_order_app() -> FastAPI:
+    app = FastAPI()
+
+    @app.post("/orders")
+    def create_order(order: Order):
+        total_amount = sum(item.quantity * 10 for item in order.items)
+        response = OrderResponse(
+            orderId="ORDER-001",
+            status="CREATED",
+            totalAmount=total_amount,
+        )
+        return JSONResponse(content=response.dict(), status_code=201)
+
+    return app
+
+
+class TestComplexRequestBody:
+
+    @pytest.mark.parametrize("spec_file_path", ["openapi_order_service.yml", "openapi_order_service.json"])
+    def test_create_order(self, spec_file_path, test_files_path):
+        client = OpenAPIServiceClient(
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / spec_file_path, http_client=FastAPITestClient(create_order_app())
+            )
+        )
+        order_json = {
+            "customer": {"name": "John Doe", "email": "john@example.com"},
+            "items": [
+                {"product": "Product A", "quantity": 2},
+                {"product": "Product B", "quantity": 1},
+            ],
+        }
+        payload = {
+            "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
+            "function": {
+                "arguments": json.dumps(order_json),
+                "name": "createOrder",
+            },
+            "type": "function",
+        }
+        response = client.invoke(payload)
+        assert response == {
+            "orderId": "ORDER-001",
+            "status": "CREATED",
+            "totalAmount": 30,
+        }
```

### Comparing `openapi_service_client-0.0.2/src/openapi_service_client/config/configuration.py` & `openapi_service_client-0.0.3/src/openapi_service_client/config/configuration.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/src/openapi_service_client/http_client/client.py` & `openapi_service_client-0.0.3/src/openapi_service_client/http_client/client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/src/openapi_service_client/request_builder/builder.py` & `openapi_service_client-0.0.3/src/openapi_service_client/request_builder/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 
+from openapi_service_client.client import OpenAPIServiceClientConfiguration
 from openapi_service_client.config import (
-    AuthenticationStrategy,
     PassThroughAuthentication,
 )
-from openapi_service_client.http_client.client import AbstractHttpClient
-from openapi_service_client.spec import OpenAPISpecification, Operation
+from openapi_service_client.spec import Operation
 
 
 class RequestBuilder:
     def __init__(
         self,
-        openapi_parser: OpenAPISpecification,
-        http_client: AbstractHttpClient,
-        auth_config: Optional[AuthenticationStrategy] = None,
+        client_config: OpenAPIServiceClientConfiguration,
     ):
-        self.openapi_parser = openapi_parser
-        self.http_client = http_client
-        self.auth_config = auth_config or PassThroughAuthentication()
+        self.openapi_parser = client_config.get_openapi_spec()
+        self.http_client = client_config.get_http_client()
+        self.auth_config = client_config.get_auth_config() or PassThroughAuthentication()
 
     def build_request(self, operation: Operation, **kwargs) -> Any:
         url = self._build_url(operation, **kwargs)
         method = operation.method.lower()
         headers = self._build_headers(operation)
         query_params = self._build_query_params(operation, **kwargs)
         body = self._build_request_body(operation, **kwargs)
```

### Comparing `openapi_service_client-0.0.2/src/openapi_service_client/spec/open_api_spec.py` & `openapi_service_client-0.0.3/src/openapi_service_client/spec/open_api_spec.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/src/openapi_service_client/spec/operation.py` & `openapi_service_client-0.0.3/src/openapi_service_client/spec/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/tests/conftest.py` & `openapi_service_client-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/tests/client/test_client.py` & `openapi_service_client-0.0.3/tests/client/test_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from fastapi import FastAPI
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel
 
 from openapi_service_client import OpenAPIServiceClient
+from openapi_service_client.client_configuration import DefaultOpenAPIServiceClientConfiguration
 from tests.conftest import FastAPITestClient
 
 """
 Tests OpenAPIServiceClient with three FastAPI apps for different parameter types:
 
 - **greet_mix_params_body**: A POST endpoint `/greet/<name>` accepting a JSON payload with a message, returning a
 greeting with the name from the URL and the message from the payload.
@@ -64,48 +65,54 @@
     return app
 
 
 class TestOpenAPI:
 
     def test_greet_mix_params_body(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_mix_params_body_app()),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_mix_params_body_app()),
+            )
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John", "message": "Bonjour"}',
                 "name": "greet",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Bonjour, John from mix_params_body!"}
 
     def test_greet_params_only(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_params_only_app()),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_params_only_app()),
+            )
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetParams",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from params_only!"}
 
     def test_greet_request_body_only(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_request_body_only_app()),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_request_body_only_app()),
+            )
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John", "message": "Hola"}',
                 "name": "greetBody",
             },
```

### Comparing `openapi_service_client-0.0.2/tests/client/test_client_auth.py` & `openapi_service_client-0.0.3/tests/client/test_client_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     HTTPAuthorizationCredentials,
     HTTPBasic,
     HTTPBasicCredentials,
     HTTPBearer,
 )
 
 from openapi_service_client import OpenAPIServiceClient
+from openapi_service_client.client_configuration import DefaultOpenAPIServiceClientConfiguration
 from openapi_service_client.config import ApiKeyAuthentication
 from openapi_service_client.config.configuration import HTTPAuthentication, OAuthAuthentication
 from tests.conftest import FastAPITestClient
 
 API_KEY = "secret_api_key"
 BASIC_AUTH_USERNAME = "admin"
 BASIC_AUTH_PASSWORD = "secret_password"
@@ -131,102 +132,114 @@
     return app
 
 
 class TestOpenAPIAuth:
 
     def test_greet_api_key_auth(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_api_key_auth_app()),
-            ApiKeyAuthentication(API_KEY),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_api_key_auth_app()),
+                credentials=ApiKeyAuthentication(API_KEY),
+            )
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetApiKey",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from api_key_auth, using secret_api_key"}
 
     def test_greet_basic_auth(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_basic_auth_app()),
-            HTTPAuthentication(BASIC_AUTH_USERNAME, BASIC_AUTH_PASSWORD),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_basic_auth_app()),
+                credentials=HTTPAuthentication(BASIC_AUTH_USERNAME, BASIC_AUTH_PASSWORD),
+            )
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetBasicAuth",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from basic_auth, using admin"}
 
     def test_greet_api_key_query_auth(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_api_key_query_app()),
-            ApiKeyAuthentication(API_KEY_QUERY),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_api_key_query_app()),
+                credentials=ApiKeyAuthentication(API_KEY_QUERY),
+            ),
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetApiKeyQuery",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from api_key_query_auth, using secret_api_key_query"}
 
     def test_greet_api_key_cookie_auth(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_api_key_cookie_app()),
-            ApiKeyAuthentication(API_KEY_COOKIE),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_api_key_cookie_app()),
+                credentials=ApiKeyAuthentication(API_KEY_COOKIE),
+            )
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetApiKeyCookie",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from api_key_cookie_auth, using secret_api_key_cookie"}
 
     def test_greet_bearer_auth(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_bearer_auth_app()),
-            HTTPAuthentication(token=BEARER_TOKEN),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_bearer_auth_app()),
+                credentials=HTTPAuthentication(token=BEARER_TOKEN),
+            )
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetBearerAuth",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from bearer_auth, using secret_bearer_token"}
 
     def test_greet_oauth_auth(self, test_files_path):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_greeting_service.yml",
-            FastAPITestClient(create_greet_oauth_auth_app()),
-            OAuthAuthentication(OAUTH_TOKEN),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_greeting_service.yml",
+                http_client=FastAPITestClient(create_greet_oauth_auth_app()),
+                credentials=OAuthAuthentication(OAUTH_TOKEN),
+            )
         )
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetOAuth",
             },
```

### Comparing `openapi_service_client-0.0.2/tests/client/test_client_error_handling.py` & `openapi_service_client-0.0.3/tests/client/test_client_error_handling.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 
 import pytest
 from fastapi import FastAPI, HTTPException
 
 from openapi_service_client import OpenAPIServiceClient
+from openapi_service_client.client_configuration import DefaultOpenAPIServiceClientConfiguration
 from openapi_service_client.http_client import HttpClientError
 from tests.conftest import FastAPITestClient
 
 
 def create_error_handling_app() -> FastAPI:
     app = FastAPI()
 
@@ -18,16 +19,18 @@
     return app
 
 
 class TestErrorHandling:
     @pytest.mark.parametrize("status_code", [400, 401, 403, 404, 500])
     def test_http_error_handling(self, test_files_path, status_code):
         client = OpenAPIServiceClient(
-            test_files_path / "openapi_error_handling.yml",
-            FastAPITestClient(create_error_handling_app()),
+            DefaultOpenAPIServiceClientConfiguration(
+                openapi_spec=test_files_path / "openapi_error_handling.yml",
+                http_client=FastAPITestClient(create_error_handling_app()),
+            )
         )
         json_error = {"status_code": status_code}
         payload = {
             "type": "function",
             "function": {
                 "arguments": json.dumps(json_error),
                 "name": "raiseHttpError",
```

### Comparing `openapi_service_client-0.0.2/tests/client/test_client_live.py` & `openapi_service_client-0.0.3/tests/client/test_client_live.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import json
 import os
 
 import pytest
 
 from openapi_service_client.client import OpenAPIServiceClient
-from openapi_service_client.config.configuration import ApiKeyAuthentication
+from openapi_service_client.client_configuration import (
+    OpenAPIServiceClientConfigurationBuilder,
+)
 
 
 class TestClientLive:
 
     @pytest.mark.skipif("SERPERDEV_API_KEY" not in os.environ, reason="SERPERDEV_API_KEY not set")
     def test_serperdev(self, test_files_path):
-        serper_api = OpenAPIServiceClient(
-            openapi_spec=test_files_path / "serper.yaml",
-            auth_config=ApiKeyAuthentication(api_key=os.getenv("SERPERDEV_API_KEY")),
+        builder = OpenAPIServiceClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "serper.yaml")
+            .with_credentials(os.getenv("SERPERDEV_API_KEY"))
+            .build()
         )
+        serper_api = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"q": "Who was Zoran Djindjic?"}',
                 "name": "search",
             },
             "type": "function",
         }
         response = serper_api.invoke(payload)
         assert "politician" in str(response)
 
     def test_github(self, test_files_path):
-        api = OpenAPIServiceClient(
-            openapi_spec=test_files_path / "github_compare.yml",
-            auth_config=ApiKeyAuthentication("real_token_not_needed_here"),
-        )
+        builder = OpenAPIServiceClientConfigurationBuilder()
+        config = builder.with_openapi_spec(test_files_path / "github_compare.yml").build()
+        api = OpenAPIServiceClient(config)
 
         params = {"owner": "deepset-ai", "repo": "haystack", "basehead": "main...add_default_adapter_filters"}
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": json.dumps(params),
                 "name": "compare",
```

### Comparing `openapi_service_client-0.0.2/tests/test_files/github_compare.yml` & `openapi_service_client-0.0.3/tests/test_files/github_compare.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/tests/test_files/openapi_greeting_service.yml` & `openapi_service_client-0.0.3/tests/test_files/openapi_greeting_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/tests/test_files/openapi_order_service.json` & `openapi_service_client-0.0.3/tests/test_files/openapi_order_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/tests/test_files/openapi_order_service.yml` & `openapi_service_client-0.0.3/tests/test_files/openapi_order_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/tests/test_files/serper.yaml` & `openapi_service_client-0.0.3/tests/test_files/serper.yaml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/.gitignore` & `openapi_service_client-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/LICENSE` & `openapi_service_client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.2/README.md` & `openapi_service_client-0.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -18,80 +18,114 @@
 You can install OpenAPI Service Client using pip:
 
 ```shell
 pip install openapi-service-client
 ```
 
 ## Usage
-To use the `OpenAPIServiceClient`, you need to have an OpenAPI specification file (in YAML or JSON format) that describes the API you want to interact with. Below are examples of how to use the library with both explicit and implicit authentication configurations.
 
-### Explicit Authentication
-In this example, we explicitly define the authentication mechanism by using ApiKeyAuthentication to provide the API key.
+To effectively use the `OpenAPIServiceClient`, follow these steps to configure and invoke operations on your target API defined by an OpenAPI specification.
+
+### Step 1: Configuration
+
+Begin by creating a client configuration using the `OpenAPIServiceClientConfigurationBuilder`. This configuration includes the path to your OpenAPI specification and the authentication details.
+
+#### Configuration Example:
 
 ```python
 from openapi_service_client import OpenAPIServiceClient
-from openapi_service_client.config import ApiKeyAuthentication
+from openapi_service_client.client_configuration import OpenAPIServiceClientConfigurationBuilder
+
+# Initialize the configuration builder
+config_builder = OpenAPIServiceClientConfigurationBuilder()
+
+# Build the configuration
+config = (config_builder
+          .with_openapi_spec("/path/to/your/openapi_spec.yaml")
+          .with_credentials("your_api_key_or_bearer_token")
+          .build())
+
+# Create the client with the configured settings
+api_client = OpenAPIServiceClient(config)
+```
+
+This example demonstrates a basic setup. You can further customize the configuration by specifying additional parameters such as a custom HTTP client or advanced authentication strategies.
 
-api = OpenAPIServiceClient(
-    openapi_spec="/path/to/weather_service.yml",
-    auth_config=ApiKeyAuthentication(api_key="your_api_key")
-)
+### Step 2: Invoking API Operations
+With the client configured, you can invoke operations defined in your OpenAPI specification. Simply pass OpenAI function-calling JSON payloads to the `invoke` method to call the desired operation.
 
-payload = {
+```python
+operation_payload = {
     "type": "function",
     "name": "weather_forecast",
     "arguments": {
         "location": "San Francisco, CA",
         "num_days": 3
     }
 }
 
-response = api.invoke(payload)
+# Execute the operation
+response = api_client.invoke(operation_payload)
 print(response)
 ```
 
-In this scenario, ApiKeyAuthentication is utilized to directly provide the API key as part of the authentication configuration. You might want to use this approach when you want to explicitly specify the authentication method and provide the necessary credentials.
+In this example, operation_payload contains the necessary information to call the weather_forecast operation, specifying the city and the number of forecast days as arguments. The invoke method sends the request to the API and returns the response.
 
-### Implicit Authentication
-Alternatively, you can pass your secret token directly, and `OpenAPIServiceClient` will deduce the appropriate authentication method based on the OpenAPI specification. This approach is useful when you want the library to automatically select the correct authentication strategy.
+### Notes on Authentication
 
-```python
+The `with_credentials` method in the configuration builder accommodates a variety of authentication mechanisms to suit different API security requirements:
 
-from openapi_service_client import OpenAPIServiceClient
+- **API Key Authentication:** Use `ApiKeyAuthentication` when your API requires an API key. This class supports adding the API key in the request header, query parameters, or cookies, based on the API's specification.
 
-api = OpenAPIServiceClient(
-    openapi_spec="/path/to/weather_service.yml",
-    auth_config="your_secret_token"
-)
+    ```python
+    from openapi_service_client.config import ApiKeyAuthentication
+    config_builder.with_credentials(ApiKeyAuthentication(api_key="your_api_key"))
+    ```
 
-payload = {
-    "type": "function",
-    "name": "weather_forecast",
-    "arguments": {
-        "location": "San Francisco, CA",
-        "num_days": 3
-    }
-}
+- **HTTP Authentication:** For APIs using HTTP Basic or Bearer Authentication, `HTTPAuthentication` allows you to specify credentials. Provide a username and password for Basic authentication, or a token for Bearer authentication.
 
-response = api.invoke(payload)
-print(response)
+    ```python
+    from openapi_service_client.config import HTTPAuthentication
+
+    # For Basic Auth
+    config_builder.with_credentials(HTTPAuthentication(username="user", password="pass"))
+
+    # For Bearer Token
+    config_builder.with_credentials(HTTPAuthentication(token="your_bearer_token"))
+    ```
+
+- **OAuth2 Authentication:** Use `OAuthAuthentication` for APIs secured with OAuth2. Specify your access token and, if necessary, the token type (defaults to "Bearer").
+
+    ```python
+    from openapi_service_client.config import OAuthAuthentication
+
+    config_builder.with_credentials(OAuthAuthentication(access_token="your_access_token", token_type="Bearer"))
+    ```
+
+Each authentication strategy is designed to integrate seamlessly with the OpenAPI specification's security schemes, ensuring your API calls are correctly authenticated according to the API's requirements.
+
+#### Implicit Credentials
+
+For a more straightforward setup, the `with_credentials` method allows passing a token directly as a string (or a dictionary), enabling implicit determination of the appropriate authentication strategy based on the API's security requirements.
+
+```python
+config_builder.with_credentials("your_bearer_token")
 ```
-In this example, by providing a secret token as a string to auth_config, the library examines the OpenAPI specification to identify and apply the necessary authentication method (e.g., API key, OAuth2 token). This flexibility allows for a more straightforward setup when the authentication strategy can be inferred from the OpenAPI spec and the provided token.
+
+This method simplifies client configuration for APIs that accept a single token, automatically applying the correct authentication strategy without manual selection.
+
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
 
 The client handles the REST invocation by constructing the appropriate HTTP request based on the OpenAPI specification. It takes care of parameter placing (path, query, requestBody etc.), payload formatting, authentication, and error handling. The response from the API is then returned to the caller for further processing.
 
 By leveraging the OpenAPI specification, `OpenAPIServiceClient` eliminates the need for manual request setup and simplifies the integration process. It allows you to focus on working with LLM-generated function calls and seamlessly invoke the underlying services.
-## Configuration
-
-OpenAPI Service Client provides various configuration options to customize the behavior of the client. You can configure authentication, HTTP client settings, and more. Refer to the documentation for detailed information on the available configuration options.
 
 ## Contributing
 
 Contributions to OpenAPI Service Client are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
```

### Comparing `openapi_service_client-0.0.2/pyproject.toml` & `openapi_service_client-0.0.3/pyproject.toml`

 * *Files identical despite different names*

