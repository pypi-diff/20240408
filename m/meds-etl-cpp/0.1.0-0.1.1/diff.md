# Comparing `tmp/meds_etl_cpp-0.1.0.tar.gz` & `tmp/meds_etl_cpp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meds_etl_cpp-0.1.0.tar", last modified: Wed Apr  3 01:13:01 2024, max compression
+gzip compressed data, was "meds_etl_cpp-0.1.1.tar", last modified: Mon Apr  8 05:18:12 2024, max compression
```

## Comparing `meds_etl_cpp-0.1.0.tar` & `meds_etl_cpp-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 ethanid  (312007) ethanid  (312007)        0 2024-04-03 01:13:01.138323 meds_etl_cpp-0.1.0/
-drwxrwxr-x   0 ethanid  (312007) ethanid  (312007)        0 2024-04-03 01:13:01.069094 meds_etl_cpp-0.1.0/.github/
-drwxrwxr-x   0 ethanid  (312007) ethanid  (312007)        0 2024-04-03 01:13:01.085276 meds_etl_cpp-0.1.0/.github/workflows/
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)     3194 2024-04-03 01:11:57.000000 meds_etl_cpp-0.1.0/.github/workflows/python-build.yml
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)       35 2024-04-03 00:15:12.000000 meds_etl_cpp-0.1.0/.gitignore
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)    11356 2024-04-03 00:34:03.000000 meds_etl_cpp-0.1.0/LICENSE
--rw-r--r--   0 ethanid  (312007) ethanid  (312007)      223 2024-04-03 01:13:01.135764 meds_etl_cpp-0.1.0/PKG-INFO
-drwxrwxr-x   0 ethanid  (312007) ethanid  (312007)        0 2024-04-03 01:13:01.133470 meds_etl_cpp-0.1.0/meds_etl_cpp.egg-info/
--rw-r--r--   0 ethanid  (312007) ethanid  (312007)      223 2024-04-03 01:13:00.000000 meds_etl_cpp-0.1.0/meds_etl_cpp.egg-info/PKG-INFO
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)      516 2024-04-03 01:13:01.000000 meds_etl_cpp-0.1.0/meds_etl_cpp.egg-info/SOURCES.txt
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)        1 2024-04-03 01:13:00.000000 meds_etl_cpp-0.1.0/meds_etl_cpp.egg-info/dependency_links.txt
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)        1 2024-04-03 00:30:30.000000 meds_etl_cpp-0.1.0/meds_etl_cpp.egg-info/not-zip-safe
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)       13 2024-04-03 01:13:00.000000 meds_etl_cpp-0.1.0/meds_etl_cpp.egg-info/top_level.txt
-drwxrwxr-x   0 ethanid  (312007) ethanid  (312007)        0 2024-04-03 01:13:01.125592 meds_etl_cpp-0.1.0/native/
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)       95 2024-03-30 01:59:37.000000 meds_etl_cpp-0.1.0/native/.bazelrc
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)       35 2024-04-02 22:58:21.000000 meds_etl_cpp-0.1.0/native/.clang-format
--rw-r--r--   0 ethanid  (312007) ethanid  (312007)     1541 2024-04-03 00:25:42.000000 meds_etl_cpp-0.1.0/native/BUILD
--rw-r--r--   0 ethanid  (312007) ethanid  (312007)     3439 2024-04-03 00:51:05.000000 meds_etl_cpp-0.1.0/native/WORKSPACE
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)       50 2024-04-02 22:17:29.000000 meds_etl_cpp-0.1.0/native/backupbazelrc
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)      347 2024-04-03 00:35:56.000000 meds_etl_cpp-0.1.0/native/main.cc
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)      130 2024-04-03 00:35:56.000000 meds_etl_cpp-0.1.0/native/meds_etl_cpp.cc
-drwxrwxr-x   0 ethanid  (312007) ethanid  (312007)        0 2024-04-03 01:13:01.130771 meds_etl_cpp-0.1.0/native/patches/
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)       51 2024-04-03 00:15:01.000000 meds_etl_cpp-0.1.0/native/patches/BUILD
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)      526 2024-04-03 00:12:04.000000 meds_etl_cpp-0.1.0/native/patches/ThirdpartyToolchain.cmake.patch
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)    38768 2024-04-03 00:35:56.000000 meds_etl_cpp-0.1.0/native/perform_etl.cc
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)      160 2024-04-03 00:35:54.000000 meds_etl_cpp-0.1.0/native/perform_etl.hh
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)       89 2024-04-02 22:16:22.000000 meds_etl_cpp-0.1.0/native/simple_test.cc
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)      689 2024-04-03 00:49:05.000000 meds_etl_cpp-0.1.0/pyproject.toml
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)       38 2024-04-03 01:13:01.138597 meds_etl_cpp-0.1.0/setup.cfg
--rw-rw-r--   0 ethanid  (312007) ethanid  (312007)     3475 2024-04-03 00:48:33.000000 meds_etl_cpp-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.051821 meds_etl_cpp-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.043821 meds_etl_cpp-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.047821 meds_etl_cpp-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/.github/workflows/python-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 05:18:12.051821 meds_etl_cpp-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.051821 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 05:18:12.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 05:18:12.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:18:12.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:18:11.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 05:18:12.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.047821 meds_etl_cpp-0.1.1/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/.bazelrc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/WORKSPACE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/backupbazelrc
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/meds_etl_cpp.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.047821 meds_etl_cpp-0.1.1/native/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/patches/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/patches/ThirdpartyToolchain.cmake.patch
+-rw-r--r--   0 runner    (1001) docker     (127)    48502 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/perform_etl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/perform_etl.hh
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/simple_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:18:12.051821 meds_etl_cpp-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/setup.py
```

### Comparing `meds_etl_cpp-0.1.0/.github/workflows/python-build.yml` & `meds_etl_cpp-0.1.1/.github/workflows/python-build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -64,16 +64,17 @@
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
-        name: python-package-distributions
+        name: artifact
         path: dist/
+
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
     name: >-
       Sign the Python 🐍 distribution 📦 with Sigstore
       and upload them to GitHub Release
@@ -85,16 +86,17 @@
       contents: write  # IMPORTANT: mandatory for making GitHub Releases
       id-token: write  # IMPORTANT: mandatory for sigstore
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
-        name: python-package-distributions
-        path: dist/
+        name: artifact
+        path: dist
+        
     - name: Sign the dists with Sigstore
       uses: sigstore/gh-action-sigstore-python@v1.2.3
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
```

### Comparing `meds_etl_cpp-0.1.0/LICENSE` & `meds_etl_cpp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.0/meds_etl_cpp.egg-info/SOURCES.txt` & `meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.0/native/BUILD` & `meds_etl_cpp-0.1.1/native/BUILD`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     srcs=["perform_etl.cc"],
     hdrs=["perform_etl.hh"],
     deps=[
         ":arrow", 
         "@com_google_absl//absl/types:optional",
         "@readerwriterqueue",
         "@concurrentqueue",
-        "@snappy",
+        ":zstd",
     ],
 )
 
 cc_binary(
     name="main",
     srcs=["main.cc"],
     deps=[
@@ -51,18 +51,27 @@
         "ARROW_BUILD_TESTS": "OFF",
         "ARROW_PARQUET": "ON",
         "ARROW_WITH_SNAPPY": "ON",
         "ARROW_WITH_ZSTD": "ON",
         "EP_COMMON_CMAKE_ARGS": "-DWITH_OPENSSL=OFF",
         "ARROW_DEPENDENCY_SOURCE": "BUNDLED",
     },
-    deps = [
-    ],
     tags = ["requires-network"],
     generate_args = ["-DCMAKE_RANLIB=/usr/bin/ranlib"],
     working_directory="cpp",
     lib_source = "@arrow//:all",
     out_lib_dir = "lib64",
     out_static_libs = ["libparquet.a", "libarrow.a", "libarrow_bundled_dependencies.a"],
     linkopts = ["-pthread"],
-
 )
+
+cmake(
+    name = "zstd",
+    cache_entries = {
+        "CMAKE_C_FLAGS": "-fPIC",
+        "CMAKE_CXX_FLAGS": "-fPIC",
+    },
+    working_directory="build/cmake",
+    lib_source = "@zstd//:all",
+    out_lib_dir = "lib64",
+    out_static_libs = ["libzstd.a"],
+)
```

### Comparing `meds_etl_cpp-0.1.0/native/WORKSPACE` & `meds_etl_cpp-0.1.1/native/WORKSPACE`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,14 @@
 http_archive(
   name = "com_google_absl",
   urls = ["https://github.com/abseil/abseil-cpp/archive/2f9e432cce407ce0ae50676696666f33a77d42ac.zip"],
   strip_prefix = "abseil-cpp-2f9e432cce407ce0ae50676696666f33a77d42ac",
   sha256 = "efa465b26da194f82320b4e39e2ca637ebe3129d7f3732ee71d9942099e3c773",
 )
 
-http_archive(
-  name = "snappy",
-  urls = ["https://github.com/google/snappy/archive/27f34a580be4a3becf5f8c0cba13433f53c21337.zip"],
-  strip_prefix = "snappy-27f34a580be4a3becf5f8c0cba13433f53c21337",
-  sha256 = "6c18c64264a2b15531896824b85c47e85da3e42059631661fbe0c588e4e3aa99",
-)
-
 new_git_repository(
     name = "concurrentqueue",
     remote = "https://github.com/cameron314/concurrentqueue.git",
     commit = "79cec4c3bf1ca23ea4a03adfcd3c2c3659684dd2",
     shallow_since = "1580387311 -0500",
     build_file_content = """
 
@@ -86,7 +79,14 @@
     name="arrow",
     strip_prefix="arrow-apache-arrow-15.0.2",
     urls = ["https://github.com/apache/arrow/archive/refs/tags/apache-arrow-15.0.2.zip"],
     build_file_content = all_content,
     sha256 = "c0ebc13e9bc428c0c9f617444dcd161140e2bf9a7c65c5ae6bf239e5567175fd",
     patches = ["//patches:ThirdpartyToolchain.cmake.patch"],
 )
+
+http_archive(
+    name="zstd",
+    strip_prefix="zstd-1.5.6",
+    urls = ["https://github.com/facebook/zstd/archive/refs/tags/v1.5.6.zip"],
+    build_file_content = all_content,
+)
```

### Comparing `meds_etl_cpp-0.1.0/native/patches/ThirdpartyToolchain.cmake.patch` & `meds_etl_cpp-0.1.1/native/patches/ThirdpartyToolchain.cmake.patch`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.0/native/perform_etl.cc` & `meds_etl_cpp-0.1.1/native/perform_etl.cc`

 * *Files 12% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 #include "arrow/array/builder_primitive.h"
 #include "arrow/io/file.h"
 #include "arrow/memory_pool.h"
 #include "arrow/record_batch.h"
 #include "arrow/table.h"
 #include "arrow/util/type_fwd.h"
 #include "blockingconcurrentqueue.h"
+#include "lightweightsemaphore.h"
 #include "parquet/arrow/reader.h"
 #include "parquet/arrow/schema.h"
 #include "parquet/arrow/writer.h"
-#include "readerwritercircularbuffer.h"
-#include "snappy.h"
+#include "zstd.h"
 
 namespace fs = std::filesystem;
 
-const size_t SHARD_PIECE_SIZE = 1000 * 1000 * 1000;  // Roughly 1 gigabyte
-const size_t SNAPPY_BUFFER_SIZE = 4 * 1000 * 1000;   // Roughly 4 megabytes
+const size_t SHARD_PIECE_SIZE = 2 * 1000 * 1000 * 1000;  // Roughly 2 gigabytes
+const size_t COMPRESSION_BUFFER_SIZE = 4 * 1000 * 1000;  // Roughly 4 megabytes
 
 std::vector<std::shared_ptr<::arrow::Field>> get_fields_for_file(
     arrow::MemoryPool* pool, const std::string& filename) {
     // Configure general Parquet reader settings
     auto reader_properties = parquet::ReaderProperties(pool);
     reader_properties.set_buffer_size(4096 * 4);
     reader_properties.enable_buffered_stream();
@@ -70,53 +70,46 @@
     return fields;
 }
 
 const std::vector<std::string> known_fields = {
     "patient_id",    "time",           "code",
     "numeric_value", "datetime_value", "text_value"};
 
-bool is_string_type(const arrow::Field& field) {
-    return field.type()->Equals(arrow::LargeStringType());
-}
-
-std::set<std::string> get_metadata_fields(
-    const std::vector<std::string>& files) {
+std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>>
+get_metadata_fields(const std::vector<std::string>& files) {
     arrow::MemoryPool* pool = arrow::default_memory_pool();
-    std::set<std::string> result;
+    std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>> result;
 
     for (const auto& file : files) {
         auto fields = get_fields_for_file(pool, file);
         for (const auto& field : fields) {
             if (field->name() == "value") {
                 throw std::runtime_error(
                     "The C++ MEDS-Flat ETL does not currently support generic "
                     "value fields " +
                     field->ToString());
             }
 
             if (std::find(std::begin(known_fields), std::end(known_fields),
                           field->name()) == std::end(known_fields)) {
-                if (!is_string_type(*field)) {
-                    throw std::runtime_error(
-                        "The C++ MEDS-Flat ETL only supports large_string "
-                        "metadata for now, but found " +
-                        field->ToString());
-                }
-                result.insert(field->name());
+                result.insert(std::make_pair(field->name(), field->type()));
             }
         }
     }
 
     return result;
 }
 
-std::set<std::string> get_metadata_fields_multithreaded(
-    const std::vector<std::string>& files, size_t num_threads) {
+std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>>
+get_metadata_fields_multithreaded(const std::vector<std::string>& files,
+                                  size_t num_threads) {
     std::vector<std::thread> threads;
-    std::vector<std::set<std::string>> results(num_threads);
+    std::vector<
+        std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>>>
+        results(num_threads);
 
     size_t files_per_thread = (files.size() + num_threads - 1) / num_threads;
 
     for (size_t i = 0; i < num_threads; i++) {
         threads.emplace_back([&files, i, &results, files_per_thread]() {
             std::vector<std::string> fraction;
             for (size_t j = files_per_thread * i;
@@ -127,15 +120,15 @@
         });
     }
 
     for (auto& thread : threads) {
         thread.join();
     }
 
-    std::set<std::string> result;
+    std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>> result;
 
     for (auto& res : results) {
         result.merge(std::move(res));
     }
 
     return result;
 }
@@ -150,52 +143,61 @@
 
     absl::optional<float> numeric_value;
     absl::optional<int64_t> datetime_value; // Actually an Arrow Timestamp with
 microsecond precision absl::optional<std::string> text_value;
 
     std::vector<absl::optional<std::string>> metadata_columns;
 };
-*/
 
 struct Row {
     int64_t patient_id;
     int64_t time;
 
     std::vector<char> data;
 
     bool operator<(const Row& rhs) {
         return std::make_pair(patient_id, time) <
                std::make_pair(rhs.patient_id, rhs.time);
     }
 };
+*/
 
 template <typename T>
 void add_literal_to_vector(std::vector<char>& data, T to_add) {
     const char* bytes = reinterpret_cast<const char*>(&to_add);
     data.insert(std::end(data), bytes, bytes + sizeof(T));
 }
 
 void add_string_to_vector(std::vector<char>& data, std::string_view to_add) {
     add_literal_to_vector(data, to_add.size());
     data.insert(std::end(data), std::begin(to_add), std::end(to_add));
 }
 
-using QueueItem = absl::optional<Row>;
-using QueueType = moodycamel::BlockingReaderWriterCircularBuffer<QueueItem>;
+using QueueItem = absl::optional<std::vector<char>>;
+
+constexpr ssize_t SEMAPHORE_BLOCK_SIZE = 1000;
 
-void sort_reader(
+void shard_reader(
     size_t reader_index, size_t num_shards,
     moodycamel::BlockingConcurrentQueue<absl::optional<std::string>>&
         file_queue,
-    std::vector<
-        std::vector<moodycamel::BlockingReaderWriterCircularBuffer<QueueItem>>>&
+    std::vector<moodycamel::BlockingConcurrentQueue<QueueItem>>&
         all_write_queues,
-    const std::vector<std::string>& metadata_columns) {
+    moodycamel::LightweightSemaphore& all_write_semaphore,
+    const std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>&
+        metadata_columns) {
     arrow::MemoryPool* pool = arrow::default_memory_pool();
 
+    std::vector<moodycamel::ProducerToken> ptoks;
+    for (size_t i = 0; i < num_shards; i++) {
+        ptoks.emplace_back(all_write_queues[i]);
+    }
+
+    ssize_t slots_to_write = all_write_semaphore.waitMany(SEMAPHORE_BLOCK_SIZE);
+
     absl::optional<std::string> item;
     while (true) {
         file_queue.wait_dequeue(item);
 
         if (!item) {
             break;
         } else {
@@ -225,14 +227,17 @@
 
             int numeric_value_index = -1;
             int datetime_value_index = -1;
             int text_value_index = -1;
 
             std::vector<int> metadata_indices(metadata_columns.size(), -1);
 
+            std::bitset<std::numeric_limits<unsigned long long>::digits>
+                is_text_metadata;
+
             const auto& manifest = arrow_reader->manifest();
             for (const auto& schema_field : manifest.schema_fields) {
                 if (schema_field.children.size() != 0 ||
                     !schema_field.is_leaf()) {
                     throw std::runtime_error(
                         "For MEDS-Flat fields should not be nested, but we "
                         "have a non-nested field " +
@@ -254,15 +259,16 @@
                         throw std::runtime_error(
                             "C++ MEDS-Flat requires microsecond timestamp "
                             "times but found " +
                             schema_field.field->ToString());
                     }
                     time_index = schema_field.column_index;
                 } else if (schema_field.field->name() == "code") {
-                    if (!is_string_type(*(schema_field.field))) {
+                    if (!schema_field.field->type()->Equals(
+                            arrow::LargeStringType())) {
                         throw std::runtime_error(
                             "The C++ MEDS-Flat ETL requires large_string codes "
                             "but found " +
                             schema_field.field->ToString());
                     }
 
                     code_index = schema_field.column_index;
@@ -281,33 +287,58 @@
                         throw std::runtime_error(
                             "C++ MEDS-Flat requires microsecond timestamp "
                             "datetime_value but found " +
                             schema_field.field->ToString());
                     }
                     datetime_value_index = schema_field.column_index;
                 } else if (schema_field.field->name() == "text_value") {
-                    if (!is_string_type(*(schema_field.field))) {
+                    if (!schema_field.field->type()->Equals(
+                            arrow::LargeStringType())) {
                         throw std::runtime_error(
                             "C++ MEDS-Flat requires Float32 numeric_value but "
                             "found " +
                             schema_field.field->ToString());
                     }
                     text_value_index = schema_field.column_index;
                 } else {
                     // Must be metadata
-                    auto iter = std::find(std::begin(metadata_columns),
-                                          std::end(metadata_columns),
-                                          schema_field.field->name());
-                    if (!is_string_type(*(schema_field.field))) {
+                    auto iter = std::find_if(
+                        std::begin(metadata_columns),
+                        std::end(metadata_columns), [&](const auto& entry) {
+                            return entry.first == schema_field.field->name();
+                        });
+                    if (iter == std::end(metadata_columns)) {
+                        throw std::runtime_error(
+                            "Had an extra column in the metadata that "
+                            "shouldn't exist? " +
+                            schema_field.field->ToString());
+                    }
+
+                    if (!schema_field.field->type()->Equals(iter->second)) {
                         throw std::runtime_error(
                             "C++ MEDS-Flat requires large_string metadata but "
                             "found " +
                             schema_field.field->ToString());
                     }
+
                     int offset = (iter - std::begin(metadata_columns));
+
+                    if (iter->second->Equals(arrow::LargeStringType())) {
+                        is_text_metadata[offset] = true;
+                    } else {
+                        is_text_metadata[offset] = false;
+
+                        if (iter->second->byte_width() == -1) {
+                            throw std::runtime_error(
+                                "Found non text metadata with unknown byte "
+                                "width? " +
+                                iter->second->ToString());
+                        }
+                    }
+
                     metadata_indices[offset] = schema_field.column_index;
                 }
             }
 
             if (patient_id_index == -1) {
                 throw std::runtime_error(
                     "Could not find patient_id column index");
@@ -375,296 +406,205 @@
                     std::dynamic_pointer_cast<arrow::LargeStringArray>(
                         record_batch->column(text_value_index));
                 if (!text_value_array) {
                     throw std::runtime_error("Could not cast text_value array");
                 }
 
                 std::vector<std::shared_ptr<arrow::LargeStringArray>>
-                    metadata_arrays(metadata_columns.size());
+                    text_metadata_arrays(metadata_columns.size());
+                std::vector<std::shared_ptr<arrow::FixedSizeBinaryArray>>
+                    primitive_metadata_arrays(metadata_columns.size());
 
                 for (size_t i = 0; i < metadata_columns.size(); i++) {
                     if (metadata_indices[i] == -1) {
                         continue;
                     }
 
-                    auto metadata_array =
-                        std::dynamic_pointer_cast<arrow::LargeStringArray>(
-                            record_batch->column(metadata_indices[i]));
-                    if (!metadata_array) {
-                        throw std::runtime_error(
-                            "Could not cast metadata array " +
-                            metadata_columns[i]);
+                    if (is_text_metadata[i]) {
+                        auto metadata_array =
+                            std::dynamic_pointer_cast<arrow::LargeStringArray>(
+                                record_batch->column(metadata_indices[i]));
+                        if (!metadata_array) {
+                            throw std::runtime_error(
+                                "Could not cast metadata array to text" +
+                                metadata_columns[i].first + " " +
+                                metadata_columns[i].second->ToString());
+                        }
+                        text_metadata_arrays[i] = metadata_array;
+                    } else {
+                        std::shared_ptr<arrow::Array> fixed_size_array;
+                        PARQUET_ASSIGN_OR_THROW(
+                            fixed_size_array,
+                            record_batch->column(metadata_indices[i])
+                                ->View(std::make_shared<
+                                       arrow::FixedSizeBinaryType>(
+                                    metadata_columns[i].second->byte_width())));
+
+                        auto metadata_array = std::dynamic_pointer_cast<
+                            arrow::FixedSizeBinaryArray>(fixed_size_array);
+                        if (!metadata_array) {
+                            throw std::runtime_error(
+                                "Could not cast metadata array to fixed size " +
+                                metadata_columns[i].first + " " +
+                                metadata_columns[i].second->ToString());
+                        }
+                        primitive_metadata_arrays[i] = metadata_array;
                     }
-                    metadata_arrays[i] = metadata_array;
                 }
 
-                std::cout << source << " " << time_array->length() << " "
-                          << text_value_array->length() << " "
-                          << numeric_value_array->length() << std::endl;
-
                 for (int64_t i = 0; i < text_value_array->length(); i++) {
-                    Row row;
-
                     if (!patient_id_array->IsValid(i)) {
                         throw std::runtime_error(
                             "patient_id incorrectly has null value " + source);
                     }
                     if (!time_array->IsValid(i)) {
                         throw std::runtime_error(
                             "time incorrectly has null value " + source);
                     }
                     if (!code_array->IsValid(i)) {
                         throw std::runtime_error(
                             "code incorrectly has null value " + source);
                     }
 
-                    row.patient_id = patient_id_array->Value(i);
-                    row.time = time_array->Value(i);
+                    std::vector<char> data;
+
+                    int64_t patient_id = patient_id_array->Value(i);
+                    int64_t time = time_array->Value(i);
 
                     std::bitset<std::numeric_limits<unsigned long long>::digits>
                         non_null;
 
-                    add_literal_to_vector(row.data, row.patient_id);
-                    add_literal_to_vector(row.data, row.time);
+                    add_literal_to_vector(data, patient_id);
+                    add_literal_to_vector(data, time);
 
-                    add_string_to_vector(row.data, code_array->Value(i));
+                    add_string_to_vector(data, code_array->Value(i));
 
                     if (numeric_value_array->IsValid(i)) {
                         non_null[0] = true;
-                        add_literal_to_vector(row.data,
+                        add_literal_to_vector(data,
                                               numeric_value_array->Value(i));
                     }
 
                     if (datetime_value_array->IsValid(i)) {
                         non_null[1] = true;
-                        add_literal_to_vector(row.data,
+                        add_literal_to_vector(data,
                                               datetime_value_array->Value(i));
                     }
 
                     if (text_value_array->IsValid(i)) {
                         non_null[2] = true;
-                        add_string_to_vector(row.data,
-                                             text_value_array->Value(i));
+                        add_string_to_vector(data, text_value_array->Value(i));
                     }
 
                     for (size_t j = 0; j < metadata_columns.size(); j++) {
-                        if (metadata_arrays[j] &&
-                            metadata_arrays[j]->IsValid(i)) {
-                            non_null[3 + j] = true;
-                            add_string_to_vector(row.data,
-                                                 metadata_arrays[j]->Value(i));
+                        if (is_text_metadata[j]) {
+                            if (text_metadata_arrays[j] &&
+                                text_metadata_arrays[j]->IsValid(i)) {
+                                non_null[3 + j] = true;
+                                add_string_to_vector(
+                                    data, text_metadata_arrays[j]->Value(i));
+                            }
+                        } else {
+                            if (primitive_metadata_arrays[j] &&
+                                primitive_metadata_arrays[j]->IsValid(i)) {
+                                non_null[3 + j] = true;
+                                add_string_to_vector(
+                                    data,
+                                    primitive_metadata_arrays[j]->GetView(i));
+                            }
                         }
                     }
 
-                    add_literal_to_vector(row.data, non_null.to_ullong());
+                    add_literal_to_vector(data, non_null.to_ullong());
 
                     size_t index =
-                        std::hash<int64_t>()(row.patient_id) % num_shards;
-                    all_write_queues[index][reader_index].wait_enqueue(
-                        std::move(row));
+                        std::hash<int64_t>()(patient_id) % num_shards;
+                    all_write_queues[index].enqueue(ptoks[index],
+                                                    std::move(data));
+
+                    slots_to_write--;
+                    if (slots_to_write == 0) {
+                        slots_to_write =
+                            all_write_semaphore.waitMany(SEMAPHORE_BLOCK_SIZE);
+                    }
                 }
             }
         }
     }
 
     for (size_t j = 0; j < num_shards; j++) {
-        all_write_queues[j][reader_index].wait_enqueue(absl::nullopt);
+        all_write_queues[j].enqueue(ptoks[j], absl::nullopt);
     }
-}
 
-template <typename T, typename F>
-void dequeue_many_loop(T& in_queues, F f) {
-    std::vector<size_t> good_indices;
-    good_indices.reserve(in_queues.size());
-    for (size_t i = 0; i < in_queues.size(); i++) {
-        good_indices.push_back(i);
-    }
-
-    typename T::value_type::value_type next_entry;
-
-    while (good_indices.size() > 0) {
-        for (size_t i = 1; i <= good_indices.size(); i++) {
-            size_t index = good_indices[i - 1];
-            while (true) {
-                bool found = in_queues[index].try_dequeue(next_entry);
-
-                if (!found) {
-                    break;
-                }
-
-                if (!next_entry) {
-                    std::swap(good_indices[i - 1], good_indices.back());
-                    good_indices.pop_back();
-                    i -= 1;
-                    break;
-                } else {
-                    f(*next_entry);
-                }
-            }
-        }
+    if (slots_to_write > 0) {
+        all_write_semaphore.signal(slots_to_write);
     }
 }
 
-void sort_writer(
-    size_t writer_index, size_t num_shards,
-    std::vector<moodycamel::BlockingReaderWriterCircularBuffer<QueueItem>>&
-        write_queues,
-    const std::filesystem::path& target_dir) {
-    std::filesystem::create_directory(target_dir);
-
-    std::vector<Row> rows;
-    std::vector<std::tuple<int64_t, int64_t, size_t>> row_indices;
-
-    size_t current_size = 0;
-
-    size_t current_file_index = 0;
-
-    std::vector<char> uncompressed_data;
-    std::vector<char> compressed_data;
-
-    auto flush_file = [&]() {
-        auto target_file = target_dir / std::to_string(current_file_index);
-
-        std::sort(std::begin(row_indices), std::end(row_indices));
-
-        std::ofstream writer(target_file,
-                             std::ofstream::binary | std::ofstream::out);
-
-        auto flush_compressed = [&]() {
-            if (compressed_data.size() <
-                snappy::MaxCompressedLength(uncompressed_data.size())) {
-                compressed_data.resize(
-                    snappy::MaxCompressedLength(uncompressed_data.size()) * 2);
-            }
-
-            size_t compressed_length;
-            snappy::RawCompress(uncompressed_data.data(),
-                                uncompressed_data.size(),
-                                compressed_data.data(), &compressed_length);
-
-            writer.write(reinterpret_cast<char*>(&compressed_length),
-                         sizeof(compressed_length));
-            writer.write(compressed_data.data(), compressed_length);
-
-            uncompressed_data.clear();
-        };
-
-        for (const auto& row_index : row_indices) {
-            const auto& row_to_insert = rows[std::get<2>(row_index)];
-            add_string_to_vector(uncompressed_data,
-                                 std::string_view(row_to_insert.data.data(),
-                                                  row_to_insert.data.size()));
+class ZstdRowWriter {
+   public:
+    ZstdRowWriter(const std::string& path, ZSTD_CCtx* ctx)
+        : fname(path),
+          fstream(path, std::ifstream::out | std::ifstream::binary),
+          context(ctx) {}
 
-            if (uncompressed_data.size() > SNAPPY_BUFFER_SIZE) {
-                flush_compressed();
-            }
-        }
+    void add_next(std::string_view data) {
+        add_string_to_vector(uncompressed_buffer,
+                             std::string_view(data.data(), data.size()));
 
-        if (uncompressed_data.size() > 0) {
+        if (uncompressed_buffer.size() > COMPRESSION_BUFFER_SIZE) {
             flush_compressed();
         }
-
-        rows.clear();
-        row_indices.clear();
-
-        current_size = 0;
-    };
-
-    dequeue_many_loop(write_queues, [&](Row& r) {
-        current_size += sizeof(size_t) + r.data.size();
-
-        rows.emplace_back(std::move(r));
-        row_indices.emplace_back(
-            std::make_tuple(r.patient_id, r.time, row_indices.size()));
-
-        if (current_size > SHARD_PIECE_SIZE) {
-            flush_file();
-        }
-    });
-
-    if (current_size > 0) {
-        flush_file();
-    }
-}
-
-const int QUEUE_SIZE = 1000;
-
-std::vector<std::string> sort_and_shard(
-    const std::filesystem::path& source_directory,
-    const std::filesystem::path& target_directory, size_t num_shards) {
-    std::filesystem::create_directory(target_directory);
-
-    std::vector<std::string> paths;
-
-    for (const auto& entry : fs::directory_iterator(source_directory)) {
-        paths.push_back(entry.path());
     }
 
-    auto set_metadata_fields =
-        get_metadata_fields_multithreaded(paths, num_shards);
-
-    std::vector<std::string> metadata_columns(std::begin(set_metadata_fields),
-                                              std::end(set_metadata_fields));
-
-    if (metadata_columns.size() + 3 >
-        std::numeric_limits<unsigned long long>::digits) {
-        throw std::runtime_error(
-            "C++ MEDS-ETL currently only supports at most " +
-            std::to_string(std::numeric_limits<unsigned long long>::digits) +
-            " metadata columns");
+    ~ZstdRowWriter() {
+        if (uncompressed_buffer.size() > 0) {
+            flush_compressed();
+        }
     }
 
-    moodycamel::BlockingConcurrentQueue<absl::optional<std::string>> file_queue;
+    const std::string fname;
 
-    for (const auto& path : paths) {
-        file_queue.enqueue(path);
-    }
+   private:
+    void flush_compressed() {
+        size_t needed_size = ZSTD_compressBound(uncompressed_buffer.size());
 
-    for (size_t i = 0; i < num_shards; i++) {
-        file_queue.enqueue({});
-    }
+        if (compressed_buffer.size() < needed_size) {
+            compressed_buffer.resize(needed_size * 2);
+        }
 
-    std::vector<
-        std::vector<moodycamel::BlockingReaderWriterCircularBuffer<QueueItem>>>
-        write_queues(num_shards);
+        size_t compressed_length = ZSTD_compressCCtx(
+            context, compressed_buffer.data(), compressed_buffer.size(),
+            uncompressed_buffer.data(), uncompressed_buffer.size(), 1);
 
-    for (size_t i = 0; i < num_shards; i++) {
-        for (size_t j = 0; j < num_shards; j++) {
-            write_queues[i].emplace_back(QUEUE_SIZE);
+        if (ZSTD_isError(compressed_length)) {
+            throw std::runtime_error("Could not compress using zstd?");
         }
-    }
 
-    std::vector<std::thread> threads;
-
-    for (size_t i = 0; i < num_shards; i++) {
-        threads.emplace_back(
-            [i, &file_queue, &write_queues, num_shards, &metadata_columns]() {
-                sort_reader(i, num_shards, file_queue, write_queues,
-                            metadata_columns);
-            });
+        fstream.write(reinterpret_cast<char*>(&compressed_length),
+                      sizeof(compressed_length));
+        fstream.write(compressed_buffer.data(), compressed_length);
 
-        threads.emplace_back(
-            [i, &write_queues, num_shards, target_directory]() {
-                sort_writer(i, num_shards, write_queues[i],
-                            target_directory / std::to_string(i));
-            });
+        uncompressed_buffer.clear();
     }
 
-    for (auto& thread : threads) {
-        thread.join();
-    }
+    std::ofstream fstream;
 
-    return metadata_columns;
-}
+    ZSTD_CCtx* context;
+
+    std::vector<char> compressed_buffer;
+    std::vector<char> uncompressed_buffer;
+};
 
-class SnappyRowReader {
+class ZstdRowReader {
    public:
-    SnappyRowReader(const std::string& path)
+    ZstdRowReader(const std::string& path, ZSTD_DCtx* ctx)
         : fname(path),
           fstream(path, std::ifstream::in | std::ifstream::binary),
+          context(ctx),
           current_offset(0),
           uncompressed_size(0) {}
 
     absl::optional<std::tuple<int64_t, int64_t, std::string_view>> get_next() {
         if (current_offset == uncompressed_size) {
             bool could_load_more = try_to_load_more_data();
 
@@ -710,51 +650,332 @@
 
         if (compressed_buffer.size() < size) {
             compressed_buffer.resize(size * 2);
         }
 
         fstream.read(compressed_buffer.data(), size);
 
-        bool is_valid = snappy::GetUncompressedLength(compressed_buffer.data(),
-                                                      size, &uncompressed_size);
-        if (!is_valid) {
+        uncompressed_size =
+            ZSTD_getFrameContentSize(compressed_buffer.data(), size);
+
+        if (uncompressed_size == ZSTD_CONTENTSIZE_ERROR ||
+            uncompressed_size == ZSTD_CONTENTSIZE_UNKNOWN) {
             throw std::runtime_error(
-                "Could not get size of compressed snappy data?");
+                "Could not get the size of the zstd compressed stream?");
         }
 
         if (uncompressed_buffer.size() < uncompressed_size) {
             uncompressed_buffer.resize(uncompressed_size * 2);
         }
 
-        is_valid = snappy::RawUncompress(compressed_buffer.data(), size,
-                                         uncompressed_buffer.data());
-        if (!is_valid) {
-            throw std::runtime_error("Could not decompress snappy data?");
+        size_t read_size = ZSTD_decompressDCtx(
+            context, uncompressed_buffer.data(), uncompressed_size,
+            compressed_buffer.data(), size);
+
+        if (ZSTD_isError(read_size) || read_size != uncompressed_size) {
+            throw std::runtime_error("Could not decompress zstd data?");
         }
 
         current_offset = 0;
         return true;
     }
 
-    std::string fname;
+    const std::string fname;
     std::ifstream fstream;
 
+    ZSTD_DCtx* context;
+
     std::vector<char> compressed_buffer;
     std::vector<char> uncompressed_buffer;
     size_t current_offset;
     size_t uncompressed_size;
 };
 
-void join_and_write_single(const std::filesystem::path& source_directory,
-                           const std::filesystem::path& target_path,
-                           const std::vector<std::string>& metadata_columns) {
+void shard_writer(
+    size_t writer_index, size_t num_shards,
+    moodycamel::BlockingConcurrentQueue<QueueItem>& write_queue,
+    moodycamel::LightweightSemaphore& write_semaphore,
+    const std::filesystem::path& target_dir,
+    moodycamel::BlockingConcurrentQueue<std::string>& sort_file_queue,
+    std::atomic<ssize_t>& remaining_live_writers) {
+    std::filesystem::create_directory(target_dir);
+
+    size_t current_size = 0;
+
+    size_t current_file_index = 0;
+
+    auto context_deleter = [](ZSTD_CCtx* context) { ZSTD_freeCCtx(context); };
+
+    std::unique_ptr<ZSTD_CCtx, decltype(context_deleter)> context{
+        ZSTD_createCCtx(), context_deleter};
+
+    std::optional<ZstdRowWriter> current_writer;
+
+    auto init_file = [&]() {
+        auto target_file = target_dir / std::to_string(current_file_index);
+        current_writer.emplace(target_file, context.get());
+    };
+
+    auto flush_file = [&]() {
+        std::string target_file = current_writer->fname;
+        current_writer.reset();
+
+        sort_file_queue.enqueue(target_file);
+
+        current_size = 0;
+        current_file_index += 1;
+    };
+
+    QueueItem item;
+    size_t readers_remaining = num_shards;
+
+    moodycamel::ConsumerToken ctok(write_queue);
+
+    size_t num_read = 0;
+
+    while (true) {
+        write_queue.wait_dequeue(ctok, item);
+
+        if (!item) {
+            readers_remaining--;
+            if (readers_remaining == 0) {
+                break;
+            } else {
+                continue;
+            }
+        }
+
+        num_read++;
+        if (num_read == SEMAPHORE_BLOCK_SIZE) {
+            write_semaphore.signal(num_read);
+            num_read = 0;
+        }
+
+        std::vector<char>& r = *item;
+
+        if (!current_writer) {
+            init_file();
+        }
+
+        current_writer->add_next(std::string_view(r.data(), r.size()));
+
+        current_size += sizeof(size_t) + r.size();
+
+        if (current_size > SHARD_PIECE_SIZE) {
+            flush_file();
+        }
+    }
+
+    write_semaphore.signal(num_read);
+
+    if (current_writer) {
+        flush_file();
+    }
+
+    remaining_live_writers.fetch_sub(1, std::memory_order_release);
+}
+
+void shard_sort(
+    moodycamel::BlockingConcurrentQueue<std::string>& sort_file_queue,
+    const std::atomic<ssize_t>& remaining_live_writers) {
+    absl::optional<std::string> next_entry;
+
+    std::vector<char> data;
+    std::vector<std::tuple<int64_t, int64_t, size_t, size_t>> row_indices;
+
+    auto compression_context_deleter = [](ZSTD_CCtx* context) {
+        ZSTD_freeCCtx(context);
+    };
+    auto decompression_context_deleter = [](ZSTD_DCtx* context) {
+        ZSTD_freeDCtx(context);
+    };
+
+    std::unique_ptr<ZSTD_CCtx, decltype(compression_context_deleter)>
+        compression_context{ZSTD_createCCtx(), compression_context_deleter};
+
+    std::unique_ptr<ZSTD_DCtx, decltype(decompression_context_deleter)>
+        decompression_context{ZSTD_createDCtx(), decompression_context_deleter};
+
+    std::string filename;
+    while (true) {
+        while (true) {
+            bool found = sort_file_queue.wait_dequeue_timed(filename, 1e6);
+            if (found) {
+                break;
+            }
+
+            // No items are available. This could be due to being fully done.
+
+            // Check if we are done
+            if (remaining_live_writers.load(std::memory_order_acquire) == 0) {
+                return;
+            }
+
+            // Need to wait more
+        }
+
+        data.clear();
+        row_indices.clear();
+
+        {
+            ZstdRowReader reader(filename, decompression_context.get());
+
+            while (true) {
+                auto next = reader.get_next();
+
+                if (!next) {
+                    break;
+                }
+
+                size_t start = data.size();
+                size_t length = std::get<2>(*next).size();
+
+                data.insert(std::end(data), std::begin(std::get<2>(*next)),
+                            std::end(std::get<2>(*next)));
+                row_indices.push_back(std::make_tuple(
+                    std::get<0>(*next), std::get<1>(*next), start, length));
+            }
+        }
+
+        std::sort(std::begin(row_indices), std::end(row_indices));
+
+        {
+            ZstdRowWriter writer(filename, compression_context.get());
+
+            for (const auto& row_index : row_indices) {
+                writer.add_next(
+                    std::string_view(data.data() + std::get<2>(row_index),
+                                     std::get<3>(row_index)));
+            }
+        }
+    }
+}
+
+constexpr int QUEUE_SIZE = 10000;
+
+std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>
+sort_and_shard(const std::filesystem::path& source_directory,
+               const std::filesystem::path& target_directory,
+               size_t num_shards) {
+    std::filesystem::create_directory(target_directory);
+
+    std::vector<std::string> paths;
+
+    for (const auto& entry : fs::directory_iterator(source_directory)) {
+        paths.push_back(entry.path());
+    }
+
+    auto set_metadata_fields =
+        get_metadata_fields_multithreaded(paths, num_shards);
+
+    std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>
+        metadata_columns(std::begin(set_metadata_fields),
+                         std::end(set_metadata_fields));
+    std::sort(std::begin(metadata_columns), std::end(metadata_columns));
+
+    metadata_columns.erase(
+        std::unique(std::begin(metadata_columns), std::end(metadata_columns),
+                    [](const auto& a, const auto& b) {
+                        return (a.first == b.first) &&
+                               a.second->Equals(b.second);
+                    }),
+        std::end(metadata_columns));
+
+    for (ssize_t i = 0; i < static_cast<ssize_t>(metadata_columns.size()) - 1;
+         i++) {
+        if (metadata_columns[i].first == metadata_columns[i + 1].first) {
+            throw std::runtime_error(
+                "Got conflicting types for column " +
+                metadata_columns[i].first +
+                ", types: " + metadata_columns[i].second->ToString() + " vs " +
+                metadata_columns[i + 1].second->ToString());
+        }
+    }
+
+    if (metadata_columns.size() + 3 >
+        std::numeric_limits<unsigned long long>::digits) {
+        throw std::runtime_error(
+            "C++ MEDS-ETL currently only supports at most " +
+            std::to_string(std::numeric_limits<unsigned long long>::digits) +
+            " metadata columns");
+    }
+
+    moodycamel::BlockingConcurrentQueue<absl::optional<std::string>> file_queue;
+
+    for (const auto& path : paths) {
+        file_queue.enqueue(path);
+    }
+
+    for (size_t i = 0; i < num_shards; i++) {
+        file_queue.enqueue({});
+    }
+
+    std::vector<moodycamel::BlockingConcurrentQueue<QueueItem>> write_queues(
+        num_shards);
+
+    std::vector<std::thread> threads;
+
+    moodycamel::LightweightSemaphore write_semaphore(QUEUE_SIZE * num_shards);
+
+    moodycamel::BlockingConcurrentQueue<std::string> sort_queue;
+    std::atomic<ssize_t> remaining_live_writers(num_shards);
+
+    for (size_t i = 0; i < num_shards; i++) {
+        threads.emplace_back([i, &file_queue, &write_queues, &write_semaphore,
+                              num_shards, &metadata_columns]() {
+            shard_reader(i, num_shards, file_queue, write_queues,
+                         write_semaphore, metadata_columns);
+        });
+
+        threads.emplace_back([i, &write_queues, &write_semaphore, num_shards,
+                              target_directory, &sort_queue,
+                              &remaining_live_writers]() {
+            shard_writer(i, num_shards, write_queues[i], write_semaphore,
+                         target_directory / std::to_string(i), sort_queue,
+                         remaining_live_writers);
+        });
+
+        threads.emplace_back([&sort_queue, &remaining_live_writers]() {
+            shard_sort(sort_queue, remaining_live_writers);
+        });
+    }
+
+    for (auto& thread : threads) {
+        thread.join();
+    }
+
+    absl::optional<std::string> next_entry;
+    if (sort_queue.try_dequeue(next_entry)) {
+        // This should not be possible
+        throw std::runtime_error(
+            "Had excess unsorted items. This should not be possible");
+    }
+
+    return metadata_columns;
+}
+
+void join_and_write_single(
+    const std::filesystem::path& source_directory,
+    const std::filesystem::path& target_path,
+    const std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>&
+        metadata_columns) {
     arrow::FieldVector metadata_fields;
-    for (const auto& metadata_column : metadata_columns) {
-        metadata_fields.push_back(arrow::field(
-            metadata_column, std::make_shared<arrow::StringType>()));
+    std::bitset<std::numeric_limits<unsigned long long>::digits>
+        is_text_metadata;
+    for (size_t i = 0; i < metadata_columns.size(); i++) {
+        const auto& metadata_column = metadata_columns[i];
+        if (metadata_column.second->Equals(arrow::LargeStringType())) {
+            is_text_metadata[i] = true;
+            metadata_fields.push_back(arrow::field(
+                metadata_column.first, std::make_shared<arrow::StringType>()));
+        } else {
+            is_text_metadata[i] = false;
+            metadata_fields.push_back(
+                arrow::field(metadata_column.first, metadata_column.second));
+        }
     }
 
     auto metadata_type = std::make_shared<arrow::StructType>(metadata_fields);
 
     auto timestamp_type =
         std::make_shared<arrow::TimestampType>(arrow::TimeUnit::MICRO);
 
@@ -774,20 +995,21 @@
     auto event_type_fields = {
         arrow::field("time", std::make_shared<arrow::TimestampType>(
                                  arrow::TimeUnit::MICRO)),
         arrow::field("measurements",
                      std::make_shared<arrow::ListType>(measurement_type)),
     };
     auto event_type = std::make_shared<arrow::StructType>(event_type_fields);
+    auto events_type = std::make_shared<arrow::ListType>(event_type);
 
     auto schema_fields = {
         arrow::field("patient_id", std::make_shared<arrow::Int64Type>()),
         arrow::field("static_measurements",
                      std::make_shared<arrow::NullType>()),
-        arrow::field("events", std::make_shared<arrow::ListType>(event_type)),
+        arrow::field("events", events_type),
     };
     auto schema = std::make_shared<arrow::Schema>(schema_fields);
 
     using parquet::ArrowWriterProperties;
     using parquet::WriterProperties;
 
     size_t amount_written = 0;
@@ -809,21 +1031,30 @@
     PARQUET_ASSIGN_OR_THROW(
         outfile, arrow::io::FileOutputStream::Open(target_path.string()));
     std::unique_ptr<parquet::arrow::FileWriter> writer;
     PARQUET_ASSIGN_OR_THROW(
         writer, parquet::arrow::FileWriter::Open(*schema, pool, outfile, props,
                                                  arrow_props));
 
-    std::vector<SnappyRowReader> source_files;
+    std::vector<ZstdRowReader> source_files;
+
+    auto context_deleter = [](ZSTD_DCtx* context) { ZSTD_freeDCtx(context); };
+
+    std::unique_ptr<ZSTD_DCtx, decltype(context_deleter)> context{
+        ZSTD_createDCtx(), context_deleter};
 
     for (const auto& entry : fs::directory_iterator(source_directory)) {
-        source_files.emplace_back(entry.path());
+        source_files.emplace_back(entry.path(), context.get());
     }
 
-    std::priority_queue<std::tuple<int64_t, int64_t, size_t, std::string_view>>
+    typedef std::tuple<int64_t, int64_t, size_t, std::string_view>
+        PriorityQueueItem;
+
+    std::priority_queue<PriorityQueueItem, std::vector<PriorityQueueItem>,
+                        std::greater<PriorityQueueItem>>
         queue;
 
     for (size_t i = 0; i < source_files.size(); i++) {
         auto next_entry = source_files[i].get_next();
         if (!next_entry) {
             continue;
         }
@@ -840,24 +1071,36 @@
     auto code_builder = std::make_shared<arrow::StringBuilder>(pool);
 
     auto text_value_builder = std::make_shared<arrow::StringBuilder>(pool);
     auto numeric_value_builder = std::make_shared<arrow::FloatBuilder>(pool);
     auto datetime_value_builder =
         std::make_shared<arrow::TimestampBuilder>(timestamp_type, pool);
 
-    std::vector<std::shared_ptr<arrow::StringBuilder>> metadata_builders;
-    std::vector<std::shared_ptr<arrow::ArrayBuilder>> metadata_builders_generic;
+    std::vector<std::shared_ptr<arrow::StringBuilder>> text_metadata_builders(
+        metadata_columns.size());
+    std::vector<std::shared_ptr<arrow::FixedSizeBinaryBuilder>>
+        primitive_metadata_builders(metadata_columns.size());
+    std::vector<std::shared_ptr<arrow::ArrayBuilder>> metadata_builders(
+        metadata_columns.size());
     for (size_t i = 0; i < metadata_columns.size(); i++) {
-        auto builder = std::make_shared<arrow::StringBuilder>(pool);
-        metadata_builders.push_back(builder);
-        metadata_builders_generic.push_back(builder);
+        if (is_text_metadata[i]) {
+            auto builder = std::make_shared<arrow::StringBuilder>(pool);
+            text_metadata_builders[i] = builder;
+            metadata_builders[i] = builder;
+        } else {
+            auto builder = std::make_shared<arrow::FixedSizeBinaryBuilder>(
+                std::make_shared<arrow::FixedSizeBinaryType>(
+                    metadata_columns[i].second->byte_width()));
+            primitive_metadata_builders[i] = builder;
+            metadata_builders[i] = builder;
+        }
     }
 
     auto metadata_builder = std::make_shared<arrow::StructBuilder>(
-        metadata_type, pool, metadata_builders_generic);
+        metadata_type, pool, metadata_builders);
 
     std::vector<std::shared_ptr<arrow::ArrayBuilder>>
         measurement_builder_fields{code_builder, text_value_builder,
                                    numeric_value_builder,
                                    datetime_value_builder, metadata_builder};
     auto measurement_builder = std::make_shared<arrow::StructBuilder>(
         measurement_type, pool, measurement_builder_fields);
@@ -876,15 +1119,18 @@
         std::make_shared<arrow::ListBuilder>(pool, event_builder);
 
     auto flush_arrays = [&]() {
         std::vector<std::shared_ptr<arrow::Array>> columns(3);
         PARQUET_THROW_NOT_OK(patient_id_builder->Finish(columns.data() + 0));
         PARQUET_THROW_NOT_OK(
             static_measurements_builder->Finish(columns.data() + 1));
-        PARQUET_THROW_NOT_OK(events_builder->Finish(columns.data() + 2));
+
+        std::shared_ptr<arrow::Array> events_array;
+        PARQUET_THROW_NOT_OK(events_builder->Finish(&events_array));
+        PARQUET_ASSIGN_OR_THROW(columns[2], events_array->View(events_type));
 
         std::shared_ptr<arrow::Table> table =
             arrow::Table::Make(schema, columns);
         PARQUET_THROW_NOT_OK(writer->WriteTable(*table));
 
         amount_written = 0;
     };
@@ -972,19 +1218,32 @@
 
         PARQUET_THROW_NOT_OK(metadata_builder->Append());
         for (size_t j = 0; j < metadata_columns.size(); j++) {
             if (non_null[3 + j]) {
                 size_t size = *reinterpret_cast<const size_t*>(
                     patient_record.substr(offset).data());
                 offset += sizeof(size);
-                PARQUET_THROW_NOT_OK(metadata_builders[j]->Append(
-                    patient_record.substr(offset, size)));
+                auto entry = patient_record.substr(offset, size);
+
+                if (is_text_metadata[j]) {
+                    PARQUET_THROW_NOT_OK(
+                        text_metadata_builders[j]->Append(entry));
+                } else {
+                    PARQUET_THROW_NOT_OK(
+                        primitive_metadata_builders[j]->Append(entry));
+                }
                 offset += size;
             } else {
-                PARQUET_THROW_NOT_OK(metadata_builders[j]->AppendNull());
+                if (is_text_metadata[j]) {
+                    PARQUET_THROW_NOT_OK(
+                        text_metadata_builders[j]->AppendNull());
+                } else {
+                    PARQUET_THROW_NOT_OK(
+                        primitive_metadata_builders[j]->AppendNull());
+                }
             }
         }
 
         size_t file_index = std::get<2>(next);
         auto next_entry = source_files[file_index].get_next();
         if (!next_entry) {
             continue;
@@ -997,17 +1256,19 @@
 
     flush_arrays();
 
     // Write file footer and close
     PARQUET_THROW_NOT_OK(writer->Close());
 }
 
-void join_and_write(const std::filesystem::path& source_directory,
-                    const std::filesystem::path& target_directory,
-                    const std::vector<std::string>& metadata_columns) {
+void join_and_write(
+    const std::filesystem::path& source_directory,
+    const std::filesystem::path& target_directory,
+    const std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>&
+        metadata_columns) {
     std::filesystem::create_directory(target_directory);
 
     std::vector<std::string> shards;
 
     for (const auto& entry : fs::directory_iterator(source_directory)) {
         shards.push_back(fs::relative(entry.path(), source_directory));
     }
@@ -1044,8 +1305,8 @@
     std::filesystem::path data_path = target_path / "data";
 
     auto metadata_columns =
         sort_and_shard(source_path / "flat_data", shard_path, num_shards);
     join_and_write(shard_path, data_path, metadata_columns);
 
     fs::remove_all(shard_path);
-}
+}
```

### Comparing `meds_etl_cpp-0.1.0/pyproject.toml` & `meds_etl_cpp-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.0/setup.py` & `meds_etl_cpp-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,14 @@
 
             bazel_extra_args: List[str] = []
             extra_args: List[str] = []
 
             if source_env.get("DISTDIR"):
                 extra_args.extend(["--distdir", source_env["DISTDIR"]])
 
-            if has_nvcc():
-                extra_args.extend(["--//:cuda=enabled"])
-
             if source_env.get("MACOSX_DEPLOYMENT_TARGET"):
                 extra_args.extend(["--macos_minimum_os", source_env["MACOSX_DEPLOYMENT_TARGET"]])
 
             if source_env.get("DISABLE_CPU_ARCH") or not can_build_simple(
                 sourcedir=ext.sourcedir, env=env, bazel_extra_args=bazel_extra_args
             ):
                 bazel_extra_args.extend(["--noworkspace_rc", "--bazelrc=backupbazelrc"])
```

