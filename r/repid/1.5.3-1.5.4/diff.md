# Comparing `tmp/repid-1.5.3.tar.gz` & `tmp/repid-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repid-1.5.3.tar", last modified: Mon Apr  1 23:29:47 2024, max compression
+gzip compressed data, was "repid-1.5.4.tar", last modified: Sun Apr  7 23:11:29 2024, max compression
```

## Comparing `repid-1.5.3.tar` & `repid-1.5.4.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     1089 2024-04-01 23:29:30.139399 repid-1.5.3/LICENSE
--rw-r--r--   0        0        0     2604 2024-04-01 23:29:30.139399 repid-1.5.3/README.md
--rw-r--r--   0        0        0     4379 2024-04-01 23:29:47.795714 repid-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     1397 2024-04-01 23:29:30.143399 repid-1.5.3/repid/__init__.py
--rw-r--r--   0        0        0     1544 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_asyncify.py
--rw-r--r--   0        0        0     8009 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_processor.py
--rw-r--r--   0        0        0     5664 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_runner.py
--rw-r--r--   0        0        0      551 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/__init__.py
--rw-r--r--   0        0        0      501 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/args_bucket_in_message_id.py
--rw-r--r--   0        0        0      272 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/dataclass_hacks.py
--rw-r--r--   0        0        0      834 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/get_dependency.py
--rw-r--r--   0        0        0      432 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/internal_exceptions.py
--rw-r--r--   0        0        0     1268 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/is_installed.py
--rw-r--r--   0        0        0     1012 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/json_encoder.py
--rw-r--r--   0        0        0      135 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/regex_validators.py
--rw-r--r--   0        0        0      536 2024-04-01 23:29:30.143399 repid-1.5.3/repid/actor.py
--rw-r--r--   0        0        0     2499 2024-04-01 23:29:30.143399 repid-1.5.3/repid/config.py
--rw-r--r--   0        0        0     4493 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connection.py
--rw-r--r--   0        0        0      736 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/__init__.py
--rw-r--r--   0        0        0     6765 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/abc.py
--rw-r--r--   0        0        0      314 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/dummy/__init__.py
--rw-r--r--   0        0        0      260 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/__init__.py
--rw-r--r--   0        0        0     1823 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/bucket_broker.py
--rw-r--r--   0        0        0     3856 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/consumer.py
--rw-r--r--   0        0        0     4093 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/message_broker.py
--rw-r--r--   0        0        0      859 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/utils.py
--rw-r--r--   0        0        0       90 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/__init__.py
--rw-r--r--   0        0        0     8826 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/consumer.py
--rw-r--r--   0        0        0     7289 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/message_broker.py
--rw-r--r--   0        0        0      803 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/protocols.py
--rw-r--r--   0        0        0     1809 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/utils.py
--rw-r--r--   0        0        0      158 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/__init__.py
--rw-r--r--   0        0        0     1544 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/bucket_broker.py
--rw-r--r--   0        0        0    11878 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/consumer.py
--rw-r--r--   0        0        0     8025 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/message_broker.py
--rw-r--r--   0        0        0     4107 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/utils.py
--rw-r--r--   0        0        0     8405 2024-04-01 23:29:30.143399 repid-1.5.3/repid/converter.py
--rw-r--r--   0        0        0      355 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/__init__.py
--rw-r--r--   0        0        0     2268 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/_buckets.py
--rw-r--r--   0        0        0      820 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/_key.py
--rw-r--r--   0        0        0     5504 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/_parameters.py
--rw-r--r--   0        0        0       95 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/priorities.py
--rw-r--r--   0        0        0     3733 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/protocols.py
--rw-r--r--   0        0        0      282 2024-04-01 23:29:30.143399 repid-1.5.3/repid/dependencies/__init__.py
--rw-r--r--   0        0        0     3171 2024-04-01 23:29:30.143399 repid-1.5.3/repid/dependencies/depends.py
--rw-r--r--   0        0        0     7327 2024-04-01 23:29:30.143399 repid-1.5.3/repid/dependencies/message_dependency.py
--rw-r--r--   0        0        0      866 2024-04-01 23:29:30.147399 repid-1.5.3/repid/dependencies/protocols.py
--rw-r--r--   0        0        0      587 2024-04-01 23:29:30.147399 repid-1.5.3/repid/dependencies/resolver_context.py
--rw-r--r--   0        0        0     3421 2024-04-01 23:29:30.147399 repid-1.5.3/repid/health_check_server.py
--rw-r--r--   0        0        0     7478 2024-04-01 23:29:30.147399 repid-1.5.3/repid/job.py
--rw-r--r--   0        0        0      548 2024-04-01 23:29:30.147399 repid-1.5.3/repid/logger.py
--rw-r--r--   0        0        0     1887 2024-04-01 23:29:30.147399 repid-1.5.3/repid/main.py
--rw-r--r--   0        0        0     3791 2024-04-01 23:29:30.147399 repid-1.5.3/repid/message.py
--rw-r--r--   0        0        0      257 2024-04-01 23:29:30.147399 repid-1.5.3/repid/middlewares/__init__.py
--rw-r--r--   0        0        0      347 2024-04-01 23:29:30.147399 repid-1.5.3/repid/middlewares/consts.py
--rw-r--r--   0        0        0     3685 2024-04-01 23:29:30.147399 repid-1.5.3/repid/middlewares/middleware.py
--rw-r--r--   0        0        0     3639 2024-04-01 23:29:30.147399 repid-1.5.3/repid/middlewares/wrapper.py
--rw-r--r--   0        0        0        0 2024-04-01 23:29:30.147399 repid-1.5.3/repid/py.typed
--rw-r--r--   0        0        0     1930 2024-04-01 23:29:30.147399 repid-1.5.3/repid/queue.py
--rw-r--r--   0        0        0     1319 2024-04-01 23:29:30.147399 repid-1.5.3/repid/retry_policy.py
--rw-r--r--   0        0        0     5006 2024-04-01 23:29:30.147399 repid-1.5.3/repid/router.py
--rw-r--r--   0        0        0      512 2024-04-01 23:29:30.147399 repid-1.5.3/repid/serializer.py
--rw-r--r--   0        0        0      781 2024-04-01 23:29:30.147399 repid-1.5.3/repid/testing/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-01 23:29:30.147399 repid-1.5.3/repid/testing/modifiers.py
--rw-r--r--   0        0        0     6163 2024-04-01 23:29:30.147399 repid-1.5.3/repid/testing/plugin.py
--rw-r--r--   0        0        0     4920 2024-04-01 23:29:30.147399 repid-1.5.3/repid/worker.py
--rw-r--r--   0        0        0        0 2024-04-01 23:29:30.147399 repid-1.5.3/tests/__init__.py
--rw-r--r--   0        0        0     1145 2024-04-01 23:29:30.147399 repid-1.5.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/__init__.py
--rw-r--r--   0        0        0     3241 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/conftest.py
--rw-r--r--   0        0        0     1337 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_buckets.py
--rw-r--r--   0        0        0     4335 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_consumer.py
--rw-r--r--   0        0        0     4678 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_consumer_different_categories.py
--rw-r--r--   0        0        0     4005 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_default_flow.py
--rw-r--r--   0        0        0     1904 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_no_messages_lost.py
--rw-r--r--   0        0        0     1402 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_rabbitmq_specific.py
--rw-r--r--   0        0        0      431 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_actor.py
--rw-r--r--   0        0        0     4608 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_config.py
--rw-r--r--   0        0        0     2986 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_connection.py
--rw-r--r--   0        0        0     3834 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_consumer.py
--rw-r--r--   0        0        0     2835 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_consumer_abc.py
--rw-r--r--   0        0        0    10230 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_default_data_models.py
--rw-r--r--   0        0        0    13979 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_dependencies.py
--rw-r--r--   0        0        0     2110 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_health_check_server.py
--rw-r--r--   0        0        0     3004 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_hypothesis.py
--rw-r--r--   0        0        0     3591 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_job.py
--rw-r--r--   0        0        0     2298 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_json.py
--rw-r--r--   0        0        0     1366 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_main.py
--rw-r--r--   0        0        0     5627 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_message.py
--rw-r--r--   0        0        0     7842 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_middleware.py
--rw-r--r--   0        0        0     1097 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     7360 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_pydantic.py
--rw-r--r--   0        0        0     3819 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_pytest_plugin.py
--rw-r--r--   0        0        0      414 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_queue.py
--rw-r--r--   0        0        0     3180 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_router.py
--rw-r--r--   0        0        0     3673 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_runner.py
--rw-r--r--   0        0        0      762 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_serializer.py
--rw-r--r--   0        0        0     1893 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_utils.py
--rw-r--r--   0        0        0     9065 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_worker.py
--rw-r--r--   0        0        0     4123 1970-01-01 00:00:00.000000 repid-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-07 23:11:12.295230 repid-1.5.4/LICENSE
+-rw-r--r--   0        0        0     2604 2024-04-07 23:11:12.295230 repid-1.5.4/README.md
+-rw-r--r--   0        0        0     4379 2024-04-07 23:11:29.975276 repid-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1397 2024-04-07 23:11:12.299230 repid-1.5.4/repid/__init__.py
+-rw-r--r--   0        0        0     1544 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_asyncify.py
+-rw-r--r--   0        0        0     8009 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_processor.py
+-rw-r--r--   0        0        0     5664 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_runner.py
+-rw-r--r--   0        0        0      551 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_utils/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_utils/args_bucket_in_message_id.py
+-rw-r--r--   0        0        0      272 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_utils/dataclass_hacks.py
+-rw-r--r--   0        0        0      834 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_utils/get_dependency.py
+-rw-r--r--   0        0        0      432 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_utils/internal_exceptions.py
+-rw-r--r--   0        0        0     1268 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_utils/is_installed.py
+-rw-r--r--   0        0        0     1012 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_utils/json_encoder.py
+-rw-r--r--   0        0        0      135 2024-04-07 23:11:12.299230 repid-1.5.4/repid/_utils/regex_validators.py
+-rw-r--r--   0        0        0      536 2024-04-07 23:11:12.299230 repid-1.5.4/repid/actor.py
+-rw-r--r--   0        0        0     2499 2024-04-07 23:11:12.299230 repid-1.5.4/repid/config.py
+-rw-r--r--   0        0        0     4493 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connection.py
+-rw-r--r--   0        0        0      736 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/__init__.py
+-rw-r--r--   0        0        0     6765 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/abc.py
+-rw-r--r--   0        0        0      314 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/dummy/__init__.py
+-rw-r--r--   0        0        0      260 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/in_memory/__init__.py
+-rw-r--r--   0        0        0     1823 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/in_memory/bucket_broker.py
+-rw-r--r--   0        0        0     3856 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/in_memory/consumer.py
+-rw-r--r--   0        0        0     4093 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/in_memory/message_broker.py
+-rw-r--r--   0        0        0      859 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/in_memory/utils.py
+-rw-r--r--   0        0        0       90 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     8826 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/rabbitmq/consumer.py
+-rw-r--r--   0        0        0     7289 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/rabbitmq/message_broker.py
+-rw-r--r--   0        0        0      803 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/rabbitmq/protocols.py
+-rw-r--r--   0        0        0     1809 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/rabbitmq/utils.py
+-rw-r--r--   0        0        0      158 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/redis/__init__.py
+-rw-r--r--   0        0        0     1544 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/redis/bucket_broker.py
+-rw-r--r--   0        0        0    11878 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/redis/consumer.py
+-rw-r--r--   0        0        0     8025 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/redis/message_broker.py
+-rw-r--r--   0        0        0     4107 2024-04-07 23:11:12.299230 repid-1.5.4/repid/connections/redis/utils.py
+-rw-r--r--   0        0        0     8405 2024-04-07 23:11:12.299230 repid-1.5.4/repid/converter.py
+-rw-r--r--   0        0        0      355 2024-04-07 23:11:12.299230 repid-1.5.4/repid/data/__init__.py
+-rw-r--r--   0        0        0     2268 2024-04-07 23:11:12.299230 repid-1.5.4/repid/data/_buckets.py
+-rw-r--r--   0        0        0      820 2024-04-07 23:11:12.299230 repid-1.5.4/repid/data/_key.py
+-rw-r--r--   0        0        0     5504 2024-04-07 23:11:12.299230 repid-1.5.4/repid/data/_parameters.py
+-rw-r--r--   0        0        0       95 2024-04-07 23:11:12.299230 repid-1.5.4/repid/data/priorities.py
+-rw-r--r--   0        0        0     3733 2024-04-07 23:11:12.299230 repid-1.5.4/repid/data/protocols.py
+-rw-r--r--   0        0        0      282 2024-04-07 23:11:12.299230 repid-1.5.4/repid/dependencies/__init__.py
+-rw-r--r--   0        0        0     3171 2024-04-07 23:11:12.299230 repid-1.5.4/repid/dependencies/depends.py
+-rw-r--r--   0        0        0     7327 2024-04-07 23:11:12.303230 repid-1.5.4/repid/dependencies/message_dependency.py
+-rw-r--r--   0        0        0      866 2024-04-07 23:11:12.303230 repid-1.5.4/repid/dependencies/protocols.py
+-rw-r--r--   0        0        0      587 2024-04-07 23:11:12.303230 repid-1.5.4/repid/dependencies/resolver_context.py
+-rw-r--r--   0        0        0     3421 2024-04-07 23:11:12.303230 repid-1.5.4/repid/health_check_server.py
+-rw-r--r--   0        0        0     7478 2024-04-07 23:11:12.303230 repid-1.5.4/repid/job.py
+-rw-r--r--   0        0        0      548 2024-04-07 23:11:12.303230 repid-1.5.4/repid/logger.py
+-rw-r--r--   0        0        0     1887 2024-04-07 23:11:12.303230 repid-1.5.4/repid/main.py
+-rw-r--r--   0        0        0     3791 2024-04-07 23:11:12.303230 repid-1.5.4/repid/message.py
+-rw-r--r--   0        0        0      257 2024-04-07 23:11:12.303230 repid-1.5.4/repid/middlewares/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-07 23:11:12.303230 repid-1.5.4/repid/middlewares/consts.py
+-rw-r--r--   0        0        0     3685 2024-04-07 23:11:12.303230 repid-1.5.4/repid/middlewares/middleware.py
+-rw-r--r--   0        0        0     3639 2024-04-07 23:11:12.303230 repid-1.5.4/repid/middlewares/wrapper.py
+-rw-r--r--   0        0        0        0 2024-04-07 23:11:12.303230 repid-1.5.4/repid/py.typed
+-rw-r--r--   0        0        0     1930 2024-04-07 23:11:12.303230 repid-1.5.4/repid/queue.py
+-rw-r--r--   0        0        0     1319 2024-04-07 23:11:12.303230 repid-1.5.4/repid/retry_policy.py
+-rw-r--r--   0        0        0     5006 2024-04-07 23:11:12.303230 repid-1.5.4/repid/router.py
+-rw-r--r--   0        0        0      512 2024-04-07 23:11:12.303230 repid-1.5.4/repid/serializer.py
+-rw-r--r--   0        0        0      781 2024-04-07 23:11:12.303230 repid-1.5.4/repid/testing/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-07 23:11:12.303230 repid-1.5.4/repid/testing/modifiers.py
+-rw-r--r--   0        0        0     6163 2024-04-07 23:11:12.303230 repid-1.5.4/repid/testing/plugin.py
+-rw-r--r--   0        0        0     5071 2024-04-07 23:11:12.303230 repid-1.5.4/repid/worker.py
+-rw-r--r--   0        0        0        0 2024-04-07 23:11:12.303230 repid-1.5.4/tests/__init__.py
+-rw-r--r--   0        0        0     1145 2024-04-07 23:11:12.303230 repid-1.5.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-07 23:11:12.303230 repid-1.5.4/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3241 2024-04-07 23:11:12.303230 repid-1.5.4/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1337 2024-04-07 23:11:12.303230 repid-1.5.4/tests/integration/test_buckets.py
+-rw-r--r--   0        0        0     4335 2024-04-07 23:11:12.303230 repid-1.5.4/tests/integration/test_consumer.py
+-rw-r--r--   0        0        0     4678 2024-04-07 23:11:12.303230 repid-1.5.4/tests/integration/test_consumer_different_categories.py
+-rw-r--r--   0        0        0     4005 2024-04-07 23:11:12.303230 repid-1.5.4/tests/integration/test_default_flow.py
+-rw-r--r--   0        0        0     1904 2024-04-07 23:11:12.303230 repid-1.5.4/tests/integration/test_no_messages_lost.py
+-rw-r--r--   0        0        0     1402 2024-04-07 23:11:12.303230 repid-1.5.4/tests/integration/test_rabbitmq_specific.py
+-rw-r--r--   0        0        0      431 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_actor.py
+-rw-r--r--   0        0        0     4608 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_config.py
+-rw-r--r--   0        0        0     2986 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_connection.py
+-rw-r--r--   0        0        0     3834 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_consumer.py
+-rw-r--r--   0        0        0     2835 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_consumer_abc.py
+-rw-r--r--   0        0        0    10230 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_default_data_models.py
+-rw-r--r--   0        0        0    13979 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2110 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_health_check_server.py
+-rw-r--r--   0        0        0     3004 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_hypothesis.py
+-rw-r--r--   0        0        0     3591 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_job.py
+-rw-r--r--   0        0        0     2298 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_json.py
+-rw-r--r--   0        0        0     1366 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_main.py
+-rw-r--r--   0        0        0     5627 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_message.py
+-rw-r--r--   0        0        0     7842 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_middleware.py
+-rw-r--r--   0        0        0     1097 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     7360 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_pydantic.py
+-rw-r--r--   0        0        0     3819 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0      414 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_queue.py
+-rw-r--r--   0        0        0     3180 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_router.py
+-rw-r--r--   0        0        0     3673 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_runner.py
+-rw-r--r--   0        0        0      762 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_serializer.py
+-rw-r--r--   0        0        0     1893 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_utils.py
+-rw-r--r--   0        0        0     9065 2024-04-07 23:11:12.303230 repid-1.5.4/tests/test_worker.py
+-rw-r--r--   0        0        0     4123 1970-01-01 00:00:00.000000 repid-1.5.4/PKG-INFO
```

### Comparing `repid-1.5.3/LICENSE` & `repid-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/README.md` & `repid-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/pyproject.toml` & `repid-1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "packaging>=22.0",
 ]
 description = "Repid framework: simple to use, fast to run and extensible to adopt job scheduler"
 dynamic = []
 name = "repid"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.5.3"
+version = "1.5.4"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.pytest11]
 repid = "repid.testing.plugin"
```

### Comparing `repid-1.5.3/repid/__init__.py` & `repid-1.5.4/repid/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/_asyncify.py` & `repid-1.5.4/repid/_asyncify.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/_processor.py` & `repid-1.5.4/repid/_processor.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/_runner.py` & `repid-1.5.4/repid/_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/_utils/__init__.py` & `repid-1.5.4/repid/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/_utils/get_dependency.py` & `repid-1.5.4/repid/_utils/get_dependency.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/_utils/is_installed.py` & `repid-1.5.4/repid/_utils/is_installed.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/_utils/json_encoder.py` & `repid-1.5.4/repid/_utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/actor.py` & `repid-1.5.4/repid/actor.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/config.py` & `repid-1.5.4/repid/config.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connection.py` & `repid-1.5.4/repid/connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/__init__.py` & `repid-1.5.4/repid/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/abc.py` & `repid-1.5.4/repid/connections/abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/in_memory/bucket_broker.py` & `repid-1.5.4/repid/connections/in_memory/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/in_memory/consumer.py` & `repid-1.5.4/repid/connections/in_memory/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/in_memory/message_broker.py` & `repid-1.5.4/repid/connections/in_memory/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/in_memory/utils.py` & `repid-1.5.4/repid/connections/in_memory/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/rabbitmq/consumer.py` & `repid-1.5.4/repid/connections/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/rabbitmq/message_broker.py` & `repid-1.5.4/repid/connections/rabbitmq/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/rabbitmq/protocols.py` & `repid-1.5.4/repid/connections/rabbitmq/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/rabbitmq/utils.py` & `repid-1.5.4/repid/connections/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/redis/bucket_broker.py` & `repid-1.5.4/repid/connections/redis/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/redis/consumer.py` & `repid-1.5.4/repid/connections/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/redis/message_broker.py` & `repid-1.5.4/repid/connections/redis/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/connections/redis/utils.py` & `repid-1.5.4/repid/connections/redis/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/converter.py` & `repid-1.5.4/repid/converter.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/data/_buckets.py` & `repid-1.5.4/repid/data/_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/data/_key.py` & `repid-1.5.4/repid/data/_key.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/data/_parameters.py` & `repid-1.5.4/repid/data/_parameters.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/data/protocols.py` & `repid-1.5.4/repid/data/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/dependencies/depends.py` & `repid-1.5.4/repid/dependencies/depends.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/dependencies/message_dependency.py` & `repid-1.5.4/repid/dependencies/message_dependency.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/dependencies/protocols.py` & `repid-1.5.4/repid/dependencies/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/dependencies/resolver_context.py` & `repid-1.5.4/repid/dependencies/resolver_context.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/health_check_server.py` & `repid-1.5.4/repid/health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/job.py` & `repid-1.5.4/repid/job.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/logger.py` & `repid-1.5.4/repid/logger.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/main.py` & `repid-1.5.4/repid/main.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/message.py` & `repid-1.5.4/repid/message.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/middlewares/middleware.py` & `repid-1.5.4/repid/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/middlewares/wrapper.py` & `repid-1.5.4/repid/middlewares/wrapper.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/queue.py` & `repid-1.5.4/repid/queue.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/retry_policy.py` & `repid-1.5.4/repid/retry_policy.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/router.py` & `repid-1.5.4/repid/router.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/serializer.py` & `repid-1.5.4/repid/serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/testing/__init__.py` & `repid-1.5.4/repid/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/testing/modifiers.py` & `repid-1.5.4/repid/testing/modifiers.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/testing/plugin.py` & `repid-1.5.4/repid/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/repid/worker.py` & `repid-1.5.4/repid/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,16 @@
             *(
                 Queue(queue_name, _connection=self._conn).declare()
                 for queue_name in self.topics_by_queue
             ),
         )
 
     async def run(self) -> _Runner:
+        logger.info("Starting to run worker.")
+
         if self.health_check_server is not None:
             await self.health_check_server.start()
 
         runner = _Runner(
             max_tasks=self.messages_limit,
             tasks_concurrency_limit=self.tasks_limit,
             health_check_server=self.health_check_server,
@@ -83,15 +85,15 @@
 
         if self.auto_declare:
             await self.declare_all_queues()
 
         loop = asyncio.get_running_loop()
         self._register_signals(loop, runner)
 
-        logger.debug("Starting consumers.")
+        logger.info("Starting consumers.")
         try:
             consumers = await asyncio.gather(
                 *(
                     runner.run_one_queue(
                         queue_name,
                         self.topics_by_queue[queue_name],
                         self.actors,
@@ -102,32 +104,35 @@
         except asyncio.CancelledError as exc:
             logger.critical("Worker was cancelled.", exc_info=exc)
             raise
 
         await runner.finish_gracefully(timeout=self.graceful_shutdown_time)
 
         if consumers:
-            logger.debug("Gracefully finishing consumers.")
+            logger.info("Gracefully finishing consumers.")
             await asyncio.wait_for(
                 asyncio.gather(*(c.finish() for c in consumers)),
                 timeout=self.graceful_consumer_finish_time,
             )
 
         if self.health_check_server is not None:
             await asyncio.wait_for(
                 self.health_check_server.stop(),
                 timeout=self.graceful_health_check_server_finish_time,
             )
 
         self._unregister_signals(loop)
 
+        logger.info("Exiting worker run.")
+
         return runner
 
     def _register_signals(self, loop: asyncio.AbstractEventLoop, runner: _Runner) -> None:
         def signal_handler() -> None:
+            logger.info("Received signal, stopping runner.")
             runner.sync_stop_wait_and_cancel(self.graceful_shutdown_time)
             self._unregister_signals(loop)
 
         if self.handle_signals:
             logger.debug(
                 "Registering signal ({signals}) handlers.",
                 extra={"signals": self.handle_signals},
```

### Comparing `repid-1.5.3/tests/conftest.py` & `repid-1.5.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/integration/conftest.py` & `repid-1.5.4/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/integration/test_buckets.py` & `repid-1.5.4/tests/integration/test_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/integration/test_consumer.py` & `repid-1.5.4/tests/integration/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/integration/test_consumer_different_categories.py` & `repid-1.5.4/tests/integration/test_consumer_different_categories.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/integration/test_default_flow.py` & `repid-1.5.4/tests/integration/test_default_flow.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/integration/test_no_messages_lost.py` & `repid-1.5.4/tests/integration/test_no_messages_lost.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/integration/test_rabbitmq_specific.py` & `repid-1.5.4/tests/integration/test_rabbitmq_specific.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_config.py` & `repid-1.5.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_connection.py` & `repid-1.5.4/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_consumer.py` & `repid-1.5.4/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_consumer_abc.py` & `repid-1.5.4/tests/test_consumer_abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_default_data_models.py` & `repid-1.5.4/tests/test_default_data_models.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_dependencies.py` & `repid-1.5.4/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_health_check_server.py` & `repid-1.5.4/tests/test_health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_hypothesis.py` & `repid-1.5.4/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_job.py` & `repid-1.5.4/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_json.py` & `repid-1.5.4/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_main.py` & `repid-1.5.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_message.py` & `repid-1.5.4/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_middleware.py` & `repid-1.5.4/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_multiprocessing.py` & `repid-1.5.4/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_pydantic.py` & `repid-1.5.4/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_pytest_plugin.py` & `repid-1.5.4/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_router.py` & `repid-1.5.4/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_runner.py` & `repid-1.5.4/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_serializer.py` & `repid-1.5.4/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_utils.py` & `repid-1.5.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/tests/test_worker.py` & `repid-1.5.4/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.3/PKG-INFO` & `repid-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repid
-Version: 1.5.3
+Version: 1.5.4
 Summary: Repid framework: simple to use, fast to run and extensible to adopt job scheduler
 Author-Email: aleksul <me@aleksul.space>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repid Version: 1.5.3 Summary: Repid framework:
+Metadata-Version: 2.1 Name: repid Version: 1.5.4 Summary: Repid framework:
 simple to use, fast to run and extensible to adopt job scheduler Author-Email:
 aleksul
 aleksul.space> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

