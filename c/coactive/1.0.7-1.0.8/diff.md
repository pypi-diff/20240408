# Comparing `tmp/coactive-1.0.7.tar.gz` & `tmp/coactive-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coactive-1.0.7.tar", max compression
+gzip compressed data, was "coactive-1.0.8.tar", max compression
```

## Comparing `coactive-1.0.7.tar` & `coactive-1.0.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     4126 2024-03-01 21:33:44.141688 coactive-1.0.7/README.md
--rw-r--r--   0        0        0      402 2024-03-01 21:33:44.141688 coactive-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2782 2024-03-01 21:33:44.141688 coactive-1.0.7/src/coactive/__init__.py
--rw-r--r--   0        0        0     3229 2024-03-01 21:33:44.141688 coactive-1.0.7/src/coactive/client.py
--rw-r--r--   0        0        0      519 2024-03-01 21:33:44.141688 coactive-1.0.7/src/coactive/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-01 21:33:44.141688 coactive-1.0.7/src/coactive/core/api_error.py
--rw-r--r--   0        0        0     1382 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      157 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/environment.py
--rw-r--r--   0        0        0      296 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/errors/__init__.py
--rw-r--r--   0        0        0      285 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/errors/not_found_error.py
--rw-r--r--   0        0        0      313 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/py.typed
--rw-r--r--   0        0        0      308 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/__init__.py
--rw-r--r--   0        0        0      143 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/asset/__init__.py
--rw-r--r--   0        0        0     9326 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/asset/client.py
--rw-r--r--   0        0        0      162 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/asset/types/__init__.py
--rw-r--r--   0        0        0      209 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/asset/types/image_or_keyframe_detail.py
--rw-r--r--   0        0        0       65 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/classification/__init__.py
--rw-r--r--   0        0        0     5995 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/classification/client.py
--rw-r--r--   0        0        0       65 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/concept/__init__.py
--rw-r--r--   0        0        0    31983 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/concept/client.py
--rw-r--r--   0        0        0       65 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/credentials/__init__.py
--rw-r--r--   0        0        0    10437 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/credentials/client.py
--rw-r--r--   0        0        0       65 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/dataset/__init__.py
--rw-r--r--   0        0        0    37754 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/dataset/client.py
--rw-r--r--   0        0        0       65 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/query/__init__.py
--rw-r--r--   0        0        0    20726 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/query/client.py
--rw-r--r--   0        0        0       65 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/search/__init__.py
--rw-r--r--   0        0        0    10133 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/resources/search/client.py
--rw-r--r--   0        0        0     3554 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/__init__.py
--rw-r--r--   0        0        0     1408 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/add_assets_confirmation.py
--rw-r--r--   0        0        0     1220 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/add_image_request.py
--rw-r--r--   0        0        0     1129 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/add_video_request.py
--rw-r--r--   0        0        0     2096 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/added_image.py
--rw-r--r--   0        0        0     2027 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/added_video.py
--rw-r--r--   0        0        0     1419 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/audio_segment.py
--rw-r--r--   0        0        0     1156 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/candidates_to_label.py
--rw-r--r--   0        0        0     1131 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/classification.py
--rw-r--r--   0        0        0     1454 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/classification_score.py
--rw-r--r--   0        0        0     1968 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/concept.py
--rw-r--r--   0        0        0     1572 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/concept_label.py
--rw-r--r--   0        0        0      534 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/concept_label_enum.py
--rw-r--r--   0        0        0     1659 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/concept_label_request.py
--rw-r--r--   0        0        0     1237 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/credentials.py
--rw-r--r--   0        0        0     1537 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/credentials_validation.py
--rw-r--r--   0        0        0     2305 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/dataset.py
--rw-r--r--   0        0        0     1888 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/dataset_status_enum.py
--rw-r--r--   0        0        0      998 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/error_response.py
--rw-r--r--   0        0        0      966 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/http_validation_error.py
--rw-r--r--   0        0        0     1819 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/image.py
--rw-r--r--   0        0        0      185 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/image_or_keyframe.py
--rw-r--r--   0        0        0      194 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/image_or_keyframe_candidate.py
--rw-r--r--   0        0        0      471 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/key_type_enum.py
--rw-r--r--   0        0        0     1627 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/keyframe.py
--rw-r--r--   0        0        0     1185 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_concept_labels.py
--rw-r--r--   0        0        0     1174 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_concepts.py
--rw-r--r--   0        0        0     1170 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_datasets.py
--rw-r--r--   0        0        0     1173 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_images.py
--rw-r--r--   0        0        0     1251 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_links_response.py
--rw-r--r--   0        0        0     1429 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_meta_response.py
--rw-r--r--   0        0        0     1438 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_page_details_response.py
--rw-r--r--   0        0        0     1163 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_queries.py
--rw-r--r--   0        0        0     1173 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/paged_videos.py
--rw-r--r--   0        0        0     2255 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/query.py
--rw-r--r--   0        0        0     1327 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/query_result.py
--rw-r--r--   0        0        0     1131 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/query_results_download_url.py
--rw-r--r--   0        0        0     1033 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/query_row.py
--rw-r--r--   0        0        0     1139 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/query_status_enum.py
--rw-r--r--   0        0        0     2400 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/query_with_result.py
--rw-r--r--   0        0        0     1200 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/search_result.py
--rw-r--r--   0        0        0     1326 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/shot.py
--rw-r--r--   0        0        0      528 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/sort_direction_enum.py
--rw-r--r--   0        0        0     1119 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/sort_item.py
--rw-r--r--   0        0        0      724 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/storage_type_enum.py
--rw-r--r--   0        0        0     1353 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/update_assets_metadata_confirmation.py
--rw-r--r--   0        0        0     1383 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/update_image_metadata_request.py
--rw-r--r--   0        0        0     1382 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/update_video_metadata_request.py
--rw-r--r--   0        0        0     2096 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/updated_image.py
--rw-r--r--   0        0        0     2028 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/updated_video.py
--rw-r--r--   0        0        0      992 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1750 2024-03-01 21:33:44.145688 coactive-1.0.7/src/coactive/types/video.py
--rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 coactive-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     4126 2024-04-08 18:42:18.773704 coactive-1.0.8/README.md
+-rw-r--r--   0        0        0      402 2024-04-08 18:42:18.777704 coactive-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2782 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/__init__.py
+-rw-r--r--   0        0        0     3229 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/client.py
+-rw-r--r--   0        0        0      519 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/api_error.py
+-rw-r--r--   0        0        0     1382 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      157 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/environment.py
+-rw-r--r--   0        0        0      296 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/errors/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/errors/not_found_error.py
+-rw-r--r--   0        0        0      313 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/py.typed
+-rw-r--r--   0        0        0      308 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/asset/__init__.py
+-rw-r--r--   0        0        0     9326 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/asset/client.py
+-rw-r--r--   0        0        0      162 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/asset/types/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/asset/types/image_or_keyframe_detail.py
+-rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/classification/__init__.py
+-rw-r--r--   0        0        0     5995 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/classification/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/concept/__init__.py
+-rw-r--r--   0        0        0    31777 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/concept/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/credentials/__init__.py
+-rw-r--r--   0        0        0    10437 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/credentials/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/dataset/__init__.py
+-rw-r--r--   0        0        0    38568 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/dataset/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/query/__init__.py
+-rw-r--r--   0        0        0    20726 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/search/__init__.py
+-rw-r--r--   0        0        0    10133 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/search/client.py
+-rw-r--r--   0        0        0     3554 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/__init__.py
+-rw-r--r--   0        0        0     1408 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/add_assets_confirmation.py
+-rw-r--r--   0        0        0     1220 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/add_image_request.py
+-rw-r--r--   0        0        0     1129 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/add_video_request.py
+-rw-r--r--   0        0        0     2096 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/added_image.py
+-rw-r--r--   0        0        0     2027 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/added_video.py
+-rw-r--r--   0        0        0     1419 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/audio_segment.py
+-rw-r--r--   0        0        0     1156 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/candidates_to_label.py
+-rw-r--r--   0        0        0     1131 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/classification.py
+-rw-r--r--   0        0        0     1454 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/classification_score.py
+-rw-r--r--   0        0        0     1968 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/concept.py
+-rw-r--r--   0        0        0     1572 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/concept_label.py
+-rw-r--r--   0        0        0      534 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/concept_label_enum.py
+-rw-r--r--   0        0        0     1659 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/concept_label_request.py
+-rw-r--r--   0        0        0     1237 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/credentials.py
+-rw-r--r--   0        0        0     1537 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/credentials_validation.py
+-rw-r--r--   0        0        0     2305 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/dataset.py
+-rw-r--r--   0        0        0     1888 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/dataset_status_enum.py
+-rw-r--r--   0        0        0      998 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/error_response.py
+-rw-r--r--   0        0        0      966 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/http_validation_error.py
+-rw-r--r--   0        0        0     1819 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/image.py
+-rw-r--r--   0        0        0      185 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/image_or_keyframe.py
+-rw-r--r--   0        0        0      194 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/image_or_keyframe_candidate.py
+-rw-r--r--   0        0        0      471 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/key_type_enum.py
+-rw-r--r--   0        0        0     1627 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/keyframe.py
+-rw-r--r--   0        0        0     1185 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_concept_labels.py
+-rw-r--r--   0        0        0     1174 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_concepts.py
+-rw-r--r--   0        0        0     1170 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_datasets.py
+-rw-r--r--   0        0        0     1173 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_images.py
+-rw-r--r--   0        0        0     1251 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_links_response.py
+-rw-r--r--   0        0        0     1429 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_meta_response.py
+-rw-r--r--   0        0        0     1438 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_page_details_response.py
+-rw-r--r--   0        0        0     1163 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_queries.py
+-rw-r--r--   0        0        0     1173 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_videos.py
+-rw-r--r--   0        0        0     2255 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query.py
+-rw-r--r--   0        0        0     1327 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_result.py
+-rw-r--r--   0        0        0     1131 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_results_download_url.py
+-rw-r--r--   0        0        0     1033 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_row.py
+-rw-r--r--   0        0        0     1139 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_status_enum.py
+-rw-r--r--   0        0        0     2400 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_with_result.py
+-rw-r--r--   0        0        0     1200 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/search_result.py
+-rw-r--r--   0        0        0     1326 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/shot.py
+-rw-r--r--   0        0        0      528 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/sort_direction_enum.py
+-rw-r--r--   0        0        0     1119 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/sort_item.py
+-rw-r--r--   0        0        0      724 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/storage_type_enum.py
+-rw-r--r--   0        0        0     1353 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/update_assets_metadata_confirmation.py
+-rw-r--r--   0        0        0     1383 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/update_image_metadata_request.py
+-rw-r--r--   0        0        0     1382 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/update_video_metadata_request.py
+-rw-r--r--   0        0        0     2096 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/updated_image.py
+-rw-r--r--   0        0        0     2028 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/updated_video.py
+-rw-r--r--   0        0        0      992 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1750 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/video.py
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 coactive-1.0.8/PKG-INFO
```

### Comparing `coactive-1.0.7/README.md` & `coactive-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/__init__.py` & `coactive-1.0.8/src/coactive/__init__.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/client.py` & `coactive-1.0.8/src/coactive/client.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/core/__init__.py` & `coactive-1.0.8/src/coactive/core/__init__.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/core/client_wrapper.py` & `coactive-1.0.8/src/coactive/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._token = token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "coactive",
-            "X-Fern-SDK-Version": "1.0.7",
+            "X-Fern-SDK-Version": "1.0.8",
         }
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
         if isinstance(self._token, str):
             return self._token
```

### Comparing `coactive-1.0.7/src/coactive/core/datetime_utils.py` & `coactive-1.0.8/src/coactive/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/core/jsonable_encoder.py` & `coactive-1.0.8/src/coactive/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/resources/asset/client.py` & `coactive-1.0.8/src/coactive/resources/asset/client.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/resources/classification/client.py` & `coactive-1.0.8/src/coactive/resources/classification/client.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/resources/concept/client.py` & `coactive-1.0.8/src/coactive/resources/concept/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,23 +276,21 @@
 
             - offset: typing.Optional[int]. Starting index to return
 
             - limit: typing.Optional[int]. Max number of items to return
 
             - labels_to_include: typing.Optional[typing.Union[ConceptLabelEnum, typing.List[ConceptLabelEnum]]]. List of labels types to include, leave blank to return all
         ---
-        from coactive import ConceptLabelEnum
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.concept.get_labels(
             concept_id="string",
-            labels_to_include=ConceptLabelEnum.POSITIVE,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}/labels"),
             params=remove_none_from_dict({"offset": offset, "limit": limit, "labels_to_include": labels_to_include}),
             headers=self._client_wrapper.get_headers(),
@@ -637,23 +635,21 @@
 
             - offset: typing.Optional[int]. Starting index to return
 
             - limit: typing.Optional[int]. Max number of items to return
 
             - labels_to_include: typing.Optional[typing.Union[ConceptLabelEnum, typing.List[ConceptLabelEnum]]]. List of labels types to include, leave blank to return all
         ---
-        from coactive import ConceptLabelEnum
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.concept.get_labels(
             concept_id="string",
-            labels_to_include=ConceptLabelEnum.POSITIVE,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}/labels"),
             params=remove_none_from_dict({"offset": offset, "limit": limit, "labels_to_include": labels_to_include}),
             headers=self._client_wrapper.get_headers(),
```

### Comparing `coactive-1.0.7/src/coactive/resources/credentials/client.py` & `coactive-1.0.8/src/coactive/resources/credentials/client.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/resources/dataset/client.py` & `coactive-1.0.8/src/coactive/resources/dataset/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,19 +353,26 @@
         )
         client.dataset.add_assets(
             dataset_id="string",
             images=[
                 AddImageRequest(
                     path="s3://coactive-public/logo.png",
                     id="kingslanding_041711",
+                    metadata={"artist": "Marc Simonetti"},
                 )
             ],
             videos=[
                 AddVideoRequest(
                     path="s3://your-s3-bucket/path/to/video.mp4",
+                    metadata={
+                        "show": "The Boys",
+                        "season": 1,
+                        "episode": 1,
+                        "title": "The Name of the Game",
+                    },
                 )
             ],
             data_path="s3://your-s3-bucket/path/prefix",
             csv_path="path/to/file.csv",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
@@ -421,20 +428,22 @@
         )
         client.dataset.update_asset_metadata(
             dataset_id="string",
             images=[
                 UpdateImageMetadataRequest(
                     path="s3://coactive-public/logo.png",
                     coactive_image_id="a6894d72-612d-4c20-b4d0-8f3f21c2bb10",
+                    metadata={"artist": "Marc Simonetti"},
                 )
             ],
             videos=[
                 UpdateVideoMetadataRequest(
                     path="s3://your-s3-bucket/path/to/video.mp4",
                     coactive_video_id="5cf18348-8336-4db7-bb35-db7fbfe8951d",
+                    metadata={"artist": "Marc Simonetti"},
                 )
             ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if images is not OMIT:
             _request["images"] = images
@@ -782,19 +791,26 @@
         )
         await client.dataset.add_assets(
             dataset_id="string",
             images=[
                 AddImageRequest(
                     path="s3://coactive-public/logo.png",
                     id="kingslanding_041711",
+                    metadata={"artist": "Marc Simonetti"},
                 )
             ],
             videos=[
                 AddVideoRequest(
                     path="s3://your-s3-bucket/path/to/video.mp4",
+                    metadata={
+                        "show": "The Boys",
+                        "season": 1,
+                        "episode": 1,
+                        "title": "The Name of the Game",
+                    },
                 )
             ],
             data_path="s3://your-s3-bucket/path/prefix",
             csv_path="path/to/file.csv",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
@@ -850,20 +866,22 @@
         )
         await client.dataset.update_asset_metadata(
             dataset_id="string",
             images=[
                 UpdateImageMetadataRequest(
                     path="s3://coactive-public/logo.png",
                     coactive_image_id="a6894d72-612d-4c20-b4d0-8f3f21c2bb10",
+                    metadata={"artist": "Marc Simonetti"},
                 )
             ],
             videos=[
                 UpdateVideoMetadataRequest(
                     path="s3://your-s3-bucket/path/to/video.mp4",
                     coactive_video_id="5cf18348-8336-4db7-bb35-db7fbfe8951d",
+                    metadata={"artist": "Marc Simonetti"},
                 )
             ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if images is not OMIT:
             _request["images"] = images
```

### Comparing `coactive-1.0.7/src/coactive/resources/query/client.py` & `coactive-1.0.8/src/coactive/resources/query/client.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/resources/search/client.py` & `coactive-1.0.8/src/coactive/resources/search/client.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/__init__.py` & `coactive-1.0.8/src/coactive/types/__init__.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/add_assets_confirmation.py` & `coactive-1.0.8/src/coactive/types/add_assets_confirmation.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/add_image_request.py` & `coactive-1.0.8/src/coactive/types/add_image_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/add_video_request.py` & `coactive-1.0.8/src/coactive/types/add_video_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/added_image.py` & `coactive-1.0.8/src/coactive/types/added_image.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/added_video.py` & `coactive-1.0.8/src/coactive/types/added_video.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/audio_segment.py` & `coactive-1.0.8/src/coactive/types/audio_segment.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/candidates_to_label.py` & `coactive-1.0.8/src/coactive/types/candidates_to_label.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/classification.py` & `coactive-1.0.8/src/coactive/types/classification.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/classification_score.py` & `coactive-1.0.8/src/coactive/types/classification_score.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/concept.py` & `coactive-1.0.8/src/coactive/types/concept.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/concept_label.py` & `coactive-1.0.8/src/coactive/types/concept_label.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/concept_label_enum.py` & `coactive-1.0.8/src/coactive/types/concept_label_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/concept_label_request.py` & `coactive-1.0.8/src/coactive/types/concept_label_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/credentials.py` & `coactive-1.0.8/src/coactive/types/credentials.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/credentials_validation.py` & `coactive-1.0.8/src/coactive/types/credentials_validation.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/dataset.py` & `coactive-1.0.8/src/coactive/types/dataset.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/dataset_status_enum.py` & `coactive-1.0.8/src/coactive/types/dataset_status_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/error_response.py` & `coactive-1.0.8/src/coactive/types/error_response.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/http_validation_error.py` & `coactive-1.0.8/src/coactive/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/image.py` & `coactive-1.0.8/src/coactive/types/image.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/keyframe.py` & `coactive-1.0.8/src/coactive/types/keyframe.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_concept_labels.py` & `coactive-1.0.8/src/coactive/types/paged_concept_labels.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_concepts.py` & `coactive-1.0.8/src/coactive/types/paged_concepts.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_datasets.py` & `coactive-1.0.8/src/coactive/types/paged_datasets.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_images.py` & `coactive-1.0.8/src/coactive/types/paged_images.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_links_response.py` & `coactive-1.0.8/src/coactive/types/paged_links_response.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_meta_response.py` & `coactive-1.0.8/src/coactive/types/paged_meta_response.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_page_details_response.py` & `coactive-1.0.8/src/coactive/types/paged_page_details_response.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_queries.py` & `coactive-1.0.8/src/coactive/types/paged_queries.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/paged_videos.py` & `coactive-1.0.8/src/coactive/types/paged_videos.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/query.py` & `coactive-1.0.8/src/coactive/types/query.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/query_result.py` & `coactive-1.0.8/src/coactive/types/query_result.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/query_results_download_url.py` & `coactive-1.0.8/src/coactive/types/query_results_download_url.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/query_row.py` & `coactive-1.0.8/src/coactive/types/query_row.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/query_status_enum.py` & `coactive-1.0.8/src/coactive/types/query_status_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/query_with_result.py` & `coactive-1.0.8/src/coactive/types/query_with_result.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/search_result.py` & `coactive-1.0.8/src/coactive/types/search_result.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/shot.py` & `coactive-1.0.8/src/coactive/types/shot.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/sort_direction_enum.py` & `coactive-1.0.8/src/coactive/types/sort_direction_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/sort_item.py` & `coactive-1.0.8/src/coactive/types/sort_item.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/storage_type_enum.py` & `coactive-1.0.8/src/coactive/types/storage_type_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/update_assets_metadata_confirmation.py` & `coactive-1.0.8/src/coactive/types/update_assets_metadata_confirmation.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/update_image_metadata_request.py` & `coactive-1.0.8/src/coactive/types/update_image_metadata_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/update_video_metadata_request.py` & `coactive-1.0.8/src/coactive/types/update_video_metadata_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/updated_image.py` & `coactive-1.0.8/src/coactive/types/updated_image.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/updated_video.py` & `coactive-1.0.8/src/coactive/types/updated_video.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/validation_error.py` & `coactive-1.0.8/src/coactive/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/src/coactive/types/video.py` & `coactive-1.0.8/src/coactive/types/video.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.7/PKG-INFO` & `coactive-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coactive
-Version: 1.0.7
+Version: 1.0.8
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

