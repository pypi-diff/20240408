# Comparing `tmp/dynamicpdf_api-1.3.0.tar.gz` & `tmp/dynamicpdf_api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicpdf_api-1.3.0.tar", max compression
+gzip compressed data, was "dynamicpdf_api-1.4.0.tar", max compression
```

## Comparing `dynamicpdf_api-1.3.0.tar` & `dynamicpdf_api-1.4.0.tar`

### file list

```diff
@@ -1,108 +1,112 @@
--rw-r--r--   0        0        0        0 2024-02-09 09:09:40.662020 dynamicpdf_api-1.3.0/dynamicpdf_api/__init__.py
--rw-r--r--   0        0        0      178 2024-02-09 09:09:40.664067 dynamicpdf_api-1.3.0/dynamicpdf_api/action.py
--rw-r--r--   0        0        0     3333 2024-02-09 09:09:40.665026 dynamicpdf_api-1.3.0/dynamicpdf_api/additional_resource.py
--rw-r--r--   0        0        0      250 2024-02-09 09:09:40.667065 dynamicpdf_api-1.3.0/dynamicpdf_api/additional_resource_type.py
--rw-r--r--   0        0        0     2393 2024-02-09 09:09:40.668022 dynamicpdf_api-1.3.0/dynamicpdf_api/aes128_security.py
--rw-r--r--   0        0        0     2389 2024-02-09 09:09:40.669025 dynamicpdf_api-1.3.0/dynamicpdf_api/aes256_security.py
--rw-r--r--   0        0        0      245 2024-02-09 09:09:40.670023 dynamicpdf_api-1.3.0/dynamicpdf_api/align.py
--rw-r--r--   0        0        0     1776 2024-02-09 09:09:40.672022 dynamicpdf_api-1.3.0/dynamicpdf_api/cmyk_color.py
--rw-r--r--   0        0        0      131 2024-02-09 09:09:40.673021 dynamicpdf_api-1.3.0/dynamicpdf_api/color.py
--rw-r--r--   0        0        0      458 2024-02-09 09:09:40.674025 dynamicpdf_api-1.3.0/dynamicpdf_api/color_space_type.py
--rw-r--r--   0        0        0     2017 2024-02-09 09:09:40.675023 dynamicpdf_api-1.3.0/dynamicpdf_api/dlex_input.py
--rw-r--r--   0        0        0     4597 2024-02-09 09:09:40.677025 dynamicpdf_api-1.3.0/dynamicpdf_api/dlex_layout.py
--rw-r--r--   0        0        0     1087 2024-02-09 09:09:40.678024 dynamicpdf_api-1.3.0/dynamicpdf_api/dlex_resource.py
--rw-r--r--   0        0        0        0 2024-02-09 09:09:40.680024 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/__init__.py
--rw-r--r--   0        0        0     2617 2024-02-09 09:09:40.681024 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/aztec_barcode_element.py
--rw-r--r--   0        0        0     2504 2024-02-09 09:09:40.682024 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/aztec_symbol_size.py
--rw-r--r--   0        0        0     1001 2024-02-09 09:09:40.684024 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/barcode_element.py
--rw-r--r--   0        0        0     1906 2024-02-09 09:09:40.686025 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code11_barcode_element.py
--rw-r--r--   0        0        0     3232 2024-02-09 09:09:40.687099 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code128_barcode_element.py
--rw-r--r--   0        0        0     1912 2024-02-09 09:09:40.688084 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code25_barcode_element.py
--rw-r--r--   0        0        0     1888 2024-02-09 09:09:40.689045 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code39_barcode_element.py
--rw-r--r--   0        0        0     1830 2024-02-09 09:09:40.690026 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code93_barcode_element.py
--rw-r--r--   0        0        0      246 2024-02-09 09:09:40.692110 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/compaction.py
--rw-r--r--   0        0        0     2790 2024-02-09 09:09:40.693051 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/data_matrix_barcode_element.py
--rw-r--r--   0        0        0      672 2024-02-09 09:09:40.694021 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/data_matrix_encoding_type.py
--rw-r--r--   0        0        0      393 2024-02-09 09:09:40.696025 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/data_matrix_function_character.py
--rw-r--r--   0        0        0     1908 2024-02-09 09:09:40.697021 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/data_matrix_symbol_size.py
--rw-r--r--   0        0        0      728 2024-02-09 09:09:40.698049 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/dim2_barcode_element.py
--rw-r--r--   0        0        0      977 2024-02-09 09:09:40.699028 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/element.py
--rw-r--r--   0        0        0      529 2024-02-09 09:09:40.701022 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/element_placement.py
--rw-r--r--   0        0        0     1378 2024-02-09 09:09:40.702021 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/element_type.py
--rw-r--r--   0        0        0      673 2024-02-09 09:09:40.703051 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/error_correction.py
--rw-r--r--   0        0        0     2080 2024-02-09 09:09:40.705052 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/gs1_data_bar_barcode_element.py
--rw-r--r--   0        0        0      289 2024-02-09 09:09:40.706024 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/gs1_data_bar_type.py
--rw-r--r--   0        0        0     2225 2024-02-09 09:09:40.707022 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/iata25_barcode_element.py
--rw-r--r--   0        0        0     2288 2024-02-09 09:09:40.708017 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/image_element.py
--rw-r--r--   0        0        0     2620 2024-02-09 09:09:40.710019 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/line_element.py
--rw-r--r--   0        0        0      359 2024-02-09 09:09:40.711066 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/msi_barcode_check_digit_mode.py
--rw-r--r--   0        0        0     2141 2024-02-09 09:09:40.712021 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/msi_barcode_element.py
--rw-r--r--   0        0        0     4507 2024-02-09 09:09:40.714023 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/page_numbering_element.py
--rw-r--r--   0        0        0     2912 2024-02-09 09:09:40.715024 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/pdf417_barcode_element.py
--rw-r--r--   0        0        0     1964 2024-02-09 09:09:40.716021 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/qr_code_element.py
--rw-r--r--   0        0        0      191 2024-02-09 09:09:40.717029 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/qr_code_fnc1.py
--rw-r--r--   0        0        0     3725 2024-02-09 09:09:40.718021 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/rectangle_element.py
--rw-r--r--   0        0        0     2666 2024-02-09 09:09:40.719019 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/stacked_gs1_data_bar_barcode_element.py
--rw-r--r--   0        0        0      305 2024-02-09 09:09:40.720016 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/stacked_gs1_data_bar_type.py
--rw-r--r--   0        0        0     1636 2024-02-09 09:09:40.722086 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/text_barcode_element.py
--rw-r--r--   0        0        0     2934 2024-02-09 09:09:40.723019 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/text_element.py
--rw-r--r--   0        0        0      184 2024-02-09 09:09:40.725029 dynamicpdf_api-1.3.0/dynamicpdf_api/elements/value_type.py
--rw-r--r--   0        0        0      266 2024-02-09 09:09:40.726019 dynamicpdf_api-1.3.0/dynamicpdf_api/encrypt_document_components.py
--rw-r--r--   0        0        0      779 2024-02-09 09:09:40.727055 dynamicpdf_api-1.3.0/dynamicpdf_api/endpoint.py
--rw-r--r--   0        0        0      319 2024-02-09 09:09:40.728052 dynamicpdf_api-1.3.0/dynamicpdf_api/endpoint_exception.py
--rw-r--r--   0        0        0    11480 2024-02-09 09:09:40.730058 dynamicpdf_api-1.3.0/dynamicpdf_api/font.py
--rw-r--r--   0        0        0      145 2024-02-09 09:09:40.731073 dynamicpdf_api-1.3.0/dynamicpdf_api/font_information.py
--rw-r--r--   0        0        0      666 2024-02-09 09:09:40.732049 dynamicpdf_api-1.3.0/dynamicpdf_api/font_resource.py
--rw-r--r--   0        0        0     1108 2024-02-09 09:09:40.733047 dynamicpdf_api-1.3.0/dynamicpdf_api/form_field.py
--rw-r--r--   0        0        0     3397 2024-02-09 09:09:40.735021 dynamicpdf_api-1.3.0/dynamicpdf_api/full_name_table.py
--rw-r--r--   0        0        0     1166 2024-02-09 09:09:40.736021 dynamicpdf_api-1.3.0/dynamicpdf_api/go_to_action.py
--rw-r--r--   0        0        0     1054 2024-02-09 09:09:40.737020 dynamicpdf_api-1.3.0/dynamicpdf_api/grayscale.py
--rw-r--r--   0        0        0     3721 2024-02-09 09:09:40.739016 dynamicpdf_api-1.3.0/dynamicpdf_api/html_input.py
--rw-r--r--   0        0        0      694 2024-02-09 09:09:40.740041 dynamicpdf_api-1.3.0/dynamicpdf_api/html_resource.py
--rw-r--r--   0        0        0     2050 2024-02-09 09:09:40.741021 dynamicpdf_api-1.3.0/dynamicpdf_api/image_info.py
--rw-r--r--   0        0        0     3076 2024-02-09 09:09:40.742019 dynamicpdf_api-1.3.0/dynamicpdf_api/image_input.py
--rw-r--r--   0        0        0     3201 2024-02-09 09:09:40.743018 dynamicpdf_api-1.3.0/dynamicpdf_api/image_resource.py
--rw-r--r--   0        0        0      532 2024-02-09 09:09:40.745024 dynamicpdf_api-1.3.0/dynamicpdf_api/image_response.py
--rw-r--r--   0        0        0     1097 2024-02-09 09:09:40.746019 dynamicpdf_api-1.3.0/dynamicpdf_api/input.py
--rw-r--r--   0        0        0      307 2024-02-09 09:09:40.748018 dynamicpdf_api-1.3.0/dynamicpdf_api/input_type.py
--rw-r--r--   0        0        0      287 2024-02-09 09:09:40.749020 dynamicpdf_api-1.3.0/dynamicpdf_api/json_response.py
--rw-r--r--   0        0        0     1562 2024-02-09 09:09:40.750021 dynamicpdf_api-1.3.0/dynamicpdf_api/layout_data_resource.py
--rw-r--r--   0        0        0     2190 2024-02-09 09:09:40.751013 dynamicpdf_api-1.3.0/dynamicpdf_api/line_style.py
--rw-r--r--   0        0        0     3889 2024-02-09 09:09:40.752014 dynamicpdf_api-1.3.0/dynamicpdf_api/merge_options.py
--rw-r--r--   0        0        0     2691 2024-02-09 09:09:40.754016 dynamicpdf_api-1.3.0/dynamicpdf_api/outline.py
--rw-r--r--   0        0        0     1620 2024-02-09 09:09:40.755013 dynamicpdf_api-1.3.0/dynamicpdf_api/outline_list.py
--rw-r--r--   0        0        0      257 2024-02-09 09:09:40.756020 dynamicpdf_api-1.3.0/dynamicpdf_api/outline_style.py
--rw-r--r--   0        0        0     4187 2024-02-09 09:09:40.757019 dynamicpdf_api-1.3.0/dynamicpdf_api/page_input.py
--rw-r--r--   0        0        0      236 2024-02-09 09:09:40.759013 dynamicpdf_api-1.3.0/dynamicpdf_api/page_orientation.py
--rw-r--r--   0        0        0     1395 2024-02-09 09:09:40.760050 dynamicpdf_api-1.3.0/dynamicpdf_api/page_size.py
--rw-r--r--   0        0        0      369 2024-02-09 09:09:40.761019 dynamicpdf_api-1.3.0/dynamicpdf_api/page_zoom.py
--rw-r--r--   0        0        0    12989 2024-02-09 09:09:40.762019 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf.py
--rw-r--r--   0        0        0      235 2024-02-09 09:09:40.764016 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_content.py
--rw-r--r--   0        0        0     1991 2024-02-09 09:09:40.765016 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_info.py
--rw-r--r--   0        0        0      539 2024-02-09 09:09:40.766013 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_info_response.py
--rw-r--r--   0        0        0     1339 2024-02-09 09:09:40.767020 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_input.py
--rw-r--r--   0        0        0     2224 2024-02-09 09:09:40.768019 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_instruction.py
--rw-r--r--   0        0        0      712 2024-02-09 09:09:40.769018 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_resource.py
--rw-r--r--   0        0        0      442 2024-02-09 09:09:40.770030 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_response.py
--rw-r--r--   0        0        0     2347 2024-02-09 09:09:40.772018 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_text.py
--rw-r--r--   0        0        0      565 2024-02-09 09:09:40.773012 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_text_response.py
--rw-r--r--   0        0        0     2009 2024-02-09 09:09:40.775011 dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_xmp.py
--rw-r--r--   0        0        0     2420 2024-02-09 09:09:40.776052 dynamicpdf_api-1.3.0/dynamicpdf_api/rc4128_security.py
--rw-r--r--   0        0        0     2124 2024-02-09 09:09:40.777020 dynamicpdf_api-1.3.0/dynamicpdf_api/resource.py
--rw-r--r--   0        0        0      386 2024-02-09 09:09:40.778019 dynamicpdf_api-1.3.0/dynamicpdf_api/resource_type.py
--rw-r--r--   0        0        0      472 2024-02-09 09:09:40.781018 dynamicpdf_api-1.3.0/dynamicpdf_api/response.py
--rw-r--r--   0        0        0    21195 2024-02-09 09:09:40.782018 dynamicpdf_api-1.3.0/dynamicpdf_api/rgb_color.py
--rw-r--r--   0        0        0     1407 2024-02-09 09:09:40.784014 dynamicpdf_api-1.3.0/dynamicpdf_api/security.py
--rw-r--r--   0        0        0      251 2024-02-09 09:09:40.785013 dynamicpdf_api-1.3.0/dynamicpdf_api/security_type.py
--rw-r--r--   0        0        0      708 2024-02-09 09:09:40.786035 dynamicpdf_api-1.3.0/dynamicpdf_api/template.py
--rw-r--r--   0        0        0     1007 2024-02-09 09:09:40.787019 dynamicpdf_api-1.3.0/dynamicpdf_api/text_replace.py
--rw-r--r--   0        0        0     3531 2024-02-09 09:09:40.789017 dynamicpdf_api-1.3.0/dynamicpdf_api/unit_converter.py
--rw-r--r--   0        0        0      472 2024-02-09 09:09:40.790042 dynamicpdf_api-1.3.0/dynamicpdf_api/url_action.py
--rw-r--r--   0        0        0      215 2024-02-09 09:09:40.791019 dynamicpdf_api-1.3.0/dynamicpdf_api/v_align.py
--rw-r--r--   0        0        0      428 2024-02-09 09:09:40.792017 dynamicpdf_api-1.3.0/dynamicpdf_api/web_color.py
--rw-r--r--   0        0        0     3841 2024-02-09 09:09:40.793018 dynamicpdf_api-1.3.0/dynamicpdf_api/word_input.py
--rw-r--r--   0        0        0     2049 2024-02-09 09:09:40.794017 dynamicpdf_api-1.3.0/dynamicpdf_api/word_resource.py
--rw-r--r--   0        0        0      456 2024-02-09 09:09:40.795035 dynamicpdf_api-1.3.0/dynamicpdf_api/xml_response.py
--rw-r--r--   0        0        0      867 2024-02-09 09:10:09.818289 dynamicpdf_api-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5645 2024-02-09 09:09:40.660025 dynamicpdf_api-1.3.0/README.md
--rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 dynamicpdf_api-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-05 12:27:21.536795 dynamicpdf_api-1.4.0/dynamicpdf_api/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-05 12:27:21.538742 dynamicpdf_api-1.4.0/dynamicpdf_api/action.py
+-rw-r--r--   0        0        0     3333 2024-04-05 12:27:21.539742 dynamicpdf_api-1.4.0/dynamicpdf_api/additional_resource.py
+-rw-r--r--   0        0        0      250 2024-04-05 12:27:21.541740 dynamicpdf_api-1.4.0/dynamicpdf_api/additional_resource_type.py
+-rw-r--r--   0        0        0     2393 2024-04-05 12:27:21.542743 dynamicpdf_api-1.4.0/dynamicpdf_api/aes128_security.py
+-rw-r--r--   0        0        0     2389 2024-04-05 12:27:21.543742 dynamicpdf_api-1.4.0/dynamicpdf_api/aes256_security.py
+-rw-r--r--   0        0        0      245 2024-04-05 12:27:21.544741 dynamicpdf_api-1.4.0/dynamicpdf_api/align.py
+-rw-r--r--   0        0        0     1776 2024-04-05 12:27:21.545738 dynamicpdf_api-1.4.0/dynamicpdf_api/cmyk_color.py
+-rw-r--r--   0        0        0      131 2024-04-05 12:27:21.547788 dynamicpdf_api-1.4.0/dynamicpdf_api/color.py
+-rw-r--r--   0        0        0      458 2024-04-05 12:27:21.548741 dynamicpdf_api-1.4.0/dynamicpdf_api/color_space_type.py
+-rw-r--r--   0        0        0     2219 2024-04-05 12:27:21.549741 dynamicpdf_api-1.4.0/dynamicpdf_api/converter_input.py
+-rw-r--r--   0        0        0     2017 2024-04-05 12:27:21.551741 dynamicpdf_api-1.4.0/dynamicpdf_api/dlex_input.py
+-rw-r--r--   0        0        0     4597 2024-04-05 12:27:21.552742 dynamicpdf_api-1.4.0/dynamicpdf_api/dlex_layout.py
+-rw-r--r--   0        0        0     1087 2024-04-05 12:27:21.553741 dynamicpdf_api-1.4.0/dynamicpdf_api/dlex_resource.py
+-rw-r--r--   0        0        0        0 2024-04-05 12:27:21.555740 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/__init__.py
+-rw-r--r--   0        0        0     2617 2024-04-05 12:27:21.556740 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/aztec_barcode_element.py
+-rw-r--r--   0        0        0     2504 2024-04-05 12:27:21.558744 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/aztec_symbol_size.py
+-rw-r--r--   0        0        0     1001 2024-04-05 12:27:21.560731 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/barcode_element.py
+-rw-r--r--   0        0        0     1906 2024-04-05 12:27:21.561741 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code11_barcode_element.py
+-rw-r--r--   0        0        0     3232 2024-04-05 12:27:21.562740 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code128_barcode_element.py
+-rw-r--r--   0        0        0     1912 2024-04-05 12:27:21.564734 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code25_barcode_element.py
+-rw-r--r--   0        0        0     1888 2024-04-05 12:27:21.565741 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code39_barcode_element.py
+-rw-r--r--   0        0        0     1830 2024-04-05 12:27:21.566740 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code93_barcode_element.py
+-rw-r--r--   0        0        0      246 2024-04-05 12:27:21.567758 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/compaction.py
+-rw-r--r--   0        0        0     2790 2024-04-05 12:27:21.569733 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/data_matrix_barcode_element.py
+-rw-r--r--   0        0        0      672 2024-04-05 12:27:21.570741 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/data_matrix_encoding_type.py
+-rw-r--r--   0        0        0      393 2024-04-05 12:27:21.571740 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/data_matrix_function_character.py
+-rw-r--r--   0        0        0     1908 2024-04-05 12:27:21.573736 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/data_matrix_symbol_size.py
+-rw-r--r--   0        0        0      728 2024-04-05 12:27:21.574741 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/dim2_barcode_element.py
+-rw-r--r--   0        0        0      977 2024-04-05 12:27:21.575738 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/element.py
+-rw-r--r--   0        0        0      529 2024-04-05 12:27:21.576741 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/element_placement.py
+-rw-r--r--   0        0        0     1378 2024-04-05 12:27:21.578735 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/element_type.py
+-rw-r--r--   0        0        0      673 2024-04-05 12:27:21.580735 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/error_correction.py
+-rw-r--r--   0        0        0     2080 2024-04-05 12:27:21.581740 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/gs1_data_bar_barcode_element.py
+-rw-r--r--   0        0        0      289 2024-04-05 12:27:21.582737 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/gs1_data_bar_type.py
+-rw-r--r--   0        0        0     2225 2024-04-05 12:27:21.583729 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/iata25_barcode_element.py
+-rw-r--r--   0        0        0     2288 2024-04-05 12:27:21.585734 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/image_element.py
+-rw-r--r--   0        0        0     2620 2024-04-05 12:27:21.586738 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/line_element.py
+-rw-r--r--   0        0        0      359 2024-04-05 12:27:21.587737 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/msi_barcode_check_digit_mode.py
+-rw-r--r--   0        0        0     2141 2024-04-05 12:27:21.588735 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/msi_barcode_element.py
+-rw-r--r--   0        0        0     4507 2024-04-05 12:27:21.590754 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/page_numbering_element.py
+-rw-r--r--   0        0        0     2912 2024-04-05 12:27:21.591744 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/pdf417_barcode_element.py
+-rw-r--r--   0        0        0     1964 2024-04-05 12:27:21.592727 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/qr_code_element.py
+-rw-r--r--   0        0        0      191 2024-04-05 12:27:21.593727 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/qr_code_fnc1.py
+-rw-r--r--   0        0        0     3725 2024-04-05 12:27:21.595735 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/rectangle_element.py
+-rw-r--r--   0        0        0     2666 2024-04-05 12:27:21.596776 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/stacked_gs1_data_bar_barcode_element.py
+-rw-r--r--   0        0        0      305 2024-04-05 12:27:21.597737 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/stacked_gs1_data_bar_type.py
+-rw-r--r--   0        0        0     1636 2024-04-05 12:27:21.598734 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/text_barcode_element.py
+-rw-r--r--   0        0        0     2934 2024-04-05 12:27:21.600749 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/text_element.py
+-rw-r--r--   0        0        0      184 2024-04-05 12:27:21.601757 dynamicpdf_api-1.4.0/dynamicpdf_api/elements/value_type.py
+-rw-r--r--   0        0        0      266 2024-04-05 12:27:21.602736 dynamicpdf_api-1.4.0/dynamicpdf_api/encrypt_document_components.py
+-rw-r--r--   0        0        0      779 2024-04-05 12:27:21.603733 dynamicpdf_api-1.4.0/dynamicpdf_api/endpoint.py
+-rw-r--r--   0        0        0      319 2024-04-05 12:27:21.605747 dynamicpdf_api-1.4.0/dynamicpdf_api/endpoint_exception.py
+-rw-r--r--   0        0        0     1523 2024-04-05 12:27:21.606745 dynamicpdf_api-1.4.0/dynamicpdf_api/excel_input.py
+-rw-r--r--   0        0        0     1861 2024-04-05 12:27:21.607736 dynamicpdf_api-1.4.0/dynamicpdf_api/excel_resource.py
+-rw-r--r--   0        0        0    11480 2024-04-05 12:27:21.609733 dynamicpdf_api-1.4.0/dynamicpdf_api/font.py
+-rw-r--r--   0        0        0      145 2024-04-05 12:27:21.610731 dynamicpdf_api-1.4.0/dynamicpdf_api/font_information.py
+-rw-r--r--   0        0        0      666 2024-04-05 12:27:21.611735 dynamicpdf_api-1.4.0/dynamicpdf_api/font_resource.py
+-rw-r--r--   0        0        0     1108 2024-04-05 12:27:21.612727 dynamicpdf_api-1.4.0/dynamicpdf_api/form_field.py
+-rw-r--r--   0        0        0     3397 2024-04-05 12:27:21.614730 dynamicpdf_api-1.4.0/dynamicpdf_api/full_name_table.py
+-rw-r--r--   0        0        0     1166 2024-04-05 12:27:21.615736 dynamicpdf_api-1.4.0/dynamicpdf_api/go_to_action.py
+-rw-r--r--   0        0        0     1054 2024-04-05 12:27:21.616736 dynamicpdf_api-1.4.0/dynamicpdf_api/grayscale.py
+-rw-r--r--   0        0        0     1904 2024-04-05 12:27:21.617735 dynamicpdf_api-1.4.0/dynamicpdf_api/html_input.py
+-rw-r--r--   0        0        0      694 2024-04-05 12:27:21.618734 dynamicpdf_api-1.4.0/dynamicpdf_api/html_resource.py
+-rw-r--r--   0        0        0     2050 2024-04-05 12:27:21.620733 dynamicpdf_api-1.4.0/dynamicpdf_api/image_info.py
+-rw-r--r--   0        0        0     3076 2024-04-05 12:27:21.622734 dynamicpdf_api-1.4.0/dynamicpdf_api/image_input.py
+-rw-r--r--   0        0        0     3201 2024-04-05 12:27:21.623763 dynamicpdf_api-1.4.0/dynamicpdf_api/image_resource.py
+-rw-r--r--   0        0        0      532 2024-04-05 12:27:21.624730 dynamicpdf_api-1.4.0/dynamicpdf_api/image_response.py
+-rw-r--r--   0        0        0     1097 2024-04-05 12:27:21.626746 dynamicpdf_api-1.4.0/dynamicpdf_api/input.py
+-rw-r--r--   0        0        0      354 2024-04-05 12:27:21.627737 dynamicpdf_api-1.4.0/dynamicpdf_api/input_type.py
+-rw-r--r--   0        0        0      287 2024-04-05 12:27:21.628736 dynamicpdf_api-1.4.0/dynamicpdf_api/json_response.py
+-rw-r--r--   0        0        0     1562 2024-04-05 12:27:21.629733 dynamicpdf_api-1.4.0/dynamicpdf_api/layout_data_resource.py
+-rw-r--r--   0        0        0     2190 2024-04-05 12:27:21.631734 dynamicpdf_api-1.4.0/dynamicpdf_api/line_style.py
+-rw-r--r--   0        0        0     3889 2024-04-05 12:27:21.632732 dynamicpdf_api-1.4.0/dynamicpdf_api/merge_options.py
+-rw-r--r--   0        0        0     2691 2024-04-05 12:27:21.633735 dynamicpdf_api-1.4.0/dynamicpdf_api/outline.py
+-rw-r--r--   0        0        0     1620 2024-04-05 12:27:21.634734 dynamicpdf_api-1.4.0/dynamicpdf_api/outline_list.py
+-rw-r--r--   0        0        0      257 2024-04-05 12:27:21.636726 dynamicpdf_api-1.4.0/dynamicpdf_api/outline_style.py
+-rw-r--r--   0        0        0        4 2023-01-23 08:55:17.215254 dynamicpdf_api-1.4.0/dynamicpdf_api/package.json
+-rw-r--r--   0        0        0     4187 2024-04-05 12:27:21.637735 dynamicpdf_api-1.4.0/dynamicpdf_api/page_input.py
+-rw-r--r--   0        0        0      236 2024-04-05 12:27:21.638737 dynamicpdf_api-1.4.0/dynamicpdf_api/page_orientation.py
+-rw-r--r--   0        0        0     1395 2024-04-05 12:27:21.640733 dynamicpdf_api-1.4.0/dynamicpdf_api/page_size.py
+-rw-r--r--   0        0        0      369 2024-04-05 12:27:21.641741 dynamicpdf_api-1.4.0/dynamicpdf_api/page_zoom.py
+-rw-r--r--   0        0        0    13654 2024-04-05 12:27:21.642735 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf.py
+-rw-r--r--   0        0        0      235 2024-04-05 12:27:21.643733 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_content.py
+-rw-r--r--   0        0        0     1991 2024-04-05 12:27:21.644734 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_info.py
+-rw-r--r--   0        0        0      539 2024-04-05 12:27:21.646732 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_info_response.py
+-rw-r--r--   0        0        0     1339 2024-04-05 12:27:21.647735 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_input.py
+-rw-r--r--   0        0        0     2212 2024-04-05 12:27:21.649727 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_instruction.py
+-rw-r--r--   0        0        0      712 2024-04-05 12:27:21.650741 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_resource.py
+-rw-r--r--   0        0        0      442 2024-04-05 12:27:21.651722 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_response.py
+-rw-r--r--   0        0        0     2347 2024-04-05 12:27:21.653727 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_text.py
+-rw-r--r--   0        0        0      565 2024-04-05 12:27:21.654723 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_text_response.py
+-rw-r--r--   0        0        0     2009 2024-04-05 12:27:21.655722 dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_xmp.py
+-rw-r--r--   0        0        0     2420 2024-04-05 12:27:21.656723 dynamicpdf_api-1.4.0/dynamicpdf_api/rc4128_security.py
+-rw-r--r--   0        0        0     2124 2024-04-05 12:27:21.657723 dynamicpdf_api-1.4.0/dynamicpdf_api/resource.py
+-rw-r--r--   0        0        0      436 2024-04-05 12:27:21.658723 dynamicpdf_api-1.4.0/dynamicpdf_api/resource_type.py
+-rw-r--r--   0        0        0      472 2024-04-05 12:27:21.659725 dynamicpdf_api-1.4.0/dynamicpdf_api/response.py
+-rw-r--r--   0        0        0    21195 2024-04-05 12:27:21.661732 dynamicpdf_api-1.4.0/dynamicpdf_api/rgb_color.py
+-rw-r--r--   0        0        0     1407 2024-04-05 12:27:21.662723 dynamicpdf_api-1.4.0/dynamicpdf_api/security.py
+-rw-r--r--   0        0        0      251 2024-04-05 12:27:21.663723 dynamicpdf_api-1.4.0/dynamicpdf_api/security_type.py
+-rw-r--r--   0        0        0      708 2024-04-05 12:27:21.664733 dynamicpdf_api-1.4.0/dynamicpdf_api/template.py
+-rw-r--r--   0        0        0     1007 2024-04-05 12:27:21.666730 dynamicpdf_api-1.4.0/dynamicpdf_api/text_replace.py
+-rw-r--r--   0        0        0     3531 2024-04-05 12:27:21.667729 dynamicpdf_api-1.4.0/dynamicpdf_api/unit_converter.py
+-rw-r--r--   0        0        0      472 2024-04-05 12:27:21.668734 dynamicpdf_api-1.4.0/dynamicpdf_api/url_action.py
+-rw-r--r--   0        0        0      215 2024-04-05 12:27:21.669733 dynamicpdf_api-1.4.0/dynamicpdf_api/v_align.py
+-rw-r--r--   0        0        0      428 2024-04-05 12:27:21.670732 dynamicpdf_api-1.4.0/dynamicpdf_api/web_color.py
+-rw-r--r--   0        0        0     1989 2024-04-05 12:27:21.671732 dynamicpdf_api-1.4.0/dynamicpdf_api/word_input.py
+-rw-r--r--   0        0        0     2049 2024-04-05 12:27:21.673731 dynamicpdf_api-1.4.0/dynamicpdf_api/word_resource.py
+-rw-r--r--   0        0        0      456 2024-04-05 12:27:21.674735 dynamicpdf_api-1.4.0/dynamicpdf_api/xml_response.py
+-rw-r--r--   0        0        0      835 2024-04-05 12:28:35.612897 dynamicpdf_api-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5256 2024-04-05 12:27:21.535736 dynamicpdf_api-1.4.0/README.md
+-rw-r--r--   0        0        0     6237 1970-01-01 00:00:00.000000 dynamicpdf_api-1.4.0/PKG-INFO
```

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/additional_resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/additional_resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/aes128_security.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/aes128_security.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/aes256_security.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/aes256_security.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/cmyk_color.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/cmyk_color.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/dlex_input.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/dlex_input.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/dlex_layout.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/dlex_layout.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/dlex_resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/dlex_resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/aztec_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/aztec_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/aztec_symbol_size.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/aztec_symbol_size.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code11_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code11_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code128_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code128_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code25_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code25_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code39_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code39_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/code93_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/code93_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/data_matrix_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/data_matrix_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/data_matrix_encoding_type.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/data_matrix_encoding_type.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/data_matrix_symbol_size.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/data_matrix_symbol_size.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/dim2_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/dim2_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/element_placement.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/element_placement.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/element_type.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/element_type.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/error_correction.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/error_correction.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/gs1_data_bar_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/gs1_data_bar_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/iata25_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/iata25_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/image_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/image_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/line_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/line_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/msi_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/msi_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/page_numbering_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/page_numbering_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/pdf417_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/pdf417_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/qr_code_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/qr_code_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/rectangle_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/rectangle_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/stacked_gs1_data_bar_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/stacked_gs1_data_bar_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/text_barcode_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/text_barcode_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/elements/text_element.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/elements/text_element.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/endpoint.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/endpoint.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/font.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/font.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/font_resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/font_resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/form_field.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/form_field.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/full_name_table.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/full_name_table.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/go_to_action.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/go_to_action.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/grayscale.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/grayscale.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/html_input.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/page_input.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,139 @@
-from .input import Input
+from .input import Input 
 from .input_type import InputType
+from .unit_converter import UnitConverter
 from .page_size import PageSize
 from .page_orientation import PageOrientation
-from .unit_converter import UnitConverter
 
-class HtmlInput(Input):
-    ''' 
-    Represents a html input
+class PageInput(Input):
+    '''
+    Represents a page input.
     '''
-    
-    def __init__(self, resource, base_path = None, size = PageSize.Letter, orientation = PageOrientation.Portrait, margins = None):
+
+    def __init__(self, size = PageSize.Letter, orientation = PageOrientation.Portrait, margins = None):
         '''
-        Initializes a new instance of the HtmlInput class.
-        
+        Initializes a new instance of the PageInput class.
+
         Args:
-            resource (HtmlResource): The resource of type HtmlResource.
-            basepath (string): The basepath options for the url.
-            size (PageSize): The page size of the output PDF.
-            orientation (PageOrientation): The page orientation of the output PDF.
-            margins (integer): The page margins of the output PDF.
+            size (PageSize | float): The size of the page. | The width of the page.
+            oriientation (PageOrientation | float): The orientation of the page. | The height of the page.
+            margins (float): The margins of the page.
         '''
 
-        super().__init__(resource)
-
-        # Gets or sets the base path option.
-        self.base_path = base_path
+        super().__init__()
+        self._elements = []
+        self._default_page_height = 792.0
+        self._default_page_width = 612.0
 
         # Gets or sets the top margin.
         self.top_margin = margins
 
         # Gets or sets the bottom margin.
         self.bottom_margin = margins
 
         # Gets or sets the right margin.
         self.right_margin = margins
 
         # Gets or sets the left margin.
         self.left_margin = margins
 
+        # Gets or sets the width of the page.
         self.page_width = None
+
+        # Gets or sets the height of the page.
         self.page_height = None
-        self._page_size = None
-        self._page_orientation = None
-        self.page_size = size
-        self.page_orientation = orientation
-        self.html_string = ''
-        self._type = InputType.Html
-        
+        self._type=InputType.Page
+        if type(size) == float or type(size) == int:
+            self.page_width = size
+            self.page_height = orientation
+        else:
+            self._page_size = size
+            self._page_orientation = orientation
+            self.page_size = size
+            self.page_orientation = orientation
+
+    @property
+    def _width(self):
+        return self.page_width or self._default_page_width
+
+    @property
+    def _height(self):
+        return self.page_height or self._default_page_height
+
     @property
     def page_size(self):
         '''
-        Gets the page size.
+        Gets the Page size.
         '''
         return self._page_size
-    
+
     @page_size.setter
     def page_size(self, value):
         '''
-        Sets the page size.
+        Sets the Page size.
         '''
         self._page_size = value
         smaller, larger = UnitConverter._get_paper_size(value)
-        if self.page_orientation == PageOrientation.Portrait:
+        if self._page_orientation == PageOrientation.Portrait:
             self.page_height = larger
             self.page_width = smaller
         else:
             self.page_height = smaller
             self.page_width = larger
-    
+
     @property
     def page_orientation(self):
         '''
-        Gets the page orientation.
+        Gets page orientation.
         '''
         return self._page_orientation
 
     @page_orientation.setter
     def page_orientation(self, value):
         '''
-        Sets the page orientation.
+        Sets page orientation.
         '''
         self._page_orientation = value
-        if self.page_width > self.page_height:
-            smaller = self.page_height
-            larger = self.page_width
+        if self._width > self._height:
+            smaller = self._height
+            larger = self._width
         else:
-            smaller = self.page_width
-            larger = self.page_height
-        if self._page_orientation == PageOrientation.Portrait:
+            smaller = self._width
+            larger = self._height
+
+        if self.page_orientation == PageOrientation.Portrait:
             self.page_height = larger
             self.page_width = smaller
         else:
             self.page_height = smaller
             self.page_width = larger
 
-    
-    def to_json(self):
+    @property
+    def elements(self):
+        '''
+        Gets the elements of the page.
+        '''
+        return self._elements
+
+    def to_json(self): 
         json = {
             "type": self._type,
             "resourceName": self.resource_name,
             "id": self.id,
             "pageHeight": self.page_height,
             "pageWidth": self.page_width
         }
+        elements = []
+        for i in self.elements:
+            elements.append(i.to_json())
+        json["elements"] = elements
         if self._template_id:
             json["templateId"] = self._template_id
-        if self.base_path:
-            json["basePath"] = self.base_path
         if self.top_margin:
             json["topMargin"] = self.top_margin
         if self.left_margin:
             json["leftMargin"] = self.left_margin
         if self.bottom_margin:
             json["bottomMargin"] = self.bottom_margin
         if self.right_margin:
             json["rightMargin"] = self.right_margin
-        return json
+        return json
```

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/html_resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/html_resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/image_info.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/image_info.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/image_input.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/image_input.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/image_resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/image_resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/image_response.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/image_response.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/input.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/input.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/layout_data_resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/layout_data_resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/line_style.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/line_style.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/merge_options.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/merge_options.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/outline.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/outline.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/outline_list.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/outline_list.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/page_size.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/page_size.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .additional_resource import AdditionalResource
 from .additional_resource_type import AdditionalResourceType
 from .resource_type import ResourceType
 from .image_input import ImageInput
 from .pdf_input import PdfInput
 from .html_input import HtmlInput
 from .word_input import WordInput
+from .excel_input import ExcelInput
 from .html_resource import HtmlResource
 from .page_size import PageSize
 from .dlex_input import DlexInput
 from .page_orientation import PageOrientation
 from .pdf_response import PdfResponse
 from .input_type import InputType
 from .endpoint_exception import EndpointException 
@@ -280,14 +281,29 @@
             orientation (PageOrientation): The page orientation for the PDF pages
             margins (integer): Margins for all four sides
         '''
 
         input = WordInput(resource, size, orientation, margins)
         self.inputs.append(input)
         return input
+    
+    def add_excel(self, resource, size = PageSize.A4, orientation = PageOrientation.Portrait, margins = None):
+        '''
+        Returns a ExcelInput object containing the input pdf.
+
+        Args:
+            resource (ExcelResource):  The resource of type ExcelResource.
+            size (PageSize): the page size of the PDF pages
+            orientation (PageOrientation): The page orientation for the PDF pages
+            margins (integer): Margins for all four sides
+        '''
+
+        input = ExcelInput(resource, size, orientation, margins)
+        self.inputs.append(input)
+        return input
 
     def add_dlex(self, value, layout_data):
         '''
         Returns a DlexInput object containing the input pdf.
 
         Args:
             value (string | DlexResource): The resource path in cloud resource manager. | The resource of type DlexResource
```

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_info.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_info.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_info_response.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_info_response.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_input.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_input.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_instruction.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
         self._form_fields = []
         self._templates = set()
         self._fonts = set()
         self._outlines = OutlineList()
         self._author = "CeteSoftware"
         self._title = None
         self._subject = None
-        self._creator = "DynamicPDF Cloud Api"
-        self._producer = "DynamicPDF Cloud Api"
+        self._creator = "DynamicPDF API"
+        self._producer = "DynamicPDF API"
         self._tag = None
         self._keywords = None
         self._security = None
         self._flatten_all_form_fields = None
         self._retain_signature_form_fields = None
         self._inputs = []
```

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_text.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_text.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_text_response.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_text_response.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/pdf_xmp.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/pdf_xmp.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/rc4128_security.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/rc4128_security.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/rgb_color.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/rgb_color.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/security.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/security.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/template.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/template.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/text_replace.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/text_replace.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/unit_converter.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/unit_converter.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/dynamicpdf_api/word_resource.py` & `dynamicpdf_api-1.4.0/dynamicpdf_api/word_resource.py`

 * *Files identical despite different names*

### Comparing `dynamicpdf_api-1.3.0/README.md` & `dynamicpdf_api-1.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 ![](./logo-banner2.png)
 
 # Python Client Library (`python-client`)
 
-The python Client library (`python-client`) uses the DynamicPDF Cloud API to create, merge, split, form fill, stamp, obtain metadata, convert, and secure/encrypt PDF documents. The website for this project is available at [cloud.dynamicpdf.com](https://cloud.dynamicpdf.com/).
+The python Client library (`python-client`) uses the DynamicPDF API to create, merge, split, form fill, stamp, obtain metadata, convert, and secure/encrypt PDF documents. The website for this project is available at [https://dpdf.io](https://dpdf.io/).
 
-The DynamicPDF Cloud API consists of the following endpoints.
+The DynamicPDF API consists of the following endpoints.
 
 * `dlex-layout`
 * `image-info`
 * `pdf`
 * `pdf-info`
 * `pdf-text`
 * `pdf-xmp`
 
 ## PyPI Package
 
 * Obtain the PyPI package at https://pypi.org/project/dynamicpdf-api/
 
 ## Documentation
 
-* Obtain overview documentation for the DynamicPDF Cloud API Client libraries from the [Cloud API Users Guide](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/client-libraries/cloud-api-client-libraries).
+* Obtain overview documentation for the DynamicPDF API Client libraries from the [API Users Guide](https://dpdf.io/docs/usersguide/cloud-api/client-libraries/cloud-api-client-libraries).
 * Access the documentation for each particular endpoint from the following Users Guide pages. 
 
 | Endpoint      | REST Endpoint                                                | REST Endpoint Client Library                                 | Description                                                  |
 | ------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| `dlex-layout` | [Cloud API Users Guide - `dlex-layout`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/cloud-api-dlex-layout) | [`dlex-layout`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/client-libraries/client-api-dlex-layout) | Returns a PDF after processing a DLEX file with it's associated JSON data. |
-| `image-info`  | [Cloud API Users Guide - `image-info`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/cloud-api-image-info) | [`image-info`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/client-libraries/client-api-image-info) | Returns image metadata as a JSON document.                   |
-| `pdf`         | [Cloud API Users Guide - `pdf`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/cloud-api-pdf) | [`pdf`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/client-libraries/client-api-pdf) | Returns a PDF after performing one of the pdf endpoint's tasks (`page`, `dlex`, `image`) or merging. |
-| `pdf-info`    | [Cloud API Users Guide - `pdf-Info`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/cloud-api-pdf-info) | [`pdf-info`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/client-libraries/client-api-pdf-info) | Returns PDF metadata as a JSON document.                     |
-| `pdf-text`    | [Cloud API Users Guide - `pdf-text`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/cloud-api-pdf-text) | [`pdf-text`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/client-libraries/client-api-pdf-text) | Returns the text from a PDF as a JSON document.              |
-| `pdf-xmp`     | [Cloud API Users Guide - `pdf-xmp`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/cloud-api-pdf-xmp) | [`pdf-xmp`](https://cloud.dynamicpdf.com/docs/usersguide/cloud-api/client-libraries/client-api-pdf-xmp) | Returns XMP metadata from a PDF.                             |
+| `dlex-layout` | [API Users Guide - `dlex-layout`](https://dpdf.io/docs/usersguide/cloud-api/cloud-api-dlex-layout) | [`dlex-layout`](https://dpdf.io/docs/usersguide/cloud-api/client-libraries/client-api-dlex-layout) | Returns a PDF after processing a DLEX file with it's associated JSON data. |
+| `image-info`  | [API Users Guide - `image-info`](https://dpdf.io/docs/usersguide/cloud-api/cloud-api-image-info) | [`image-info`](https://dpdf.io/docs/usersguide/cloud-api/client-libraries/client-api-image-info) | Returns image metadata as a JSON document.                   |
+| `pdf`         | [API Users Guide - `pdf`](https://dpdf.io/docs/usersguide/cloud-api/cloud-api-pdf) | [`pdf`](https://dpdf.io/docs/usersguide/cloud-api/client-libraries/client-api-pdf) | Returns a PDF after performing one of the pdf endpoint's tasks (`page`, `dlex`, `image`) or merging. |
+| `pdf-info`    | [API Users Guide - `pdf-Info`](https://dpdf.io/docs/usersguide/cloud-api/cloud-api-pdf-info) | [`pdf-info`](https://dpdf.io/docs/usersguide/cloud-api/client-libraries/client-api-pdf-info) | Returns PDF metadata as a JSON document.                     |
+| `pdf-text`    | [API Users Guide - `pdf-text`](https://dpdf.io/docs/usersguide/cloud-api/cloud-api-pdf-text) | [`pdf-text`](https://dpdf.io/docs/usersguide/cloud-api/client-libraries/client-api-pdf-text) | Returns the text from a PDF as a JSON document.              |
+| `pdf-xmp`     | [API Users Guide - `pdf-xmp`](https://dpdf.io/docs/usersguide/cloud-api/cloud-api-pdf-xmp) | [`pdf-xmp`](https://dpdf.io/docs/usersguide/cloud-api/client-libraries/client-api-pdf-xmp) | Returns XMP metadata from a PDF.                             |
 
 ## **Tutorials**
 
 The following table lists the available tutorials.
 
 | Tutorial Title                                     | Tutorial Location                                            |
 | -------------------------------------------------- | ------------------------------------------------------------ |
-| Merging PDFs                                       | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/merging-pdfs |
-| Completing an AcroForm                             | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/form-completion |
-| Creating a PDF Using a DLEX and the `pdf` Endpoint | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/dlex-pdf-endpoint |
-| Adding Bookmarks to a PDF                          | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/bookmarks |
-| Creating a PDF Using the `dlex-layout` Endpoint    | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/dlex-layout |
-| Extracting Image Metadata                          | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/image-info |
-| Extract PDF Metadata                               | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/pdf-info |
-| Extracting PDF's Text                              | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/pdf-text |
-| Extract XMP Metadata                               | https://cloud.dynamicpdf.com/docs/tutorials/cloud-api/pdf-xmp |
+| Merging PDFs                                       | https://dpdf.io/docs/tutorials/cloud-api/merging-pdfs |
+| Completing an AcroForm                             | https://dpdf.io/docs/tutorials/cloud-api/form-completion |
+| Creating a PDF Using a DLEX and the `pdf` Endpoint | https://dpdf.io/docs/tutorials/cloud-api/dlex-pdf-endpoint |
+| Adding Bookmarks to a PDF                          | https://dpdf.io/docs/tutorials/cloud-api/bookmarks |
+| Creating a PDF Using the `dlex-layout` Endpoint    | https://dpdf.io/docs/tutorials/cloud-api/dlex-layout |
+| Extracting Image Metadata                          | https://dpdf.io/docs/tutorials/cloud-api/image-info |
+| Extract PDF Metadata                               | https://dpdf.io/docs/tutorials/cloud-api/pdf-info |
+| Extracting PDF's Text                              | https://dpdf.io/docs/tutorials/cloud-api/pdf-text |
+| Extract XMP Metadata                               | https://dpdf.io/docs/tutorials/cloud-api/pdf-xmp |
 
 # Support
 
-The primary source for the DynamicPDF Cloud API support is through [Stack Overflow](https://stackoverflow.com/questions/tagged/dynamicpdf-api). Please use the "[dynamicpdf-api](https://stackoverflow.com/questions/tagged/dynamicpdf-api)" tag to ask questions. Our support team actively monitors the tag and responds promptly to any questions. Also, let us know you asked the question by following up with an email to [support@dynamicpdf.com](mailto:support@dynamicpdf.com). 
+The primary source for the DynamicPDF API support is through [Stack Overflow](https://stackoverflow.com/questions/tagged/dynamicpdf-api). Please use the "[dynamicpdf-api](https://stackoverflow.com/questions/tagged/dynamicpdf-api)" tag to ask questions. Our support team actively monitors the tag and responds promptly to any questions. Also, let us know you asked the question by following up with an email to [support@dynamicpdf.com](mailto:support@dynamicpdf.com). 
 
-## Pro Plan Subscribers[#](https://cloud.dynamicpdf.com/support#pro-plan-subscribers)
+## Pro Plan Subscribers[#](https://dpdf.io/support#pro-plan-subscribers)
 
-Ticket support is available to Pro Plan subscribers. But we still encourage you to help the community by posting on Stack Overflow when possible. You can also email [support@dynamicpdf.com](mailto:support@dynamicpdf.com) if you need to ask something specific to your use case that may not help the DynamicPDF Cloud API community.
+Ticket support is available to Pro Plan subscribers. But we still encourage you to help the community by posting on Stack Overflow when possible. You can also email [support@dynamicpdf.com](mailto:support@dynamicpdf.com) if you need to ask something specific to your use case that may not help the DynamicPDF API community.
 
 # License
 
 The `python-client` library is licensed under the [MIT License](./LICENSE).
```

