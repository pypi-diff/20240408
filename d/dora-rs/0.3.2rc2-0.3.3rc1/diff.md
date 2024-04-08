# Comparing `tmp/dora_rs-0.3.2rc2.tar.gz` & `tmp/dora_rs-0.3.3rc1.tar.gz`

## Comparing `dora_rs-0.3.2rc2.tar` & `dora_rs-0.3.3rc1.tar`

### file list

```diff
@@ -1,145 +1,117 @@
--rw-r--r--   0     1001      127      490 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/telemetry/metrics/Cargo.toml
--rw-r--r--   0     1001      127     1317 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/telemetry/metrics/src/lib.rs
--rw-r--r--   0     1001      127      593 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/shared-memory-server/Cargo.toml
--rw-r--r--   0     1001      127     3249 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/shared-memory-server/src/bin/bench.rs
--rw-r--r--   0     1001      127     7343 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/shared-memory-server/src/channel.rs
--rw-r--r--   0     1001      127     2019 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/shared-memory-server/src/lib.rs
--rw-r--r--   0     1001      127      661 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/Cargo.toml
--rw-r--r--   0     1001      127     9127 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/src/config.rs
--rw-r--r--   0     1001      127      957 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/src/coordinator_messages.rs
--rw-r--r--   0     1001      127     6895 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/src/daemon_messages.rs
--rw-r--r--   0     1001      127     8998 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/src/descriptor/mod.rs
--rw-r--r--   0     1001      127     7070 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/src/descriptor/validate.rs
--rw-r--r--   0     1001      127     7349 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/src/descriptor/visualize.rs
--rw-r--r--   0     1001      127     2397 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/src/lib.rs
--rw-r--r--   0     1001      127     2066 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/core/src/topics.rs
--rw-r--r--   0     1001      127      323 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/arrow-convert/Cargo.toml
--rw-r--r--   0     1001      127     5495 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/arrow-convert/src/from_impls.rs
--rw-r--r--   0     1001      127     3744 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/arrow-convert/src/into_impls.rs
--rw-r--r--   0     1001      127      485 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/arrow-convert/src/lib.rs
--rw-r--r--   0     1001      127     1118 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/Cargo.toml
--rw-r--r--   0     1001      127      451 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/src/_core/mod.rs
--rw-r--r--   0     1001      127     4114 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/src/_core/sequence.rs
--rw-r--r--   0     1001      127     5495 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/src/_core/string.rs
--rw-r--r--   0     1001      127     2444 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/src/_core/traits.rs
--rw-r--r--   0     1001      127      145 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/src/lib.rs
--rw-r--r--   0     1001      127      288 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/Cargo.toml
--rw-r--r--   0     1001      127      787 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/build.rs
--rw-r--r--   0     1001      127      282 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs
--rw-r--r--   0     1001      127     3703 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs
--rw-r--r--   0     1001      127     2848 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs
--rw-r--r--   0     1001      127      776 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs
--rw-r--r--   0     1001      127     2257 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs
--rw-r--r--   0     1001      127     9363 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs
--rw-r--r--   0     1001      127     4376 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs
--rw-r--r--   0     1001      127     4024 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs
--rw-r--r--   0     1001      127      191 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/mod.rs
--rw-r--r--   0     1001      127     4316 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs
--rw-r--r--   0     1001      127     2607 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs
--rw-r--r--   0     1001      127    10849 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs
--rw-r--r--   0     1001      127     7208 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs
--rw-r--r--   0     1001      127     1942 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs
--rw-r--r--   0     1001      127     4429 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs
--rw-r--r--   0     1001      127     9102 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs
--rw-r--r--   0     1001      127      299 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/mod.rs
--rw-r--r--   0     1001      127     2220 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs
--rw-r--r--   0     1001      127    12273 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs
--rw-r--r--   0     1001      127     3402 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs
--rw-r--r--   0     1001      127     1982 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs
--rw-r--r--   0     1001      127      100 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/action/Fibonacci.action
--rw-r--r--   0     1001      127     1271 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg
--rw-r--r--   0     1001      127      240 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BasicTypes.msg
--rw-r--r--   0     1001      127     1346 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg
--rw-r--r--   0     1001      127      315 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Constants.msg
--rw-r--r--   0     1001      127      315 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Defaults.msg
--rw-r--r--   0     1001      127        0 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Empty.msg
--rw-r--r--   0     1001      127      484 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/MultiNested.msg
--rw-r--r--   0     1001      127       29 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Nested.msg
--rw-r--r--   0     1001      127      591 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg
--rw-r--r--   0     1001      127     1255 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg
--rw-r--r--   0     1001      127      415 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/WStrings.msg
--rw-r--r--   0     1001      127     2282 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv
--rw-r--r--   0     1001      127      524 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv
--rw-r--r--   0     1001      127        4 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Empty.srv
--rw-r--r--   0     1001      127      370 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/Cargo.toml
--rw-r--r--   0     1001      127      787 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/build.rs
--rw-r--r--   0     1001      127     1135 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/src/lib.rs
--rw-r--r--   0     1001      127      100 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/action/Fibonacci.action
--rw-r--r--   0     1001      127     1271 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/Arrays.msg
--rw-r--r--   0     1001      127      240 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/BasicTypes.msg
--rw-r--r--   0     1001      127     1346 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/BoundedSequences.msg
--rw-r--r--   0     1001      127      315 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/Constants.msg
--rw-r--r--   0     1001      127      315 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/Defaults.msg
--rw-r--r--   0     1001      127        0 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/Empty.msg
--rw-r--r--   0     1001      127      484 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/MultiNested.msg
--rw-r--r--   0     1001      127       29 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/Nested.msg
--rw-r--r--   0     1001      127      591 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/Strings.msg
--rw-r--r--   0     1001      127     1255 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/UnboundedSequences.msg
--rw-r--r--   0     1001      127      415 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/msg/WStrings.msg
--rw-r--r--   0     1001      127     2282 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/srv/Arrays.srv
--rw-r--r--   0     1001      127      524 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/srv/BasicTypes.srv
--rw-r--r--   0     1001      127        4 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen-macro/test_msgs/srv/Empty.srv
--rw-r--r--   0     1001      127      549 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/python/operator/Cargo.toml
--rw-r--r--   0     1001      127     7969 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/python/operator/src/lib.rs
--rw-r--r--   0     1001      127     1647 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/runtime/Cargo.toml
--rw-r--r--   0     1001      127    13520 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/runtime/src/lib.rs
--rw-r--r--   0     1001      127     4296 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/runtime/src/operator/channel.rs
--rw-r--r--   0     1001      127     2639 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/runtime/src/operator/mod.rs
--rw-r--r--   0     1001      127    15170 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/runtime/src/operator/python.rs
--rw-r--r--   0     1001      127    10650 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/runtime/src/operator/shared_lib.rs
--rw-r--r--   0     1001      127      424 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/Cargo.toml
--rw-r--r--   0     1001      127     9105 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/lib.rs
--rw-r--r--   0     1001      127     3515 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/qos.rs
--rw-r--r--   0     1001      127      729 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs
--rw-r--r--   0     1001      127     6330 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs
--rw-r--r--   0     1001      127     4726 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs
--rw-r--r--   0     1001      127     6326 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs
--rw-r--r--   0     1001      127     1154 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs
--rw-r--r--   0     1001      127     4263 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/mod.rs
--rw-r--r--   0     1001      127     9390 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs
--rw-r--r--   0     1001      127     9481 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs
--rw-r--r--   0     1001      127     7776 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs
--rw-r--r--   0     1001      127     3086 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs
--rw-r--r--   0     1001      127     9552 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs
--rw-r--r--   0     1001      127    11898 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/test_utils.py
--rw-r--r--   0     1001      127     1128 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/Cargo.toml
--rw-r--r--   0     1001      127     4399 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/coordinator.rs
--rw-r--r--   0     1001      127     4602 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/inter_daemon.rs
--rw-r--r--   0     1001      127    56723 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/lib.rs
--rw-r--r--   0     1001      127      200 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/log.rs
--rw-r--r--   0     1001      127    21735 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/node_communication/mod.rs
--rw-r--r--   0     1001      127     2624 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/node_communication/shmem.rs
--rw-r--r--   0     1001      127     2864 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/node_communication/tcp.rs
--rw-r--r--   0     1001      127     6427 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/pending.rs
--rw-r--r--   0     1001      127    12404 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/spawn.rs
--rw-r--r--   0     1001      127      722 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/binaries/daemon/src/tcp_utils.rs
--rw-r--r--   0     1001      127      461 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/operator/types/Cargo.toml
--rw-r--r--   0     1001      127     4237 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/operator/types/src/lib.rs
--rw-r--r--   0     1001      127      452 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/download/Cargo.toml
--rw-r--r--   0     1001      127     1285 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/download/src/lib.rs
--rw-r--r--   0     1001      127      583 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/telemetry/tracing/Cargo.toml
--rw-r--r--   0     1001      127     1620 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/telemetry/tracing/src/lib.rs
--rw-r--r--   0     1001      127     2388 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/extensions/telemetry/tracing/src/telemetry.rs
--rw-r--r--   0     1001      127      451 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/message/Cargo.toml
--rw-r--r--   0     1001      127     4223 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/libraries/message/src/lib.rs
--rw-r--r--   0     1001      127      733 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/Cargo.toml
--rw-r--r--   0     1001      127     2429 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/daemon_connection/mod.rs
--rw-r--r--   0     1001      127     2149 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/daemon_connection/tcp.rs
--rw-r--r--   0     1001      127     3457 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/event_stream/event.rs
--rw-r--r--   0     1001      127     3100 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/event_stream/merged.rs
--rw-r--r--   0     1001      127     8375 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/event_stream/mod.rs
--rw-r--r--   0     1001      127     9280 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/event_stream/thread.rs
--rw-r--r--   0     1001      127      764 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/lib.rs
--rw-r--r--   0     1001      127     2597 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/node/arrow_utils.rs
--rw-r--r--   0     1001      127     3654 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/node/control_channel.rs
--rw-r--r--   0     1001      127     5795 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/node/drop_stream.rs
--rw-r--r--   0     1001      127    14194 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/rust/node/src/node/mod.rs
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 dora_rs-0.3.2rc2/apis/python/node/Cargo.toml
--rw-r--r--   0     1001      127      201 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/python/node/README.md
--rw-r--r--   0     1001      127      518 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/python/node/dora/__init__.py
--rw-r--r--   0     1001      127     6852 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/apis/python/node/src/lib.rs
--rw-r--r--   0     1001      127   166279 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/Cargo.lock
--rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 dora_rs-0.3.2rc2/Cargo.toml
--rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dora_rs-0.3.2rc2/pyproject.toml
--rw-r--r--   0     1001      127      518 2024-01-29 09:45:56.000000 dora_rs-0.3.2rc2/dora/__init__.py
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 dora_rs-0.3.2rc2/PKG-INFO
+-rw-r--r--   0     1001      127      323 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/Cargo.toml
+-rw-r--r--   0     1001      127     5495 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/from_impls.rs
+-rw-r--r--   0     1001      127     3744 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/into_impls.rs
+-rw-r--r--   0     1001      127      485 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/lib.rs
+-rw-r--r--   0     1001      127      452 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/download/Cargo.toml
+-rw-r--r--   0     1001      127     1285 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/download/src/lib.rs
+-rw-r--r--   0     1001      127      461 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/operator/types/Cargo.toml
+-rw-r--r--   0     1001      127     4911 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/operator/types/src/lib.rs
+-rw-r--r--   0     1001      127      288 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/Cargo.toml
+-rw-r--r--   0     1001      127      787 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/build.rs
+-rw-r--r--   0     1001      127    10910 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs
+-rw-r--r--   0     1001      127     3703 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs
+-rw-r--r--   0     1001      127     2848 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs
+-rw-r--r--   0     1001      127      776 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs
+-rw-r--r--   0     1001      127     2257 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs
+-rw-r--r--   0     1001      127     9363 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs
+-rw-r--r--   0     1001      127     4376 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs
+-rw-r--r--   0     1001      127     4024 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs
+-rw-r--r--   0     1001      127      191 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/mod.rs
+-rw-r--r--   0     1001      127     4327 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs
+-rw-r--r--   0     1001      127     2607 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs
+-rw-r--r--   0     1001      127    10849 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs
+-rw-r--r--   0     1001      127     7208 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs
+-rw-r--r--   0     1001      127     1942 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs
+-rw-r--r--   0     1001      127     4429 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs
+-rw-r--r--   0     1001      127    20805 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs
+-rw-r--r--   0     1001      127      299 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/mod.rs
+-rw-r--r--   0     1001      127     3789 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs
+-rw-r--r--   0     1001      127    12158 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs
+-rw-r--r--   0     1001      127     3382 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs
+-rw-r--r--   0     1001      127    11907 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs
+-rw-r--r--   0     1001      127      100 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/action/Fibonacci.action
+-rw-r--r--   0     1001      127     1271 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg
+-rw-r--r--   0     1001      127      240 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BasicTypes.msg
+-rw-r--r--   0     1001      127     1346 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg
+-rw-r--r--   0     1001      127      315 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Constants.msg
+-rw-r--r--   0     1001      127      315 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Defaults.msg
+-rw-r--r--   0     1001      127        0 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Empty.msg
+-rw-r--r--   0     1001      127      484 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/MultiNested.msg
+-rw-r--r--   0     1001      127       29 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Nested.msg
+-rw-r--r--   0     1001      127      591 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg
+-rw-r--r--   0     1001      127     1255 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg
+-rw-r--r--   0     1001      127      415 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/WStrings.msg
+-rw-r--r--   0     1001      127     2282 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv
+-rw-r--r--   0     1001      127      524 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv
+-rw-r--r--   0     1001      127        4 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Empty.srv
+-rw-r--r--   0     1001      127      593 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/Cargo.toml
+-rw-r--r--   0     1001      127     3249 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/bin/bench.rs
+-rw-r--r--   0     1001      127     7343 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/channel.rs
+-rw-r--r--   0     1001      127     2019 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/lib.rs
+-rw-r--r--   0     1001      127      733 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/Cargo.toml
+-rw-r--r--   0     1001      127     2429 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/mod.rs
+-rw-r--r--   0     1001      127     2149 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/tcp.rs
+-rw-r--r--   0     1001      127     3457 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/event.rs
+-rw-r--r--   0     1001      127     3100 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/merged.rs
+-rw-r--r--   0     1001      127     8375 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/mod.rs
+-rw-r--r--   0     1001      127     9280 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/thread.rs
+-rw-r--r--   0     1001      127      764 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/lib.rs
+-rw-r--r--   0     1001      127     2553 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/arrow_utils.rs
+-rw-r--r--   0     1001      127     3654 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/control_channel.rs
+-rw-r--r--   0     1001      127     5795 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/drop_stream.rs
+-rw-r--r--   0     1001      127    14352 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/mod.rs
+-rw-r--r--   0     1001      127      561 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/Cargo.toml
+-rw-r--r--   0     1001      127     1836 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/src/lib.rs
+-rw-r--r--   0     1001      127      424 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/Cargo.toml
+-rw-r--r--   0     1001      127     9105 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/lib.rs
+-rw-r--r--   0     1001      127     3515 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/qos.rs
+-rw-r--r--   0     1001      127      729 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs
+-rw-r--r--   0     1001      127     6330 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs
+-rw-r--r--   0     1001      127     4726 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs
+-rw-r--r--   0     1001      127     6326 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs
+-rw-r--r--   0     1001      127     1154 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs
+-rw-r--r--   0     1001      127     4263 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/mod.rs
+-rw-r--r--   0     1001      127     9390 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs
+-rw-r--r--   0     1001      127     9481 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs
+-rw-r--r--   0     1001      127     7776 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs
+-rw-r--r--   0     1001      127     3086 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs
+-rw-r--r--   0     1001      127     9552 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs
+-rw-r--r--   0     1001      127    11898 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/test_utils.py
+-rw-r--r--   0     1001      127      451 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/message/Cargo.toml
+-rw-r--r--   0     1001      127     4223 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/message/src/lib.rs
+-rw-r--r--   0     1001      127      549 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/operator/Cargo.toml
+-rw-r--r--   0     1001      127     7968 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/operator/src/lib.rs
+-rw-r--r--   0     1001      127      665 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/Cargo.toml
+-rw-r--r--   0     1001      127     9127 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/config.rs
+-rw-r--r--   0     1001      127      957 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/coordinator_messages.rs
+-rw-r--r--   0     1001      127     6944 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/daemon_messages.rs
+-rw-r--r--   0     1001      127    10351 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/mod.rs
+-rw-r--r--   0     1001      127     7260 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/validate.rs
+-rw-r--r--   0     1001      127     7349 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/visualize.rs
+-rw-r--r--   0     1001      127     2397 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/lib.rs
+-rw-r--r--   0     1001      127     2066 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/topics.rs
+-rw-r--r--   0     1001      127     1431 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/Cargo.toml
+-rw-r--r--   0     1001      127    13120 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/lib.rs
+-rw-r--r--   0     1001      127     4296 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/channel.rs
+-rw-r--r--   0     1001      127     2639 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/mod.rs
+-rw-r--r--   0     1001      127    15169 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/python.rs
+-rw-r--r--   0     1001      127    10280 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/shared_lib.rs
+-rw-r--r--   0     1001      127      583 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/Cargo.toml
+-rw-r--r--   0     1001      127     1620 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/lib.rs
+-rw-r--r--   0     1001      127     2388 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/telemetry.rs
+-rw-r--r--   0     1001      127     1364 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/Cargo.toml
+-rw-r--r--   0     1001      127     1493 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/build.rs
+-rw-r--r--   0     1001      127      276 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/mod.rs
+-rw-r--r--   0     1001      127     4114 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/sequence.rs
+-rw-r--r--   0     1001      127     5495 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/string.rs
+-rw-r--r--   0     1001      127     2337 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/traits.rs
+-rw-r--r--   0     1001      127      223 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/lib.rs
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/apis/python/node/Cargo.toml
+-rw-r--r--   0     1001      127      201 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/README.md
+-rw-r--r--   0     1001      127      518 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/dora/__init__.py
+-rw-r--r--   0     1001      127     6852 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/src/lib.rs
+-rw-r--r--   0     1001      127   169924 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/Cargo.lock
+-rw-r--r--   0        0        0     3959 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/Cargo.toml
+-rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/pyproject.toml
+-rw-r--r--   0     1001      127      518 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/dora/__init__.py
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/PKG-INFO
```

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/telemetry/metrics/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -6,33 +6,44 @@
 //! - CPU usage.
 //! - Memory and Virtual memory usage.
 //! - disk usage (read and write).
 //!
 //! [`sysinfo`]: https://github.com/GuillaumeGomez/sysinfo
 //! [`opentelemetry-rust`]: https://github.com/open-telemetry/opentelemetry-rust
 
-use opentelemetry::metrics::{self};
-use opentelemetry_sdk::{metrics::MeterProvider, runtime};
+use std::time::Duration;
 
+use eyre::{Context, Result};
+use opentelemetry::metrics::{self, MeterProvider as _};
 use opentelemetry_otlp::{ExportConfig, WithExportConfig};
+use opentelemetry_sdk::{metrics::SdkMeterProvider, runtime};
+use opentelemetry_system_metrics::init_process_observer;
 /// Init opentelemetry meter
 ///
 /// Use the default Opentelemetry exporter with default config
 /// TODO: Make Opentelemetry configurable
 ///
-pub fn init_metrics() -> metrics::Result<MeterProvider> {
+pub fn init_metrics() -> metrics::Result<SdkMeterProvider> {
     let endpoint = std::env::var("OTEL_EXPORTER_OTLP_METRICS_ENDPOINT")
         .unwrap_or_else(|_| "http://localhost:4317".to_string());
     let export_config = ExportConfig {
         endpoint,
         ..ExportConfig::default()
     };
 
     opentelemetry_otlp::new_pipeline()
         .metrics(runtime::Tokio)
         .with_exporter(
             opentelemetry_otlp::new_exporter()
                 .tonic()
                 .with_export_config(export_config),
         )
+        .with_period(Duration::from_secs(10))
         .build()
 }
+
+pub fn init_meter_provider(meter_id: String) -> Result<SdkMeterProvider> {
+    let meter_provider = init_metrics().context("Could not create opentelemetry meter")?;
+    let meter = meter_provider.meter(meter_id);
+    let _ = init_process_observer(meter).context("could not initiale system metrics observer")?;
+    Ok(meter_provider)
+}
```

### Comparing `dora_rs-0.3.2rc2/libraries/shared-memory-server/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/shared-memory-server/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/shared-memory-server/src/bin/bench.rs` & `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/bin/bench.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/shared-memory-server/src/channel.rs` & `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/shared-memory-server/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/core/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
 [dependencies]
 eyre = "0.6.8"
 serde = { version = "1.0.136", features = ["derive"] }
 serde_yaml = "0.9.11"
 once_cell = "1.13.0"
 which = "5.0.0"
-uuid = { version = "1.2.1", features = ["serde"] }
+uuid = { version = "1.7", features = ["serde", "v7"] }
 dora-message = { workspace = true }
 tracing = "0.1"
 serde-with-expand-env = "1.1.0"
 tokio = { version = "1.24.1", features = ["fs", "process", "sync"] }
 aligned-vec = { version = "0.5.0", features = ["serde"] }
```

### Comparing `dora_rs-0.3.2rc2/libraries/core/src/config.rs` & `dora_rs-0.3.3rc1/libraries/core/src/config.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/core/src/coordinator_messages.rs` & `dora_rs-0.3.3rc1/libraries/core/src/coordinator_messages.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/core/src/daemon_messages.rs` & `dora_rs-0.3.3rc1/libraries/core/src/daemon_messages.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 use crate::{
     config::{DataId, NodeId, NodeRunConfig, OperatorId},
     descriptor::{Descriptor, OperatorDefinition, ResolvedNode},
 };
 use aligned_vec::{AVec, ConstAlign};
 use dora_message::{uhlc, Metadata};
-use uuid::Uuid;
+use uuid::{NoContext, Timestamp, Uuid};
 
 #[derive(Debug, serde::Serialize, serde::Deserialize)]
 pub struct NodeConfig {
     pub dataflow_id: DataflowId,
     pub node_id: NodeId,
     pub run_config: NodeRunConfig,
     pub daemon_communication: DaemonCommunication,
@@ -174,15 +174,15 @@
 #[derive(
     Debug, Copy, Clone, PartialEq, Eq, PartialOrd, Ord, Hash, serde::Serialize, serde::Deserialize,
 )]
 pub struct DropToken(Uuid);
 
 impl DropToken {
     pub fn generate() -> Self {
-        Self(Uuid::new_v4())
+        Self(Uuid::new_v7(Timestamp::now(NoContext)))
     }
 }
 
 #[derive(Debug, serde::Serialize, serde::Deserialize)]
 pub enum InputData {
     SharedMemory(SharedMemoryInput),
     Vec(Vec<u8>),
```

### Comparing `dora_rs-0.3.2rc2/libraries/core/src/descriptor/mod.rs` & `dora_rs-0.3.3rc1/libraries/core/src/descriptor/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 use crate::config::{
     CommunicationConfig, DataId, Input, InputMapping, NodeId, NodeRunConfig, OperatorId,
 };
-use eyre::{bail, Context, Result};
+use eyre::{bail, eyre, Context, Result};
 use serde::{Deserialize, Serialize};
 use serde_with_expand_env::with_expand_envs;
 use std::{
     collections::{BTreeMap, BTreeSet, HashMap},
     env::consts::EXE_EXTENSION,
     fmt,
     path::{Path, PathBuf},
 };
+use tracing::warn;
 pub use visualize::collect_dora_timers;
 
 mod validate;
 mod visualize;
 pub const SHELL_SOURCE: &str = "shell";
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
@@ -160,14 +161,41 @@
     #[serde(default)]
     pub deploy: ResolvedDeploy,
 
     #[serde(flatten)]
     pub kind: CoreNodeKind,
 }
 
+impl ResolvedNode {
+    pub fn send_stdout_as(&self) -> Result<Option<String>> {
+        match &self.kind {
+            // TODO: Split stdout between operators
+            CoreNodeKind::Runtime(n) => {
+                let count = n
+                    .operators
+                    .iter()
+                    .filter(|op| op.config.send_stdout_as.is_some())
+                    .count();
+                if count == 1 && n.operators.len() > 1 {
+                    warn!("All stdout from all operators of a runtime are going to be sent in the selected `send_stdout_as` operator.")
+                } else if count > 1 {
+                    return Err(eyre!("More than one `send_stdout_as` entries for a runtime node. Please only use one `send_stdout_as` per runtime."));
+                }
+                Ok(n.operators.iter().find_map(|op| {
+                    op.config
+                        .send_stdout_as
+                        .clone()
+                        .map(|stdout| format!("{}/{}", op.id, stdout))
+                }))
+            }
+            CoreNodeKind::Custom(n) => Ok(n.send_stdout_as.clone()),
+        }
+    }
+}
+
 #[derive(Debug, Clone, Default, Serialize, Deserialize)]
 pub struct ResolvedDeploy {
     pub machine: String,
 }
 impl ResolvedDeploy {
     fn new(deploy: Deploy, descriptor: &Descriptor) -> Self {
         let default_machine = descriptor.deploy.machine.as_deref().unwrap_or_default();
@@ -220,14 +248,16 @@
     pub outputs: BTreeSet<DataId>,
 
     #[serde(flatten)]
     pub source: OperatorSource,
 
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub build: Option<String>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub send_stdout_as: Option<String>,
 }
 
 #[derive(Debug, Serialize, Deserialize, Clone)]
 #[serde(rename_all = "kebab-case")]
 pub enum OperatorSource {
     SharedLibrary(String),
     Python(String),
@@ -271,14 +301,16 @@
 pub struct CustomNode {
     pub source: String,
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub args: Option<String>,
     pub envs: Option<BTreeMap<String, EnvValue>>,
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub build: Option<String>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub send_stdout_as: Option<String>,
 
     #[serde(flatten)]
     pub run_config: NodeRunConfig,
 }
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 #[serde(untagged)]
```

### Comparing `dora_rs-0.3.2rc2/libraries/core/src/descriptor/validate.rs` & `dora_rs-0.3.3rc1/libraries/core/src/descriptor/validate.rs`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,20 @@
                         )?;
                     }
                 }
             }
         };
     }
 
+    // Check that nodes can resolve `send_stdout_as`
+    for node in &nodes {
+        node.send_stdout_as()
+            .context("Could not resolve `send_stdout_as` configuration")?;
+    }
+
     if has_python_operator {
         check_python_runtime()?;
     }
 
     Ok(())
 }
```

### Comparing `dora_rs-0.3.2rc2/libraries/core/src/descriptor/visualize.rs` & `dora_rs-0.3.3rc1/libraries/core/src/descriptor/visualize.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/core/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/core/src/topics.rs` & `dora_rs-0.3.3rc1/libraries/core/src/topics.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/arrow-convert/src/from_impls.rs` & `dora_rs-0.3.3rc1/libraries/arrow-convert/src/from_impls.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/arrow-convert/src/into_impls.rs` & `dora_rs-0.3.3rc1/libraries/arrow-convert/src/into_impls.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 [package]
 name = "dora-ros2-bridge"
 version = "0.1.0"
 edition = "2021"
+links = "dora-ros2-bridge"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [features]
 default = ["generate-messages"]
-generate-messages = ["dep:dora-ros2-bridge-msg-gen-macro"]
+generate-messages = ["dep:dora-ros2-bridge-msg-gen", "dep:rust-format"]
 # enables examples that depend on a sourced ROS2 installation
-ros2-examples = ["eyre", "tokio", "dora-daemon"]
+ros2-examples = ["dep:eyre", "tokio", "dora-daemon"]
 
 [dependencies]
 array-init = "2.1.0"
-dora-ros2-bridge-msg-gen-macro = { path = "msg-gen-macro", optional = true }
 serde = { version = "1.0.164", features = ["derive"] }
 serde-big-array = "0.5.1"
 widestring = "1.0.2"
 ros2-client = { git = "https://github.com/dora-rs/ros2-client.git", branch = "deserialize-seed-2" }
 rustdds = { git = "https://github.com/dora-rs/RustDDS.git", branch = "deserialize-seed-2" }
 eyre = { version = "0.6.8", optional = true }
 tokio = { version = "1.29.1", features = ["full"], optional = true }
 dora-daemon = { path = "../../../binaries/daemon", optional = true }
 tracing = "0.1.37"
 tracing-subscriber = "0.3.17"
+flume = "0.11.0"
+futures = { version = "0.3.21", features = ["thread-pool"] }
+futures-timer = "3.0.3"
 
 [dev-dependencies]
 rand = "0.8.5"
 futures = { version = "0.3.28", default-features = false }
+
+[build-dependencies]
+dora-ros2-bridge-msg-gen = { workspace = true, optional = true }
+rust-format = { version = "0.3.4", features = [
+    "pretty_please",
+], optional = true }
```

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/src/_core/sequence.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/src/_core/string.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/string.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/src/_core/traits.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/traits.rs`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,20 @@
     }
 
     unsafe fn to_raw_ref(&self) -> Self::RawRef {
         Self::RawRef::from_rust(self)
     }
 }
 
-pub trait ServiceT: Send {
-    type Request: MessageT;
-    type Response: MessageT;
-}
-
 pub trait ActionT: Send {
     type Goal: MessageT;
     type Result: MessageT;
     type Feedback: MessageT;
-    type SendGoal: ServiceT;
-    type GetResult: ServiceT;
+    type SendGoal;
+    type GetResult;
     type FeedbackMessage: MessageT;
 }
 
 // I was going to use `std::default::Default`, however generic arrays do not implement `std::default::Default`.
 pub trait InternalDefault {
     fn _default() -> Self;
 }
```

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/build.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/build.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,21 @@
             }
         }
         packages.push(package);
     }
     Ok(packages)
 }
 
-pub fn get_packages(paths: &[&Path]) -> Result<Vec<Package>> {
+pub fn get_packages<P>(paths: &[P]) -> Result<Vec<Package>>
+where
+    P: AsRef<Path>,
+{
     let mut packages = paths
         .iter()
-        .map(|&path| get_ros_msgs_each_package(path))
+        .map(get_ros_msgs_each_package)
         .collect::<Result<Vec<_>>>()?
         .into_iter()
         .flatten()
         .filter(|p| !p.is_empty())
         .collect::<Vec<_>>();
 
     packages.sort_by_key(|p| p.name.clone());
```

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs`

 * *Files 2% similar despite different names*

```diff
@@ -127,17 +127,17 @@
 /// A type identified by the name
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub struct NamedType(pub String);
 
 impl NamedType {
     fn type_tokens(&self, package: &str) -> impl ToTokens {
         let package = Ident::new(package, Span::call_site());
-        let namespace = Ident::new("msg", Span::call_site());
         let name = Ident::new(&self.0, Span::call_site());
-        quote! { crate::#package::#namespace::#name }
+        let ident = format_ident!("{package}__{name}");
+        quote! { #ident }
     }
 
     fn raw_type_tokens(&self, package: &str) -> impl ToTokens {
         let package = Ident::new(package, Span::call_site());
         let namespace = Ident::new("msg", Span::call_site());
         let name = format_ident!("{}_Raw", self.0);
         quote! { crate::#package::#namespace::#name }
@@ -169,17 +169,17 @@
     /// e.g. `Bool`
     pub name: String,
 }
 
 impl NamespacedType {
     fn type_tokens(&self) -> impl ToTokens {
         let package = Ident::new(&self.package, Span::call_site());
-        let namespace = Ident::new(&self.namespace, Span::call_site());
         let name = Ident::new(&self.name, Span::call_site());
-        quote! { crate::#package::#namespace::#name }
+        let ident = format_ident!("{package}__{name}");
+        quote! { #ident }
     }
 
     fn raw_type_tokens(&self) -> impl ToTokens {
         let package = Ident::new(&self.package, Span::call_site());
         let namespace = Ident::new(&self.namespace, Span::call_site());
         let name = format_ident!("{}_Raw", self.name);
         quote! { crate::#package::#namespace::#name }
@@ -211,17 +211,17 @@
 impl GenericString {
     const fn is_wide(self) -> bool {
         matches!(self, Self::WString | Self::BoundedWString(_))
     }
 
     fn type_tokens(self) -> impl ToTokens {
         if self.is_wide() {
-            quote! { crate::_core::string::U16String }
+            quote! { U16String }
         } else {
-            quote! { ::std::string::String }
+            quote! { String }
         }
     }
 
     fn raw_type_tokens(self) -> impl ToTokens {
         if self.is_wide() {
             quote! { crate::_core::FFIWString }
         } else {
```

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     /// The type of the elements
     pub value_type: NestableType,
 }
 
 impl Sequence {
     pub fn type_tokens(&self, package: &str) -> impl ToTokens {
         let inner_type = self.value_type.type_tokens(package);
-        quote! { std::vec::Vec<#inner_type> }
+        quote! { Vec<#inner_type> }
     }
 
     pub fn raw_type_tokens(&self, package: &str) -> impl ToTokens {
         let inner_type = self.value_type.raw_type_tokens(package);
         quote! { crate::_core::FFISeq<#inner_type> }
     }
 
@@ -68,15 +68,15 @@
     /// The maximum number of elements in the sequence
     pub max_size: usize,
 }
 
 impl BoundedSequence {
     pub fn type_tokens(&self, package: &str) -> impl ToTokens {
         let inner_type = self.value_type.type_tokens(package);
-        quote! { std::vec::Vec<#inner_type> }
+        quote! { Vec<#inner_type> }
     }
 
     pub fn raw_type_tokens(&self, package: &str) -> impl ToTokens {
         let inner_type = self.value_type.raw_type_tokens(package);
         quote! { crate::_core::FFISeq<#inner_type> }
     }
```

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/python/operator/Cargo.toml` & `dora_rs-0.3.3rc1/apis/python/operator/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/python/operator/src/lib.rs` & `dora_rs-0.3.3rc1/apis/python/operator/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     };
     use eyre::{Context, Result};
 
     fn assert_roundtrip(arrow_array: &ArrayData) -> Result<()> {
         let size = required_data_size(arrow_array);
         let mut sample: AVec<u8, ConstAlign<128>> = AVec::__from_elem(128, 0, size);
 
-        let info = copy_array_into_sample(&mut sample, arrow_array)?;
+        let info = copy_array_into_sample(&mut sample, arrow_array);
 
         let serialized_deserialized_arrow_array = RawData::Vec(sample)
             .into_arrow_array(&info)
             .context("Could not create arrow array")?;
         assert_eq!(arrow_array, &serialized_deserialized_arrow_array);
 
         Ok(())
```

### Comparing `dora_rs-0.3.2rc2/binaries/runtime/Cargo.toml` & `dora_rs-0.3.3rc1/binaries/runtime/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 [dependencies]
 dora-node-api = { workspace = true, default-features = false }
 dora-operator-api-python = { workspace = true, optional = true }
 dora-operator-api-types = { workspace = true }
 dora-core = { workspace = true }
 dora-tracing = { workspace = true, optional = true }
 dora-metrics = { workspace = true, optional = true }
-opentelemetry = { version = "0.21.0", features = ["metrics"], optional = true }
-opentelemetry-system-metrics = { version = "0.1.6", optional = true }
 eyre = "0.6.8"
 futures = "0.3.21"
 futures-concurrency = "7.1.0"
 libloading = "0.7.3"
 serde_yaml = "0.8.23"
 tokio = { version = "1.24.2", features = ["full"] }
 tokio-stream = "0.1.8"
@@ -33,10 +31,10 @@
 pythonize = { workspace = true, optional = true }
 arrow = { workspace = true, features = ["ffi"] }
 aligned-vec = "0.5.0"
 
 [features]
 default = ["tracing", "metrics"]
 tracing = ["dora-tracing"]
-telemetry = ["tracing", "opentelemetry", "tracing-opentelemetry"]
-metrics = ["opentelemetry", "opentelemetry-system-metrics", "dora-metrics"]
+telemetry = ["tracing", "tracing-opentelemetry"]
+metrics = ["dora-metrics"]
 python = ["pyo3", "dora-operator-api-python", "pythonize", "arrow/pyarrow"]
```

### Comparing `dora_rs-0.3.2rc2/binaries/runtime/src/lib.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #![warn(unsafe_op_in_unsafe_fn)]
 
 use dora_core::{
     config::{DataId, OperatorId},
     daemon_messages::{NodeConfig, RuntimeConfig},
     descriptor::OperatorConfig,
 };
+use dora_metrics::init_meter_provider;
 use dora_node_api::{DoraNode, Event};
 use eyre::{bail, Context, Result};
 use futures::{Stream, StreamExt};
 use futures_concurrency::stream::Merge;
 use operator::{run_operator, OperatorEvent, StopReason};
 
 #[cfg(feature = "tracing")]
 use dora_tracing::set_up_tracing;
 use std::{
-    borrow::Cow,
     collections::{BTreeMap, BTreeSet, HashMap},
     mem,
 };
 use tokio::{
     runtime::Builder,
     sync::{mpsc, oneshot},
 };
@@ -119,27 +119,15 @@
     operators: HashMap<OperatorId, OperatorConfig>,
     config: NodeConfig,
     operator_events: impl Stream<Item = RuntimeEvent> + Unpin,
     mut operator_channels: HashMap<OperatorId, flume::Sender<Event>>,
     init_done: oneshot::Receiver<Result<()>>,
 ) -> eyre::Result<()> {
     #[cfg(feature = "metrics")]
-    let _started = {
-        use dora_metrics::init_metrics;
-        use opentelemetry::global;
-        use opentelemetry_system_metrics::init_process_observer;
-
-        let _started = init_metrics().context("Could not create opentelemetry meter")?;
-        let meter = global::meter(Cow::Borrowed(Box::leak(
-            config.node_id.to_string().into_boxed_str(),
-        )));
-        init_process_observer(meter).context("could not initiale system metrics observer")?;
-        _started
-    };
-
+    let _meter_provider = init_meter_provider(config.node_id.to_string());
     init_done
         .await
         .wrap_err("the `init_done` channel was closed unexpectedly")?
         .wrap_err("failed to init an operator")?;
     tracing::info!("All operators are ready, starting runtime");
 
     let (mut node, mut daemon_events) = DoraNode::init(config)?;
```

### Comparing `dora_rs-0.3.2rc2/binaries/runtime/src/operator/channel.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/operator/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/binaries/runtime/src/operator/mod.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/binaries/runtime/src/operator/python.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/operator/python.rs`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
                 let mut sample = allocate_sample(data.len())?;
                 sample.copy_from_slice(data);
                 (sample, ArrowTypeInfo::byte_array(data.len()))
             } else if let Ok(arrow_array) = ArrayData::from_pyarrow(data.as_ref(py)) {
                 let total_len = required_data_size(&arrow_array);
                 let mut sample = allocate_sample(total_len)?;
 
-                let type_info = copy_array_into_sample(&mut sample, &arrow_array)?;
+                let type_info = copy_array_into_sample(&mut sample, &arrow_array);
 
                 (sample, type_info)
             } else {
                 eyre::bail!("invalid `data` type, must by `PyBytes` or arrow array")
             };
 
             py.allow_threads(|| {
```

### Comparing `dora_rs-0.3.2rc2/binaries/runtime/src/operator/shared_lib.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/operator/shared_lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             let DoraInitResult {
                 result,
                 operator_context,
             } = unsafe { (self.bindings.init_operator.init_operator)() };
             let raw = match result.error {
                 Some(error) => {
                     let _ = init_done.send(Err(eyre!(error.to_string())));
-                    bail!("init_operator failed: {}", String::from(error))
+                    bail!("init_operator failed: {}", *error)
                 }
                 None => operator_context,
             };
             OperatorContext {
                 raw,
                 drop_fn: self.bindings.drop_operator.clone(),
             }
@@ -122,51 +122,38 @@
             let parameters = MetadataParameters {
                 open_telemetry_context: open_telemetry_context.into(),
                 ..Default::default()
             };
 
             let arrow_array = match arrow::ffi::from_ffi(data_array, &schema) {
                 Ok(a) => a,
-                Err(err) => {
-                    return DoraResult {
-                        error: Some(err.to_string().into()),
-                    }
-                }
+                Err(err) => return DoraResult::from_error(err.to_string()),
             };
 
             let total_len = required_data_size(&arrow_array);
             let mut sample: AVec<u8, ConstAlign<128>> = AVec::__from_elem(128, 0, total_len);
 
-            let type_info = match copy_array_into_sample(&mut sample, &arrow_array) {
-                Ok(t) => t,
-                Err(err) => {
-                    return DoraResult {
-                        error: Some(err.to_string().into()),
-                    }
-                }
-            };
+            let type_info = copy_array_into_sample(&mut sample, &arrow_array);
 
             let event = OperatorEvent::Output {
                 output_id: DataId::from(String::from(output_id)),
                 type_info,
                 parameters,
                 data: Some(sample.into()),
             };
 
             let result = self
                 .events_tx
                 .blocking_send(event)
                 .map_err(|_| eyre!("failed to send output to runtime"));
 
-            let error = match result {
-                Ok(()) => None,
-                Err(_) => Some(String::from("runtime process closed unexpectedly").into()),
-            };
-
-            DoraResult { error }
+            match result {
+                Ok(()) => DoraResult::SUCCESS,
+                Err(_) => DoraResult::from_error("runtime process closed unexpectedly".into()),
+            }
         });
 
         let reason = loop {
             #[allow(unused_mut)]
             let Ok(mut event) = self.incoming_events.recv() else {
                 break StopReason::InputsClosed;
             };
@@ -257,15 +244,15 @@
                 (self.bindings.on_event.on_event)(
                     &mut operator_event,
                     &send_output,
                     operator_context.raw,
                 )
             };
             match error {
-                Some(error) => bail!("on_input failed: {}", String::from(error)),
+                Some(error) => bail!("on_input failed: {}", *error),
                 None => match status {
                     DoraStatus::Continue => {}
                     DoraStatus::Stop => break StopReason::ExplicitStop,
                     DoraStatus::StopAll => break StopReason::ExplicitStopAll,
                 },
             }
         };
```

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/qos.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/qos.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/mod.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/ros2-bridge/python/test_utils.py` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/operator/types/src/lib.rs` & `dora_rs-0.3.3rc1/apis/rust/operator/types/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 };
 use core::slice;
 use safer_ffi::{
     char_p::{self, char_p_boxed},
     closure::ArcDynFn1,
     derive_ReprC, ffi_export,
 };
-use std::path::Path;
+use std::{ops::Deref, path::Path};
 
 #[derive_ReprC]
 #[ffi_export]
 #[repr(C)]
 pub struct DoraInitOperator {
     pub init_operator: unsafe extern "C" fn() -> DoraInitResult,
 }
@@ -40,15 +40,39 @@
 }
 
 #[derive_ReprC]
 #[ffi_export]
 #[repr(C)]
 #[derive(Debug)]
 pub struct DoraResult {
-    pub error: Option<safer_ffi::String>,
+    pub error: Option<safer_ffi::boxed::Box<safer_ffi::String>>,
+}
+
+impl DoraResult {
+    pub const SUCCESS: Self = Self { error: None };
+
+    pub fn from_error(error: String) -> Self {
+        Self {
+            error: Some(Box::new(safer_ffi::String::from(error)).into()),
+        }
+    }
+
+    pub fn error(&self) -> Option<&str> {
+        self.error.as_deref().map(|s| s.deref())
+    }
+
+    pub fn into_result(self) -> Result<(), String> {
+        match self.error {
+            None => Ok(()),
+            Some(error) => {
+                let converted = safer_ffi::boxed::Box_::into(error);
+                Err((*converted).into())
+            }
+        }
+    }
 }
 
 #[derive_ReprC]
 #[ffi_export]
 #[repr(C)]
 pub struct DoraOnEvent {
     pub on_event: OnEventFn,
@@ -171,15 +195,15 @@
             },
         };
         Result::<_, String>::Ok(output)
     };
     match result() {
         Ok(output) => send_output.send_output.call(output),
         Err(error) => DoraResult {
-            error: Some(error.into()),
+            error: Some(Box::new(safer_ffi::String::from(error)).into()),
         },
     }
 }
 
 pub fn generate_headers(target_file: &Path) -> ::std::io::Result<()> {
     ::safer_ffi::headers::builder()
         .to_file(target_file)?
```

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/download/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/download/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/telemetry/tracing/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/telemetry/tracing/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/extensions/telemetry/tracing/src/telemetry.rs` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/libraries/message/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/message/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/Cargo.toml` & `dora_rs-0.3.3rc1/apis/rust/node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/daemon_connection/mod.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/daemon_connection/tcp.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/tcp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/event_stream/event.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/event.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/event_stream/merged.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/merged.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/event_stream/mod.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/event_stream/thread.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/thread.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/lib.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/node/arrow_utils.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/node/arrow_utils.rs`

 * *Files 11% similar despite different names*

```diff
@@ -16,27 +16,24 @@
         *next_offset += buffer.len();
     }
     for child in array.child_data() {
         required_data_size_inner(child, next_offset);
     }
 }
 
-pub fn copy_array_into_sample(
-    target_buffer: &mut [u8],
-    arrow_array: &ArrayData,
-) -> eyre::Result<ArrowTypeInfo> {
+pub fn copy_array_into_sample(target_buffer: &mut [u8], arrow_array: &ArrayData) -> ArrowTypeInfo {
     let mut next_offset = 0;
     copy_array_into_sample_inner(target_buffer, &mut next_offset, arrow_array)
 }
 
 fn copy_array_into_sample_inner(
     target_buffer: &mut [u8],
     next_offset: &mut usize,
     arrow_array: &ArrayData,
-) -> eyre::Result<ArrowTypeInfo> {
+) -> ArrowTypeInfo {
     let mut buffer_offsets = Vec::new();
     let layout = arrow::array::layout(arrow_array.data_type());
     for (buffer, spec) in arrow_array.buffers().iter().zip(&layout.buffers) {
         let len = buffer.len();
         assert!(
             target_buffer[*next_offset..].len() >= len,
             "target buffer too small (total_len: {}, offset: {}, required_len: {len})",
@@ -54,21 +51,21 @@
             len,
         });
         *next_offset += len;
     }
 
     let mut child_data = Vec::new();
     for child in arrow_array.child_data() {
-        let child_type_info = copy_array_into_sample_inner(target_buffer, next_offset, child)?;
+        let child_type_info = copy_array_into_sample_inner(target_buffer, next_offset, child);
         child_data.push(child_type_info);
     }
 
-    Ok(ArrowTypeInfo {
+    ArrowTypeInfo {
         data_type: arrow_array.data_type().clone(),
         len: arrow_array.len(),
         null_count: arrow_array.null_count(),
         validity: arrow_array.nulls().map(|b| b.validity().to_owned()),
         offset: arrow_array.offset(),
         buffer_offsets,
         child_data,
-    })
+    }
 }
```

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/node/control_channel.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/node/control_channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/node/drop_stream.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/node/drop_stream.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/apis/rust/node/src/node/mod.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/node/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     control_channel::ControlChannel,
     drop_stream::DropStream,
 };
 use aligned_vec::{AVec, ConstAlign};
 use arrow::array::Array;
 use dora_core::{
     config::{DataId, NodeId, NodeRunConfig},
-    daemon_messages::{DataMessage, DropToken, NodeConfig},
+    daemon_messages::{DataMessage, DataflowId, DropToken, NodeConfig},
     descriptor::Descriptor,
     message::{uhlc, ArrowTypeInfo, Metadata, MetadataParameters},
 };
 use eyre::{bail, WrapErr};
 use shared_memory_extended::{Shmem, ShmemConf};
 use std::{
     collections::{HashMap, VecDeque},
@@ -29,14 +29,15 @@
 mod control_channel;
 mod drop_stream;
 
 pub const ZERO_COPY_THRESHOLD: usize = 4096;
 
 pub struct DoraNode {
     id: NodeId,
+    dataflow_id: DataflowId,
     node_config: NodeRunConfig,
     control_channel: ControlChannel,
     clock: Arc<uhlc::HLC>,
 
     sent_out_shared_memory: HashMap<DropToken, ShmemHandle>,
     drop_stream: DropStream,
     cache: VecDeque<ShmemHandle>,
@@ -85,14 +86,15 @@
                 .wrap_err("failed to init drop stream")?;
         let control_channel =
             ControlChannel::init(dataflow_id, &node_id, &daemon_communication, clock.clone())
                 .wrap_err("failed to init control channel")?;
 
         let node = Self {
             id: node_id,
+            dataflow_id: dataflow_id,
             node_config: run_config,
             control_channel,
             clock,
             sent_out_shared_memory: HashMap::new(),
             drop_stream,
             cache: VecDeque::new(),
 
@@ -149,15 +151,15 @@
         data: impl Array,
     ) -> eyre::Result<()> {
         let arrow_array = data.to_data();
 
         let total_len = required_data_size(&arrow_array);
 
         let mut sample = self.allocate_data_sample(total_len)?;
-        let type_info = copy_array_into_sample(&mut sample, &arrow_array)?;
+        let type_info = copy_array_into_sample(&mut sample, &arrow_array);
 
         self.send_output_sample(output_id, type_info, parameters, Some(sample))
             .wrap_err("failed to send output")?;
 
         Ok(())
     }
 
@@ -239,14 +241,18 @@
         Ok(())
     }
 
     pub fn id(&self) -> &NodeId {
         &self.id
     }
 
+    pub fn dataflow_id(&self) -> &DataflowId {
+        &self.dataflow_id
+    }
+
     pub fn node_config(&self) -> &NodeRunConfig {
         &self.node_config
     }
 
     pub fn allocate_data_sample(&mut self, data_len: usize) -> eyre::Result<DataSample> {
         let data = if data_len >= ZERO_COPY_THRESHOLD {
             // create shared memory region
```

### Comparing `dora_rs-0.3.2rc2/apis/python/node/Cargo.toml` & `dora_rs-0.3.3rc1/apis/python/node/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [dependencies]
 dora-node-api = { workspace = true }
 dora-operator-api-python = { workspace = true }
 pyo3 = { workspace = true, features = ["eyre", "abi3-py37"] }
 eyre = "0.6"
 serde_yaml = "0.8.23"
 flume = "0.10.14"
-dora-runtime = { workspace = true, features = ["tracing", "python"] }
+dora-runtime = { workspace = true, features = ["tracing", "metrics", "python"] }
 arrow = { workspace = true, features = ["pyarrow"] }
 pythonize = { workspace = true }
 futures = "0.3.28"
 dora-ros2-bridge-python = { workspace = true }
 
 [lib]
 name = "dora"
```

### Comparing `dora_rs-0.3.2rc2/apis/python/node/dora/__init__.py` & `dora_rs-0.3.3rc1/apis/python/node/dora/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from enum import Enum
 
 from .dora import *
 
 __author__ = "Dora-rs Authors"
-__version__ = "0.3.2-rc2"
+__version__ = "0.3.3-rc1"
 
 
 class DoraStatus(Enum):
     """Dora status to indicate if operator `on_input` loop
      should be stopped.
 
     Args:
```

### Comparing `dora_rs-0.3.2rc2/apis/python/node/src/lib.rs` & `dora_rs-0.3.3rc1/apis/python/node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.2rc2/Cargo.lock` & `dora_rs-0.3.3rc1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4aa90d7ce82d4be67b64039a3d588d38dbcc6736577de4a847025ce5b0c468d1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "alloc-no-stdlib"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cc7bb162ec39d46ab1ca8c77bf72e890535becd1751bb45f64c597edb4c8c6b3"
+
+[[package]]
+name = "alloc-stdlib"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
+dependencies = [
+ "alloc-no-stdlib",
+]
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
@@ -401,45 +416,45 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c1da3ae8dabd9c00f453a329dfe1fb28da3c0a72e2478cdcd93171740c20499"
 dependencies = [
  "async-lock",
  "async-task",
  "concurrent-queue",
  "fastrand 2.0.1",
- "futures-lite",
+ "futures-lite 1.13.0",
  "slab",
 ]
 
 [[package]]
 name = "async-global-executor"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1b6f5d7df27bd294849f8eec66ecfc63d11814df7a4f5d74168a2394467b776"
 dependencies = [
  "async-channel 1.9.0",
  "async-executor",
  "async-io",
  "async-lock",
  "blocking",
- "futures-lite",
+ "futures-lite 1.13.0",
  "once_cell",
  "tokio",
 ]
 
 [[package]]
 name = "async-io"
 version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fc5b45d93ef0529756f812ca52e44c221b35341892d3dcc34132ac02f3dd2af"
 dependencies = [
  "async-lock",
  "autocfg",
  "cfg-if 1.0.0",
  "concurrent-queue",
- "futures-lite",
+ "futures-lite 1.13.0",
  "log",
  "parking",
  "polling",
  "rustix 0.37.25",
  "slab",
  "socket2 0.4.9",
  "waker-fn",
@@ -462,15 +477,15 @@
 dependencies = [
  "async-io",
  "async-lock",
  "autocfg",
  "blocking",
  "cfg-if 1.0.0",
  "event-listener 2.5.3",
- "futures-lite",
+ "futures-lite 1.13.0",
  "rustix 0.37.25",
  "signal-hook",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-rustls"
@@ -495,27 +510,49 @@
  "async-io",
  "async-lock",
  "async-process",
  "crossbeam-utils",
  "futures-channel",
  "futures-core",
  "futures-io",
- "futures-lite",
+ "futures-lite 1.13.0",
  "gloo-timers",
  "kv-log-macro",
  "log",
  "memchr",
  "once_cell",
  "pin-project-lite",
  "pin-utils",
  "slab",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
+name = "async-stream"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
+dependencies = [
+ "async-stream-impl",
+ "futures-core",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "async-stream-impl"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "async-task"
 version = "4.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9441c6b2fe128a7c2bf680a44c34d0df31ce09e5b7e401fcca3faa483dbc921"
 
 [[package]]
 name = "async-trait"
@@ -525,14 +562,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
+name = "atomic"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c59bdb34bc650a32731b31bd8f0829cc15d24a708ee31559e0bb34f2bc320cba"
+
+[[package]]
 name = "atomic-waker"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
 
 [[package]]
 name = "atty"
@@ -627,65 +670,65 @@
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
 [[package]]
 name = "bat"
-version = "0.23.0"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4b13b0233143ae151a66e0135d715b65f631d1028c40502cc88182bcb9f4fa"
+checksum = "9dcc9e5637c2330d8eb7b920f2aa5d9e184446c258466f825ea1412c7614cc86"
 dependencies = [
  "ansi_colours",
- "atty",
  "bincode",
  "bugreport",
  "bytesize",
  "clap 4.4.6",
  "clircle",
  "console",
  "content_inspector",
- "dirs 5.0.1",
- "encoding",
+ "encoding_rs",
+ "etcetera",
  "flate2",
  "git2",
  "globset",
  "grep-cli",
- "nu-ansi-term 0.47.0",
+ "home",
+ "nu-ansi-term 0.49.0",
  "once_cell",
  "path_abs",
  "plist",
  "regex",
  "semver",
  "serde",
- "serde_yaml 0.8.26",
+ "serde_yaml 0.9.30",
  "shell-words",
  "syntect",
  "thiserror",
  "unicode-width",
  "walkdir",
  "wild",
 ]
 
 [[package]]
 name = "benchmark-example-node"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "benchmark-example-sink"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
  "tracing",
  "tracing-subscriber",
 ]
 
@@ -744,20 +787,41 @@
 checksum = "94c4ef1f913d78636d78d538eec1f18de81e481f44b1be0a81060090530846e1"
 dependencies = [
  "async-channel 1.9.0",
  "async-lock",
  "async-task",
  "fastrand 2.0.1",
  "futures-io",
- "futures-lite",
+ "futures-lite 1.13.0",
  "piper",
  "tracing",
 ]
 
 [[package]]
+name = "brotli"
+version = "3.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "516074a47ef4bce09577a3b379392300159ce5b1ba2e501ff1c819950066100f"
+dependencies = [
+ "alloc-no-stdlib",
+ "alloc-stdlib",
+ "brotli-decompressor",
+]
+
+[[package]]
+name = "brotli-decompressor"
+version = "2.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e2e4afe60d7dd600fdd3de8d0f08c2b7ec039712e3b6137ff98b7004e82de4f"
+dependencies = [
+ "alloc-no-stdlib",
+ "alloc-stdlib",
+]
+
+[[package]]
 name = "bstr"
 version = "1.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c2f7349907b712260e64b0afe2f84692af14a454be26187d9df565c7f69266a"
 dependencies = [
  "memchr",
  "regex-automata 0.3.9",
@@ -965,17 +1029,17 @@
 name = "clap_lex"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd7cc57abe963c6d3b9d8be5b06ba7c8957a930305ca90304f24ef040aa6f961"
 
 [[package]]
 name = "clircle"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e68bbd985a63de680ab4d1ad77b6306611a8f961b282c8b5ab513e6de934e396"
+checksum = "c8e87cbed5354f17bd8ca8821a097fb62599787fe8f611743fad7ee156a0a600"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
  "serde",
  "winapi 0.3.9",
 ]
 
@@ -1003,23 +1067,23 @@
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "communication-layer-pub-sub"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
- "flume",
+ "flume 0.10.14",
  "zenoh",
 ]
 
 [[package]]
 name = "communication-layer-request-reply"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 
 [[package]]
 name = "concurrent-queue"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f057a694a54f12365049b0958a1685bb52d567f5593b355fbf685838e873d400"
 dependencies = [
@@ -1156,15 +1220,15 @@
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e64e6c0fbe2c17357405f7c758c1ef960fce08bdfb2c03d88d2a18d7e09c4b67"
 dependencies = [
  "bitflags 1.3.2",
  "crossterm_winapi",
  "libc",
- "mio 0.8.8",
+ "mio 0.8.11",
  "parking_lot",
  "signal-hook",
  "signal-hook-mio",
  "winapi 0.3.9",
 ]
 
 [[package]]
@@ -1231,50 +1295,50 @@
 dependencies = [
  "nix 0.27.1",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.107"
+version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe98ba1789d56fb3db3bee5e032774d4f421b685de7ba703643584ba24effbe"
+checksum = "2673ca5ae28334544ec2a6b18ebe666c42a2650abfb48abbd532ed409a44be2b"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxx-build"
-version = "1.0.111"
+version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51bc81d2664db24cf1d35405f66e18a85cffd4d49ab930c71a5c6342a410f38c"
+checksum = "9df46fe0eb43066a332586114174c449a62c25689f85a08f28fdcc8e12c380b9"
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.107"
+version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20888d9e1d2298e2ff473cee30efe7d5036e437857ab68bbfea84c74dba91da2"
+checksum = "886acf875df67811c11cd015506b3392b9e1820b1627af1a6f4e93ccdfc74d11"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.107"
+version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fa16a70dd58129e4dfffdff535fb1bce66673f7bbeec4a5a1765a504e1ccd84"
+checksum = "1d151cc139c3080e07f448f93a1284577ab2283d2a44acd902c6fba9ec20b6de"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
@@ -1393,23 +1457,23 @@
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "dora-arrow-convert"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow",
  "eyre",
 ]
 
 [[package]]
 name = "dora-cli"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "bat",
  "clap 4.4.6",
  "communication-layer-request-reply",
  "ctrlc",
  "dora-coordinator",
  "dora-core",
@@ -1431,15 +1495,15 @@
  "tracing",
  "uuid",
  "webbrowser",
 ]
 
 [[package]]
 name = "dora-coordinator"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "ctrlc",
  "dora-core",
  "dora-tracing",
  "eyre",
  "futures",
  "futures-concurrency",
@@ -1449,15 +1513,15 @@
  "tokio-stream",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-core"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "dora-message",
  "eyre",
  "once_cell",
  "serde",
  "serde-with-expand-env",
@@ -1466,40 +1530,42 @@
  "tracing",
  "uuid",
  "which",
 ]
 
 [[package]]
 name = "dora-daemon"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "async-trait",
  "bincode",
  "ctrlc",
+ "dora-arrow-convert",
  "dora-core",
  "dora-download",
+ "dora-node-api",
  "dora-tracing",
  "eyre",
- "flume",
+ "flume 0.10.14",
  "futures",
  "futures-concurrency",
  "serde_json",
  "serde_yaml 0.8.26",
  "shared-memory-server",
  "tokio",
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
  "uuid",
 ]
 
 [[package]]
 name = "dora-download"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "eyre",
  "reqwest",
  "tokio",
  "tracing",
 ]
 
@@ -1519,169 +1585,183 @@
  "tokio-stream",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-message"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow-data",
  "arrow-schema",
  "eyre",
  "serde",
  "uhlc",
 ]
 
 [[package]]
 name = "dora-metrics"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
- "opentelemetry 0.21.0",
+ "eyre",
+ "opentelemetry 0.22.0",
  "opentelemetry-otlp",
- "opentelemetry_sdk 0.21.1",
+ "opentelemetry-system-metrics",
+ "opentelemetry_sdk 0.22.1",
 ]
 
 [[package]]
 name = "dora-node-api"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "arrow",
  "bincode",
  "dora-arrow-convert",
  "dora-core",
  "dora-tracing",
  "eyre",
- "flume",
+ "flume 0.10.14",
  "futures",
  "futures-concurrency",
  "futures-timer",
  "serde_yaml 0.8.26",
  "shared-memory-server",
  "shared_memory_extended",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-c"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow-array",
  "dora-node-api",
  "eyre",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-cxx"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-node-api",
+ "dora-ros2-bridge",
+ "dora-ros2-bridge-msg-gen",
  "eyre",
+ "futures-lite 2.2.0",
+ "prettyplease",
+ "rust-format",
+ "serde",
+ "serde-big-array",
 ]
 
 [[package]]
 name = "dora-node-api-python"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-ros2-bridge-python",
  "dora-runtime",
  "eyre",
- "flume",
+ "flume 0.10.14",
  "futures",
  "pyo3",
  "pythonize",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-arrow-convert",
  "dora-operator-api-macros",
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-c"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-cxx"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-operator-api",
 ]
 
 [[package]]
 name = "dora-operator-api-macros"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dora-operator-api-python"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "arrow",
  "arrow-schema",
  "dora-node-api",
  "eyre",
- "flume",
+ "flume 0.10.14",
  "pyo3",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api-types"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow",
  "dora-arrow-convert",
  "safer-ffi",
 ]
 
 [[package]]
 name = "dora-record"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "chrono",
  "dora-node-api",
  "dora-tracing",
  "eyre",
+ "parquet",
+ "tokio",
 ]
 
 [[package]]
 name = "dora-ros2-bridge"
 version = "0.1.0"
 dependencies = [
  "array-init",
  "dora-daemon",
- "dora-ros2-bridge-msg-gen-macro",
+ "dora-ros2-bridge-msg-gen",
  "eyre",
+ "flume 0.11.0",
  "futures",
+ "futures-timer",
  "rand",
  "ros2-client",
+ "rust-format",
  "rustdds",
  "serde",
  "serde-big-array",
  "tokio",
  "tracing",
  "tracing-subscriber",
  "widestring",
@@ -1698,29 +1778,14 @@
  "quote",
  "regex",
  "syn 1.0.109",
  "thiserror",
 ]
 
 [[package]]
-name = "dora-ros2-bridge-msg-gen-macro"
-version = "0.1.0"
-dependencies = [
- "anyhow",
- "dora-ros2-bridge-msg-gen",
- "heck 0.3.3",
- "nom",
- "proc-macro2",
- "quote",
- "regex",
- "syn 1.0.109",
- "thiserror",
-]
-
-[[package]]
 name = "dora-ros2-bridge-python"
 version = "0.1.0"
 dependencies = [
  "arrow",
  "dora-ros2-bridge",
  "dora-ros2-bridge-msg-gen",
  "eyre",
@@ -1728,44 +1793,42 @@
  "pyo3",
  "serde",
  "serde_assert",
 ]
 
 [[package]]
 name = "dora-runtime"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "arrow",
  "dora-core",
  "dora-download",
  "dora-metrics",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-operator-api-types",
  "dora-tracing",
  "eyre",
- "flume",
+ "flume 0.10.14",
  "futures",
  "futures-concurrency",
  "libloading",
- "opentelemetry 0.21.0",
- "opentelemetry-system-metrics",
  "pyo3",
  "pythonize",
  "serde_yaml 0.8.26",
  "tokio",
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
 ]
 
 [[package]]
 name = "dora-tracing"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "eyre",
  "opentelemetry 0.18.0",
  "opentelemetry-jaeger",
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
@@ -1792,78 +1855,14 @@
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
 [[package]]
-name = "encoding"
-version = "0.2.33"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b0d943856b990d12d3b55b359144ff341533e516d94098b1d3fc1ac666d36ec"
-dependencies = [
- "encoding-index-japanese",
- "encoding-index-korean",
- "encoding-index-simpchinese",
- "encoding-index-singlebyte",
- "encoding-index-tradchinese",
-]
-
-[[package]]
-name = "encoding-index-japanese"
-version = "1.20141219.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04e8b2ff42e9a05335dbf8b5c6f7567e5591d0d916ccef4e0b1710d32a0d0c91"
-dependencies = [
- "encoding_index_tests",
-]
-
-[[package]]
-name = "encoding-index-korean"
-version = "1.20141219.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dc33fb8e6bcba213fe2f14275f0963fd16f0a02c878e3095ecfdf5bee529d81"
-dependencies = [
- "encoding_index_tests",
-]
-
-[[package]]
-name = "encoding-index-simpchinese"
-version = "1.20141219.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d87a7194909b9118fc707194baa434a4e3b0fb6a5a757c73c3adb07aa25031f7"
-dependencies = [
- "encoding_index_tests",
-]
-
-[[package]]
-name = "encoding-index-singlebyte"
-version = "1.20141219.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3351d5acffb224af9ca265f435b859c7c01537c0849754d3db3fdf2bfe2ae84a"
-dependencies = [
- "encoding_index_tests",
-]
-
-[[package]]
-name = "encoding-index-tradchinese"
-version = "1.20141219.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd0e20d5688ce3cab59eb3ef3a2083a5c77bf496cb798dc6fcdb75f323890c18"
-dependencies = [
- "encoding_index_tests",
-]
-
-[[package]]
-name = "encoding_index_tests"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a246d82be1c9d791c5dfde9a2bd045fc3cbba3fa2b11ad558f27d01712f00569"
-
-[[package]]
 name = "encoding_rs"
 version = "0.8.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
 dependencies = [
  "cfg-if 1.0.0",
 ]
@@ -1915,14 +1914,25 @@
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "etcetera"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "136d1b5283a1ab77bd9257427ffd09d8667ced0570b6f938942bc7568ed5b943"
+dependencies = [
+ "cfg-if 1.0.0",
+ "home",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "event-listener"
 version = "2.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "event-listener"
@@ -1972,17 +1982,17 @@
 checksum = "a296e5a895621edf9fa8329c83aa1cb69a964643e36cf54d8d7a69b789089537"
 dependencies = [
  "ext-trait",
 ]
 
 [[package]]
 name = "eyre"
-version = "0.6.8"
+version = "0.6.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c2b6b5a29c02cdc822728b7d7b8ae1bab3e3b05d44522770ddd49722eeac7eb"
+checksum = "7cd915d99f24784cdc19fd37ef22b97e3ff0ae756c7e492e9fbfe897d61e2aec"
 dependencies = [
  "indenter",
  "once_cell",
 ]
 
 [[package]]
 name = "fastrand"
@@ -2047,14 +2057,26 @@
  "futures-sink",
  "nanorand",
  "pin-project",
  "spin 0.9.8",
 ]
 
 [[package]]
+name = "flume"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55ac459de2512911e4b674ce33cf20befaba382d05b62b008afc1c8b57cbf181"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+ "nanorand",
+ "spin 0.9.8",
+]
+
+[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
@@ -2145,14 +2167,15 @@
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
+ "num_cpus",
 ]
 
 [[package]]
 name = "futures-io"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
@@ -2169,14 +2192,27 @@
  "memchr",
  "parking",
  "pin-project-lite",
  "waker-fn",
 ]
 
 [[package]]
+name = "futures-lite"
+version = "2.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "445ba825b27408685aaecefd65178908c36c6e96aaf6d8599419d46e624192ba"
+dependencies = [
+ "fastrand 2.0.1",
+ "futures-core",
+ "futures-io",
+ "parking",
+ "pin-project-lite",
+]
+
+[[package]]
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -2193,17 +2229,17 @@
 name = "futures-task"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-timer"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e64b03909df88034c26dc1547e8970b91f98bdb65165d6a4e9110d94263dbb2c"
+checksum = "f288b0a4f20f9a56b5d1da57e2227c661b7b16168e2f72365f57b63326e29b24"
 
 [[package]]
 name = "futures-util"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
@@ -2279,19 +2315,19 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "git2"
-version = "0.16.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccf7f68c2995f392c49fffb4f95ae2c873297830eb25c6bc4c114ce8f4562acc"
+checksum = "1b3ba52851e73b46a4c3df1d89343741112003f0f6f13beb0dfac9e457c3fdcd"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.4.0",
  "libc",
  "libgit2-sys",
  "log",
  "url",
 ]
 
 [[package]]
@@ -2339,17 +2375,17 @@
  "same-file",
  "termcolor",
  "winapi-util",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.24"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -2964,17 +3000,17 @@
 name = "libc"
 version = "0.2.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
 
 [[package]]
 name = "libgit2-sys"
-version = "0.14.2+1.5.1"
+version = "0.16.2+1.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f3d95f6b51075fe9810a7ae22c7095f12b98005ab364d8544797a825ce946a4"
+checksum = "ee4126d8b4ee5c9d9ea891dd875cfdc1e9d0950437179104b183d7d8a74d24e8"
 dependencies = [
  "cc",
  "libc",
  "libz-sys",
  "pkg-config",
 ]
 
@@ -3070,14 +3106,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 dependencies = [
  "value-bag",
 ]
 
 [[package]]
+name = "lz4_flex"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "912b45c753ff5f7f5208307e8ace7d2a2e30d024e26d3509f3dce546c044ce15"
+dependencies = [
+ "twox-hash",
+]
+
+[[package]]
 name = "macro_rules_attribute"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf0c9b980bf4f3a37fd7b1c066941dd1b1d0152ce6ee6e8fe8c49b9f6810d862"
 dependencies = [
  "macro_rules_attribute-proc_macro",
  "paste",
@@ -3199,17 +3244,17 @@
  "net2",
  "slab",
  "winapi 0.2.8",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.8"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
@@ -3235,33 +3280,33 @@
  "net2",
  "winapi 0.2.8",
  "ws2_32-sys",
 ]
 
 [[package]]
 name = "multiple-daemons-example-node"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "multiple-daemons-example-operator"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "multiple-daemons-example-sink"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "names"
@@ -3395,15 +3440,15 @@
  "bitflags 1.3.2",
  "crossbeam-channel",
  "filetime",
  "fsevent-sys",
  "inotify",
  "kqueue",
  "libc",
- "mio 0.8.8",
+ "mio 0.8.11",
  "walkdir",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "ntapi"
 version = "0.4.1"
@@ -3421,19 +3466,19 @@
 dependencies = [
  "overload",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "nu-ansi-term"
-version = "0.47.0"
+version = "0.49.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1df031e117bca634c262e9bd3173776844b6c17a90b3741c9163663b4385af76"
+checksum = "c073d3c1930d0751774acf49e66653acecb416c3a54c6ec095a9b11caddb5a68"
 dependencies = [
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "num"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
@@ -3630,21 +3675,20 @@
 dependencies = [
  "opentelemetry_api",
  "opentelemetry_sdk 0.18.0",
 ]
 
 [[package]]
 name = "opentelemetry"
-version = "0.21.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e32339a5dc40459130b3bd269e9892439f55b33e772d2a9d402a789baaf4e8a"
+checksum = "900d57987be3f2aeb70d385fff9b27fb74c5723cc9a52d904d4f9c807a0667bf"
 dependencies = [
  "futures-core",
  "futures-sink",
- "indexmap 2.0.2",
  "js-sys",
  "once_cell",
  "pin-project-lite",
  "thiserror",
  "urlencoding",
 ]
 
@@ -3657,45 +3701,45 @@
  "async-trait",
  "futures",
  "futures-executor",
  "once_cell",
  "opentelemetry 0.18.0",
  "opentelemetry-semantic-conventions 0.10.0",
  "thiserror",
- "thrift",
+ "thrift 0.16.0",
  "tokio",
 ]
 
 [[package]]
 name = "opentelemetry-otlp"
-version = "0.14.0"
+version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f24cda83b20ed2433c68241f918d0f6fdec8b1d43b7a9590ab4420c5095ca930"
+checksum = "1a016b8d9495c639af2145ac22387dcb88e44118e45320d9238fbf4e7889abcb"
 dependencies = [
  "async-trait",
  "futures-core",
  "http",
- "opentelemetry 0.21.0",
+ "opentelemetry 0.22.0",
  "opentelemetry-proto",
- "opentelemetry-semantic-conventions 0.13.0",
- "opentelemetry_sdk 0.21.1",
+ "opentelemetry-semantic-conventions 0.14.0",
+ "opentelemetry_sdk 0.22.1",
  "prost",
  "thiserror",
  "tokio",
  "tonic",
 ]
 
 [[package]]
 name = "opentelemetry-proto"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2e155ce5cc812ea3d1dffbd1539aed653de4bf4882d60e6e04dcf0901d674e1"
+checksum = "3a8fddc9b68f5b80dae9d6f510b88e02396f006ad48cac349411fbecc80caae4"
 dependencies = [
- "opentelemetry 0.21.0",
- "opentelemetry_sdk 0.21.1",
+ "opentelemetry 0.22.0",
+ "opentelemetry_sdk 0.22.1",
  "prost",
  "tonic",
 ]
 
 [[package]]
 name = "opentelemetry-semantic-conventions"
 version = "0.10.0"
@@ -3703,31 +3747,28 @@
 checksum = "9b02e0230abb0ab6636d18e2ba8fa02903ea63772281340ccac18e0af3ec9eeb"
 dependencies = [
  "opentelemetry 0.18.0",
 ]
 
 [[package]]
 name = "opentelemetry-semantic-conventions"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5774f1ef1f982ef2a447f6ee04ec383981a3ab99c8e77a1a7b30182e65bbc84"
-dependencies = [
- "opentelemetry 0.21.0",
-]
+checksum = "f9ab5bd6c42fb9349dcf28af2ba9a0667f697f9bdcca045d39f2cec5543e2910"
 
 [[package]]
 name = "opentelemetry-system-metrics"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a4662d72a3d0cd5242067ba15da95bc4d83bce5151337ffcc971fc76d261455"
+checksum = "1dca748d4fe59e208f6c71bde86573d326f98ed29696d31dbf7d2454b8f1af2d"
 dependencies = [
  "eyre",
  "indexmap 1.9.3",
  "nvml-wrapper",
- "opentelemetry 0.21.0",
+ "opentelemetry 0.22.0",
  "sysinfo",
  "tracing",
 ]
 
 [[package]]
 name = "opentelemetry_api"
 version = "0.18.0"
@@ -3764,26 +3805,26 @@
  "thiserror",
  "tokio",
  "tokio-stream",
 ]
 
 [[package]]
 name = "opentelemetry_sdk"
-version = "0.21.1"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "968ba3f2ca03e90e5187f5e4f46c791ef7f2c163ae87789c8ce5f5ca3b7b7de5"
+checksum = "9e90c7113be649e31e9a0f8b5ee24ed7a16923b322c3c5ab6367469c049d6b7e"
 dependencies = [
  "async-trait",
  "crossbeam-channel",
  "futures-channel",
  "futures-executor",
  "futures-util",
  "glob",
  "once_cell",
- "opentelemetry 0.21.0",
+ "opentelemetry 0.22.0",
  "ordered-float 4.1.1",
  "percent-encoding",
  "rand",
  "thiserror",
  "tokio",
  "tokio-stream",
 ]
@@ -3801,14 +3842,23 @@
 checksum = "3305af35278dd29f46fcdd139e0b1fbfae2153f0e5928b39b035542dd31e37b7"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "ordered-float"
+version = "2.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68f19d67e5a2795c94e73e0bb1cc1a7edeb2e28efd39e2e1c9b7a40c1108b11c"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "ordered-float"
 version = "3.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a54938017eacd63036332b4ae5c8a49fc8c0c1d6d629893057e4f13609edd06"
 dependencies = [
  "num-traits",
 ]
 
@@ -3831,17 +3881,17 @@
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "parking"
-version = "2.1.1"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e52c774a4c39359c1d1c52e43f73dd91a75a614652c825408eec30c95a9b2067"
+checksum = "bb813b8af86854136c6922af0598d719255ecb2179515e6e7730d468f05c9cae"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -3859,14 +3909,47 @@
  "libc",
  "redox_syscall 0.3.5",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "parquet"
+version = "48.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "239229e6a668ab50c61de3dce61cf0fa1069345f7aa0f4c934491f92205a4945"
+dependencies = [
+ "ahash",
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-cast",
+ "arrow-data",
+ "arrow-ipc",
+ "arrow-schema",
+ "arrow-select",
+ "base64 0.21.4",
+ "brotli",
+ "bytes",
+ "chrono",
+ "flate2",
+ "futures",
+ "hashbrown 0.14.3",
+ "lz4_flex",
+ "num",
+ "num-bigint",
+ "paste",
+ "seq-macro",
+ "snap",
+ "thrift 0.17.0",
+ "tokio",
+ "twox-hash",
+ "zstd",
+]
+
+[[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "path_abs"
@@ -4190,33 +4273,33 @@
 checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
-version = "0.11.9"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
+checksum = "d0f5d036824e4761737860779c906171497f6d55681139d8312388f8fe398922"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
 name = "prost-derive"
-version = "0.11.9"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
+checksum = "19de2de2a00075bf566bee3bd4db014b11587e84184d3f7a791bc17f1a8e9e48"
 dependencies = [
  "anyhow",
- "itertools 0.10.5",
+ "itertools 0.11.0",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04e8453b658fe480c3e70c8ed4e3d3ec33eb74988bd186561b0cc66b85c3bc4b"
@@ -4654,46 +4737,58 @@
  "smallvec",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rust-dataflow-example-node"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "rust-dataflow-example-operator"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "rust-dataflow-example-sink"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
+name = "rust-format"
+version = "0.3.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60e7c00b6c3bf5e38a880eec01d7e829d12ca682079f8238a464def3c4b31627"
+dependencies = [
+ "prettyplease",
+ "proc-macro2",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "rust-ros2-dataflow-example-node"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "dora-ros2-bridge",
  "eyre",
  "futures",
+ "futures-timer",
  "rand",
  "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "rustc-demangle"
@@ -4730,23 +4825,23 @@
  "futures",
  "if-addrs",
  "io-extras",
  "local-ip-address",
  "log",
  "md5",
  "mio 0.6.23",
- "mio 0.8.8",
+ "mio 0.8.11",
  "mio-extras",
  "num-derive",
  "num-traits",
  "paste",
  "rand",
  "serde",
  "serde_repr",
- "socket2 0.5.4",
+ "socket2 0.5.6",
  "socketpair",
  "speedy",
  "static_assertions",
  "thiserror",
 ]
 
 [[package]]
@@ -4847,17 +4942,17 @@
 name = "safemem"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef703b7cb59335eae2eb93ceb664c0eb7ea6bf567079d843e09420219668e072"
 
 [[package]]
 name = "safer-ffi"
-version = "0.1.4"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "395ace5aff9629c7268ca8255aceb945525b2cb644015f3caec5131a6a537c11"
+checksum = "4483c5ab47f222d2c297e73a520c9003e09e2fe1f1b04edcb572e6939f303003"
 dependencies = [
  "inventory 0.1.11",
  "inventory 0.3.12",
  "libc",
  "macro_rules_attribute",
  "paste",
  "safer_ffi-proc_macros",
@@ -4865,17 +4960,17 @@
  "uninit",
  "unwind_safe",
  "with_builtin_macros",
 ]
 
 [[package]]
 name = "safer_ffi-proc_macros"
-version = "0.1.4"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9255504d5467bae9e07d58b8de446ba6739b29bf72e1fa35b2387e30d29dcbfe"
+checksum = "bf04ebd3786110e64269a74eea58c5564dd92a1e790c0f6f9871d6fe1b8e34db"
 dependencies = [
  "macro_rules_attribute",
  "prettyplease",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
@@ -4946,14 +5041,20 @@
 [[package]]
 name = "semver"
 version = "1.0.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad977052201c6de01a8ef2aa3378c4bd23217a056337d1d6da40468d267a4fb0"
 
 [[package]]
+name = "seq-macro"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
+
+[[package]]
 name = "serde"
 version = "1.0.195"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
 dependencies = [
  "serde_derive",
 ]
@@ -5084,15 +5185,15 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "shared-memory-server"
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 dependencies = [
  "bincode",
  "eyre",
  "raw_sync_2",
  "serde",
  "shared_memory_extended",
  "tracing",
@@ -5154,15 +5255,15 @@
 [[package]]
 name = "signal-hook-mio"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29ad2e15f37ec9a6cc544097b78a1ec90001e9f71b81338ca39f430adaca99af"
 dependencies = [
  "libc",
- "mio 0.8.8",
+ "mio 0.8.11",
  "signal-hook",
 ]
 
 [[package]]
 name = "signal-hook-registry"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -5193,31 +5294,37 @@
 [[package]]
 name = "smallvec"
 version = "1.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "942b4a808e05215192e39f4ab80813e599068285906cc91aa64f923db842bd5a"
 
 [[package]]
+name = "snap"
+version = "1.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b6b67fb9a61334225b5b790716f609cd58395f895b3fe8b328786812a40bc3b"
+
+[[package]]
 name = "socket2"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.4"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4031e820eb552adee9295814c0ced9e5cf38ddf1e8b7d566d6de8e2538ea989e"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "socketpair"
 version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a004c141c54615778c01a6722f6453fae7013e501b2b1f2dfe5684037174721"
@@ -5498,14 +5605,25 @@
  "integer-encoding",
  "log",
  "ordered-float 1.1.1",
  "threadpool",
 ]
 
 [[package]]
+name = "thrift"
+version = "0.17.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
+dependencies = [
+ "byteorder",
+ "integer-encoding",
+ "ordered-float 2.10.1",
+]
+
+[[package]]
 name = "time"
 version = "0.3.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "426f806f4089c493dcac0d24c29c01e2c38baf8e30f1b716ee37e83d200b18fe"
 dependencies = [
  "deranged",
  "itoa",
@@ -5551,27 +5669,27 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.32.0"
+version = "1.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17ed6077ed6cd6c74735e21f37eb16dc3935f96878b1fe961074089cc80893f9"
+checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
- "mio 0.8.8",
+ "mio 0.8.11",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
- "socket2 0.5.4",
+ "socket2 0.5.6",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-io-timeout"
 version = "1.2.0"
@@ -5580,17 +5698,17 @@
 dependencies = [
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
+checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
@@ -5626,24 +5744,23 @@
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "tonic"
-version = "0.9.2"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3082666a3a6433f7f511c7192923fa1fe07c69332d3c6a2e6bb040b569199d5a"
+checksum = "76c4eb7a4e9ef9d4763600161f12f5070b92a578e1b634db88a6887844c91a13"
 dependencies = [
+ "async-stream",
  "async-trait",
  "axum",
  "base64 0.21.4",
  "bytes",
- "futures-core",
- "futures-util",
  "h2",
  "http",
  "http-body",
  "hyper",
  "hyper-timeout",
  "percent-encoding",
  "pin-project",
@@ -5766,14 +5883,24 @@
 [[package]]
 name = "try-lock"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
 
 [[package]]
+name = "twox-hash"
+version = "1.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
+dependencies = [
+ "cfg-if 1.0.0",
+ "static_assertions",
+]
+
+[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "ucd-trie"
@@ -5900,29 +6027,30 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.4.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79daa5ed5740825c40b389c5e50312b9c86df53fccd33f281df655642b43869d"
+checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
 dependencies = [
+ "atomic",
  "getrandom",
  "rand",
  "serde",
  "uuid-macro-internal",
 ]
 
 [[package]]
 name = "uuid-macro-internal"
-version = "1.4.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7e1ba1f333bd65ce3c9f27de592fcbc256dafe3af2717f56d7c87761fbaccf4"
+checksum = "7abb14ae1a50dad63eaa768a458ef43d298cd1bd44951677bd10b732a9ba2a2d"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
@@ -6551,15 +6679,15 @@
 dependencies = [
  "async-global-executor",
  "async-std",
  "async-trait",
  "base64 0.13.1",
  "env_logger",
  "event-listener 2.5.3",
- "flume",
+ "flume 0.10.14",
  "form_urlencoded",
  "futures",
  "git-version",
  "hex",
  "lazy_static",
  "log",
  "ordered-float 3.9.1",
@@ -6615,27 +6743,27 @@
 name = "zenoh-collections"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e256d7aff2c9af765d77efbfae7fcb708d2d7f4e179aa201bff2f81ad7a3845"
 dependencies = [
  "async-std",
  "async-trait",
- "flume",
+ "flume 0.10.14",
  "log",
  "zenoh-core",
  "zenoh-sync",
 ]
 
 [[package]]
 name = "zenoh-config"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bad1ff61abf28c57e8879ec4286fa29becf7e9bf12555df9a7faddff3bc9ea1b"
 dependencies = [
- "flume",
+ "flume 0.10.14",
  "json5",
  "num_cpus",
  "serde",
  "serde_json",
  "serde_yaml 0.9.30",
  "validated_struct",
  "zenoh-cfg-properties",
@@ -6694,15 +6822,15 @@
 name = "zenoh-link-commons"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21aab9eeb2aba53e37aae57467ffca1268d209811c5e2f39761aab4c1343bce3"
 dependencies = [
  "async-std",
  "async-trait",
- "flume",
+ "flume 0.10.14",
  "serde",
  "zenoh-buffers",
  "zenoh-cfg-properties",
  "zenoh-core",
  "zenoh-protocol",
  "zenoh-protocol-core",
 ]
@@ -6866,15 +6994,15 @@
 name = "zenoh-sync"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "821070b62a55d4c8a22e1e06c939c1f2d94767e660df9fcbea377781f72f59bf"
 dependencies = [
  "async-std",
  "event-listener 2.5.3",
- "flume",
+ "flume 0.10.14",
  "futures",
  "tokio",
  "zenoh-core",
 ]
 
 [[package]]
 name = "zenoh-transport"
@@ -6882,15 +7010,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce4387cfc02cb86383de8e65ab1eb204e3908c5f1db9e6b4defd8ad530c9ddea"
 dependencies = [
  "async-executor",
  "async-global-executor",
  "async-std",
  "async-trait",
- "flume",
+ "flume 0.10.14",
  "log",
  "paste",
  "rand",
  "ringbuffer-spsc",
  "rsa",
  "serde",
  "zenoh-buffers",
@@ -6953,7 +7081,35 @@
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
+
+[[package]]
+name = "zstd"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
+dependencies = [
+ "zstd-safe",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "7.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
+dependencies = [
+ "zstd-sys",
+]
+
+[[package]]
+name = "zstd-sys"
+version = "2.0.9+zstd.1.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+dependencies = [
+ "cc",
+ "pkg-config",
+]
```

### Comparing `dora_rs-0.3.2rc2/Cargo.toml` & `dora_rs-0.3.3rc1/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [workspace]
 members = ["apis/python/node", "apis/rust/*", "libraries/extensions/telemetry/*"]
 
 [workspace.package]
 # Make sure to also bump `apis/node/python/__init__.py` version.
-version = "0.3.2-rc2"
+version = "0.3.3-rc1"
 description = "`dora` goal is to be a low latency, composable, and distributed data flow."
 documentation = "https://dora.carsmos.ai"
 license = "Apache-2.0"
 
 [workspace.dependencies]
-dora-node-api = { version = "0.3.2-rc2", path = "apis/rust/node", default-features = false }
-dora-node-api-python = { version = "0.3.2-rc2", path = "apis/python/node", default-features = false }
-dora-operator-api = { version = "0.3.2-rc2", path = "apis/rust/operator", default-features = false }
-dora-operator-api-macros = { version = "0.3.2-rc2", path = "apis/rust/operator/macros" }
-dora-operator-api-types = { version = "0.3.2-rc2", path = "apis/rust/operator/types" }
-dora-operator-api-python = { version = "0.3.2-rc2", path = "apis/python/operator" }
-dora-operator-api-c = { version = "0.3.2-rc2", path = "apis/c/operator" }
-dora-node-api-c = { version = "0.3.2-rc2", path = "apis/c/node" }
-dora-core = { version = "0.3.2-rc2", path = "libraries/core" }
-dora-arrow-convert = { version = "0.3.2-rc2", path = "libraries/arrow-convert" }
-dora-tracing = { version = "0.3.2-rc2", path = "libraries/extensions/telemetry/tracing" }
-dora-metrics = { version = "0.3.2-rc2", path = "libraries/extensions/telemetry/metrics" }
-dora-download = { version = "0.3.2-rc2", path = "libraries/extensions/download" }
-shared-memory-server = { version = "0.3.2-rc2", path = "libraries/shared-memory-server" }
-communication-layer-request-reply = { version = "0.3.2-rc2", path = "libraries/communication-layer/request-reply" }
-dora-message = { version = "0.3.2-rc2", path = "libraries/message" }
-dora-runtime = { version = "0.3.2-rc2", path = "binaries/runtime" }
-dora-daemon = { version = "0.3.2-rc2", path = "binaries/daemon" }
-dora-coordinator = { version = "0.3.2-rc2", path = "binaries/coordinator" }
+dora-node-api = { version = "0.3.3-rc1", path = "apis/rust/node", default-features = false }
+dora-node-api-python = { version = "0.3.3-rc1", path = "apis/python/node", default-features = false }
+dora-operator-api = { version = "0.3.3-rc1", path = "apis/rust/operator", default-features = false }
+dora-operator-api-macros = { version = "0.3.3-rc1", path = "apis/rust/operator/macros" }
+dora-operator-api-types = { version = "0.3.3-rc1", path = "apis/rust/operator/types" }
+dora-operator-api-python = { version = "0.3.3-rc1", path = "apis/python/operator" }
+dora-operator-api-c = { version = "0.3.3-rc1", path = "apis/c/operator" }
+dora-node-api-c = { version = "0.3.3-rc1", path = "apis/c/node" }
+dora-core = { version = "0.3.3-rc1", path = "libraries/core" }
+dora-arrow-convert = { version = "0.3.3-rc1", path = "libraries/arrow-convert" }
+dora-tracing = { version = "0.3.3-rc1", path = "libraries/extensions/telemetry/tracing" }
+dora-metrics = { version = "0.3.3-rc1", path = "libraries/extensions/telemetry/metrics" }
+dora-download = { version = "0.3.3-rc1", path = "libraries/extensions/download" }
+shared-memory-server = { version = "0.3.3-rc1", path = "libraries/shared-memory-server" }
+communication-layer-request-reply = { version = "0.3.3-rc1", path = "libraries/communication-layer/request-reply" }
+dora-message = { version = "0.3.3-rc1", path = "libraries/message" }
+dora-runtime = { version = "0.3.3-rc1", path = "binaries/runtime" }
+dora-daemon = { version = "0.3.3-rc1", path = "binaries/daemon" }
+dora-coordinator = { version = "0.3.3-rc1", path = "binaries/coordinator" }
 dora-ros2-bridge = { path = "libraries/extensions/ros2-bridge" }
+dora-ros2-bridge-msg-gen = { path = "libraries/extensions/ros2-bridge/msg-gen" }
 dora-ros2-bridge-python = { path = "libraries/extensions/ros2-bridge/python" }
 arrow = "48.0.0"
 arrow-schema = "48.0.0"
 arrow-data = "48.0.0"
 arrow-array = "48.0.0"
 pyo3 = "0.20.0"
 pythonize = "0.20.0"
@@ -53,17 +54,17 @@
 tokio = "1.24.2"
 dora-coordinator = { workspace = true }
 dora-core = { workspace = true }
 dora-tracing = { workspace = true }
 dora-download = { workspace = true }
 dunce = "1.0.2"
 serde_yaml = "0.8.23"
-uuid = { version = "1.2.1", features = ["v4", "serde"] }
+uuid = { version = "1.7", features = ["v7", "serde"] }
 tracing = "0.1.36"
-futures = "0.3.25"
+futures = "0.3.3-rc15"
 tokio-stream = "0.1.11"
 
 [[example]]
 name = "c-dataflow"
 path = "examples/c-dataflow/run.rs"
 
 [[example]]
@@ -104,7 +105,12 @@
 [[example]]
 name = "multiple-daemons"
 path = "examples/multiple-daemons/run.rs"
 
 [[example]]
 name = "cmake-dataflow"
 path = "examples/cmake-dataflow/run.rs"
+
+[[example]]
+name = "cxx-ros2-dataflow"
+path = "examples/c++-ros2-dataflow/run.rs"
+required-features = ["ros2-examples"]
```

### Comparing `dora_rs-0.3.2rc2/dora/__init__.py` & `dora_rs-0.3.3rc1/dora/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from enum import Enum
 
 from .dora import *
 
 __author__ = "Dora-rs Authors"
-__version__ = "0.3.2-rc2"
+__version__ = "0.3.3-rc1"
 
 
 class DoraStatus(Enum):
     """Dora status to indicate if operator `on_input` loop
      should be stopped.
 
     Args:
```

