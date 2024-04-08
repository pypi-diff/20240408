# Comparing `tmp/hdfs_native-0.8.0.tar.gz` & `tmp/hdfs_native-0.9.1.tar.gz`

## Comparing `hdfs_native-0.8.0.tar` & `hdfs_native-0.9.1.tar`

### file list

```diff
@@ -1,81 +1,82 @@
--rw-r--r--   0     1001      127     1668 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/Cargo.toml
--rw-r--r--   0     1001      127    47324 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/Cargo.lock
--rw-r--r--   0     1001      127     2127 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/benches/ec.rs
--rw-r--r--   0     1001      127     5698 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/benches/io.rs
--rw-r--r--   0     1001      127     1069 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/benches/rpc.rs
--rw-r--r--   0     1001      127     1127 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/build.rs
--rw-r--r--   0     1001      127     1918 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/examples/simple.rs
--rw-r--r--   0     1001      127     1754 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/minidfs/pom.xml
--rw-r--r--   0     1001      127     9575 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/minidfs/src/main/java/main/Main.java
--rw-r--r--   0     1001      127      334 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/minidfs/src/main/resources/log4j.properties
--rw-r--r--   0     1001      127    24957 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/client.rs
--rw-r--r--   0     1001      127     6384 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/common/config.rs
--rw-r--r--   0     1001      127       16 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/common/mod.rs
--rw-r--r--   0     1001      127     6685 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/ec/gf256.rs
--rw-r--r--   0     1001      127     7576 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/ec/matrix.rs
--rw-r--r--   0     1001      127     4952 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/ec/mod.rs
--rw-r--r--   0     1001      127     1711 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/error.rs
--rw-r--r--   0     1001      127     9964 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/file.rs
--rw-r--r--   0     1001      127    15137 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/block_reader.rs
--rw-r--r--   0     1001      127    19247 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/block_writer.rs
--rw-r--r--   0     1001      127    25997 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/connection.rs
--rw-r--r--   0     1001      127      132 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/mod.rs
--rw-r--r--   0     1001      127    12406 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/protocol.rs
--rw-r--r--   0     1001      127     5913 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/proxy.rs
--rw-r--r--   0     1001      127     1414 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/lib.rs
--rw-r--r--   0     1001      127     5014 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/minidfs.rs
--rw-r--r--   0     1001      127     2863 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/FSProtos.proto
--rw-r--r--   0     1001      127     2090 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/GenericRefreshProtocol.proto
--rw-r--r--   0     1001      127     1760 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/GetUserMappingsProtocol.proto
--rw-r--r--   0     1001      127     3715 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/HAServiceProtocol.proto
--rw-r--r--   0     1001      127     1922 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/IpcConnectionContext.proto
--rw-r--r--   0     1001      127     2924 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/ProtobufRpcEngine.proto
--rw-r--r--   0     1001      127     2915 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/ProtobufRpcEngine2.proto
--rw-r--r--   0     1001      127     2725 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/ProtocolInfo.proto
--rw-r--r--   0     1001      127     1767 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/RefreshAuthorizationPolicyProtocol.proto
--rw-r--r--   0     1001      127     1673 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/RefreshCallQueueProtocol.proto
--rw-r--r--   0     1001      127     2160 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/RefreshUserMappingsProtocol.proto
--rw-r--r--   0     1001      127     7706 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/RpcHeader.proto
--rw-r--r--   0     1001      127     2236 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/Security.proto
--rw-r--r--   0     1001      127     2193 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/TraceAdmin.proto
--rw-r--r--   0     1001      127     1867 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/ZKFCProtocol.proto
--rw-r--r--   0     1001      127    27673 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hadoop.common.rs
--rw-r--r--   0     1001      127   168627 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hadoop.hdfs.rs
--rw-r--r--   0     1001      127     8411 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/ClientDatanodeProtocol.proto
--rw-r--r--   0     1001      127    31840 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/ClientNamenodeProtocol.proto
--rw-r--r--   0     1001      127     2523 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/ReconfigurationProtocol.proto
--rw-r--r--   0     1001      127     2794 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/acl.proto
--rw-r--r--   0     1001      127     9922 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/datatransfer.proto
--rw-r--r--   0     1001      127     3028 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/encryption.proto
--rw-r--r--   0     1001      127     3281 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/erasurecoding.proto
--rw-r--r--   0     1001      127    21153 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/hdfs.proto
--rw-r--r--   0     1001      127     3607 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/inotify.proto
--rw-r--r--   0     1001      127     1996 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/xattr.proto
--rw-r--r--   0     1001      127      463 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/proto/mod.rs
--rw-r--r--   0     1001      127     5289 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/security/gssapi.rs
--rw-r--r--   0     1001      127       69 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/security/mod.rs
--rw-r--r--   0     1001      127    21086 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/security/sasl.rs
--rw-r--r--   0     1001      127    14514 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/security/user.rs
--rw-r--r--   0     1001      127      171 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/src/test.rs
--rw-r--r--   0     1001      127     1498 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/tests/common/mod.rs
--rw-r--r--   0     1001      127     6989 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/tests/test_ec.rs
--rw-r--r--   0     1001      127     7506 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/tests/test_integration.rs
--rw-r--r--   0     1001      127     1381 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/tests/test_read.rs
--rw-r--r--   0     1001      127     3512 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/tests/test_viewfs.rs
--rw-r--r--   0     1001      127     3671 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/tests/test_write.rs
--rw-r--r--   0     1001      127     1629 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/crates/hdfs-native/tests/test_write_resiliency.rs
--rw-r--r--   0     1001      127     4478 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/README.md
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 hdfs_native-0.8.0/python/Cargo.toml
--rw-r--r--   0     1001      127      550 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/README.md
--rw-r--r--   0     1001      127     3812 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/python/hdfs_native/__init__.py
--rw-r--r--   0     1001      127     1596 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/python/hdfs_native/_internal.pyi
--rw-r--r--   0     1001      127       25 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/requirements-dev.txt
--rw-r--r--   0     1001      127      741 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/src/error.rs
--rw-r--r--   0     1001      127     6563 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/src/lib.rs
--rw-r--r--   0     1001      127      682 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/tests/conftest.py
--rw-r--r--   0     1001      127     1538 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/tests/test_integration.py
--rw-r--r--   0     1001      127    48664 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/Cargo.lock
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 hdfs_native-0.8.0/pyproject.toml
--rw-r--r--   0     1001      127     3812 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/hdfs_native/__init__.py
--rw-r--r--   0     1001      127     1596 2024-03-21 21:52:37.000000 hdfs_native-0.8.0/python/hdfs_native/_internal.pyi
--rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 hdfs_native-0.8.0/PKG-INFO
+-rw-r--r--   0     1001      127     1723 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/Cargo.toml
+-rw-r--r--   0     1001      127     2127 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/benches/ec.rs
+-rw-r--r--   0     1001      127     5698 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/benches/io.rs
+-rw-r--r--   0     1001      127     1069 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/benches/rpc.rs
+-rw-r--r--   0     1001      127     1052 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/build.rs
+-rw-r--r--   0     1001      127     1918 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/examples/simple.rs
+-rw-r--r--   0     1001      127     1754 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/minidfs/pom.xml
+-rw-r--r--   0     1001      127    10183 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/minidfs/src/main/java/main/Main.java
+-rw-r--r--   0     1001      127      334 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/minidfs/src/main/resources/log4j.properties
+-rw-r--r--   0     1001      127    24644 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/client.rs
+-rw-r--r--   0     1001      127     6384 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/common/config.rs
+-rw-r--r--   0     1001      127       16 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/common/mod.rs
+-rw-r--r--   0     1001      127     6685 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/ec/gf256.rs
+-rw-r--r--   0     1001      127     7576 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/ec/matrix.rs
+-rw-r--r--   0     1001      127     4952 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/ec/mod.rs
+-rw-r--r--   0     1001      127     1711 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/error.rs
+-rw-r--r--   0     1001      127    10044 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/file.rs
+-rw-r--r--   0     1001      127    16386 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/block_reader.rs
+-rw-r--r--   0     1001      127    19697 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/block_writer.rs
+-rw-r--r--   0     1001      127    24269 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/connection.rs
+-rw-r--r--   0     1001      127      132 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/mod.rs
+-rw-r--r--   0     1001      127    14973 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/protocol.rs
+-rw-r--r--   0     1001      127     5913 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/proxy.rs
+-rw-r--r--   0     1001      127     1257 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/lib.rs
+-rw-r--r--   0     1001      127     4855 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/minidfs.rs
+-rw-r--r--   0     1001      127     2863 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/FSProtos.proto
+-rw-r--r--   0     1001      127     2090 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/GenericRefreshProtocol.proto
+-rw-r--r--   0     1001      127     1760 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/GetUserMappingsProtocol.proto
+-rw-r--r--   0     1001      127     3715 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/HAServiceProtocol.proto
+-rw-r--r--   0     1001      127     1922 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/IpcConnectionContext.proto
+-rw-r--r--   0     1001      127     2924 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/ProtobufRpcEngine.proto
+-rw-r--r--   0     1001      127     2915 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/ProtobufRpcEngine2.proto
+-rw-r--r--   0     1001      127     2725 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/ProtocolInfo.proto
+-rw-r--r--   0     1001      127     1767 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/RefreshAuthorizationPolicyProtocol.proto
+-rw-r--r--   0     1001      127     1673 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/RefreshCallQueueProtocol.proto
+-rw-r--r--   0     1001      127     2160 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/RefreshUserMappingsProtocol.proto
+-rw-r--r--   0     1001      127     7706 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/RpcHeader.proto
+-rw-r--r--   0     1001      127     2236 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/Security.proto
+-rw-r--r--   0     1001      127     2193 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/TraceAdmin.proto
+-rw-r--r--   0     1001      127     1867 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/ZKFCProtocol.proto
+-rw-r--r--   0     1001      127    27673 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hadoop.common.rs
+-rw-r--r--   0     1001      127   168627 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hadoop.hdfs.rs
+-rw-r--r--   0     1001      127     8411 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/ClientDatanodeProtocol.proto
+-rw-r--r--   0     1001      127    31840 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/ClientNamenodeProtocol.proto
+-rw-r--r--   0     1001      127     2523 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/ReconfigurationProtocol.proto
+-rw-r--r--   0     1001      127     2794 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/acl.proto
+-rw-r--r--   0     1001      127     9922 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/datatransfer.proto
+-rw-r--r--   0     1001      127     3028 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/encryption.proto
+-rw-r--r--   0     1001      127     3281 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/erasurecoding.proto
+-rw-r--r--   0     1001      127    21153 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/hdfs.proto
+-rw-r--r--   0     1001      127     3607 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/inotify.proto
+-rw-r--r--   0     1001      127     1996 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/xattr.proto
+-rw-r--r--   0     1001      127      463 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/proto/mod.rs
+-rw-r--r--   0     1001      127    22064 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/security/digest.rs
+-rw-r--r--   0     1001      127     5289 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/security/gssapi.rs
+-rw-r--r--   0     1001      127       81 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/security/mod.rs
+-rw-r--r--   0     1001      127    27171 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/security/sasl.rs
+-rw-r--r--   0     1001      127    14514 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/security/user.rs
+-rw-r--r--   0     1001      127      171 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/src/test.rs
+-rw-r--r--   0     1001      127     1498 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/tests/common/mod.rs
+-rw-r--r--   0     1001      127     6989 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/tests/test_ec.rs
+-rw-r--r--   0     1001      127     9145 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/tests/test_integration.rs
+-rw-r--r--   0     1001      127     2203 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/tests/test_read.rs
+-rw-r--r--   0     1001      127     3512 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/tests/test_viewfs.rs
+-rw-r--r--   0     1001      127     4512 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/tests/test_write.rs
+-rw-r--r--   0     1001      127     1629 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/crates/hdfs-native/tests/test_write_resiliency.rs
+-rw-r--r--   0     1001      127     4247 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/README.md
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 hdfs_native-0.9.1/python/Cargo.toml
+-rw-r--r--   0     1001      127      550 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/README.md
+-rw-r--r--   0     1001      127     3812 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/python/hdfs_native/__init__.py
+-rw-r--r--   0     1001      127     1596 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/python/hdfs_native/_internal.pyi
+-rw-r--r--   0     1001      127       25 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/requirements-dev.txt
+-rw-r--r--   0     1001      127      741 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/src/error.rs
+-rw-r--r--   0     1001      127     6563 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/src/lib.rs
+-rw-r--r--   0     1001      127      682 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/tests/conftest.py
+-rw-r--r--   0     1001      127     1538 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/tests/test_integration.py
+-rw-r--r--   0     1001      127    64559 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/Cargo.lock
+-rw-r--r--   0        0        0      199 1970-01-01 00:00:00.000000 hdfs_native-0.9.1/Cargo.toml
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 hdfs_native-0.9.1/pyproject.toml
+-rw-r--r--   0     1001      127     1596 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/hdfs_native/_internal.pyi
+-rw-r--r--   0     1001      127     3812 2024-04-08 01:50:42.000000 hdfs_native-0.9.1/python/hdfs_native/__init__.py
+-rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 hdfs_native-0.9.1/PKG-INFO
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/Cargo.toml` & `hdfs_native-0.9.1/crates/hdfs-native/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 [package]
 name = "hdfs-native"
-version = "0.8.0"
+version = "0.9.1"
 edition = "2021"
 authors = ["Adam Binford <adamq43@gmail.com>"]
 homepage = "https://github.com/Kimahriman/hdfs-native"
 repository = "https://github.com/Kimahriman/hdfs-native"
 keywords = ["hadoop", "hdfs"]
 description = "Native HDFS client implementation in Rust"
 readme = "../../README.md"
 license = "Apache-2.0"
 
 [dependencies]
+aes = "0.8"
 base64 = "0.21"
 bytes = { workspace = true }
+cbc = "0.1"
 chrono = { workspace = true }
-crc = "3.1.0-beta.1"
+cipher = "0.4"
+crc = "3.2"
+ctr = "0.9"
+des = "0.8"
 futures = { workspace = true }
 g2p = "1"
-gsasl-sys = { version = "0.2", default-features = false, optional = true }
+hex = "0.4"
+hmac = "0.12"
 libc = "0.2"
 libgssapi = { version = "0.7", default-features = false, optional = true }
-log = "0.4"
+log = { workspace = true }
+md-5 = "0.10"
 num-traits = "0.2"
 once_cell = "1"
 prost = "0.12"
 prost-types = "0.12"
+rand = "0.8"
+regex = "1"
 roxmltree = "0.18"
 socket2 = "0.5"
-thiserror = "1"
+thiserror = { workspace = true }
 tokio = { workspace = true, features = ["rt", "rt-multi-thread", "net", "io-util", "macros", "sync", "time"] }
 url = "2"
 users = { version = "0.11", default-features = false }
 uuid = { version = "1", features = ["v4"] }
 which = { version = "4", optional = true }
 
 [build-dependencies]
@@ -44,15 +53,14 @@
 fs-hdfs3 = "0.1.12"
 serial_test = "2.0.0"
 tempfile = "3"
 which = "4"
 
 [features]
 kerberos = ["libgssapi"]
-token = ["gsasl-sys"]
 
 generate-protobuf = ["prost-build", "protobuf-src"]
 integration-test = ["which"]
 benchmark = ["which"]
 
 [[bench]]
 name = "ec"
@@ -60,8 +68,8 @@
 
 [[bench]]
 name = "io"
 harness = false
 
 [[bench]]
 name = "rpc"
-harness = false
+harness = false
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/Cargo.lock` & `hdfs_native-0.9.1/Cargo.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "acid_io"
-version = "0.1.0"
+name = "addr2line"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e08a77c8b11dbd46fd3ba4f0aa0bf7ed078793201540779b0841a297acdad2c"
+checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
 dependencies = [
- "byteorder",
- "libc",
- "memchr",
- "windows 0.29.0",
+ "gimli",
 ]
 
 [[package]]
-name = "aho-corasick"
+name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
+name = "aes"
+version = "0.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b169f7a6d4742236a0a00c541b845991d0ac43e546831af1249753ab4c3aa3a0"
+dependencies = [
+ "cfg-if",
+ "cipher",
+ "cpufeatures",
+]
+
+[[package]]
+name = "aho-corasick"
+version = "1.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
@@ -35,256 +49,443 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "ansi_term"
-version = "0.12.1"
+name = "anes"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
-dependencies = [
- "winapi",
-]
+checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
+
+[[package]]
+name = "anstyle"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.77"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
-]
-
-[[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
-name = "base64"
-version = "0.13.1"
+name = "autotools"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+checksum = "aef8da1805e028a172334c3b680f93e71126f2327622faef2ec3d893c0a4ad77"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "backtrace"
+version = "0.3.69"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
 
 [[package]]
 name = "base64"
-version = "0.21.2"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bindgen"
-version = "0.55.1"
+version = "0.64.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75b13ce559e6433d360c26305643803cb52cfbabbc2b9c47ce04a58493dfb443"
+checksum = "c4243e6031260db77ede97ad86c27e501d646a27ab57b59a574f725d98ab1fb4"
 dependencies = [
  "bitflags 1.3.2",
- "cexpr 0.4.0",
- "cfg-if 0.1.10",
+ "cexpr",
  "clang-sys",
- "clap",
- "env_logger 0.7.1",
  "lazy_static",
  "lazycell",
  "log",
  "peeking_take_while",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
- "shlex 0.1.1",
- "which 3.1.1",
+ "shlex",
+ "syn 1.0.109",
+ "which",
 ]
 
 [[package]]
 name = "bindgen"
-version = "0.64.0"
+version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4243e6031260db77ede97ad86c27e501d646a27ab57b59a574f725d98ab1fb4"
+checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
 dependencies = [
- "bitflags 1.3.2",
- "cexpr 0.6.0",
+ "bitflags 2.4.2",
+ "cexpr",
  "clang-sys",
+ "itertools 0.12.1",
  "lazy_static",
  "lazycell",
  "log",
- "peeking_take_while",
+ "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
- "shlex 1.1.0",
- "syn 1.0.109",
- "which 4.4.0",
+ "shlex",
+ "syn 2.0.50",
+ "which",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.3.1"
+version = "2.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6776fc96284a0bb647b615056fc496d1fe1644a7ab01829818a6d91cae888b84"
+checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
-name = "bumpalo"
-version = "3.13.0"
+name = "block-padding"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+checksum = "a8894febbff9f758034a5b8e12d87918f56dfc64a8e1fe757d65e29041538d93"
+dependencies = [
+ "generic-array",
+]
 
 [[package]]
-name = "byteorder"
-version = "1.4.3"
+name = "bumpalo"
+version = "3.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+checksum = "d32a994c2b3ca201d9b263612a374263f05e7adde37c4707f693dcd375076d1f"
 
 [[package]]
 name = "bytes"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
+checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
 
 [[package]]
-name = "cc"
-version = "1.0.79"
+name = "cast"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
-name = "cexpr"
-version = "0.4.0"
+name = "cbc"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4aedb84272dbe89af497cf81375129abda4fc0a9e7c5d317498c15cc30c0d27"
+checksum = "26b52a9543ae338f279b96b0b9fed9c8093744685043739079ce85cd58f289a6"
 dependencies = [
- "nom 5.1.3",
+ "cipher",
 ]
 
 [[package]]
-name = "cexpr"
-version = "0.6.0"
+name = "cc"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
+checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
 dependencies = [
- "nom 7.1.3",
+ "libc",
 ]
 
 [[package]]
-name = "cfg-if"
-version = "0.1.10"
+name = "cexpr"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4785bdd1c96b2a846b2bd7cc02e86b6b3dbf14e7e53446c4f54c92a361040822"
+checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
+dependencies = [
+ "nom",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.26"
+version = "0.4.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
+checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
- "time",
+ "serde",
  "wasm-bindgen",
- "winapi",
+ "windows-targets 0.52.0",
+]
+
+[[package]]
+name = "ciborium"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
+dependencies = [
+ "ciborium-io",
+ "ciborium-ll",
+ "serde",
+]
+
+[[package]]
+name = "ciborium-io"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
+
+[[package]]
+name = "ciborium-ll"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57663b653d948a338bfb3eeba9bb2fd5fcfaecb9e199e87e1eda4d9e8b240fd9"
+dependencies = [
+ "ciborium-io",
+ "half",
+]
+
+[[package]]
+name = "cipher"
+version = "0.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
+dependencies = [
+ "crypto-common",
+ "inout",
 ]
 
 [[package]]
 name = "clang-sys"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c688fc74432808e3eb684cae8830a86be1d66a2bd58e1f248ed0960a590baf6f"
+checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
 dependencies = [
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
 name = "clap"
-version = "2.34.0"
+version = "4.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
+checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
 dependencies = [
- "ansi_term",
- "atty",
- "bitflags 1.3.2",
- "strsim",
- "textwrap",
- "unicode-width",
- "vec_map",
+ "clap_builder",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9f3e7391dad68afb0c2ede1bf619f579a3dc9c2ec67f089baa397123a2f3d1eb"
+dependencies = [
+ "anstyle",
+ "clap_lex",
+]
+
+[[package]]
+name = "clap_lex"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
+
+[[package]]
+name = "core-foundation"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.7"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "crc"
+version = "3.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c2b432c56615136f8dba245fed7ec3d5518c500a31108661067e61e72fe7e6bc"
+dependencies = [
+ "crc-catalog",
+]
+
+[[package]]
+name = "crc-catalog"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19d374276b40fb8bbdee95aef7c7fa6b5316ec764510eb64b8dd0e2ed0d7e7f5"
+
+[[package]]
+name = "criterion"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
+dependencies = [
+ "anes",
+ "cast",
+ "ciborium",
+ "clap",
+ "criterion-plot",
+ "futures",
+ "is-terminal",
+ "itertools 0.10.5",
+ "num-traits",
+ "once_cell",
+ "oorandom",
+ "plotters",
+ "rayon",
+ "regex",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "tinytemplate",
+ "tokio",
+ "walkdir",
+]
+
+[[package]]
+name = "criterion-plot"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
+dependencies = [
+ "cast",
+ "itertools 0.10.5",
+]
+
+[[package]]
+name = "crossbeam-deque"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
+dependencies = [
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
+name = "ctr"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0369ee1ad671834580515889b80f2ea915f23b8be8d0daa4bbaf2ac5c7590835"
+dependencies = [
+ "cipher",
+]
+
+[[package]]
+name = "dashmap"
+version = "5.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
+dependencies = [
+ "cfg-if",
+ "hashbrown",
+ "lock_api",
+ "once_cell",
+ "parking_lot_core",
+]
+
+[[package]]
+name = "des"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffdd80ce8ce993de27e9f063a444a4d53ce8e8db4c1f00cc03af5ad5a9867a1e"
+dependencies = [
+ "cipher",
+]
+
+[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
@@ -295,389 +496,586 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
-name = "env_logger"
-version = "0.7.1"
+name = "encoding_rs"
+version = "0.8.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44533bbbb3bb3c1fa17d9f2e4e38bbbaf8396ba82193c4cb1b6445d711445d36"
+checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
 dependencies = [
- "atty",
- "humantime 1.3.0",
- "log",
- "regex",
- "termcolor",
+ "cfg-if",
 ]
 
 [[package]]
 name = "env_logger"
-version = "0.10.0"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85cdab6a89accf66733ad5a1693a4dcced6aeff64602b634530dd73c1f3ee9f0"
+checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
 dependencies = [
- "humantime 2.1.0",
+ "humantime",
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
-name = "errno"
-version = "0.3.1"
+name = "equivalent"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "windows-sys 0.48.0",
-]
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
+name = "errno"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
- "cc",
  "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "1.9.0"
+version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
-dependencies = [
- "instant",
-]
+checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
+name = "fs-hdfs3"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0f38e500596a428817fd4fd8a9a21da32f4edb3250e87886039670b12ea02f5d"
+dependencies = [
+ "bindgen 0.64.0",
+ "cc",
+ "lazy_static",
+ "libc",
+ "log",
+ "url",
+]
+
+[[package]]
 name = "futures"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
+name = "g2gen"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fc2c7625b2fc250dd90b63f7887a6bb0f7ec1d714c8278415bea2669ef20820e"
+dependencies = [
+ "g2poly",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "g2p"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fc36d9bdc3d2da057775a9f4fa7d7b09edab3e0eda7a92cc353358fa63b8519e"
+dependencies = [
+ "g2gen",
+ "g2poly",
+]
+
+[[package]]
+name = "g2poly"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af6a86e750338603ea2c14b1c0bfe58cd61f87ca67a0021d9334996024608e12"
+
+[[package]]
 name = "generic-array"
 version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
- "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasi",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.28.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
-name = "gsasl-sys"
-version = "0.2.4"
+name = "h2"
+version = "0.3.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd377f206007e661591b4c6a6ba9907a75ae24e2a9ef40f3d0750a1db6bd5dbd"
+checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
 dependencies = [
- "bindgen 0.55.1",
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
+name = "half"
+version = "2.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+dependencies = [
+ "cfg-if",
+ "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
+version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "hdfs-native"
-version = "0.1.0"
+version = "0.9.1"
 dependencies = [
- "async-trait",
- "base64 0.21.2",
+ "aes",
+ "base64",
  "bytes",
+ "cbc",
  "chrono",
- "env_logger 0.10.0",
+ "cipher",
+ "crc",
+ "criterion",
+ "ctr",
+ "des",
+ "env_logger",
+ "fs-hdfs3",
  "futures",
- "gsasl-sys",
+ "g2p",
+ "hex",
+ "hmac",
  "libc",
  "libgssapi",
  "log",
- "object_store",
+ "md-5",
+ "num-traits",
+ "once_cell",
  "prost",
  "prost-build",
  "prost-types",
+ "protobuf-src",
+ "rand",
+ "regex",
  "roxmltree",
- "rsasl",
+ "serial_test",
+ "socket2",
  "tempfile",
  "thiserror",
  "tokio",
  "url",
  "users",
  "uuid",
- "which 4.4.0",
+ "which",
+]
+
+[[package]]
+name = "hdfs-native-object-store"
+version = "0.9.1"
+dependencies = [
+ "async-trait",
+ "bytes",
+ "chrono",
+ "criterion",
+ "env_logger",
+ "futures",
+ "hdfs-native",
+ "object_store",
+ "serial_test",
+ "tempfile",
+ "thiserror",
+ "tokio",
+ "which",
+]
+
+[[package]]
+name = "hdfs-native-python"
+version = "0.9.1"
+dependencies = [
+ "bytes",
+ "env_logger",
+ "hdfs-native",
+ "log",
+ "pyo3",
+ "thiserror",
+ "tokio",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.1.19"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
+checksum = "bd5256b483761cd23699d0da46cc6fd2ee3be420bbe6d020ae4a091e70b7e9fd"
 
 [[package]]
-name = "hermit-abi"
-version = "0.3.1"
+name = "hex"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
-name = "humantime"
-version = "1.3.0"
+name = "home"
+version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df004cfca50ef23c36850aaaa59ad52cc70d0e90243c3c7737a4dd32dc7a3c4f"
+checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
- "quick-error",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "http"
+version = "0.2.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8947b1a6fad4393052c7ba1f4cd97bed3e953a95c79c92ad9b051a04611d9fbb"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
+name = "http-body"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
+dependencies = [
+ "bytes",
+ "http",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "httparse"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
+
+[[package]]
+name = "httpdate"
+version = "1.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
+
+[[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
+name = "hyper"
+version = "0.14.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower-service",
+ "tracing",
+ "want",
+]
+
+[[package]]
+name = "hyper-rustls"
+version = "0.24.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
+dependencies = [
+ "futures-util",
+ "http",
+ "hyper",
+ "rustls",
+ "tokio",
+ "tokio-rustls",
+]
+
+[[package]]
 name = "iana-time-zone"
-version = "0.1.57"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "windows 0.48.0",
+ "windows-core",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.3"
+version = "2.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+checksum = "233cf39063f058ea2caae4091bf4a3ef70a653afbc026f5c4a4135d114e3c177"
 dependencies = [
- "autocfg",
+ "equivalent",
  "hashbrown",
 ]
 
 [[package]]
-name = "instant"
-version = "0.1.12"
+name = "indoc"
+version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
-dependencies = [
- "cfg-if 1.0.0",
-]
+checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
 
 [[package]]
-name = "io-lifetimes"
-version = "1.0.10"
+name = "inout"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
- "hermit-abi 0.3.1",
- "libc",
- "windows-sys 0.48.0",
+ "block-padding",
+ "generic-array",
 ]
 
 [[package]]
+name = "ipnet"
+version = "2.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
+
+[[package]]
 name = "is-terminal"
-version = "0.4.7"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
- "rustix",
- "windows-sys 0.48.0",
+ "hermit-abi",
+ "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+dependencies = [
+ "either",
+]
+
+[[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -688,332 +1086,475 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.147"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libgssapi"
-version = "0.6.4"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dcfb7f77cbefc242a46ea667491c4f1129712f563cd368623d3f1b261a90e5f"
+checksum = "c22f0430969e524b2177498ca3eeed48faca6f6c80f1b098d27ecbec84222f3a"
 dependencies = [
- "bitflags 2.3.1",
+ "bitflags 2.4.2",
  "bytes",
  "lazy_static",
  "libgssapi-sys",
 ]
 
 [[package]]
 name = "libgssapi-sys"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efdcdd31923aa6280d41ff2636fd93a18cc60fe25983b24887d1a8d24478cbfb"
+checksum = "b57d9a71c774ec53b1b9119dbbcc589b5209831f0ddc0ff4210640051f545372"
 dependencies = [
- "bindgen 0.64.0",
+ "bindgen 0.69.4",
+ "pkg-config",
 ]
 
 [[package]]
 name = "libloading"
-version = "0.7.4"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
+checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
 dependencies = [
- "cfg-if 1.0.0",
- "winapi",
+ "cfg-if",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "linkme"
-version = "0.2.10"
+name = "linux-raw-sys"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "edd4ad156b9934dc21cad96fd17278a7cb6f30a5657a9d976cd7b71d6d49c02c"
-dependencies = [
- "linkme-impl",
-]
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
-name = "linkme-impl"
-version = "0.2.10"
+name = "lock_api"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73fd9dc7072de7168cbdaba9125e8f742cd3a965aa12bde994b4611a174488d8"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
+ "autocfg",
+ "scopeguard",
 ]
 
 [[package]]
-name = "linux-raw-sys"
-version = "0.3.7"
+name = "log"
+version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
+checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 
 [[package]]
-name = "lock_api"
-version = "0.4.10"
+name = "md-5"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "d89e7ee0cfbedfc4da3340218492196241d89eefb6dab27de5df917a6d2e78cf"
 dependencies = [
- "autocfg",
- "scopeguard",
+ "cfg-if",
+ "digest",
 ]
 
 [[package]]
-name = "log"
-version = "0.4.18"
+name = "memchr"
+version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
-name = "memchr"
-version = "2.5.0"
+name = "memoffset"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "mime"
+version = "0.3.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
 name = "mio"
-version = "0.8.8"
+version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
+checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
 dependencies = [
  "libc",
- "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "nom"
-version = "5.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08959a387a676302eebf4ddbcbc611da04285579f76f88ee0506c63b1a61dd4b"
-dependencies = [
- "memchr",
- "version_check",
-]
-
-[[package]]
-name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "num_cpus"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
+dependencies = [
+ "hermit-abi",
+ "libc",
+]
+
+[[package]]
+name = "object"
+version = "0.32.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "object_store"
-version = "0.6.1"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "27c776db4f332b571958444982ff641d2531417a326ca368995073b639205d58"
+checksum = "d139f545f64630e2e3688fd9f81c470888ab01edeb72d13b4e86c566f1130000"
 dependencies = [
  "async-trait",
+ "base64",
  "bytes",
  "chrono",
  "futures",
- "humantime 2.1.0",
- "itertools",
+ "humantime",
+ "hyper",
+ "itertools 0.12.1",
  "parking_lot",
  "percent-encoding",
+ "quick-xml",
+ "rand",
+ "reqwest",
+ "ring",
+ "serde",
+ "serde_json",
  "snafu",
  "tokio",
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
+
+[[package]]
+name = "oorandom"
+version = "11.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
+
+[[package]]
+name = "openssl-probe"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "pbkdf2"
-version = "0.10.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "271779f35b581956db91a3e55737327a03aa051e90b1c47aeb189508533adfd7"
-dependencies = [
- "digest",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "petgraph"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
+checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
+name = "pkg-config"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
+
+[[package]]
+name = "plotters"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
+dependencies = [
+ "num-traits",
+ "plotters-backend",
+ "plotters-svg",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
+name = "plotters-backend"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
+
+[[package]]
+name = "plotters-svg"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
+dependencies = [
+ "plotters-backend",
+]
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
-version = "0.1.25"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c8646e95016a7a6c4adea95bafa8a16baab64b583356217f2c85db4a39d9a86"
+checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
 dependencies = [
  "proc-macro2",
- "syn 1.0.109",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
-version = "0.11.9"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
+checksum = "146c289cda302b98a28d40c8b3b90498d6e526dd24ac2ecea73e4e491685b94a"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
 name = "prost-build"
-version = "0.11.9"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "119533552c9a7ffacc21e099c24a0ac8bb19c2a2a3f363de84cd9b844feab270"
+checksum = "c55e02e35260070b6f716a2423c2ff1c3bb1642ddca6f99e1f26d06268a0e2d2"
 dependencies = [
  "bytes",
  "heck",
- "itertools",
- "lazy_static",
+ "itertools 0.11.0",
  "log",
  "multimap",
+ "once_cell",
  "petgraph",
  "prettyplease",
  "prost",
  "prost-types",
  "regex",
- "syn 1.0.109",
+ "syn 2.0.50",
  "tempfile",
- "which 4.4.0",
+ "which",
 ]
 
 [[package]]
 name = "prost-derive"
-version = "0.11.9"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
+checksum = "efb6c9a1dd1def8e2124d17e83a20af56f1570d6c2d2bd9e266ccb768df3840e"
 dependencies = [
  "anyhow",
- "itertools",
+ "itertools 0.11.0",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "prost-types"
-version = "0.11.9"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213622a1460818959ac1181aaeb2dc9c7f63df720db7d788b3e24eacd1983e13"
+checksum = "193898f59edcf43c26227dcd4c8427f00d99d61e95dcde58dabd49fa291d470e"
 dependencies = [
  "prost",
 ]
 
 [[package]]
-name = "quick-error"
-version = "1.2.3"
+name = "protobuf-src"
+version = "1.1.0+21.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7ac8852baeb3cc6fb83b93646fb93c0ffe5d14bf138c945ceb4b9948ee0e3c1"
+dependencies = [
+ "autotools",
+]
+
+[[package]]
+name = "pyo3"
+version = "0.20.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+dependencies = [
+ "cfg-if",
+ "indoc",
+ "libc",
+ "memoffset",
+ "parking_lot",
+ "pyo3-build-config",
+ "pyo3-ffi",
+ "pyo3-macros",
+ "unindent",
+]
+
+[[package]]
+name = "pyo3-build-config"
+version = "0.20.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+dependencies = [
+ "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.20.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
+]
+
+[[package]]
+name = "pyo3-macros"
+version = "0.20.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+dependencies = [
+ "proc-macro2",
+ "pyo3-macros-backend",
+ "quote",
+ "syn 2.0.50",
+]
+
+[[package]]
+name = "pyo3-macros-backend"
+version = "0.20.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.50",
+]
+
+[[package]]
+name = "quick-xml"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
+checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
+dependencies = [
+ "memchr",
+ "serde",
+]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1041,237 +1582,395 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
+name = "rayon"
+version = "1.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+dependencies = [
+ "either",
+ "rayon-core",
+]
+
+[[package]]
+name = "rayon-core"
+version = "1.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
+dependencies = [
+ "crossbeam-deque",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
-name = "roxmltree"
-version = "0.18.0"
+name = "reqwest"
+version = "0.11.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8f595a457b6b8c6cda66a48503e92ee8d19342f905948f29c383200ec9eb1d8"
+checksum = "c6920094eb85afde5e4a138be3f2de8bbdf28000f0029e72c45025a56b042251"
 dependencies = [
- "xmlparser",
+ "base64",
+ "bytes",
+ "encoding_rs",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-rustls",
+ "ipnet",
+ "js-sys",
+ "log",
+ "mime",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "rustls",
+ "rustls-native-certs",
+ "rustls-pemfile",
+ "serde",
+ "serde_json",
+ "serde_urlencoded",
+ "sync_wrapper",
+ "system-configuration",
+ "tokio",
+ "tokio-rustls",
+ "tokio-util",
+ "tower-service",
+ "url",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "wasm-streams",
+ "web-sys",
+ "winreg",
 ]
 
 [[package]]
-name = "rsasl"
-version = "2.0.0"
+name = "ring"
+version = "0.17.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
- "acid_io",
- "base64 0.13.1",
- "bitflags 1.3.2",
- "digest",
- "hmac",
- "libgssapi",
- "linkme",
- "pbkdf2",
- "rand",
- "serde",
- "serde_json",
- "sha-1",
- "sha2",
- "stringprep",
- "thiserror",
+ "cc",
+ "cfg-if",
+ "getrandom",
+ "libc",
+ "spin",
+ "untrusted",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
+name = "roxmltree"
+version = "0.18.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "862340e351ce1b271a378ec53f304a5558f7db87f3769dc655a8f6ecbb68b302"
+dependencies = [
+ "xmlparser",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.19"
+version = "0.38.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.4.2",
  "errno",
- "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
+name = "rustls"
+version = "0.21.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+dependencies = [
+ "log",
+ "ring",
+ "rustls-webpki",
+ "sct",
+]
+
+[[package]]
+name = "rustls-native-certs"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a9aace74cb666635c918e9c12bc0d348266037aa8eb599b5cba565709a8dff00"
+dependencies = [
+ "openssl-probe",
+ "rustls-pemfile",
+ "schannel",
+ "security-framework",
+]
+
+[[package]]
+name = "rustls-pemfile"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
+dependencies = [
+ "base64",
+]
+
+[[package]]
+name = "rustls-webpki"
+version = "0.101.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
+dependencies = [
+ "ring",
+ "untrusted",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
+name = "schannel"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
+dependencies = [
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
+
+[[package]]
+name = "sct"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
+name = "security-framework"
+version = "2.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
+dependencies = [
+ "bitflags 1.3.2",
+ "core-foundation",
+ "core-foundation-sys",
+ "libc",
+ "security-framework-sys",
+]
+
+[[package]]
+name = "security-framework-sys"
+version = "2.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.114"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
-name = "sha-1"
-version = "0.10.1"
+name = "serde_urlencoded"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5058ada175748e33390e40e872bd0fe59a19f265d0158daa551c5a88a76009c"
+checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
 dependencies = [
- "cfg-if 1.0.0",
- "cpufeatures",
- "digest",
+ "form_urlencoded",
+ "itoa",
+ "ryu",
+ "serde",
 ]
 
 [[package]]
-name = "sha2"
-version = "0.10.6"
+name = "serial_test"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "0e56dd856803e253c8f298af3f4d7eb0ae5e23a737252cd90bb4f3b435033b2d"
 dependencies = [
- "cfg-if 1.0.0",
- "cpufeatures",
- "digest",
+ "dashmap",
+ "futures",
+ "lazy_static",
+ "log",
+ "parking_lot",
+ "serial_test_derive",
 ]
 
 [[package]]
-name = "shlex"
-version = "0.1.1"
+name = "serial_test_derive"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fdf1b9db47230893d76faad238fd6097fd6d6a9245cd7a4d90dbd639536bbd2"
+checksum = "91d129178576168c589c9ec973feedf7d3126c01ac2bf08795109aa35b69fb8f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.50",
+]
 
 [[package]]
 name = "shlex"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
+checksum = "0fda2ff0d084019ba4d7c6f371c95d8fd75ce3524c3cb8fb653a3023f6323e64"
 
 [[package]]
 name = "slab"
-version = "0.4.8"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
+checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
 name = "snafu"
-version = "0.7.4"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb0656e7e3ffb70f6c39b3c2a86332bb74aa3c679da781642590f3c1118c5045"
+checksum = "e4de37ad025c587a29e8f3f5605c00f70b98715ef90b9061a815b9e59e9042d6"
 dependencies = [
  "doc-comment",
  "snafu-derive",
 ]
 
 [[package]]
 name = "snafu-derive"
-version = "0.7.4"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "475b3bbe5245c26f2d8a6f62d67c1f30eb9fffeccee721c45d162c3ebbdf81b2"
+checksum = "990079665f075b699031e9c08fd3ab99be5029b96f3b78dc0709e8f77e4efebf"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.4.9"
+version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
+checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
 dependencies = [
  "libc",
- "winapi",
-]
-
-[[package]]
-name = "stringprep"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ee348cb74b87454fff4b551cbf727025810a004f88aeacae7f85b87f4e9a1c1"
-dependencies = [
- "unicode-bidi",
- "unicode-normalization",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "strsim"
-version = "0.8.0"
+name = "spin"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea5119cdb4c55b55d432abb513a0429384878c15dde60cc77b1c99de1a95a6a"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
@@ -1284,83 +1983,105 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "74f1bdc9872430ce9b75da68329d1c1746faf50ffac5f19e02b71e37ff881ffb"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "tempfile"
-version = "3.5.0"
+name = "sync_wrapper"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
+
+[[package]]
+name = "system-configuration"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
+checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
 dependencies = [
- "cfg-if 1.0.0",
- "fastrand",
- "redox_syscall",
- "rustix",
- "windows-sys 0.45.0",
+ "bitflags 1.3.2",
+ "core-foundation",
+ "system-configuration-sys",
 ]
 
 [[package]]
-name = "termcolor"
-version = "1.2.0"
+name = "system-configuration-sys"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
+checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
 dependencies = [
- "winapi-util",
+ "core-foundation-sys",
+ "libc",
 ]
 
 [[package]]
-name = "textwrap"
-version = "0.11.0"
+name = "target-lexicon"
+version = "0.12.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
+checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+
+[[package]]
+name = "tempfile"
+version = "3.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a365e8cd18e44762ef95d87f284f4b5cd04107fec2ff3052bd6a3e6069669e67"
 dependencies = [
- "unicode-width",
+ "cfg-if",
+ "fastrand",
+ "rustix",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
+name = "termcolor"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
+dependencies = [
+ "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.50",
 ]
 
 [[package]]
-name = "time"
-version = "0.1.45"
+name = "tinytemplate"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
+checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
- "libc",
- "wasi 0.10.0+wasi-snapshot-preview1",
- "winapi",
+ "serde",
+ "serde_json",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -1372,109 +2093,151 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
 dependencies = [
- "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
+ "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
  "windows-sys 0.48.0",
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
- "syn 2.0.16",
+ "syn 2.0.50",
 ]
 
 [[package]]
+name = "tokio-rustls"
+version = "0.24.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
+dependencies = [
+ "rustls",
+ "tokio",
+]
+
+[[package]]
+name = "tokio-util"
+version = "0.7.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "futures-sink",
+ "pin-project-lite",
+ "tokio",
+ "tracing",
+]
+
+[[package]]
+name = "tower-service"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
+
+[[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "cfg-if 1.0.0",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.26"
+version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.31"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
+name = "try-lock"
+version = "0.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
+
+[[package]]
 name = "typenum"
-version = "1.16.0"
+version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
+name = "unindent"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
+
+[[package]]
+name = "untrusted"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
@@ -1484,127 +2247,151 @@
 checksum = "24cc0f6d6f267b73e5a2cadf007ba8f9bc39c6a6f9666f8cf25ea809a153b032"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.2"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dad5567ad0cf5b760e5665964bec1b47dfd077ba8a2544b513f3556d3d239a2"
+checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
-name = "vec_map"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
-
-[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.3.3"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
+checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
-name = "wasi"
-version = "0.10.0+wasi-snapshot-preview1"
+name = "want"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
+dependencies = [
+ "try-lock",
+]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.50",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
+name = "wasm-bindgen-futures"
+version = "0.4.41"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "877b9c3f61ceea0e56331985743b13f3d25c406a7098d45180fb5f09bc19ed97"
+dependencies = [
+ "cfg-if",
+ "js-sys",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.50",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
 
 [[package]]
-name = "which"
-version = "3.1.1"
+name = "wasm-streams"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d011071ae14a2f6671d0b74080ae0cd8ebf3a6f8c9589a2cd45f23126fe29724"
+checksum = "b65dc4c90b63b118468cf747d8bf3566c1913ef60be765b5730ead9e0a3ba129"
 dependencies = [
- "libc",
+ "futures-util",
+ "js-sys",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
+name = "web-sys"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96565907687f7aceb35bc5fc03770a8a0471d82e479f25832f54a0e3f4b28446"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "which"
-version = "4.4.0"
+version = "4.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
+checksum = "87ba24419a2078cd2b0f2ede2691b6c66d8e47836da3b6db8265ebad47afbfc7"
 dependencies = [
  "either",
- "libc",
+ "home",
  "once_cell",
+ "rustix",
 ]
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
@@ -1617,209 +2404,176 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows"
-version = "0.29.0"
+name = "windows-core"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aac7fef12f4b59cd0a29339406cc9203ab44e440ddff6b3f5a41455349fa9cf3"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows_aarch64_msvc 0.29.0",
- "windows_i686_gnu 0.29.0",
- "windows_i686_msvc 0.29.0",
- "windows_x86_64_gnu 0.29.0",
- "windows_x86_64_msvc 0.29.0",
-]
-
-[[package]]
-name = "windows"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
-dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets 0.52.0",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.42.2",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.48.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets 0.52.0",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm 0.52.0",
+ "windows_aarch64_msvc 0.52.0",
+ "windows_i686_gnu 0.52.0",
+ "windows_i686_msvc 0.52.0",
+ "windows_x86_64_gnu 0.52.0",
+ "windows_x86_64_gnullvm 0.52.0",
+ "windows_x86_64_msvc 0.52.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.29.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d027175d00b01e0cbeb97d6ab6ebe03b12330a35786cbaca5252b1c4bf5d9b"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.29.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8793f59f7b8e8b01eda1a652b2697d87b93097198ae85f823b969ca5b89bba58"
+checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.29.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8602f6c418b67024be2996c512f5f995de3ba417f4c75af68401ab8756796ae4"
+checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.29.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3d615f419543e0bd7d2b3323af0d86ff19cbc4f816e6453f36a2c2ce889c354"
+checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.29.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11d95421d9ed3672c280884da53201a5c46b7b2765ca6faf34b0d71cf34a3561"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
 
 [[package]]
-name = "windows_x86_64_msvc"
-version = "0.48.0"
+name = "winreg"
+version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
+dependencies = [
+ "cfg-if",
+ "windows-sys 0.48.0",
+]
 
 [[package]]
 name = "xmlparser"
-version = "0.13.5"
+version = "0.13.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d25c75bf9ea12c4040a97f829154768bbbce366287e2dc044af160cd79a13fd"
+checksum = "66fee0b777b0f5ac1c69bb06d361268faafa61cd4682ae064a171c16c433e9e4"
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/benches/ec.rs` & `hdfs_native-0.9.1/crates/hdfs-native/benches/ec.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/benches/io.rs` & `hdfs_native-0.9.1/crates/hdfs-native/benches/io.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/benches/rpc.rs` & `hdfs_native-0.9.1/crates/hdfs-native/benches/rpc.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/build.rs` & `hdfs_native-0.9.1/crates/hdfs-native/build.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 use std::io::Result;
 
 fn main() -> Result<()> {
-    #[cfg(feature = "token")]
-    println!("cargo:rustc-link-lib=gsasl");
-
     #[cfg(feature = "generate-protobuf")]
     {
         std::env::set_var("PROTOC", protobuf_src::protoc());
 
         prost_build::compile_protos(
             &[
                 "src/proto/hdfs/ClientNamenodeProtocol.proto",
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/examples/simple.rs` & `hdfs_native-0.9.1/crates/hdfs-native/examples/simple.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/minidfs/pom.xml` & `hdfs_native-0.9.1/crates/hdfs-native/minidfs/pom.xml`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/minidfs/src/main/java/main/Main.java` & `hdfs_native-0.9.1/crates/hdfs-native/minidfs/src/main/java/main/Main.java`

 * *Files 4% similar despite different names*

```diff
@@ -51,26 +51,35 @@
             kdc.start();
             kdc.createPrincipal(new File("target/test/hdfs.keytab"), "hdfs/localhost");
 
             conf.set(HADOOP_SECURITY_AUTHENTICATION, "kerberos");
             conf.set(HADOOP_SECURITY_AUTHORIZATION, "true");
             if (flags.contains("privacy")) {
                 conf.set(HADOOP_RPC_PROTECTION, "privacy");
+                conf.set(DFS_DATA_TRANSFER_PROTECTION_KEY, "privacy");
+                if (flags.contains("aes")) {
+                    conf.set(DFS_ENCRYPT_DATA_TRANSFER_CIPHER_SUITES_KEY, "AES/CTR/NoPadding");
+                }
+            } else if (flags.contains("integrity")) {
+                conf.set(HADOOP_RPC_PROTECTION, "integrity");
+                conf.set(DFS_DATA_TRANSFER_PROTECTION_KEY, "integrity");
             } else {
                 conf.set(HADOOP_RPC_PROTECTION, "authentication");
+                conf.set(DFS_DATA_TRANSFER_PROTECTION_KEY, "authentication");
+            }
+            if (flags.contains("data_transfer_encryption")) {
+                // Force encryption for all connections, legacy method before SASL connections were a thing
+                conf.set(DFSConfigKeys.DFS_ENCRYPT_DATA_TRANSFER_KEY, "true");
             }
             conf.set(DFSConfigKeys.DFS_NAMENODE_KEYTAB_FILE_KEY, "target/test/hdfs.keytab");
             conf.set(DFS_NAMENODE_KERBEROS_PRINCIPAL_KEY, "hdfs/localhost@" + kdc.getRealm());
             conf.set(DFSConfigKeys.DFS_DATANODE_KEYTAB_FILE_KEY, "target/test/hdfs.keytab");
             conf.set(DFS_DATANODE_KERBEROS_PRINCIPAL_KEY, "hdfs/localhost@" + kdc.getRealm());
             conf.set(DFSConfigKeys.DFS_BLOCK_ACCESS_TOKEN_ENABLE_KEY, "true");
             conf.set(DFSConfigKeys.IGNORE_SECURE_PORTS_FOR_TESTING_KEY, "true");
-            if (flags.contains("data_transfer_security")) {
-                conf.set(DFS_DATA_TRANSFER_PROTECTION_KEY, "authentication");
-            }
         }
 
         HdfsConfiguration hdfsConf = new HdfsConfiguration(conf);
 
         MiniDFSCluster dfs = null;
         StateStoreDFSCluster routerDfs = null;
         if (flags.contains("rbf")) {
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/client.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/client.rs`

 * *Files 3% similar despite different names*

```diff
@@ -282,15 +282,20 @@
                     return Err(HdfsError::UnsupportedFeature("File encryption".to_string()));
                 }
                 if status.file_type() == FileType::IsDir {
                     return Err(HdfsError::IsADirectoryError(path.to_string()));
                 }
 
                 if let Some(locations) = status.locations.take() {
-                    Ok(FileReader::new(status, locations, ec_schema))
+                    Ok(FileReader::new(
+                        Arc::clone(&link.protocol),
+                        status,
+                        locations,
+                        ec_schema,
+                    ))
                 } else {
                     Err(HdfsError::BlocksNotFound(path.to_string()))
                 }
             }
             None => Err(HdfsError::FileNotFound(path.to_string())),
         }
     }
@@ -301,32 +306,24 @@
         &self,
         src: &str,
         write_options: impl AsRef<WriteOptions>,
     ) -> Result<FileWriter> {
         let write_options = write_options.as_ref();
 
         let (link, resolved_path) = self.mount_table.resolve(src);
-        let server_defaults = link.protocol.get_server_defaults().await?.server_defaults;
-
-        let block_size = write_options
-            .block_size
-            .unwrap_or(server_defaults.block_size);
-        let replication = write_options
-            .replication
-            .unwrap_or(server_defaults.replication);
 
         let create_response = link
             .protocol
             .create(
                 &resolved_path,
                 write_options.permission,
                 write_options.overwrite,
                 write_options.create_parent,
-                replication,
-                block_size,
+                write_options.replication,
+                write_options.block_size,
             )
             .await?;
 
         match create_response.fs {
             Some(status) => {
                 if status.file_encryption_info.is_some() {
                     let _ = self.delete(src, false).await;
@@ -334,15 +331,14 @@
                 }
 
                 Ok(FileWriter::new(
                     Arc::clone(&link.protocol),
                     resolved_path,
                     status,
                     None,
-                    server_defaults,
                 ))
             }
             None => Err(HdfsError::FileNotFound(src.to_string())),
         }
     }
 
     fn needs_new_block(class: &str, msg: &str) -> bool {
@@ -350,15 +346,14 @@
     }
 
     /// Opens an existing file for appending. An Err will be returned if the file does not exist. If the
     /// file is replicated, the current block will be appended to until it is full. If the file is erasure
     /// coded, a new block will be created.
     pub async fn append(&self, src: &str) -> Result<FileWriter> {
         let (link, resolved_path) = self.mount_table.resolve(src);
-        let server_defaults = link.protocol.get_server_defaults().await?.server_defaults;
 
         // Assume the file is replicated and try to append to the current block. If the file is
         // erasure coded, then try again by appending to a new block.
         let append_response = match link.protocol.append(&resolved_path, false).await {
             Err(HdfsError::RPCError(class, msg)) if Self::needs_new_block(&class, &msg) => {
                 link.protocol.append(&resolved_path, true).await?
             }
@@ -376,15 +371,14 @@
                 }
 
                 Ok(FileWriter::new(
                     Arc::clone(&link.protocol),
                     resolved_path,
                     status,
                     append_response.block,
-                    server_defaults,
                 ))
             }
             None => Err(HdfsError::FileNotFound(src.to_string())),
         }
     }
 
     /// Create a new directory at `path` with the given `permission`.
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/common/config.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/common/config.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/ec/gf256.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/ec/gf256.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/ec/matrix.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/ec/matrix.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/ec/mod.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/ec/mod.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/error.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/error.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/file.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/file.rs`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 use crate::proto::hdfs;
 use crate::{HdfsError, Result};
 
 const COMPLETE_RETRY_DELAY_MS: u64 = 500;
 const COMPLETE_RETRIES: u32 = 5;
 
 pub struct FileReader {
+    protocol: Arc<NamenodeProtocol>,
     status: hdfs::HdfsFileStatusProto,
     located_blocks: hdfs::LocatedBlocksProto,
     ec_schema: Option<EcSchema>,
     position: usize,
 }
 
 impl FileReader {
     pub(crate) fn new(
+        protocol: Arc<NamenodeProtocol>,
         status: hdfs::HdfsFileStatusProto,
         located_blocks: hdfs::LocatedBlocksProto,
         ec_schema: Option<EcSchema>,
     ) -> Self {
         Self {
+            protocol,
             status,
             located_blocks,
             ec_schema,
             position: 0,
         }
     }
 
@@ -121,14 +124,15 @@
                 let block_file_end = block_file_start + block.b.num_bytes() as usize;
 
                 if block_file_start < (offset + len) && block_file_end > offset {
                     // We need to read this block
                     let block_start = offset - usize::min(offset, block_file_start);
                     let block_end = usize::min(offset + len, block_file_end) - block_file_start;
                     Some(get_block_stream(
+                        Arc::clone(&self.protocol),
                         block.clone(),
                         block_start,
                         block_end - block_start,
                         self.ec_schema.clone(),
                     ))
                 } else {
                     // No data is needed from this block
@@ -141,36 +145,33 @@
     }
 }
 
 pub struct FileWriter {
     src: String,
     protocol: Arc<NamenodeProtocol>,
     status: hdfs::HdfsFileStatusProto,
-    server_defaults: hdfs::FsServerDefaultsProto,
     block_writer: Option<BlockWriter>,
     last_block: Option<hdfs::LocatedBlockProto>,
     closed: bool,
     bytes_written: usize,
 }
 
 impl FileWriter {
     pub(crate) fn new(
         protocol: Arc<NamenodeProtocol>,
         src: String,
         status: hdfs::HdfsFileStatusProto,
         // Some for append, None for create
         last_block: Option<hdfs::LocatedBlockProto>,
-        server_defaults: hdfs::FsServerDefaultsProto,
     ) -> Self {
         protocol.add_file_lease(status.file_id(), status.namespace.clone());
         Self {
             protocol,
             src,
             status,
-            server_defaults,
             block_writer: None,
             last_block,
             closed: false,
             bytes_written: 0,
         }
     }
 
@@ -202,17 +203,18 @@
             self.protocol
                 .add_block(&self.src, extended_block, self.status.file_id)
                 .await?
                 .block
         };
 
         let block_writer = BlockWriter::new(
+            Arc::clone(&self.protocol),
             new_block,
             self.status.blocksize() as usize,
-            self.server_defaults.clone(),
+            self.protocol.get_cached_server_defaults().await?,
             self.status
                 .ec_policy
                 .as_ref()
                 .map(resolve_ec_policy)
                 .transpose()?
                 .as_ref(),
         )
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/block_reader.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/block_reader.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::collections::HashMap;
+use std::{collections::HashMap, sync::Arc};
 
 use bytes::{Buf, BufMut, Bytes, BytesMut};
 use futures::{
     future::join_all,
     stream::{self, BoxStream},
     Stream, StreamExt,
 };
@@ -14,33 +14,37 @@
     proto::{
         common,
         hdfs::{self, BlockOpResponseProto},
     },
     HdfsError, Result,
 };
 
+use super::protocol::NamenodeProtocol;
+
 pub(crate) fn get_block_stream(
+    protocol: Arc<NamenodeProtocol>,
     block: hdfs::LocatedBlockProto,
     offset: usize,
     len: usize,
     ec_schema: Option<EcSchema>,
 ) -> BoxStream<'static, Result<Bytes>> {
     if let Some(ec_schema) = ec_schema {
-        StripedBlockStream::new(block, offset, len, ec_schema)
+        StripedBlockStream::new(protocol, block, offset, len, ec_schema)
             .into_stream()
             .boxed()
     } else {
-        ReplicatedBlockStream::new(block, offset, len)
+        ReplicatedBlockStream::new(protocol, block, offset, len)
             .into_stream()
             .boxed()
     }
 }
 
 /// Connects to a DataNode to do a read, attempting to used cached connections.
 async fn connect_and_send(
+    protocol: &Arc<NamenodeProtocol>,
     datanode_id: &hdfs::DatanodeIdProto,
     block: &hdfs::ExtendedBlockProto,
     token: common::TokenProto,
     offset: u64,
     len: u64,
 ) -> Result<(DatanodeConnection, BlockOpResponseProto)> {
     let mut remaining_attempts = 2;
@@ -64,15 +68,20 @@
                 }
             }
         } else {
             break;
         }
         remaining_attempts -= 1;
     }
-    let mut conn = DatanodeConnection::connect(datanode_id, &token).await?;
+    let mut conn = DatanodeConnection::connect(
+        datanode_id,
+        &token,
+        protocol.get_cached_data_encryption_key().await?,
+    )
+    .await?;
 
     let message = hdfs::OpReadBlockProto {
         header: conn.build_header(block, Some(token)),
         offset,
         len,
         send_checksums: Some(true),
         ..Default::default()
@@ -81,26 +90,33 @@
     debug!("Block read op request {:?}", &message);
     let response = conn.send(Op::ReadBlock, &message).await?;
     debug!("Block read op response {:?}", response);
     Ok((conn, response))
 }
 
 struct ReplicatedBlockStream {
+    protocol: Arc<NamenodeProtocol>,
     block: hdfs::LocatedBlockProto,
     offset: usize,
     len: usize,
 
     connection: Option<DatanodeConnection>,
     checksum_info: Option<hdfs::ReadOpChecksumInfoProto>,
     current_replica: usize,
 }
 
 impl ReplicatedBlockStream {
-    fn new(block: hdfs::LocatedBlockProto, offset: usize, len: usize) -> Self {
+    fn new(
+        protocol: Arc<NamenodeProtocol>,
+        block: hdfs::LocatedBlockProto,
+        offset: usize,
+        len: usize,
+    ) -> Self {
         Self {
+            protocol,
             block,
             offset,
             len,
             connection: None,
             checksum_info: None,
             current_replica: 0,
         }
@@ -115,14 +131,15 @@
                 ));
             }
         }
 
         let datanode = &self.block.locs[self.current_replica].id;
 
         let (connection, response) = connect_and_send(
+            &self.protocol,
             datanode,
             &self.block.b,
             self.block.block_token.clone(),
             self.offset as u64,
             self.len as u64,
         )
         .await?;
@@ -178,23 +195,31 @@
             let next = state.next_packet().await.transpose();
             next.map(|n| (n, state))
         })
     }
 }
 
 struct StripedBlockStream {
+    protocol: Arc<NamenodeProtocol>,
     block: hdfs::LocatedBlockProto,
     offset: usize,
     len: usize,
     ec_schema: EcSchema,
 }
 
 impl StripedBlockStream {
-    fn new(block: hdfs::LocatedBlockProto, offset: usize, len: usize, ec_schema: EcSchema) -> Self {
+    fn new(
+        protocol: Arc<NamenodeProtocol>,
+        block: hdfs::LocatedBlockProto,
+        offset: usize,
+        len: usize,
+        ec_schema: EcSchema,
+    ) -> Self {
         Self {
+            protocol,
             block,
             offset,
             len,
             ec_schema,
         }
     }
 
@@ -246,32 +271,41 @@
 
         // Block start/end within each vertical stripe, tail-exclusive
         let block_start = self.ec_schema.offset_for_row(starting_row);
         let block_end = self.ec_schema.offset_for_row(ending_row);
         let block_read_len = block_end - block_start;
 
         assert_eq!(self.block.block_indices().len(), self.block.locs.len());
-        let block_map: HashMap<u8, &hdfs::DatanodeInfoProto> = self
+        let datanode_infos: Vec<(&hdfs::DatanodeInfoProto, &common::TokenProto)> = self
+            .block
+            .locs
+            .iter()
+            .zip(self.block.block_tokens.iter())
+            .collect();
+
+        let block_map: HashMap<u8, (&hdfs::DatanodeInfoProto, &common::TokenProto)> = self
             .block
             .block_indices()
             .iter()
             .copied()
-            .zip(self.block.locs.iter())
+            .zip(datanode_infos.into_iter())
             .collect();
 
         let mut stripe_results: Vec<Option<Bytes>> =
             vec![None; self.ec_schema.data_units + self.ec_schema.parity_units];
 
         let mut futures = Vec::new();
 
         for index in 0..self.ec_schema.data_units as u8 {
+            let datanode_info = block_map.get(&index);
             futures.push(self.read_vertical_stripe(
                 &self.ec_schema,
                 index,
-                block_map.get(&index),
+                datanode_info.map(|(datanode, _)| datanode),
+                datanode_info.map(|(_, token)| token),
                 block_start,
                 block_read_len,
             ));
         }
 
         // Do the actual reads and count how many data blocks failed
         let mut failed_data_blocks = 0usize;
@@ -283,20 +317,21 @@
             }
         }
 
         let mut blocks_needed = failed_data_blocks;
         let mut parity_unit = 0usize;
         while blocks_needed > 0 && parity_unit < self.ec_schema.parity_units {
             let block_index = (self.ec_schema.data_units + parity_unit) as u8;
-            let datanode_info = block_map.get(&block_index).unwrap();
+            let datanode_info = block_map.get(&block_index);
             let result = self
                 .read_vertical_stripe(
                     &self.ec_schema,
                     block_index,
-                    Some(datanode_info),
+                    datanode_info.map(|(datanode, _)| datanode),
+                    datanode_info.map(|(_, token)| token),
                     block_start,
                     block_read_len,
                 )
                 .await;
 
             if let Ok(bytes) = result {
                 stripe_results[block_index as usize] = Some(bytes);
@@ -333,50 +368,51 @@
     }
 
     async fn read_vertical_stripe(
         &self,
         ec_schema: &EcSchema,
         index: u8,
         datanode: Option<&&hdfs::DatanodeInfoProto>,
+        token: Option<&&common::TokenProto>,
         offset: usize,
         len: usize,
     ) -> Result<Bytes> {
         #[cfg(feature = "integration-test")]
         if let Some(fault_injection) = crate::test::EC_FAULT_INJECTOR.lock().unwrap().as_ref() {
             if fault_injection.fail_blocks.contains(&(index as usize)) {
                 debug!("Failing block read for {}", index);
                 return Err(HdfsError::InternalError("Testing error".to_string()));
             }
         }
+        let max_block_offset =
+            ec_schema.max_offset(index as usize, self.block.b.num_bytes() as usize);
 
-        let mut buf = BytesMut::zeroed(len);
-        if let Some(datanode_info) = datanode {
-            let max_block_offset =
-                ec_schema.max_offset(index as usize, self.block.b.num_bytes() as usize);
+        let read_len = usize::min(len, max_block_offset - offset);
 
-            let read_len = usize::min(len, max_block_offset - offset);
+        if read_len == 0 {
+            // We're past the end of the file so there's nothign to read, just return a zeroed buffer
+            Ok(BytesMut::zeroed(len).freeze())
+        } else if let Some((datanode_info, token)) = datanode.zip(token) {
+            let mut buf = BytesMut::zeroed(len);
 
             // Each vertical stripe has a block ID of the original located block ID + block index
             // That was fun to figure out
             let mut block = self.block.b.clone();
             block.block_id += index as u64;
 
-            // The token of the first block is the main one, then all the rest are in the `block_tokens` list
-            let token = &self.block.block_tokens[self
-                .block
-                .block_indices()
-                .iter()
-                .position(|x| *x == index)
-                .unwrap()];
-
             self.read_from_datanode(&datanode_info.id, &block, token, offset, read_len, &mut buf)
                 .await?;
-        }
 
-        Ok(buf.freeze())
+            Ok(buf.freeze())
+        } else {
+            // There should be data to read but we didn't get block info for this index, so this shard is missing
+            Err(HdfsError::ErasureCodingError(
+                "Shard is missing".to_string(),
+            ))
+        }
     }
 
     async fn read_from_datanode(
         &self,
         datanode: &hdfs::DatanodeIdProto,
         block: &hdfs::ExtendedBlockProto,
         token: &common::TokenProto,
@@ -384,16 +420,23 @@
         len: usize,
         mut buf: &mut [u8],
     ) -> Result<()> {
         if len == 0 {
             return Ok(());
         }
 
-        let (mut connection, response) =
-            connect_and_send(datanode, block, token.clone(), offset as u64, len as u64).await?;
+        let (mut connection, response) = connect_and_send(
+            &self.protocol,
+            datanode,
+            block,
+            token.clone(),
+            offset as u64,
+            len as u64,
+        )
+        .await?;
 
         if response.status() != hdfs::Status::Success {
             return Err(HdfsError::DataTransferError(response.message().to_string()));
         }
 
         // First handle the offset into the first packet
         let mut packet = connection.read_packet().await?;
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/block_writer.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/block_writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-use std::time::Duration;
+use std::{sync::Arc, time::Duration};
 
 use bytes::{BufMut, Bytes, BytesMut};
 use futures::future::join_all;
 use log::debug;
 use tokio::{sync::mpsc, task::JoinHandle};
 
 use crate::{
     ec::{gf256::Coder, EcSchema},
     hdfs::connection::{DatanodeConnection, DatanodeReader, DatanodeWriter, Op, Packet},
     proto::hdfs,
     HdfsError, Result,
 };
 
+use super::protocol::NamenodeProtocol;
+
 const HEART_BEAT_SEQNO: i64 = -1;
 const UNKNOWN_SEQNO: i64 = -2;
 
 const HEARTBEAT_INTERVAL_SECONDS: u64 = 30;
 
 /// Wrapper around both types of block writers. This was simpler than trying to
 /// do dynamic dispatch with a BlockWriter trait.
 pub(crate) enum BlockWriter {
     Replicated(ReplicatedBlockWriter),
     Striped(StripedBlockWriter),
 }
 
 impl BlockWriter {
     pub(crate) async fn new(
+        protocol: Arc<NamenodeProtocol>,
         block: hdfs::LocatedBlockProto,
         block_size: usize,
         server_defaults: hdfs::FsServerDefaultsProto,
         ec_schema: Option<&EcSchema>,
     ) -> Result<Self> {
         let block_writer = if let Some(ec_schema) = ec_schema {
             Self::Striped(StripedBlockWriter::new(
+                protocol,
                 block,
                 ec_schema,
                 block_size,
                 server_defaults,
             ))
         } else {
-            Self::Replicated(ReplicatedBlockWriter::new(block, block_size, server_defaults).await?)
+            Self::Replicated(
+                ReplicatedBlockWriter::new(&protocol, block, block_size, server_defaults).await?,
+            )
         };
         Ok(block_writer)
     }
 
     pub(crate) async fn write(&mut self, buf: &mut Bytes) -> Result<()> {
         match self {
             Self::Replicated(writer) => writer.write(buf).await,
@@ -91,20 +97,26 @@
 
     ack_queue: mpsc::Sender<(i64, bool)>,
     packet_sender: mpsc::Sender<Packet>,
 }
 
 impl ReplicatedBlockWriter {
     async fn new(
+        protocol: &Arc<NamenodeProtocol>,
         block: hdfs::LocatedBlockProto,
         block_size: usize,
         server_defaults: hdfs::FsServerDefaultsProto,
     ) -> Result<Self> {
         let datanode = &block.locs[0].id;
-        let mut connection = DatanodeConnection::connect(datanode, &block.block_token).await?;
+        let mut connection = DatanodeConnection::connect(
+            datanode,
+            &block.block_token,
+            protocol.get_cached_data_encryption_key().await?,
+        )
+        .await?;
 
         let checksum = hdfs::ChecksumProto {
             r#type: hdfs::ChecksumTypeProto::ChecksumCrc32c as i32,
             bytes_per_checksum: server_defaults.bytes_per_checksum,
         };
 
         let append = block.b.num_bytes() > 0;
@@ -458,33 +470,36 @@
         data_slices.extend(parity_slices);
         data_slices
     }
 }
 
 // Writer for erasure coded blocks.
 pub(crate) struct StripedBlockWriter {
+    protocol: Arc<NamenodeProtocol>,
     block: hdfs::LocatedBlockProto,
     server_defaults: hdfs::FsServerDefaultsProto,
     block_size: usize,
     block_writers: Vec<Option<ReplicatedBlockWriter>>,
     cell_buffer: CellBuffer,
     bytes_written: usize,
     capacity: usize,
 }
 
 impl StripedBlockWriter {
     fn new(
+        protocol: Arc<NamenodeProtocol>,
         block: hdfs::LocatedBlockProto,
         ec_schema: &EcSchema,
         block_size: usize,
         server_defaults: hdfs::FsServerDefaultsProto,
     ) -> Self {
         let block_writers = (0..block.block_indices().len()).map(|_| None).collect();
 
         Self {
+            protocol,
             block,
             block_size,
             server_defaults,
             block_writers,
             cell_buffer: CellBuffer::new(ec_schema),
             bytes_written: 0,
             capacity: ec_schema.data_units * block_size,
@@ -515,14 +530,15 @@
                 cloned.locs = vec![cloned.locs[index].clone()];
                 cloned.block_token = cloned.block_tokens[index].clone();
                 cloned.storage_i_ds = vec![cloned.storage_i_ds[index].clone()];
                 cloned.storage_types = vec![cloned.storage_types[index]];
 
                 *writer = Some(
                     ReplicatedBlockWriter::new(
+                        &self.protocol,
                         cloned,
                         self.block_size,
                         self.server_defaults.clone(),
                     )
                     .await?,
                 )
             }
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/connection.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/connection.rs`

 * *Files 10% similar despite different names*

```diff
@@ -3,49 +3,43 @@
 use std::io::ErrorKind;
 use std::sync::atomic::{AtomicI32, Ordering};
 use std::sync::Arc;
 use std::sync::Mutex;
 
 use bytes::{Buf, BufMut, Bytes, BytesMut};
 use chrono::{prelude::*, TimeDelta};
-use crc::{Crc, Slice16, CRC_32_CKSUM, CRC_32_ISCSI};
+use crc::{Crc, Table, CRC_32_CKSUM, CRC_32_ISCSI};
 use log::{debug, warn};
 use once_cell::sync::Lazy;
 use prost::Message;
 use socket2::SockRef;
-use tokio::io::BufStream;
 use tokio::sync::{mpsc, oneshot};
 use tokio::{
-    io::{AsyncBufReadExt, AsyncReadExt, AsyncWriteExt, BufReader},
-    net::{
-        tcp::{OwnedReadHalf, OwnedWriteHalf},
-        TcpStream,
-    },
+    io::AsyncWriteExt,
+    net::TcpStream,
     task::{self, JoinHandle},
 };
 use uuid::Uuid;
 
 use crate::proto::common::rpc_response_header_proto::RpcStatusProto;
 use crate::proto::common::TokenProto;
-use crate::proto::hdfs::DatanodeIdProto;
+use crate::proto::hdfs::{DataEncryptionKeyProto, DatanodeIdProto};
 use crate::proto::{common, hdfs};
+use crate::security::sasl::{SaslDatanodeConnection, SaslDatanodeReader, SaslDatanodeWriter};
 use crate::security::sasl::{SaslReader, SaslRpcClient, SaslWriter};
 use crate::security::user::UserInfo;
 use crate::{HdfsError, Result};
 
-#[cfg(feature = "token")]
-use crate::security::sasl::SaslDatanodeConnection;
-
 const PROTOCOL: &str = "org.apache.hadoop.hdfs.protocol.ClientProtocol";
 const DATA_TRANSFER_VERSION: u16 = 28;
 const MAX_PACKET_HEADER_SIZE: usize = 33;
 const DATANODE_CACHE_EXPIRY: TimeDelta = TimeDelta::seconds(3);
 
-const CRC32: Crc<Slice16<u32>> = Crc::<Slice16<u32>>::new(&CRC_32_CKSUM);
-const CRC32C: Crc<Slice16<u32>> = Crc::<Slice16<u32>>::new(&CRC_32_ISCSI);
+const CRC32: Crc<u32, Table<16>> = Crc::<u32, Table<16>>::new(&CRC_32_CKSUM);
+const CRC32C: Crc<u32, Table<16>> = Crc::<u32, Table<16>>::new(&CRC_32_ISCSI);
 
 pub(crate) static DATANODE_CACHE: Lazy<DatanodeConnectionCache> =
     Lazy::new(DatanodeConnectionCache::new);
 
 // Connect to a remote host and return a TcpStream with standard options we want
 async fn connect(addr: &str) -> Result<TcpStream> {
     let stream = TcpStream::connect(addr).await?;
@@ -180,15 +174,15 @@
 
         Ok(conn)
     }
 
     fn start_sender(&mut self, mut rx: mpsc::Receiver<Vec<u8>>, mut writer: SaslWriter) {
         task::spawn(async move {
             while let Some(msg) = rx.recv().await {
-                match writer.write(&msg).await {
+                match writer.write_all(&msg).await {
                     Ok(_) => (),
                     Err(_) => break,
                 }
             }
         });
     }
 
@@ -392,15 +386,14 @@
     }
 }
 
 const CHECKSUM_BYTES: usize = 4;
 
 pub(crate) struct Packet {
     pub header: hdfs::PacketHeaderProto,
-    #[allow(dead_code)]
     checksum: BytesMut,
     data: BytesMut,
     bytes_per_checksum: usize,
     max_data_size: usize,
 }
 
 impl Packet {
@@ -513,70 +506,61 @@
                 }
             }
         }
         Ok(data)
     }
 }
 
-#[derive(Debug)]
 pub(crate) struct DatanodeConnection {
     client_name: String,
-    stream: BufStream<TcpStream>,
+    reader: SaslDatanodeReader,
+    writer: SaslDatanodeWriter,
     url: String,
 }
 
 impl DatanodeConnection {
-    #[allow(unused_variables)]
-    pub(crate) async fn connect(datanode_id: &DatanodeIdProto, token: &TokenProto) -> Result<Self> {
+    pub(crate) async fn connect(
+        datanode_id: &DatanodeIdProto,
+        token: &TokenProto,
+        encryption_key: Option<DataEncryptionKeyProto>,
+    ) -> Result<Self> {
         let url = format!("{}:{}", datanode_id.ip_addr, datanode_id.xfer_port);
         let stream = connect(&url).await?;
 
-        // If the token has an identifier, we can do SASL negotation
-        #[cfg(feature = "token")]
-        let stream = if token.identifier.is_empty() {
-            stream
-        } else {
-            debug!("{:?}", token);
-            let sasl_connection = SaslDatanodeConnection::create(stream);
-            sasl_connection.negotiate(datanode_id, token).await?
-        };
+        let sasl_connection = SaslDatanodeConnection::create(stream);
+        let (reader, writer) = sasl_connection
+            .negotiate(datanode_id, token, encryption_key.as_ref())
+            .await?;
 
         let conn = DatanodeConnection {
             client_name: Uuid::new_v4().to_string(),
-            stream: BufStream::new(stream),
+            reader,
+            writer,
             url: url.to_string(),
         };
         Ok(conn)
     }
 
     pub(crate) async fn send(
         &mut self,
         op: Op,
         message: &impl Message,
     ) -> Result<hdfs::BlockOpResponseProto> {
-        self.stream
+        self.writer
             .write_all(&DATA_TRANSFER_VERSION.to_be_bytes())
             .await?;
-        self.stream.write_all(&[op.value()]).await?;
-        self.stream
+        self.writer.write_all(&[op.value()]).await?;
+        self.writer
             .write_all(&message.encode_length_delimited_to_vec())
             .await?;
-        self.stream.flush().await?;
-
-        let buf = self.stream.fill_buf().await?;
-        if buf.is_empty() {
-            return Err(std::io::Error::from(std::io::ErrorKind::UnexpectedEof))?;
-        }
-        let msg_length = prost::decode_length_delimiter(buf)?;
-        let total_size = msg_length + prost::length_delimiter_len(msg_length);
+        self.writer.flush().await?;
 
-        let mut response_buf = BytesMut::zeroed(total_size);
-        self.stream.read_exact(&mut response_buf).await?;
+        let message = self.reader.read_proto().await?;
 
-        let response = hdfs::BlockOpResponseProto::decode_length_delimited(response_buf.freeze())?;
+        let response = hdfs::BlockOpResponseProto::decode(message)?;
         Ok(response)
     }
 
     pub(crate) fn build_header(
         &self,
         block: &hdfs::ExtendedBlockProto,
         token: Option<common::TokenProto>,
@@ -592,22 +576,22 @@
             client_name: self.client_name.clone(),
         }
     }
 
     pub(crate) async fn read_packet(&mut self) -> Result<Packet> {
         let mut payload_len_buf = [0u8; 4];
         let mut header_len_buf = [0u8; 2];
-        self.stream.read_exact(&mut payload_len_buf).await?;
-        self.stream.read_exact(&mut header_len_buf).await?;
+        self.reader.read_exact(&mut payload_len_buf).await?;
+        self.reader.read_exact(&mut header_len_buf).await?;
 
         let payload_length = u32::from_be_bytes(payload_len_buf) as usize;
         let header_length = u16::from_be_bytes(header_len_buf) as usize;
 
         let mut remaining_buf = BytesMut::zeroed(payload_length - 4 + header_length);
-        self.stream.read_exact(&mut remaining_buf).await?;
+        self.reader.read_exact(&mut remaining_buf).await?;
 
         let header =
             hdfs::PacketHeaderProto::decode(remaining_buf.split_to(header_length).freeze())?;
 
         let checksum_length = payload_length - 4 - header.data_len as usize;
         let checksum = remaining_buf.split_to(checksum_length);
         let data = remaining_buf;
@@ -616,106 +600,78 @@
     }
 
     pub(crate) async fn send_read_success(&mut self) -> Result<()> {
         let client_read_status = hdfs::ClientReadStatusProto {
             status: hdfs::Status::ChecksumOk as i32,
         };
 
-        self.stream
+        self.writer
             .write_all(&client_read_status.encode_length_delimited_to_vec())
             .await?;
-        self.stream.flush().await?;
+        self.writer.flush().await?;
 
         Ok(())
     }
 
     pub(crate) fn split(self) -> (DatanodeReader, DatanodeWriter) {
-        let (reader, writer) = self.stream.into_inner().into_split();
         let reader = DatanodeReader {
-            client_name: self.client_name.clone(),
-            reader: BufReader::new(reader),
-            url: self.url,
+            reader: self.reader,
         };
         let writer = DatanodeWriter {
-            client_name: self.client_name,
-            writer,
+            writer: self.writer,
         };
         (reader, writer)
     }
-
-    // For future use where we cache datanode connections
-    #[allow(dead_code)]
-    pub(crate) fn reunite(reader: DatanodeReader, writer: DatanodeWriter) -> Self {
-        assert_eq!(reader.client_name, writer.client_name);
-        let stream = BufStream::new(reader.reader.into_inner().reunite(writer.writer).unwrap());
-        Self {
-            client_name: reader.client_name,
-            stream,
-            url: reader.url,
-        }
-    }
 }
 
 /// A reader half of a Datanode connection used for reading acks during
 /// write operations.
 pub(crate) struct DatanodeReader {
-    client_name: String,
-    reader: BufReader<OwnedReadHalf>,
-    url: String,
+    reader: SaslDatanodeReader,
 }
 
 impl DatanodeReader {
     pub(crate) async fn read_ack(&mut self) -> Result<hdfs::PipelineAckProto> {
-        let buf = self.reader.fill_buf().await?;
+        let message = self.reader.read_proto().await?;
 
-        if buf.is_empty() {
-            // The stream has been closed
-            return Err(HdfsError::DataTransferError(
-                "Datanode connection closed while waiting for ack".to_string(),
-            ));
-        }
-
-        let ack_length = prost::decode_length_delimiter(buf)?;
-        let total_size = ack_length + prost::length_delimiter_len(ack_length);
-
-        let mut response_buf = BytesMut::zeroed(total_size);
-        self.reader.read_exact(&mut response_buf).await?;
-
-        let response = hdfs::PipelineAckProto::decode_length_delimited(response_buf.freeze())?;
+        let response = hdfs::PipelineAckProto::decode(message)?;
         Ok(response)
     }
 }
 
 /// A write half of a Datanode connection used for writing packets.
 pub(crate) struct DatanodeWriter {
-    client_name: String,
-    writer: OwnedWriteHalf,
+    writer: SaslDatanodeWriter,
 }
 
 impl DatanodeWriter {
     /// Create a buffer to send to the datanode
     pub(crate) async fn write_packet(&mut self, packet: &mut Packet) -> Result<()> {
         let (header, checksum, data) = packet.finalize();
 
         let payload_len = (checksum.len() + data.len() + 4) as u32;
         let header_encoded = header.encode_to_vec();
 
-        self.writer.write_u32(payload_len).await?;
-        self.writer.write_u16(header_encoded.len() as u16).await?;
+        self.writer.write_all(&payload_len.to_be_bytes()).await?;
+        self.writer
+            .write_all(&(header_encoded.len() as u16).to_be_bytes())
+            .await?;
         self.writer.write_all(&header.encode_to_vec()).await?;
         self.writer.write_all(&checksum).await?;
         self.writer.write_all(&data).await?;
         self.writer.flush().await?;
 
         Ok(())
     }
 }
 
+type DatanodeConnectionCacheEntry = VecDeque<(DateTime<Utc>, DatanodeConnection)>;
+
 pub(crate) struct DatanodeConnectionCache {
-    cache: Mutex<HashMap<String, VecDeque<(DateTime<Utc>, DatanodeConnection)>>>,
+    cache: Mutex<HashMap<String, DatanodeConnectionCacheEntry>>,
 }
 
 impl DatanodeConnectionCache {
     fn new() -> Self {
         Self {
             cache: Mutex::new(HashMap::new()),
         }
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/protocol.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/protocol.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 use std::collections::HashSet;
 use std::sync::{Arc, Mutex};
 use std::time::{Duration, SystemTime};
 
+use chrono::Utc;
 use log::{debug, warn};
 use prost::Message;
 use tokio::task::JoinHandle;
 use uuid::Uuid;
 
-use crate::proto::hdfs;
+use crate::proto::hdfs::{
+    self, DataEncryptionKeyProto, FsServerDefaultsProto, GetDataEncryptionKeyResponseProto,
+};
 use crate::Result;
 
 use super::proxy::NameServiceProxy;
 
 const LEASE_RENEWAL_INTERVAL_SECS: u64 = 30;
 
 #[derive(Debug, Eq, PartialEq, Hash)]
@@ -23,24 +26,29 @@
 #[derive(Debug)]
 pub(crate) struct NamenodeProtocol {
     proxy: NameServiceProxy,
     client_name: String,
     // Stores files currently opened for writing for lease renewal purposes
     open_files: Arc<Mutex<HashSet<LeasedFile>>>,
     lease_renewer: Mutex<Option<JoinHandle<()>>>,
+    // We need a sync mutex for these
+    server_defaults: tokio::sync::Mutex<Option<FsServerDefaultsProto>>,
+    encryption_key: tokio::sync::Mutex<Option<DataEncryptionKeyProto>>,
 }
 
 impl NamenodeProtocol {
     pub(crate) fn new(proxy: NameServiceProxy) -> Self {
         let client_name = format!("hdfs_native_client-{}", Uuid::new_v4().as_hyphenated());
         NamenodeProtocol {
             proxy,
             client_name,
             open_files: Arc::new(Mutex::new(HashSet::new())),
             lease_renewer: Mutex::new(None),
+            server_defaults: tokio::sync::Mutex::new(None),
+            encryption_key: tokio::sync::Mutex::new(None),
         }
     }
 
     pub(crate) async fn get_file_info(&self, src: &str) -> Result<hdfs::GetFileInfoResponseProto> {
         let message = hdfs::GetFileInfoRequestProto {
             src: src.to_string(),
         };
@@ -115,29 +123,84 @@
             .await?;
 
         let decoded = hdfs::GetServerDefaultsResponseProto::decode_length_delimited(response)?;
         debug!("get_server_defaults response: {:?}", &decoded);
         Ok(decoded)
     }
 
+    pub(crate) async fn get_cached_server_defaults(&self) -> Result<FsServerDefaultsProto> {
+        let mut server_defaults = self.server_defaults.lock().await;
+        if let Some(defaults) = server_defaults.as_ref() {
+            Ok(defaults.clone())
+        } else {
+            let defaults = self.get_server_defaults().await?.server_defaults;
+            *server_defaults = Some(defaults.clone());
+            Ok(defaults)
+        }
+    }
+
+    pub(crate) async fn get_data_encryption_key(
+        &self,
+    ) -> Result<GetDataEncryptionKeyResponseProto> {
+        let message = hdfs::GetDataEncryptionKeyRequestProto::default();
+
+        let response = self
+            .proxy
+            .call(
+                "getDataEncryptionKey",
+                message.encode_length_delimited_to_vec(),
+            )
+            .await?;
+
+        let decoded = hdfs::GetDataEncryptionKeyResponseProto::decode_length_delimited(response)?;
+        debug!("get_data_encryption_key response: {:?}", &decoded);
+        Ok(decoded)
+    }
+
+    pub(crate) async fn get_cached_data_encryption_key(
+        &self,
+    ) -> Result<Option<DataEncryptionKeyProto>> {
+        let server_defaults = self.get_cached_server_defaults().await?;
+        if server_defaults.encrypt_data_transfer() {
+            let mut encryption_key = self.encryption_key.lock().await;
+            // Check if we have an encryption key and that it's not expired (with a 10 second buffer)
+            if encryption_key
+                .as_ref()
+                .is_some_and(|key| (key.expiry_date as i64) > Utc::now().timestamp_millis() + 10000)
+            {
+                Ok(encryption_key.clone())
+            } else {
+                let key = self.get_data_encryption_key().await?.data_encryption_key;
+                *encryption_key = key.clone();
+                Ok(key)
+            }
+        } else {
+            Ok(None)
+        }
+    }
+
     pub(crate) async fn create(
         &self,
         src: &str,
         permission: u32,
         overwrite: bool,
         create_parent: bool,
-        replication: u32,
-        block_size: u64,
+        replication: Option<u32>,
+        block_size: Option<u64>,
     ) -> Result<hdfs::CreateResponseProto> {
         let masked = hdfs::FsPermissionProto { perm: permission };
         let mut create_flag = hdfs::CreateFlagProto::Create as u32;
         if overwrite {
             create_flag |= hdfs::CreateFlagProto::Overwrite as u32;
         }
 
+        let server_defaults = self.get_cached_server_defaults().await?;
+        let replication = replication.unwrap_or(server_defaults.replication);
+        let block_size = block_size.unwrap_or(server_defaults.block_size);
+
         let message = hdfs::CreateRequestProto {
             src: src.to_string(),
             masked,
             client_name: self.client_name.clone(),
             create_parent,
             replication,
             block_size,
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/hdfs/proxy.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/hdfs/proxy.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/lib.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 //! let client = Client::new("hdfs://ns")?;
 //! # Ok(())
 //! # }
 //! ```
 //!
 //! # Optional cargo package features
 //! - `kerberos` - include support for Kerberos authentication. Uses the libgssapi package. Supports all RPC authentication and encryption methods.
-//! - `token` - include support for Token authentication. Uses the gsasl native library. Only
-//!   supports authentication, not integrity or privacy modes.
 
 pub mod client;
 pub(crate) mod common;
 #[cfg(feature = "benchmark")]
 pub mod ec;
 #[cfg(not(feature = "benchmark"))]
 pub(crate) mod ec;
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/minidfs.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/minidfs.rs`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,36 @@
     process::{Child, Command, Stdio},
 };
 use which::which;
 
 #[derive(PartialEq, Eq, Hash, Debug)]
 pub enum DfsFeatures {
     Security,
-    DataTransferSecurity,
     Token,
+    Integrity,
     Privacy,
+    AES,
+    DataTransferEncryption,
     HA,
     ViewFS,
     EC,
     RBF,
 }
 
 impl DfsFeatures {
     pub fn as_str(&self) -> &str {
         match self {
             DfsFeatures::EC => "ec",
             DfsFeatures::HA => "ha",
             DfsFeatures::ViewFS => "viewfs",
             DfsFeatures::Privacy => "privacy",
             DfsFeatures::Security => "security",
-            DfsFeatures::DataTransferSecurity => "data_transfer_security",
+            DfsFeatures::Integrity => "integrity",
+            DfsFeatures::AES => "aes",
+            DfsFeatures::DataTransferEncryption => "data_transfer_encryption",
             DfsFeatures::Token => "token",
             DfsFeatures::RBF => "rbf",
         }
     }
 
     pub fn from(value: &str) -> Option<Self> {
         match value {
@@ -54,19 +58,14 @@
     pub fn with_features(features: &HashSet<DfsFeatures>) -> Self {
         let mvn_exec = which("mvn").expect("Failed to find java executable");
 
         let mut feature_args: Vec<&str> = Vec::new();
         for feature in features.iter() {
             feature_args.push(feature.as_str());
         }
-        // If the `token` feature is enabled, we need to force the data transfer protection
-        #[cfg(feature = "token")]
-        if !features.contains(&DfsFeatures::DataTransferSecurity) {
-            feature_args.push(DfsFeatures::DataTransferSecurity.as_str());
-        }
 
         let mut child = Command::new(mvn_exec)
             .args([
                 "-f",
                 concat!(env!("OUT_DIR"), "/minidfs"),
                 "--quiet",
                 "compile",
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/FSProtos.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/FSProtos.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/GenericRefreshProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/GenericRefreshProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/GetUserMappingsProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/GetUserMappingsProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/HAServiceProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/HAServiceProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/IpcConnectionContext.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/IpcConnectionContext.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/ProtobufRpcEngine.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/ProtobufRpcEngine.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/ProtobufRpcEngine2.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/ProtobufRpcEngine2.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/ProtocolInfo.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/ProtocolInfo.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/RefreshAuthorizationPolicyProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/RefreshAuthorizationPolicyProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/RefreshCallQueueProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/RefreshCallQueueProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/RefreshUserMappingsProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/RefreshUserMappingsProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/RpcHeader.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/RpcHeader.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/Security.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/Security.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/TraceAdmin.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/TraceAdmin.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/common/ZKFCProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/common/ZKFCProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hadoop.common.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hadoop.common.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hadoop.hdfs.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hadoop.hdfs.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/ClientDatanodeProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/ClientDatanodeProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/ClientNamenodeProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/ClientNamenodeProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/ReconfigurationProtocol.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/ReconfigurationProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/acl.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/acl.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/datatransfer.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/datatransfer.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/encryption.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/encryption.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/erasurecoding.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/erasurecoding.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/hdfs.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/hdfs.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/inotify.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/inotify.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/proto/hdfs/xattr.proto` & `hdfs_native-0.9.1/crates/hdfs-native/src/proto/hdfs/xattr.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/security/gssapi.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/security/gssapi.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/security/sasl.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/security/digest.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,652 +1,669 @@
-use bytes::{Buf, Bytes, BytesMut};
-use log::{debug, warn};
-use prost::Message;
-use std::io;
-use std::sync::{Arc, Mutex};
-use tokio::net::tcp::OwnedWriteHalf;
-use tokio::{
-    io::{AsyncReadExt, AsyncWriteExt},
-    net::tcp::OwnedReadHalf,
-    net::TcpStream,
+use std::{
+    collections::HashMap,
+    fmt::{Display, Formatter},
 };
 
-use crate::proto::common::rpc_response_header_proto::RpcStatusProto;
-use crate::proto::common::rpc_sasl_proto::{SaslAuth, SaslState};
-use crate::proto::common::{
-    RpcKindProto, RpcRequestHeaderProto, RpcResponseHeaderProto, RpcSaslProto,
+use base64::{engine::general_purpose, Engine as _};
+use cbc::cipher::{BlockEncryptMut, KeyIvInit};
+use cipher::BlockDecryptMut;
+use hmac::{Hmac, Mac};
+use md5::{Digest, Md5};
+use once_cell::sync::Lazy;
+use rand::Rng;
+use regex::Regex;
+
+use crate::{proto::hdfs::DataEncryptionKeyProto, HdfsError, Result};
+
+use super::{
+    sasl::SaslSession,
+    user::{Token, UserInfo},
 };
 
-use crate::{HdfsError, Result};
-#[cfg(feature = "token")]
-use {
-    super::user::{BlockTokenIdentifier, Token},
-    base64::{engine::general_purpose, Engine as _},
-    gsasl_sys as gsasl,
-    libc::{c_char, c_void, memcpy},
-    std::ffi::CString,
-    std::ptr,
-    std::sync::atomic::AtomicPtr,
-};
-#[cfg(feature = "token")]
-use {
-    crate::proto::{
-        common::TokenProto,
-        hdfs::{
-            data_transfer_encryptor_message_proto::DataTransferEncryptorStatus,
-            DataTransferEncryptorMessageProto, DatanodeIdProto, HandshakeSecretProto,
-        },
-    },
-    tokio::io::{AsyncBufReadExt, BufStream},
-};
-
-#[cfg(feature = "kerberos")]
-use super::gssapi::GssapiSession;
-use super::user::{User, UserInfo};
+type HmacMD5 = Hmac<Md5>;
+type TdesCBCEnc = cbc::Encryptor<des::TdesEde2>;
+type TdesCBCDec = cbc::Decryptor<des::TdesEde2>;
 
-const SASL_CALL_ID: i32 = -33;
-#[cfg(feature = "token")]
-const SASL_TRANSFER_MAGIC_NUMBER: i32 = 0xDEADBEEFu32 as i32;
-const HDFS_DELEGATION_TOKEN: &str = "HDFS_DELEGATION_TOKEN";
+static CHALLENGE_PATTERN: Lazy<Regex> =
+    Lazy::new(|| Regex::new(r#",?([a-zA-Z0-9]+)=("([^"]+)"|([^,]+)),?"#).unwrap());
+static RESPONSE_PATTERN: Lazy<Regex> = Lazy::new(|| Regex::new("rspauth=([a-f0-9]{32})").unwrap());
 
-pub(crate) enum AuthMethod {
-    Simple,
-    Kerberos,
-    Token,
-}
-impl AuthMethod {
-    fn parse(method: &str) -> Option<Self> {
-        match method {
-            "SIMPLE" => Some(Self::Simple),
-            "KERBEROS" => Some(Self::Kerberos),
-            "TOKEN" => Some(Self::Token),
-            _ => None,
-        }
-    }
+#[derive(Clone, Copy, Debug, Eq, PartialEq, Hash, Ord, PartialOrd)]
+#[repr(u8)]
+enum Qop {
+    Auth = 0,
+    AuthInt = 1,
+    AuthConf = 2,
 }
 
-pub(crate) trait SaslSession: Send + Sync {
-    fn step(&mut self, token: Option<&[u8]>) -> Result<(Vec<u8>, bool)>;
-
-    fn has_security_layer(&self) -> bool;
-
-    fn encode(&mut self, buf: &[u8]) -> Result<Vec<u8>>;
+impl TryFrom<&str> for Qop {
+    type Error = HdfsError;
 
-    fn decode(&mut self, buf: &[u8]) -> Result<Vec<u8>>;
-
-    fn get_user_info(&self) -> Result<UserInfo>;
-}
-
-pub struct SaslRpcClient {
-    reader: SaslReader,
-    writer: SaslWriter,
-    session: Option<Arc<Mutex<Box<dyn SaslSession>>>>,
+    fn try_from(value: &str) -> std::result::Result<Self, Self::Error> {
+        match value {
+            "auth" => Ok(Self::Auth),
+            "auth-int" => Ok(Self::AuthInt),
+            "auth-conf" => Ok(Self::AuthConf),
+            v => Err(HdfsError::SASLError(format!("Unknown qop value: {}", v))),
+        }
+    }
 }
 
-impl SaslRpcClient {
-    pub fn create(stream: TcpStream) -> SaslRpcClient {
-        let (reader, writer) = stream.into_split();
-        SaslRpcClient {
-            reader: SaslReader::new(reader),
-            writer: SaslWriter::new(writer),
-            session: None,
+impl From<Qop> for String {
+    fn from(value: Qop) -> Self {
+        match value {
+            Qop::Auth => "auth",
+            Qop::AuthInt => "auth-int",
+            Qop::AuthConf => "auth-conf",
         }
+        .to_string()
     }
+}
 
-    /// Service should be the connection host:port for a single NameNode connection, or the
-    /// name service name when connecting to HA NameNodes.
-    pub(crate) async fn negotiate(&mut self, service: &str) -> Result<UserInfo> {
-        let rpc_sasl = RpcSaslProto {
-            state: SaslState::Negotiate as i32,
-            ..Default::default()
+impl Display for Qop {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        let s = match self {
+            Qop::Auth => "auth",
+            Qop::AuthInt => "auth-int",
+            Qop::AuthConf => "auth-conf",
         };
 
-        self.writer.send_sasl_message(&rpc_sasl).await?;
-
-        let mut done = false;
-        let mut session: Option<Box<dyn SaslSession>> = None;
-        while !done {
-            let mut response: Option<RpcSaslProto> = None;
-            let message = self.reader.read_response().await?;
-            debug!("Handling SASL message: {:?}", message);
-            match SaslState::try_from(message.state).unwrap() {
-                SaslState::Negotiate => {
-                    let (mut selected_auth, selected_session) =
-                        self.select_method(&message.auths, service)?;
-                    session = selected_session;
-
-                    let token = if let Some(session) = session.as_mut() {
-                        let (token, finished) =
-                            session.step(selected_auth.challenge.as_ref().map(|c| &c[..]))?;
-                        if finished {
-                            return Err(HdfsError::SASLError(
-                                "SASL negotiation finished too soon".to_string(),
-                            ));
-                        }
-                        Some(token)
-                    } else {
-                        done = true;
-                        None
-                    };
-
-                    // Response shouldn't contain the challenge
-                    selected_auth.challenge = None;
-
-                    let r = RpcSaslProto {
-                        state: SaslState::Initiate as i32,
-                        auths: Vec::from([selected_auth]),
-                        token: token.or(Some(Vec::new())),
-                        ..Default::default()
-                    };
-                    response = Some(r);
-                }
-                SaslState::Challenge => {
-                    let (token, _) = session
-                        .as_mut()
-                        .unwrap()
-                        .step(message.token.as_ref().map(|t| &t[..]))?;
-
-                    let r = RpcSaslProto {
-                        state: SaslState::Response as i32,
-                        token: Some(token),
-                        ..Default::default()
-                    };
-                    response = Some(r);
-                }
-                SaslState::Success => {
-                    if let Some(token) = message.token.as_ref() {
-                        let (_, finished) = session.as_mut().unwrap().step(Some(&token[..]))?;
-                        if !finished {
-                            return Err(HdfsError::SASLError(
-                                "Client not finished after server success".to_string(),
-                            ));
-                        }
-                    }
-                    done = true;
-                }
-                _ => todo!(),
-            }
-
-            if let Some(r) = response {
-                debug!("Sending SASL response {:?}", r);
-                self.writer.send_sasl_message(&r).await?;
-            }
-        }
-
-        let user_info = if let Some(s) = session.as_ref() {
-            s.get_user_info()?
-        } else {
-            User::get_simpler_user()
-        };
-        self.session = session
-            .filter(|x| {
-                debug!("Has security layer: {:?}", x.has_security_layer());
-                x.has_security_layer()
-            })
-            .map(|s| Arc::new(Mutex::new(s)));
-
-        Ok(user_info)
-    }
-
-    fn select_method(
-        &mut self,
-        auths: &[SaslAuth],
-        service: &str,
-    ) -> Result<(SaslAuth, Option<Box<dyn SaslSession>>)> {
-        let user = User::get();
-        for auth in auths.iter() {
-            match (
-                AuthMethod::parse(&auth.method),
-                user.get_token(HDFS_DELEGATION_TOKEN, service),
-            ) {
-                (Some(AuthMethod::Simple), _) => {
-                    return Ok((auth.clone(), None));
-                }
-                #[cfg(feature = "kerberos")]
-                (Some(AuthMethod::Kerberos), _) => {
-                    let session = GssapiSession::new(auth.protocol(), auth.server_id())?;
-                    return Ok((auth.clone(), Some(Box::new(session))));
-                }
-                #[cfg(feature = "token")]
-                (Some(AuthMethod::Token), Some(token)) => {
-                    debug!("Using token {:?}", token);
-                    let session = GSASLSession::new(auth.protocol(), auth.server_id(), token)?;
+        write!(f, "{}", s)
+    }
+}
 
-                    return Ok((auth.clone(), Some(Box::new(session))));
-                }
-                _ => (),
-            }
-        }
-        Err(HdfsError::NoSASLMechanism)
+impl Qop {
+    fn has_security_layer(&self) -> bool {
+        !matches!(self, Qop::Auth)
     }
+}
 
-    pub(crate) fn split(self) -> (SaslReader, SaslWriter) {
-        let mut reader = self.reader;
-        let mut writer = self.writer;
-        if let Some(session) = self.session {
-            reader.set_session(Arc::clone(&session));
-            writer.set_session(session);
+fn choose_qop(options: Vec<Qop>) -> Result<Qop> {
+    options
+        .into_iter()
+        .max_by(|x, y| x.cmp(y))
+        .ok_or(HdfsError::SASLError(
+            "No valid QOP found for negotiation".to_string(),
+        ))
+}
+
+fn choose_cipher(options: &[String]) -> Result<String> {
+    // Only allow 3DES
+    options
+        .iter()
+        .find(|o| *o == "3des")
+        .cloned()
+        .ok_or(HdfsError::SASLError(
+            "No valid cipher found, only 3DES is supported".to_string(),
+        ))
+}
+
+// We need to take 7 bytes of key and turn it into 8 odd-parity bytes
+fn construct_des_key(key: &[u8]) -> Vec<u8> {
+    assert_eq!(key.len(), 14);
+    let mut output = Vec::with_capacity(16);
+
+    let mut bytes = [0u8; 8];
+    for byte_range in [0..7, 7..14] {
+        key[byte_range]
+            .iter()
+            .zip(bytes.iter_mut())
+            .for_each(|(k, b)| *b = *k);
+        let bits = u64::from_be_bytes(bytes);
+
+        for i in 0..8 {
+            let mut byte = (bits >> ((8 - i) * 7)) as u8 & 0xFE;
+            let ones = byte.count_ones();
+            if ones % 2 == 1 {
+                // Set odd parity bit
+                byte |= 0x01;
+            }
+            output.push(byte);
         }
-        (reader, writer)
     }
+    output
 }
 
-pub(crate) struct SaslReader {
-    stream: OwnedReadHalf,
-    session: Option<Arc<Mutex<Box<dyn SaslSession>>>>,
-    buffer: Bytes,
+fn h(b: impl AsRef<[u8]>) -> Vec<u8> {
+    let mut hasher = Md5::new();
+    hasher.update(b.as_ref());
+    hasher.finalize().to_vec()
 }
 
-impl SaslReader {
-    fn new(stream: OwnedReadHalf) -> Self {
-        SaslReader {
-            stream,
-            session: None,
-            buffer: Bytes::new(),
-        }
-    }
+fn kd(k: impl AsRef<[u8]>, v: impl AsRef<[u8]>) -> Vec<u8> {
+    h([k.as_ref(), b":", v.as_ref()].concat())
+}
 
-    fn set_session(&mut self, session: Arc<Mutex<Box<dyn SaslSession>>>) {
-        self.session = Some(session);
-    }
+fn gen_nonce() -> String {
+    let mut gen = rand::thread_rng();
+    let cnonce_bytes: Vec<u8> = (0..12).map(|_| gen.gen()).collect();
+    general_purpose::STANDARD.encode(cnonce_bytes)
+}
 
-    async fn read_response(&mut self) -> Result<RpcSaslProto> {
-        let mut buf = [0u8; 4];
-        self.stream.read_exact(&mut buf).await?;
+#[derive(Debug)]
+#[allow(unused)]
+pub(super) struct Challenge {
+    realm: String,
+    nonce: String,
+    qop: Vec<Qop>,
+    maxbuf: u32,
+    cipher: Option<Vec<String>>,
+}
 
-        let msg_length = u32::from_be_bytes(buf);
+impl TryFrom<&[u8]> for Challenge {
+    type Error = HdfsError;
 
-        let mut buf = BytesMut::zeroed(msg_length as usize);
-        self.stream.read_exact(&mut buf).await?;
+    fn try_from(value: &[u8]) -> std::prelude::v1::Result<Self, Self::Error> {
+        value.to_vec().try_into()
+    }
+}
 
-        let mut bytes = buf.freeze();
-        let rpc_response = RpcResponseHeaderProto::decode_length_delimited(&mut bytes)?;
-        debug!("{:?}", rpc_response);
+impl TryFrom<Vec<u8>> for Challenge {
+    type Error = HdfsError;
 
-        match RpcStatusProto::try_from(rpc_response.status).unwrap() {
-            RpcStatusProto::Error => {
-                return Err(HdfsError::RPCError(
-                    rpc_response.exception_class_name().to_string(),
-                    rpc_response.error_msg().to_string(),
-                ));
-            }
-            RpcStatusProto::Fatal => {
-                warn!(
-                    "RPC fatal error: {}: {}",
-                    rpc_response.exception_class_name(),
-                    rpc_response.error_msg()
-                );
-                return Err(HdfsError::FatalRPCError(
-                    rpc_response.exception_class_name().to_string(),
-                    rpc_response.error_msg().to_string(),
-                ));
-            }
-            _ => (),
-        }
+    fn try_from(value: Vec<u8>) -> core::result::Result<Self, Self::Error> {
+        let decoded = String::from_utf8(value).unwrap();
+        let mut options: HashMap<String, String> = HashMap::new();
+        for capture in CHALLENGE_PATTERN.captures_iter(&decoded) {
+            let key = capture.get(1).unwrap().as_str().to_string();
+            // Third group is quoted value, fourth is non-quoted value
+            let value = capture
+                .get(3)
+                .or(capture.get(4))
+                .unwrap()
+                .as_str()
+                .to_string();
+            options.insert(key, value);
+        }
+
+        let realm = options.remove("realm").ok_or(HdfsError::SASLError(
+            "No realm supplied in DIGEST challenge".to_string(),
+        ))?;
+        let nonce = options.remove("nonce").ok_or(HdfsError::SASLError(
+            "No nonce supplied in DIGEST challenge".to_string(),
+        ))?;
+        let qop = options
+            .remove("qop")
+            .ok_or(HdfsError::SASLError(
+                "No qop supplied in DIGEST challenge".to_string(),
+            ))?
+            .split(',')
+            .map(|s| s.try_into())
+            .collect::<Result<Vec<Qop>>>()?;
+        let maxbuf: u32 = options
+            .get("maxbuf")
+            .map(|mb| mb.parse().unwrap())
+            .unwrap_or(65536);
+        let cipher = options
+            .remove("cipher")
+            .map(|c| c.split(',').map(|s| s.to_string()).collect());
 
-        let sasl_response = RpcSaslProto::decode_length_delimited(&mut bytes)?;
-        Ok(sasl_response)
+        Ok(Self {
+            realm,
+            nonce,
+            qop,
+            maxbuf,
+            cipher,
+        })
     }
+}
 
-    pub(crate) async fn read_exact(&mut self, buf: &mut [u8]) -> Result<usize> {
-        if self.session.is_some() {
-            let read_len = buf.len();
-            let mut bytes_remaining = read_len;
-            while bytes_remaining > 0 {
-                if !self.buffer.has_remaining() {
-                    let response = self.read_response().await?;
-                    if response.state() != SaslState::Wrap {
-                        todo!();
-                    }
-
-                    // let mut writer = BytesMut::with_capacity(response.token().len()).writer();
-                    let decoded = self
-                        .session
-                        .as_ref()
-                        .unwrap()
-                        .lock()
-                        .unwrap()
-                        .decode(response.token())
-                        .unwrap_or_else(|_| todo!());
-                    self.buffer = Bytes::from(decoded)
-                }
-                let copy_len = usize::min(bytes_remaining, self.buffer.remaining());
-                let copy_start = read_len - bytes_remaining;
-                self.buffer
-                    .copy_to_slice(&mut buf[copy_start..(copy_start + copy_len)]);
-                bytes_remaining -= copy_len;
-            }
-
-            Ok(read_len)
-        } else {
-            Ok(self.stream.read_exact(buf).await?)
+struct DigestContext {
+    nonce: String,
+    cnonce: String,
+    realm: String,
+    qop: Qop,
+}
+
+struct KeyPair {
+    client: Vec<u8>,
+    server: Vec<u8>,
+}
+
+struct SecurityContext {
+    integrity_keys: KeyPair,
+    encryptor: Option<TdesCBCEnc>,
+    decryptor: Option<TdesCBCDec>,
+    seq_num: u32,
+}
+
+impl SecurityContext {
+    fn new(integrity_keys: KeyPair, encryption_keys: Option<KeyPair>) -> Self {
+        let encryptor = encryption_keys.as_ref().map(|enc_keys| {
+            TdesCBCEnc::new_from_slices(
+                &construct_des_key(&enc_keys.client[..14]),
+                &enc_keys.client[8..],
+            )
+            .unwrap()
+        });
+        let decryptor = encryption_keys.as_ref().map(|enc_keys| {
+            TdesCBCDec::new_from_slices(
+                &construct_des_key(&enc_keys.server[..14]),
+                &enc_keys.server[8..],
+            )
+            .unwrap()
+        });
+        SecurityContext {
+            integrity_keys,
+            encryptor,
+            decryptor,
+            seq_num: 0,
         }
     }
 }
 
-pub(crate) struct SaslWriter {
-    stream: OwnedWriteHalf,
-    session: Option<Arc<Mutex<Box<dyn SaslSession>>>>,
+#[allow(clippy::large_enum_variant)]
+enum DigestState {
+    Pending,
+    Stepped(DigestContext),
+    Completed(Option<SecurityContext>),
+    Errored,
 }
 
-impl SaslWriter {
-    fn new(stream: OwnedWriteHalf) -> Self {
-        SaslWriter {
-            stream,
-            session: None,
-        }
-    }
+pub(super) struct DigestSaslSession {
+    auth_id: String,
+    password: String,
+    service: String,
+    hostname: String,
+    state: DigestState,
+}
 
-    fn set_session(&mut self, session: Arc<Mutex<Box<dyn SaslSession>>>) {
-        self.session = Some(session);
+impl DigestSaslSession {
+    pub(super) fn from_token(service: String, hostname: String, token: &Token) -> Self {
+        Self {
+            auth_id: general_purpose::STANDARD.encode(&token.identifier),
+            password: general_purpose::STANDARD.encode(&token.password),
+            service,
+            hostname,
+            state: DigestState::Pending,
+        }
     }
 
-    fn create_request_header() -> RpcRequestHeaderProto {
-        RpcRequestHeaderProto {
-            rpc_kind: Some(RpcKindProto::RpcProtocolBuffer as i32),
-            // RPC_FINAL_PACKET
-            rpc_op: Some(0),
-            call_id: SASL_CALL_ID,
-            client_id: Vec::new(),
-            retry_count: Some(-1),
-            ..Default::default()
+    pub(super) fn from_encryption_key(
+        service: String,
+        hostname: String,
+        encryption_key: &DataEncryptionKeyProto,
+    ) -> Self {
+        Self {
+            auth_id: format!(
+                "{} {} {}",
+                encryption_key.key_id,
+                encryption_key.block_pool_id,
+                general_purpose::STANDARD.encode(&encryption_key.nonce)
+            ),
+            password: general_purpose::STANDARD.encode(&encryption_key.encryption_key),
+            service,
+            hostname,
+            state: DigestState::Pending,
         }
     }
 
-    async fn send_sasl_message(&mut self, message: &RpcSaslProto) -> io::Result<()> {
-        let header_buf = Self::create_request_header().encode_length_delimited_to_vec();
-        let message_buf = message.encode_length_delimited_to_vec();
-        let size = (header_buf.len() + message_buf.len()) as u32;
-
-        self.stream.write_all(&size.to_be_bytes()).await?;
-        self.stream.write_all(&header_buf).await?;
-        self.stream.write_all(&message_buf).await?;
-        self.stream.flush().await?;
-
-        Ok(())
+    fn compute(&self, ctx: &DigestContext, initial: bool) -> String {
+        let x = hex::encode(h(self.a1(ctx)));
+        let y = format!(
+            "{}:{:08x}:{}:{}:{}",
+            ctx.nonce,
+            1,
+            ctx.cnonce,
+            ctx.qop,
+            hex::encode(h(self.a2(initial, &ctx.qop)))
+        );
+
+        hex::encode(kd(x, y))
+    }
+
+    fn a1(&self, ctx: &DigestContext) -> Vec<u8> {
+        let hashed = h([
+            self.auth_id.as_bytes(),
+            b":",
+            ctx.realm.as_bytes(),
+            b":",
+            self.password.as_bytes(),
+        ]
+        .concat());
+        [
+            hashed.as_slice(),
+            b":",
+            ctx.nonce.as_bytes(),
+            b":",
+            ctx.cnonce.as_bytes(),
+        ]
+        .concat()
+    }
+
+    fn a2(&self, initial: bool, qop: &Qop) -> String {
+        let digest_uri = format!("{}/{}", self.service, self.hostname);
+        let authenticate = if initial { "AUTHENTICATE" } else { "" };
+        let tail = if qop.has_security_layer() {
+            ":00000000000000000000000000000000"
+        } else {
+            ""
+        };
+        format!("{}:{}{}", authenticate, digest_uri, tail)
     }
 
-    pub(crate) async fn write(&mut self, buf: &[u8]) -> io::Result<()> {
-        if self.session.is_some() {
-            let mut rpc_sasl = RpcSaslProto {
-                state: SaslState::Wrap as i32,
-                ..Default::default()
-            };
+    fn integrity_keys(&self, ctx: &DigestContext) -> KeyPair {
+        let kic = h([
+            &h(self.a1(ctx))[..],
+            b"Digest session key to client-to-server signing key magic constant",
+        ]
+        .concat());
+        let kis = h([
+            &h(self.a1(ctx))[..],
+            b"Digest session key to server-to-client signing key magic constant",
+        ]
+        .concat());
 
-            // let mut writer = Vec::with_capacity(buf.len()).writer();
-            let encoded = self
-                .session
-                .as_ref()
-                .unwrap()
-                .lock()
-                .unwrap()
-                .encode(buf)
-                .unwrap_or_else(|_| todo!());
+        KeyPair {
+            client: kic,
+            server: kis,
+        }
+    }
 
-            rpc_sasl.token = Some(encoded);
+    fn confidentiality_keys(&self, ctx: &DigestContext) -> KeyPair {
+        let kic = h([
+            &h(self.a1(ctx))[..],
+            b"Digest H(A1) to client-to-server sealing key magic constant",
+        ]
+        .concat());
+        let kis = h([
+            &h(self.a1(ctx))[..],
+            b"Digest H(A1) to server-to-client sealing key magic constant",
+        ]
+        .concat());
 
-            self.send_sasl_message(&rpc_sasl).await?;
-        } else {
-            self.stream.write_all(buf).await?
+        KeyPair {
+            client: kic,
+            server: kis,
         }
-        Ok(())
     }
-}
 
-impl std::fmt::Debug for SaslWriter {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("SaslWriter")
-            .field("stream", &self.stream)
-            .finish()
+    pub(crate) fn supports_encryption(&self) -> bool {
+        match &self.state {
+            DigestState::Stepped(ctx) => matches!(ctx.qop, Qop::AuthConf),
+            DigestState::Completed(ctx) => ctx.as_ref().is_some_and(|c| c.encryptor.is_some()),
+            _ => false,
+        }
     }
 }
 
-#[cfg(feature = "token")]
-struct GSASLSession {
-    ctx: AtomicPtr<gsasl::Gsasl>,
-    conn: AtomicPtr<gsasl::Gsasl_session>,
-}
-
-#[cfg(feature = "token")]
-impl GSASLSession {
-    fn new(service: &str, hostname: &str, token: &Token) -> Result<Self> {
-        let mut ctx = ptr::null_mut::<gsasl::Gsasl>();
+impl SaslSession for DigestSaslSession {
+    fn step(&mut self, token: Option<&[u8]>) -> Result<(Vec<u8>, bool)> {
+        match core::mem::replace(&mut self.state, DigestState::Errored) {
+            DigestState::Pending => {
+                // First step, token is a challenge
+                let challenge: Challenge = token.unwrap().try_into().unwrap();
+
+                let qop = choose_qop(challenge.qop)?;
+                let cipher = match (qop, &challenge.cipher) {
+                    (Qop::AuthConf, Some(cipher)) => Some(choose_cipher(cipher)?),
+                    (Qop::AuthConf, None) => {
+                        return Err(HdfsError::SASLError(
+                            "Confidentiality was chosen, but no cipher was provided".to_string(),
+                        ))
+                    }
+                    _ => None,
+                };
 
-        let ret = unsafe { gsasl::gsasl_init(&mut ctx) };
-        if ret != gsasl::Gsasl_rc::GSASL_OK as i32 {
-            return Err(HdfsError::SASLError(
-                "Failed to initialize SASL".to_string(),
-            ));
-        }
+                let ctx = DigestContext {
+                    nonce: challenge.nonce.clone(),
+                    cnonce: gen_nonce(),
+                    realm: challenge.realm.clone(),
+                    qop,
+                };
+
+                let response = self.compute(&ctx, true);
+
+                let mut message = format!(
+                    r#"username="{}",realm="{}",nonce="{}",cnonce="{}",nc={:08x},qop={},digest-uri="{}/{}",response={},charset=utf-8"#,
+                    self.auth_id,
+                    challenge.realm,
+                    ctx.nonce,
+                    ctx.cnonce,
+                    1,
+                    qop,
+                    self.service,
+                    self.hostname,
+                    response
+                );
+                if let Some(c) = cipher {
+                    message.push_str(&format!(r#",cipher="{}""#, c));
+                }
 
-        let mut conn = ptr::null_mut::<gsasl::Gsasl_session>();
-        let mechanism = CString::new("DIGEST-MD5").unwrap();
+                self.state = DigestState::Stepped(ctx);
+                Ok((message.as_bytes().to_vec(), false))
+            }
+            DigestState::Stepped(ctx) => {
+                let token_str = String::from_utf8(token.unwrap().to_vec()).map_err(|_| {
+                    HdfsError::SASLError("Failed to parse token as UTF-8 string".to_string())
+                })?;
+                if let Some(captures) = RESPONSE_PATTERN.captures(&token_str) {
+                    let rspauth = captures.get(1).unwrap();
+                    if rspauth.as_str() != self.compute(&ctx, false) {
+                        return Err(HdfsError::SASLError(
+                            "rspauth from server did not match".to_string(),
+                        ));
+                    }
+                } else {
+                    return Err(HdfsError::SASLError(
+                        "Message from server did not contain rspauth".to_string(),
+                    ));
+                }
 
-        let ret = unsafe { gsasl::gsasl_client_start(ctx, mechanism.as_ptr(), &mut conn) };
-        if ret != gsasl::Gsasl_rc::GSASL_OK as i32 {
-            return Err(HdfsError::SASLError(
-                "Failed to create new SASL client".to_string(),
-            ));
+                self.state = match ctx.qop {
+                    Qop::Auth => DigestState::Completed(None),
+                    Qop::AuthInt => DigestState::Completed(Some(SecurityContext::new(
+                        self.integrity_keys(&ctx),
+                        None,
+                    ))),
+                    Qop::AuthConf => DigestState::Completed(Some(SecurityContext::new(
+                        self.integrity_keys(&ctx),
+                        Some(self.confidentiality_keys(&ctx)),
+                    ))),
+                };
+                Ok((Vec::new(), true))
+            }
+            DigestState::Completed(_) => Err(HdfsError::SASLError(
+                "Failed to step, DIGEST-MD5 handshake already complete".to_string(),
+            )),
+            DigestState::Errored => Err(HdfsError::SASLError(
+                "Failed to step, DIGEST-MD5 authentication failed".to_string(),
+            )),
         }
+    }
 
-        debug!("Started SASL: {:?}, {:?}", conn, mechanism);
-
-        if ret != gsasl::Gsasl_rc::GSASL_OK as i32 {
-            return Err(HdfsError::SASLError(format!(
-                "Failed to start SASL client: {}",
-                ret
-            )));
+    fn has_security_layer(&self) -> bool {
+        match &self.state {
+            DigestState::Completed(ctx) => ctx.is_some(),
+            _ => false,
         }
+    }
 
-        let service_c = CString::new(service).unwrap();
-        let hostname_c = CString::new(hostname).unwrap();
-
-        unsafe {
-            gsasl::gsasl_property_set(
-                conn,
-                gsasl::Gsasl_property::GSASL_SERVICE,
-                service_c.as_ptr(),
-            );
-            gsasl::gsasl_property_set(
-                conn,
-                gsasl::Gsasl_property::GSASL_HOSTNAME,
-                hostname_c.as_ptr(),
-            );
-            let identifier =
-                CString::new(general_purpose::STANDARD.encode(&token.identifier)).unwrap();
-            let password = CString::new(general_purpose::STANDARD.encode(&token.password)).unwrap();
+    fn encode(&mut self, buf: &[u8]) -> crate::Result<Vec<u8>> {
+        match &mut self.state {
+            DigestState::Completed(Some(ctx)) => {
+                let mut mac = HmacMD5::new_from_slice(&ctx.integrity_keys.client).unwrap();
+                mac.update(&ctx.seq_num.to_be_bytes());
+                mac.update(buf);
+                let hmac = mac.finalize().into_bytes();
+
+                let mut message = if let Some(encryptor) = &mut ctx.encryptor {
+                    // 10 bytes of HMAC, 8 byte block size
+                    let padding_len = 8 - (buf.len() + 10) % 8;
+                    let mut message =
+                        [buf, &vec![padding_len as u8; padding_len], &hmac[..10]].concat();
+
+                    let enc_block: &mut [u8] = message.as_mut();
+                    let mut enc_bytes = 0;
+                    while enc_bytes < enc_block.len() {
+                        encryptor
+                            .encrypt_block_mut((&mut enc_block[enc_bytes..enc_bytes + 8]).into());
+                        enc_bytes += 8;
+                    }
+                    message
+                } else {
+                    [buf, &hmac[..10]].concat()
+                };
+
+                // let message = [&message, &[0, 1], &ctx.seq_num.to_be_bytes()].concat();
+                message.extend(&[0, 1]);
+                message.extend(ctx.seq_num.to_be_bytes());
 
-            gsasl::gsasl_property_set(
-                conn,
-                gsasl::Gsasl_property::GSASL_AUTHID,
-                identifier.as_ptr(),
-            );
-            gsasl::gsasl_property_set(
-                conn,
-                gsasl::Gsasl_property::GSASL_PASSWORD,
-                password.as_ptr(),
-            );
+                ctx.seq_num += 1;
+                Ok(message)
+            }
+            DigestState::Completed(None) => Err(HdfsError::SASLError(
+                "QOP doesn't support security layer".to_string(),
+            )),
+            _ => Err(HdfsError::SASLError(
+                "SASL negotiation not complete, can't encode message".to_string(),
+            )),
         }
-
-        Ok(Self {
-            ctx: AtomicPtr::new(ctx),
-            conn: AtomicPtr::new(conn),
-        })
     }
-}
-
-#[cfg(feature = "token")]
-impl SaslSession for GSASLSession {
-    fn step(&mut self, token: Option<&[u8]>) -> Result<(Vec<u8>, bool)> {
-        let mut clientout = ptr::null_mut::<c_char>();
-        let mut clientoutlen: u64 = 0;
 
-        // The type is different depending on the OS
-        // #[cfg(target_os = "macos")]
-        let token_ptr = token.map(|t| t.as_ptr()).unwrap_or(ptr::null_mut()) as *const c_char;
-        // #[cfg(not(target_os = "macos"))]
-        // let token_ptr = token.map(|t| t.as_ptr()).unwrap_or(ptr::null_mut()) as *const u8;
-
-        let ret = unsafe {
-            gsasl::gsasl_step(
-                self.conn.load(std::sync::atomic::Ordering::SeqCst),
-                token_ptr,
-                token.map(|t| t.len()).unwrap_or(0) as u64,
-                &mut clientout,
-                &mut clientoutlen,
-            )
-        };
+    fn decode(&mut self, buf: &[u8]) -> crate::Result<Vec<u8>> {
+        match &mut self.state {
+            DigestState::Completed(Some(ctx)) => {
+                let (message, hmac) = if let Some(decryptor) = &mut ctx.decryptor {
+                    // All but last 6 bytes are encrypted
+                    let mut message = buf[..buf.len() - 6].to_vec();
+                    let mut dec_bytes = 0;
+                    while dec_bytes < message.len() {
+                        decryptor
+                            .decrypt_block_mut((&mut message[dec_bytes..dec_bytes + 8]).into());
+                        dec_bytes += 8;
+                    }
 
-        debug!("SASL step response: {}", ret);
+                    // Split HMAC off
+                    let hmac = message.split_off(message.len() - 10);
+                    // Remove padding at the end of the message
+                    let _ = message.split_off(message.len() - *message.last().unwrap() as usize);
+
+                    (message, hmac)
+                } else {
+                    // Not encrypted, last 16 bytes are 10 bytes of HMAC, 2 bytes of type, and 4 bytes of seqno
+                    let mut message = buf[..buf.len() - 6].to_vec();
+                    let hmac = message.split_off(message.len() - 10);
+                    (message, hmac)
+                };
+
+                let mut mac = HmacMD5::new_from_slice(&ctx.integrity_keys.server).unwrap();
+                mac.update(&buf[buf.len() - 4..]);
+                mac.update(&message);
 
-        if ret != gsasl::Gsasl_rc::GSASL_OK as i32
-            && ret != gsasl::Gsasl_rc::GSASL_NEEDS_MORE as i32
-        {
-            return Err(HdfsError::SASLError(format!(
-                "Failed to make SASL client step: {}",
-                ret
-            )));
-        }
-
-        let vec = unsafe {
-            let mut vec = vec![0u8; clientoutlen as usize];
-            memcpy(
-                vec.as_mut_ptr() as *mut c_void,
-                clientout as *const c_void,
-                vec.len(),
-            );
-            vec
-        };
+                mac.verify_truncated_left(&hmac)
+                    .map_err(|_| HdfsError::SASLError("Integrity HMAC check failed".to_string()))?;
 
-        Ok((vec, ret == gsasl::Gsasl_rc::GSASL_OK as i32))
-    }
-
-    fn has_security_layer(&self) -> bool {
-        false
-    }
-
-    fn encode(&mut self, _buf: &[u8]) -> Result<Vec<u8>> {
-        todo!()
-    }
-
-    fn decode(&mut self, _buf: &[u8]) -> Result<Vec<u8>> {
-        todo!()
+                Ok(message.to_vec())
+            }
+            DigestState::Completed(None) => Err(HdfsError::SASLError(
+                "QOP doesn't support security layer".to_string(),
+            )),
+            _ => Err(HdfsError::SASLError(
+                "SASL negotiation not complete, can't decode message".to_string(),
+            )),
+        }
     }
 
-    fn get_user_info(&self) -> Result<UserInfo> {
+    fn get_user_info(&self) -> crate::Result<super::user::UserInfo> {
         // The token has all the info
         Ok(UserInfo {
             real_user: None,
             effective_user: None,
         })
     }
 }
 
-#[cfg(feature = "token")]
-impl Drop for GSASLSession {
-    fn drop(&mut self) {
-        unsafe {
-            gsasl::gsasl_finish(self.conn.load(std::sync::atomic::Ordering::SeqCst));
-            gsasl::gsasl_done(self.ctx.load(std::sync::atomic::Ordering::SeqCst))
-        }
-    }
-}
-
-#[cfg(feature = "token")]
-pub(crate) struct SaslDatanodeConnection {
-    stream: BufStream<TcpStream>,
-}
-
-#[cfg(feature = "token")]
-impl SaslDatanodeConnection {
-    pub fn create(stream: TcpStream) -> Self {
-        Self {
-            stream: BufStream::new(stream),
-        }
-    }
-
-    pub(crate) async fn negotiate(
-        mut self,
-        datanode_id: &DatanodeIdProto,
-        token: &TokenProto,
-    ) -> Result<TcpStream> {
-        // If it's a privileged port, don't do SASL negotation
-        if datanode_id.xfer_port <= 1024 {
-            return Ok(self.stream.into_inner());
-        }
-
-        self.stream.write_i32(SASL_TRANSFER_MAGIC_NUMBER).await?;
-        self.stream.flush().await?;
-
-        let mut session = GSASLSession::new("hdfs", "0", &token.clone().into())?;
-
-        let token_identifier = BlockTokenIdentifier::from_identifier(&token.identifier)?;
-
-        let handshake_secret = if !token_identifier.handshake_secret.is_empty() {
-            Some(HandshakeSecretProto {
-                bpid: token_identifier.block_pool_id.clone(),
-                secret: token_identifier.handshake_secret.clone(),
-            })
-        } else {
-            None
+#[cfg(test)]
+mod test {
+    use crate::security::{
+        digest::{Challenge, DigestContext, Qop},
+        user::Token,
+    };
+
+    use super::DigestSaslSession;
+
+    #[test]
+    fn test_challenge_parse() {
+        let token = vec![
+            114u8, 101, 97, 108, 109, 61, 34, 100, 101, 102, 97, 117, 108, 116, 34, 44, 110, 111,
+            110, 99, 101, 61, 34, 81, 117, 76, 51, 98, 121, 86, 111, 75, 83, 48, 99, 77, 47, 77,
+            52, 98, 57, 47, 68, 110, 50, 80, 97, 48, 115, 47, 69, 56, 72, 83, 106, 88, 74, 87, 55,
+            88, 80, 105, 109, 34, 44, 113, 111, 112, 61, 34, 97, 117, 116, 104, 45, 99, 111, 110,
+            102, 44, 97, 117, 116, 104, 34, 44, 99, 104, 97, 114, 115, 101, 116, 61, 117, 116, 102,
+            45, 56, 44, 99, 105, 112, 104, 101, 114, 61, 34, 51, 100, 101, 115, 44, 114, 99, 52,
+            44, 100, 101, 115, 44, 114, 99, 52, 45, 53, 54, 44, 114, 99, 52, 45, 52, 48, 34, 44,
+            97, 108, 103, 111, 114, 105, 116, 104, 109, 61, 109, 100, 53, 45, 115, 101, 115, 115,
+        ];
+
+        let challenge: Challenge = token.try_into().unwrap();
+        assert_eq!(challenge.realm, "default");
+        assert_eq!(challenge.qop, vec![Qop::AuthConf, Qop::Auth]);
+        assert_eq!(
+            challenge
+                .cipher
+                .as_ref()
+                .map(|c| c.iter().map(String::as_ref).collect()),
+            Some(vec!["3des", "rc4", "des", "rc4-56", "rc4-40"])
+        );
+    }
+
+    #[test]
+    fn test_digest_step_authentication() {
+        let token = Token {
+            alias: "127.0.0.1:9000".to_string(),
+            identifier: vec![
+                0, 26, 104, 100, 102, 115, 47, 108, 111, 99, 97, 108, 104, 111, 115, 116, 64, 69,
+                88, 65, 77, 80, 76, 69, 46, 67, 79, 77, 0, 0, 138, 1, 142, 109, 254, 210, 147, 138,
+                1, 142, 146, 11, 86, 147, 1, 2,
+            ],
+            password: vec![
+                14, 15, 143, 95, 134, 65, 129, 9, 34, 197, 119, 3, 114, 115, 76, 203, 148, 2, 171,
+                78,
+            ],
+            kind: "HDFS_DELEGATION_TOKEN".to_string(),
+            service: "127.0.0.1:9000".to_string(),
         };
 
-        let message = DataTransferEncryptorMessageProto {
-            handshake_secret,
-            status: DataTransferEncryptorStatus::Success as i32,
-            ..Default::default()
+        let session = DigestSaslSession::from_token("".to_string(), "default".to_string(), &token);
+        let ctx = DigestContext {
+            nonce: "A+DoU3+eajz9Ei11Ib0S9CUKLyLPh0qFJbwn1/OZ".to_string(),
+            cnonce: "UGP4ejVb7M54KO4yqDwCsA==".to_string(),
+            realm: "default".to_string(),
+            qop: Qop::Auth,
         };
-
-        debug!("Sending data transfer encryptor message: {:?}", message);
-
-        self.stream
-            .write_all(&message.encode_length_delimited_to_vec())
-            .await?;
-        self.stream.flush().await?;
-
-        let response = self.read_sasl_response().await?;
-        debug!("Data transfer encryptor response: {:?}", response);
-
-        let (payload, finished) = session.step(response.payload.as_ref().map(|p| &p[..]))?;
-        assert!(!finished);
-
-        let message = DataTransferEncryptorMessageProto {
-            status: DataTransferEncryptorStatus::Success as i32,
-            payload: Some(payload),
-            ..Default::default()
+        assert_eq!(
+            &session.compute(&ctx, true),
+            "6dca7e74e7ea760a91758106fa7c885c"
+        );
+    }
+
+    #[test]
+    fn test_digest_step_privacy() {
+        let token = Token {
+            alias: "127.0.0.1:9000".to_string(),
+            identifier: vec![
+                0, 26, 104, 100, 102, 115, 47, 108, 111, 99, 97, 108, 104, 111, 115, 116, 64, 69,
+                88, 65, 77, 80, 76, 69, 46, 67, 79, 77, 0, 0, 138, 1, 142, 110, 11, 155, 153, 138,
+                1, 142, 146, 24, 31, 153, 1, 2,
+            ],
+            password: vec![
+                65, 93, 14, 143, 178, 108, 30, 148, 166, 96, 31, 211, 51, 100, 5, 190, 193, 17,
+                230, 5,
+            ],
+            kind: "HDFS_DELEGATION_TOKEN".to_string(),
+            service: "127.0.0.1:9000".to_string(),
         };
 
-        debug!("Sending data transfer encryptor message: {:?}", message);
-
-        self.stream
-            .write_all(&message.encode_length_delimited_to_vec())
-            .await?;
-        self.stream.flush().await?;
-
-        let response = self.read_sasl_response().await?;
-        debug!("Data transfer encryptor response: {:?}", response);
-
-        let (_, finished) = session.step(response.payload.as_ref().map(|p| &p[..]))?;
-
-        assert!(finished);
-
-        Ok(self.stream.into_inner())
-    }
-
-    async fn read_sasl_response(&mut self) -> Result<DataTransferEncryptorMessageProto> {
-        self.stream.fill_buf().await?;
-
-        let buf = self.stream.fill_buf().await?;
-        if buf.is_empty() {
-            return Err(std::io::Error::from(std::io::ErrorKind::UnexpectedEof))?;
-        }
-        let msg_length = prost::decode_length_delimiter(buf)?;
-        let total_size = msg_length + prost::length_delimiter_len(msg_length);
-
-        let mut response_buf = BytesMut::zeroed(total_size);
-        self.stream.read_exact(&mut response_buf).await?;
-
-        Ok(DataTransferEncryptorMessageProto::decode_length_delimited(
-            response_buf.freeze(),
-        )?)
+        let session = DigestSaslSession::from_token("".to_string(), "default".to_string(), &token);
+        let ctx = DigestContext {
+            nonce: "tm3kclm9F0JMECFNJi5xk/NaGgQ75ZOqb9/vCHt5".to_string(),
+            cnonce: "kp49R9SjR4de6ynNgMwNwQ==".to_string(),
+            realm: "default".to_string(),
+            qop: Qop::Auth,
+        };
+        assert_eq!(
+            &session.compute(&ctx, true),
+            "260f34cc6e484ede6277cb9c37672d07"
+        );
     }
 }
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/src/security/user.rs` & `hdfs_native-0.9.1/crates/hdfs-native/src/security/user.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/tests/common/mod.rs` & `hdfs_native-0.9.1/crates/hdfs-native/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/tests/test_ec.rs` & `hdfs_native-0.9.1/crates/hdfs-native/tests/test_ec.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/tests/test_integration.rs` & `hdfs_native-0.9.1/crates/hdfs-native/tests/test_integration.rs`

 * *Files 12% similar despite different names*

```diff
@@ -22,30 +22,38 @@
         test_with_features(&HashSet::from([DfsFeatures::Security]))
             .await
             .unwrap();
     }
 
     #[tokio::test]
     #[serial]
-    #[cfg(feature = "token")]
     async fn test_security_token() {
         test_with_features(&HashSet::from([DfsFeatures::Security, DfsFeatures::Token]))
             .await
             .unwrap();
     }
 
     #[tokio::test]
-    #[ignore]
     #[serial]
-    #[cfg(feature = "token")]
-    async fn test_privacy_token() {
+    async fn test_integrity_kerberos() {
+        test_with_features(&HashSet::from([
+            DfsFeatures::Security,
+            DfsFeatures::Integrity,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    #[tokio::test]
+    #[serial]
+    async fn test_integrity_token() {
         test_with_features(&HashSet::from([
             DfsFeatures::Security,
             DfsFeatures::Token,
-            DfsFeatures::Privacy,
+            DfsFeatures::Integrity,
         ]))
         .await
         .unwrap();
     }
 
     #[tokio::test]
     #[serial]
@@ -57,14 +65,75 @@
         ]))
         .await
         .unwrap();
     }
 
     #[tokio::test]
     #[serial]
+    async fn test_privacy_token() {
+        test_with_features(&HashSet::from([
+            DfsFeatures::Security,
+            DfsFeatures::Token,
+            DfsFeatures::Privacy,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    #[tokio::test]
+    #[serial]
+    async fn test_aes() {
+        test_with_features(&HashSet::from([
+            DfsFeatures::Security,
+            DfsFeatures::Privacy,
+            DfsFeatures::AES,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    #[tokio::test]
+    #[serial]
+    async fn test_forced_data_transfer_encryption() {
+        // DataTransferEncryption enabled but privacy isn't, still force encryption
+        test_with_features(&HashSet::from([
+            DfsFeatures::Security,
+            DfsFeatures::DataTransferEncryption,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    #[tokio::test]
+    #[serial]
+    async fn test_data_transfer_encryption() {
+        test_with_features(&HashSet::from([
+            DfsFeatures::Security,
+            DfsFeatures::Privacy,
+            DfsFeatures::DataTransferEncryption,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    #[tokio::test]
+    #[serial]
+    async fn test_data_transfer_encryption_aes() {
+        test_with_features(&HashSet::from([
+            DfsFeatures::Security,
+            DfsFeatures::Privacy,
+            DfsFeatures::DataTransferEncryption,
+            DfsFeatures::AES,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    #[tokio::test]
+    #[serial]
     async fn test_basic_ha() {
         test_with_features(&HashSet::from([DfsFeatures::HA]))
             .await
             .unwrap();
     }
 
     #[tokio::test]
@@ -78,15 +147,14 @@
         ]))
         .await
         .unwrap();
     }
 
     #[tokio::test]
     #[serial]
-    #[cfg(feature = "token")]
     async fn test_security_token_ha() {
         test_with_features(&HashSet::from([
             DfsFeatures::Security,
             DfsFeatures::Token,
             DfsFeatures::HA,
         ]))
         .await
@@ -100,15 +168,15 @@
             .await
             .unwrap();
     }
 
     pub async fn test_with_features(features: &HashSet<DfsFeatures>) -> Result<()> {
         let _ = env_logger::builder().is_test(true).try_init();
 
-        let _dfs = setup(&features);
+        let _dfs = setup(features);
         let client = Client::default();
 
         test_file_info(&client).await?;
         test_listing(&client).await?;
         test_rename(&client).await?;
         test_dirs(&client).await?;
         test_read_write(&client).await?;
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/tests/test_read.rs` & `hdfs_native-0.9.1/crates/hdfs-native/tests/test_read.rs`

 * *Files 20% similar despite different names*

```diff
@@ -7,18 +7,51 @@
     use bytes::Buf;
     use hdfs_native::{minidfs::DfsFeatures, Client, Result};
     use serial_test::serial;
     use std::collections::HashSet;
 
     #[tokio::test]
     #[serial]
-    async fn test_read() -> Result<()> {
+    async fn test_read_simple() {
+        test_read(&HashSet::from([DfsFeatures::HA])).await.unwrap();
+    }
+
+    // These tests take a long time, so don't run by default
+    #[tokio::test]
+    #[serial]
+    #[ignore]
+    async fn test_read_sasl_encryption() {
+        test_read(&HashSet::from([
+            DfsFeatures::HA,
+            DfsFeatures::Security,
+            DfsFeatures::Privacy,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    // These tests take a long time, so don't run by default
+    #[tokio::test]
+    #[serial]
+    #[ignore]
+    async fn test_read_cipher_encryption() {
+        test_read(&HashSet::from([
+            DfsFeatures::HA,
+            DfsFeatures::Security,
+            DfsFeatures::Privacy,
+            DfsFeatures::AES,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    async fn test_read(features: &HashSet<DfsFeatures>) -> Result<()> {
         let _ = env_logger::builder().is_test(true).try_init();
 
-        let _dfs = setup(&HashSet::from([DfsFeatures::HA]));
+        let _dfs = setup(features);
         let client = Client::default();
 
         // Read the whole file
         let reader = client.read("/testfile").await?;
         let mut buf = reader.read_range(0, TEST_FILE_INTS * 4).await?;
         for i in 0..TEST_FILE_INTS as i32 {
             assert_eq!(buf.get_i32(), i);
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/tests/test_viewfs.rs` & `hdfs_native-0.9.1/crates/hdfs-native/tests/test_viewfs.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/tests/test_write.rs` & `hdfs_native-0.9.1/crates/hdfs-native/tests/test_write.rs`

 * *Files 22% similar despite different names*

```diff
@@ -7,22 +7,56 @@
     use bytes::{BufMut, BytesMut};
     use hdfs_native::{minidfs::DfsFeatures, Client, Result, WriteOptions};
     use serial_test::serial;
     use std::collections::HashSet;
 
     #[tokio::test]
     #[serial]
-    async fn test_write() {
+    async fn test_write_simple() {
+        test_write(&HashSet::from([DfsFeatures::HA])).await.unwrap();
+    }
+
+    // These tests take a long time, so don't run by default
+    #[tokio::test]
+    #[serial]
+    #[ignore]
+    async fn test_write_sasl_encryption() {
+        test_write(&HashSet::from([
+            DfsFeatures::HA,
+            DfsFeatures::Security,
+            DfsFeatures::Privacy,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    // These tests take a long time, so don't run by default
+    #[tokio::test]
+    #[serial]
+    #[ignore]
+    async fn test_write_cipher_encryption() {
+        test_write(&HashSet::from([
+            DfsFeatures::HA,
+            DfsFeatures::Security,
+            DfsFeatures::Privacy,
+            DfsFeatures::AES,
+        ]))
+        .await
+        .unwrap();
+    }
+
+    async fn test_write(features: &HashSet<DfsFeatures>) -> Result<()> {
         let _ = env_logger::builder().is_test(true).try_init();
 
-        let _dfs = setup(&HashSet::from([DfsFeatures::HA]));
+        let _dfs = setup(features);
         let client = Client::default();
 
-        test_create(&client).await.unwrap();
-        test_append(&client).await.unwrap();
+        test_create(&client).await?;
+        test_append(&client).await?;
+        Ok(())
     }
 
     async fn test_create(client: &Client) -> Result<()> {
         let write_options = WriteOptions::default().overwrite(true);
 
         // Create an empty file
         let mut writer = client.create("/newfile", &write_options).await?;
```

### Comparing `hdfs_native-0.8.0/crates/hdfs-native/tests/test_write_resiliency.rs` & `hdfs_native-0.9.1/crates/hdfs-native/tests/test_write_resiliency.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/README.md` & `hdfs_native-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 - [x] ViewFS
 - [x] Router based federation
 - [x] Erasure coded reads and writes
     - RS schema only, no support for RS-Legacy or XOR
 
 ### Security Features
 - [x] Kerberos authentication (GSSAPI SASL support)
-- [x] Token authentication (DIGEST-MD5 SASL support, no encryption support)
+- [x] Token authentication (DIGEST-MD5 SASL support)
 - [x] NameNode SASL connection
 - [x] DataNode SASL connection
-- [ ] DataNode data transfer encryption
+- [x] DataNode data transfer encryption
 - [ ] Encryption at rest (KMS support)
 
 ## Supported HDFS Settings
 The client will attempt to read Hadoop configs `core-site.xml` and `hdfs-site.xml` in the directories `$HADOOP_CONF_DIR` or if that doesn't exist, `$HADOOP_HOME/etc/hadoop`. Currently the supported configs that are used are:
 - `fs.defaultFS` - Client::default() support
 - `dfs.ha.namenodes` - name service support
 - `dfs.namenode.rpc-address.*` - name service support
@@ -39,39 +39,38 @@
 
 All other settings are generally assumed to be the defaults currently. For instance, security is assumed to be enabled and SASL negotiation is always done, but on insecure clusters this will just do SIMPLE authentication. Any setups that require other customized Hadoop client configs may not work correctly. 
 
 ## Building
 
 ### Mac
 ```
-brew install gsasl krb5
+brew install krb5
 # You might need these env vars on newer Macs
 export BINDGEN_EXTRA_CLANG_ARGS="-I/opt/homebrew/include"
 export LIBRARY_PATH=/opt/homebrew/lib
-cargo build --features token,kerberos
+cargo build --features kerberos
 ```
 
 ### Ubuntu
 ```
-apt-get install clang libkrb5-dev libgsasl-dev
-cargo build --features token,kerberos
+apt-get install clang libkrb5-dev
+cargo build --features kerberos
 ```
 
 ## Crate features
-- `token` - enables token based DIGEST-MD5 authentication support. This uses the `gsasl` native library and only supports authentication, not integrity or confidentiality
 - `kerberos` - enables kerberos GSSAPI authentication support. This uses the `libgssapi` crate and supports integrity as well as confidentiality
 
 ## Object store implementation
 An object_store implementation for HDFS is provided in the [hdfs-native-object-store](./crates/hdfs-native-object-store/) crate.
 
 ## Running tests
 The tests are mostly integration tests that utilize a small Java application in `rust/mindifs/` that runs a custom `MiniDFSCluster`. To run the tests, you need to have Java, Maven, Hadoop binaries, and Kerberos tools available and on your path. Any Java version between 8 and 17 should work.
 
 ```bash
-cargo test -p hdfs-native --features token,kerberos,intergation-test
+cargo test -p hdfs-native --features kerberos,intergation-test
 ```
 
 ### Python tests
 See the [Python README](./python/README.md)
 
 ## Running benchmarks
 Some of the benchmarks compare performance to the JVM based client through libhdfs via the fs-hdfs3 crate. Because of that, some extra setup is required to run the benchmarks:
```

### Comparing `hdfs_native-0.8.0/python/README.md` & `hdfs_native-0.9.1/python/README.md`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/python/python/hdfs_native/__init__.py` & `hdfs_native-0.9.1/python/python/hdfs_native/__init__.py`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/python/python/hdfs_native/_internal.pyi` & `hdfs_native-0.9.1/python/python/hdfs_native/_internal.pyi`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/python/src/error.rs` & `hdfs_native-0.9.1/python/src/error.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/python/src/lib.rs` & `hdfs_native-0.9.1/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/python/tests/conftest.py` & `hdfs_native-0.9.1/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/python/tests/test_integration.py` & `hdfs_native-0.9.1/python/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/pyproject.toml` & `hdfs_native-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/python/hdfs_native/__init__.py` & `hdfs_native-0.9.1/python/hdfs_native/__init__.py`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/python/hdfs_native/_internal.pyi` & `hdfs_native-0.9.1/python/hdfs_native/_internal.pyi`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.8.0/PKG-INFO` & `hdfs_native-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hdfs-native
-Version: 0.8.0
+Version: 0.9.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python bindings for hdfs-native Rust library
 Keywords: hadoop,hdfs
 Home-Page: https://github.com/Kimahriman/hdfs-native
 Author: Adam Binford <adamq43@gmail.com>
```

