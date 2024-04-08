# Comparing `tmp/apigw_manager-3.0.1-py3-none-any.whl.zip` & `tmp/apigw_manager-3.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 49998 bytes, number of entries: 40
+Zip file size: 50499 bytes, number of entries: 40
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/__init__.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/__init__.py
 -rw-r--r--  2.0 unx     1058 b- defN 80-Jan-01 00:00 apigw_manager/apigw/admin.py
 -rw-r--r--  2.0 unx      878 b- defN 80-Jan-01 00:00 apigw_manager/apigw/apps.py
 -rw-r--r--  2.0 unx     5994 b- defN 80-Jan-01 00:00 apigw_manager/apigw/authentication.py
 -rw-r--r--  2.0 unx     3927 b- defN 80-Jan-01 00:00 apigw_manager/apigw/command.py
 -rw-r--r--  2.0 unx     1565 b- defN 80-Jan-01 00:00 apigw_manager/apigw/decorators.py
@@ -32,11 +32,11 @@
 -rw-r--r--  2.0 unx     1377 b- defN 80-Jan-01 00:00 apigw_manager/core/exceptions.py
 -rw-r--r--  2.0 unx     1644 b- defN 80-Jan-01 00:00 apigw_manager/core/fetch.py
 -rw-r--r--  2.0 unx     3976 b- defN 80-Jan-01 00:00 apigw_manager/core/handler.py
 -rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 apigw_manager/core/permission.py
 -rw-r--r--  2.0 unx     1576 b- defN 80-Jan-01 00:00 apigw_manager/core/release.py
 -rw-r--r--  2.0 unx     1984 b- defN 80-Jan-01 00:00 apigw_manager/core/sync.py
 -rw-r--r--  2.0 unx     1062 b- defN 80-Jan-01 00:00 apigw_manager/core/utils.py
--rw-r--r--  2.0 unx    19664 b- defN 80-Jan-01 00:00 apigw_manager-3.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 apigw_manager-3.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3876 b- defN 16-Jan-01 00:00 apigw_manager-3.0.1.dist-info/RECORD
-40 files, 103469 bytes uncompressed, 43618 bytes compressed:  57.8%
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 apigw_manager-3.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    21135 b- defN 16-Jan-01 00:00 apigw_manager-3.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx     3876 b- defN 16-Jan-01 00:00 apigw_manager-3.0.2.dist-info/RECORD
+40 files, 104935 bytes uncompressed, 44119 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -105,17 +105,17 @@
 
 Filename: apigw_manager/core/sync.py
 Comment: 
 
 Filename: apigw_manager/core/utils.py
 Comment: 
 
-Filename: apigw_manager-3.0.1.dist-info/METADATA
+Filename: apigw_manager-3.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: apigw_manager-3.0.1.dist-info/WHEEL
+Filename: apigw_manager-3.0.2.dist-info/METADATA
 Comment: 
 
-Filename: apigw_manager-3.0.1.dist-info/RECORD
+Filename: apigw_manager-3.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `apigw_manager-3.0.1.dist-info/METADATA` & `apigw_manager-3.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: apigw-manager
-Version: 3.0.1
+Version: 3.0.2
 Summary: The SDK for managing blueking gateway resource.
 License: MIT
 Author: blueking
 Author-email: blueking@tencent.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cryptography
 Provides-Extra: demo
 Provides-Extra: django
 Provides-Extra: kubernetes
-Requires-Dist: Django (>=1.11.1) ; extra == "django" or extra == "demo"
-Requires-Dist: PyMySQL (>=1.0.2,<2.0.0) ; extra == "demo"
+Requires-Dist: Django (>=1.11.1); extra == "django" or extra == "demo"
+Requires-Dist: PyMySQL (>=1.0.2,<2.0.0); extra == "demo"
 Requires-Dist: bkapi-bk-apigateway (>=1.0.11,<2.0.0)
 Requires-Dist: bkapi-client-core (>=1.2.0)
-Requires-Dist: cryptography (>=3.1.1) ; extra == "cryptography"
-Requires-Dist: django-environ (>=0.8.1) ; extra == "demo"
-Requires-Dist: future (==0.18.2)
-Requires-Dist: kubernetes ; extra == "kubernetes"
+Requires-Dist: cryptography (>=3.1.1); extra == "cryptography"
+Requires-Dist: django-environ (>=0.8.1); extra == "demo"
+Requires-Dist: future (>=0.18.2)
+Requires-Dist: kubernetes; extra == "kubernetes"
 Requires-Dist: packaging (>=21.0)
-Requires-Dist: pyjwt (>=1.6.4) ; extra == "cryptography" or extra == "django" or extra == "demo"
+Requires-Dist: pyjwt (>=1.6.4); extra == "cryptography" or extra == "django" or extra == "demo"
 Requires-Dist: pyyaml (>=5.4.1)
 Requires-Dist: setuptools (>=21.0.0)
 Requires-Dist: urllib3 (>=1.25.3)
 Description-Content-Type: text/markdown
 
 # apigw-manager
 
@@ -99,16 +98,16 @@
 |   key: {{settings.KEY2}} |        |   key: value_from_settings |------>| api2({"key": "value_from_settings"}) |
 |                          |        |                            |       |                                      |
 |                          |        |                            |       +--------------------------------------+
 +--------------------------+        +----------------------------+
 ```
 
 definition.yaml 中可以使用 Django 模版语法引用和渲染变量，内置以下变量：
-- `settings`：Django 提供的配置对象
-- `environ`：环境变量
+- `settings`：Django 提供的配置对象,优先适合用于使用 Django Command 同步
+- `environ`：环境变量,推荐镜像同步方式使用
 
 推荐在一个文件中统一进行定义，用命名空间区分不同配置间的定义，definition.yaml 样例：
 
 ```yaml
 # definition.yaml 配置文件版本号，必填，固定值 1
 spec_version: 1
 
@@ -163,45 +162,51 @@
           weight: 100
     # Header转换；如未使用，可去除此配置
     # transform_headers:
     #   # 设置Headers
     #   set:
     #     X-Token: "token"
 
-# 主动授权，网关主动给应用，添加访问网关所有资源的权限；
+# 主动授权，网关主动给应用，添加访问网关所有资源或者具体某个资源的权限；
 # 用于命令 `grant_apigw_permissions`
 grant_permissions:
-  - bk_app_code: "{{ settings.BK_APP_CODE }}"
-    # 授权维度，可选值：gateway，按网关授权，包括网关下所有资源，以及未来新创建的资源
+  - bk_app_code: "{{ settings.BK_APP_CODE }}" ## 环境变量方式："{{ environ.BK_APP_CODE }}"
+    # 授权维度，可选值：
+    # gateway: 按网关授权，包括网关下所有资源，以及未来新创建的资源
+    # resource: 按资源维度授权
     grant_dimension: "gateway"
+    # 如果是按照 resource 维度授权,需要提供如下的具体resource_name
+    # resource_names:
+    #   - resource_name_1 
+    #   - resource_name_2   
 
 # 应用申请指定网关所有资源的权限，待网关管理员审批后，应用才可访问网关资源；
 # 用于命令 `apply_apigw_permissions`
 # apply_permissions:
-#   - gateway_name: "{{ settings.BK_APIGW_NAME }}"
+#   - gateway_name: "{{ settings.BK_APIGW_NAME }}" ## 环境变量方式："{{ environ.BK_APIGW_NAME }}"
 #     # 权限维度，可选值：gateway，按网关授权，包括网关下所有资源，以及未来新创建的资源
 #     grant_dimension: "gateway"
 
 # 为网关添加关联应用，关联应用可以通过网关 bk-apigateway 的接口操作网关数据；每个网关最多可有 10 个关联应用；
 # 用于命令 `add_related_apps`
 related_apps:
-  - "{{ settings.BK_APP_CODE }}"
+  - "{{ settings.BK_APP_CODE }}" ## 环境变量方式："{{ environ.BK_APP_CODE }}"
 
 # 定义资源文档路径，用于命令 `sync_resource_docs_by_archive`；
 # 资源文档的目录格式样例如下，en 为英文文档，zh 为中文文档，创建归档文件可使用指令 `tar czvf xxx.tgz en zh`：
 # ./
 # - en
 #   - get_user.md
 # - zh
 #   - get_user.md
 resource_docs:
   # 资源文档的归档文件，可为 tar.gz，zip 格式文件
-  archivefile: "{{ settings.BK_APIGW_RESOURCE_DOCS_ARCHIVE_FILE }}"
+  archivefile: "{{ settings.BK_APIGW_RESOURCE_DOCS_ARCHIVE_FILE }}" ## 环境变量方式："{{ environ.BK_APIGW_RESOURCE_DOCS_ARCHIVE_FILE }}"
   # 资源文档目录，basedir 与 archivefile 二者至少一个有效，若同时存在，则 archivefile 优先
-  basedir: "{{ settings.BK_APIGW_RESOURCE_DOCS_BASE_DIR }}"
+  basedir: "{{ settings.BK_APIGW_RESOURCE_DOCS_BASE_DIR }}" ## 环境变量方式："{{ environ.BK_APIGW_RESOURCE_DOCS_BASE_DIR }}"
 ```
 
 **注意：**
 - 同步资源后，需要创建版本并发布才能生效，发布数据定义于 definition.yaml `release`
 - 资源配置 resources.yaml 变更时，需要更新 definition.yaml `release` 中的版本号 version，以便正确创建资源版本及 SDK
 
 #### 2. resources.yaml
@@ -404,8 +409,17 @@
     "verified": true          # 应用是否通过认证，true 表示通过认证，false 表示未通过认证
   },
   "exp": 1701401103,      # 过期时间
   "nbf": 1701399303,      # Not Before 时间
   "iss": "APIGW"          # 签发者
 }
 ```
-
+## FAQ
+### 1.同步过程中报错：`call_definition_command_or_exit: command not found`
+这种大概率是自定义脚本有问题，参照文档，按照对应目录下的 examples 的同步脚本即可。
+
+### 2.执行同步命令时报错：`Error responded by API Gateway, status_code:_code: 404, request_id:, error_code: 1640401, API not found`
+这种大概率是网关URL `BK_API_URL_TMPL` 漏配或者配错了。eg: BK_API_URL_TMPL: http://bkapi.example.com/api/{api_name}"l, 注意 {api_name}是占位符需要保留
+
+### 3.同步过程中报错: `校验失败: api_type: api_type 为 1 时，网关名 name 需以 bk- 开头。`
+这个是因为 `definition.yaml` 定义的 apigateway.api_type为 1，标记网关为官方网关，网关名需以 `bk-` 开头，可选；非官方网关，可去除此配置
+当设置为 1 时,则 `sync-apigateway.sh`里面的 `gateway_name` 参数需要以 bk- 开头
```

## Comparing `apigw_manager-3.0.1.dist-info/RECORD` & `apigw_manager-3.0.2.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -31,10 +31,10 @@
 apigw_manager/core/exceptions.py,sha256=UF9VNXQPGlMUNxxU8PI9xCx_9GqYbbPtiecxD_5aNJ8,1377
 apigw_manager/core/fetch.py,sha256=m-DHxgACeTY9CUlK-qRvWbTukqIMPBCgQkldjibv0Eg,1644
 apigw_manager/core/handler.py,sha256=fvirbNCncPCciWkbIWnRwpgEO8eykCFm4BfaDoOT1ZA,3976
 apigw_manager/core/permission.py,sha256=RGvGbL60WZ9I0mzXnTHoEmUwP3AKlwysOV-nipdN0rk,1415
 apigw_manager/core/release.py,sha256=zu17zfYegBFx3MEpt2GjsSWEKvHd0B63IYplqtycGOc,1576
 apigw_manager/core/sync.py,sha256=aYMHOJ0BxV3m7xlwjl-p0b8kGlVdgpOK-7o6ybr2w6E,1984
 apigw_manager/core/utils.py,sha256=eUviCN04dRB5oFgM3su1uOwpf1JzgKSeahXncwThbJY,1062
-apigw_manager-3.0.1.dist-info/METADATA,sha256=oLyIrv2H2WjvC-mIUnE1acPJpx0D8s6FJdVIar50Od4,19664
-apigw_manager-3.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-apigw_manager-3.0.1.dist-info/RECORD,,
+apigw_manager-3.0.2.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
+apigw_manager-3.0.2.dist-info/METADATA,sha256=F3GRlMXeNbPNKkKm9cyUAGKY8UTln5XlWguYuj3U254,21135
+apigw_manager-3.0.2.dist-info/RECORD,,
```

