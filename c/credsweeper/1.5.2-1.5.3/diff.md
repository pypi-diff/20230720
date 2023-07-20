# Comparing `tmp/credsweeper-1.5.2.tar.gz` & `tmp/credsweeper-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsweeper-1.5.2.tar", last modified: Wed Jul  5 10:25:15 2023, max compression
+gzip compressed data, was "credsweeper-1.5.3.tar", last modified: Thu Jul 20 16:15:42 2023, max compression
```

## Comparing `credsweeper-1.5.2.tar` & `credsweeper-1.5.3.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.929459 credsweeper-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 10:25:04.000000 credsweeper-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-05 10:25:15.929459 credsweeper-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-05 10:25:04.000000 credsweeper-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.885458 credsweeper-1.5.2/credsweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.889459 credsweeper-1.5.2/credsweeper/common/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/keyword_checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/keyword_checklist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/morpheme_checklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.889459 credsweeper-1.5.2/credsweeper/config/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.893458 credsweeper-1.5.2/credsweeper/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/candidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/candidate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/line_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.897459 credsweeper-1.5.2/credsweeper/deep_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/deep_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/zip_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.901459 credsweeper-1.5.2/credsweeper/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/files_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/patch_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/text_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.917459 credsweeper-1.5.2/credsweeper/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/cred_card_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.917459 credsweeper-1.5.2/credsweeper/filters/group/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/structured_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/token_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/weird_base36_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/weird_base64_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_base32_data_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_base64_data_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_couple_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_entropy_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_entropy_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_entropy_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_grafana_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_json_web_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_method_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_not_part_encoded_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_pattern_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_pem_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_split_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_structured_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_token_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_token_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_token_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/variable_not_allowed_pattern_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.921459 credsweeper-1.5.2/credsweeper/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.921459 credsweeper-1.5.2/credsweeper/ml_model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/features.py
--rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.921459 credsweeper-1.5.2/credsweeper/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/rules/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.921459 credsweeper-1.5.2/credsweeper/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.925459 credsweeper-1.5.2/credsweeper/scanner/scan_type/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.925459 credsweeper-1.5.2/credsweeper/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/secret/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/secret/log.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.925459 credsweeper-1.5.2/credsweeper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/utils/entropy_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21920 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.929459 credsweeper-1.5.2/credsweeper/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/apply_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/github_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.889459 credsweeper-1.5.2/credsweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 10:25:15.933459 credsweeper-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-05 10:25:04.000000 credsweeper-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.929459 credsweeper-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30506 2023-07-05 10:25:04.000000 credsweeper-1.5.2/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    43642 2023-07-05 10:25:04.000000 credsweeper-1.5.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 16:15:24.000000 credsweeper-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-20 16:15:42.589390 credsweeper-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-20 16:15:24.000000 credsweeper-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.565388 credsweeper-1.5.3/credsweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.565388 credsweeper-1.5.3/credsweeper/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/morpheme_checklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.565388 credsweeper-1.5.3/credsweeper/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.569389 credsweeper-1.5.3/credsweeper/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/line_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.573389 credsweeper-1.5.3/credsweeper/deep_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/zip_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.573389 credsweeper-1.5.3/credsweeper/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/patch_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/text_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.581390 credsweeper-1.5.3/credsweeper/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/cred_card_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/filters/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/structured_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/weird_base64_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_base64_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_entropy_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_method_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_not_part_encoded_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_pem_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_structured_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_token_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/variable_not_allowed_pattern_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/ml_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/rules/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/scanner/scan_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/credsweeper/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/secret/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/secret/log.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/credsweeper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/utils/entropy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/credsweeper/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/apply_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.565388 credsweeper-1.5.3/credsweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 16:15:42.593391 credsweeper-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-20 16:15:24.000000 credsweeper-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30988 2023-07-20 16:15:24.000000 credsweeper-1.5.3/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43734 2023-07-20 16:15:24.000000 credsweeper-1.5.3/tests/test_main.py
```

### Comparing `credsweeper-1.5.2/LICENSE` & `credsweeper-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/PKG-INFO` & `credsweeper-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.5.2
+Version: 1.5.3
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.5.2/README.md` & `credsweeper-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/__init__.py` & `credsweeper-1.5.3/credsweeper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
     '__version__'
 ]
 
-__version__ = "1.5.2"
+__version__ = "1.5.3"
```

### Comparing `credsweeper-1.5.2/credsweeper/__main__.py` & `credsweeper-1.5.3/credsweeper/__main__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/app.py` & `credsweeper-1.5.3/credsweeper/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         pool_count: number of pools used to run multiprocessing scanning
         config: dictionary variable, stores analyzer features
         json_filename: string variable, credential candidates export filename
 
     """
 
     def __init__(self,
-                 rule_path: Optional[str] = None,
+                 rule_path: Union[None, str, Path] = None,
                  config_path: Optional[str] = None,
                  api_validation: bool = False,
                  json_filename: Union[None, str, Path] = None,
                  xlsx_filename: Union[None, str, Path] = None,
                  sort_output: bool = False,
                  use_filters: bool = True,
                  pool_count: int = 1,
@@ -93,17 +93,15 @@
                                             doc=doc,
                                             severity=severity,
                                             size_limit=size_limit,
                                             exclude_lines=exclude_lines,
                                             exclude_values=exclude_values)
         self.config = Config(config_dict)
         self.scanner = Scanner(self.config, rule_path)
-        self.doc_scanner = Scanner(self.config, rule_path, ["doc"])
         self.deep_scanner = DeepScanner(self.config, self.scanner)
-        self.deep_doc_scanner = DeepScanner(self.config, self.doc_scanner)
         self.credential_manager = CredentialManager()
         self.json_filename: Union[None, str, Path] = json_filename
         self.xlsx_filename: Union[None, str, Path] = xlsx_filename
         self.sort_output = sort_output
         self.ml_batch_size = ml_batch_size
         self.ml_threshold = ml_threshold
         self.ml_validator = None
@@ -301,25 +299,21 @@
         if FilePathExtractor.is_find_by_ext_file(self.config, content_provider.file_type):
             # Skip the file scanning and create fake candidate because the extension is suspicious
             dummy_candidate = Candidate.get_dummy_candidate(self.config, content_provider.file_path,
                                                             content_provider.file_type, content_provider.info)
             candidates.append(dummy_candidate)
 
         else:
-            if self.config.depth:
+            if self.config.depth or self.config.doc:
                 # deep scan with possible data representation
                 candidates = self.deep_scanner.scan(content_provider, self.config.depth, self.config.size_limit)
-            elif self.config.doc:
-                # document-specific scanning
-                candidates = self.deep_doc_scanner.scan(content_provider, 0, self.config.size_limit)
             else:
                 if content_provider.file_type not in self.config.exclude_containers:
                     # Regular file scanning
-                    analysis_targets = content_provider.get_analysis_target()
-                    candidates = self.scanner.scan(analysis_targets)
+                    candidates = self.scanner.scan(content_provider)
 
         # finally return result from 'file_scan'
         return candidates
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def post_processing(self) -> None:
```

### Comparing `credsweeper-1.5.2/credsweeper/common/constants.py` & `credsweeper-1.5.3/credsweeper/common/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,16 +114,14 @@
     highest = "highest"
 
 
 class DiffRowType(Enum):
     """Diff type of row"""
     ADDED = "added"
     DELETED = "deleted"
-    ADDED_ACCOMPANY = "added_accompany"
-    DELETED_ACCOMPANY = "deleted_accompany"
 
 
 MIN_VARIABLE_LENGTH = 1
 MIN_SEPARATOR_LENGTH = 1
 MIN_VALUE_LENGTH = 4
 MAX_LINE_LENGTH = 2000
 """ values according https://docs.python.org/3/library/codecs.html """
```

### Comparing `credsweeper-1.5.2/credsweeper/common/keyword_checklist.py` & `credsweeper-1.5.3/credsweeper/common/keyword_checklist.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.5.3/credsweeper/common/keyword_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/common/morpheme_checklist.txt` & `credsweeper-1.5.3/credsweeper/common/morpheme_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/config/config.py` & `credsweeper-1.5.3/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.5.3/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.5.3/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/credentials/candidate_key.py` & `credsweeper-1.5.3/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/credentials/credential_manager.py` & `credsweeper-1.5.3/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+import gzip
+import io
 import logging
 from abc import ABC
 from typing import List
 
 from credsweeper.credentials import Candidate
-from credsweeper.file_handler.byte_content_provider import ByteContentProvider
+from credsweeper.deep_scanner.abstract_scanner import AbstractScanner
 from credsweeper.file_handler.data_content_provider import DataContentProvider
-from .abstract_scanner import AbstractScanner
+from credsweeper.utils import Util
 
 logger = logging.getLogger(__name__)
 
 
-class ByteScanner(AbstractScanner, ABC):
-    """Implements plain data scanning"""
+class GzipScanner(AbstractScanner, ABC):
+    """Realises gzip scanning"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
-        """Tries to represent data as plain text with splitting by lines and scan as text lines"""
-        byte_content_provider = ByteContentProvider(content=data_provider.data,
-                                                    file_path=data_provider.file_path,
-                                                    file_type=data_provider.file_type,
-                                                    info=f"{data_provider.info}|RAW")
-        analysis_targets = byte_content_provider.get_analysis_target()
-        return self.scanner.scan(analysis_targets)
+        """Extracts data from gzip archive and launches data_scan"""
+        candidates = []
+        try:
+            with gzip.open(io.BytesIO(data_provider.data)) as f:
+                new_path = data_provider.file_path if ".gz" != Util.get_extension(
+                    data_provider.file_path) else data_provider.file_path[:-3]
+                gzip_content_provider = DataContentProvider(data=f.read(),
+                                                            file_path=data_provider.file_path,
+                                                            file_type=Util.get_extension(new_path),
+                                                            info=f"{data_provider.info}|GZIP|{new_path}")
+                new_limit = recursive_limit_size - len(gzip_content_provider.data)
+                gzip_candidates = self.recursive_scan(gzip_content_provider, depth, new_limit)
+                candidates.extend(gzip_candidates)
+        except Exception as gzip_exc:
+            logger.error(f"{data_provider.file_path}:{gzip_exc}")
+        return candidates
```

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/deep_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/deep_scanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,16 +89,15 @@
                                                                   int) else RECURSIVE_SCAN_LIMITATION
         candidates: List[Candidate] = []
         data: Optional[bytes] = None
         if isinstance(content_provider, TextContentProvider) or isinstance(content_provider, ByteContentProvider):
             # Feature to scan files which might be containers
             data = content_provider.data
         elif isinstance(content_provider, DiffContentProvider) and content_provider.diff:
-            analysis_targets = content_provider.get_analysis_target()
-            candidates = self.scanner.scan(analysis_targets)
+            candidates = self.scanner.scan(content_provider)
             # Feature to scan binary diffs
             diff = content_provider.diff[0].get("line")
             # the check for legal fix mypy issue
             if isinstance(diff, bytes):
                 data = diff
         else:
             logger.warning(f"Content provider {type(content_provider)} does not support deep scan")
@@ -216,26 +215,24 @@
                 # use key = "value" scan for common cases like in TOML
                 if isinstance(struct_provider.struct, dict):
                     line = f"{key} = \"{value}\""
                     str_provider = StringContentProvider([line],
                                                          file_path=struct_provider.file_path,
                                                          file_type=".toml",
                                                          info=f"{struct_provider.info}|STRING:`{line}`")
-                    str_analysis_targets = str_provider.get_analysis_target()
-                    new_candidates = self.scanner.scan(str_analysis_targets)
+                    new_candidates = self.scanner.scan(str_provider)
                     augment_candidates(candidates, new_candidates)
             elif isinstance(value, int) or isinstance(value, float):
                 pass
             else:
                 logger.debug("Not supported type:%s value(%s)", str(type(value)), str(value))
 
         # last check when dictionary is {"key": "api_key", "value": "XXXXXXX"} -> {"api_key": "XXXXXXX"}
         if isinstance(struct_key, str) and isinstance(struct_value, str):
             line = f"{struct_key} = \"{struct_value}\""
             key_value_provider = StringContentProvider([line],
                                                        file_path=struct_provider.file_path,
                                                        file_type=".toml",
                                                        info=f"{struct_provider.info}|STRING:`{line}`")
-            key_value_analysis_targets = key_value_provider.get_analysis_target()
-            new_candidates = self.scanner.scan(key_value_analysis_targets)
+            new_candidates = self.scanner.scan(key_value_provider)
             augment_candidates(candidates, new_candidates)
         return candidates
```

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/html_scanner.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,10 +21,9 @@
         """Tries to represent data as html text and scan as text lines"""
         if data_provider.represent_as_html():
             string_data_provider = StringContentProvider(lines=data_provider.lines,
                                                          line_numbers=data_provider.line_numbers,
                                                          file_path=data_provider.file_path,
                                                          file_type=data_provider.file_type,
                                                          info=f"{data_provider.info}|HTML")
-            analysis_targets = string_data_provider.get_analysis_target()
-            return self.scanner.scan(analysis_targets)
+            return self.scanner.scan(string_data_provider)
         return []
```

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/lang_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,13 +50,12 @@
                         pass
                     else:
                         logger.error(f"Unsupported {element}")
             string_data_provider = StringContentProvider(lines=pdf_lines,
                                                          file_path=data_provider.file_path,
                                                          file_type=data_provider.file_type,
                                                          info=f"{data_provider.info}|PDF")
-            analysis_targets = string_data_provider.get_analysis_target()
-            pdf_candidates = self.scanner.scan(analysis_targets)
+            pdf_candidates = self.scanner.scan(string_data_provider)
             candidates.extend(pdf_candidates)
         except Exception as pdf_exc:
             logger.error(f"{data_provider.file_path}:{pdf_exc}")
         return candidates
```

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/tar_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/xml_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/xml_scanner.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,10 +21,9 @@
         """Tries to represent data as xml text and scan as text lines"""
         if data_provider.represent_as_xml():
             string_data_provider = StringContentProvider(lines=data_provider.lines,
                                                          line_numbers=data_provider.line_numbers,
                                                          file_path=data_provider.file_path,
                                                          file_type=data_provider.file_type,
                                                          info=f"{data_provider.info}|XML")
-            analysis_targets = string_data_provider.get_analysis_target()
-            return self.scanner.scan(analysis_targets)
+            return self.scanner.scan(string_data_provider)
         return []
```

### Comparing `credsweeper-1.5.2/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.5.3/credsweeper/deep_scanner/zip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/__init__.py` & `credsweeper-1.5.3/credsweeper/file_handler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 __all__ = [
     'ByteContentProvider',  #
     'ContentProvider',  #
     'DataContentProvider',  #
     'DiffContentProvider',  #
     'StringContentProvider',  #
-    'TextContentProvider'
+    'TextContentProvider',  #
 ]
```

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.5.3/credsweeper/file_handler/byte_content_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Generator
 
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.file_handler.content_provider import ContentProvider
 from credsweeper.utils import Util
 
 
 class ByteContentProvider(ContentProvider):
@@ -41,15 +41,18 @@
         return self.__lines if self.__lines is not None else []
 
     @lines.setter
     def lines(self, lines: List[str]) -> None:
         """lines setter for ByteContentProvider"""
         self.__lines = lines
 
-    def get_analysis_target(self) -> List[AnalysisTarget]:
+    def yield_analysis_target(self, min_len: int) -> Generator[AnalysisTarget, None, None]:
         """Return lines to scan.
 
+        Args:
+            min_len: minimal line length to scan
+
         Return:
             list of analysis targets based on every row in a content
 
         """
-        return self.lines_to_targets(self.lines)
+        return self.lines_to_targets(min_len, self.lines)
```

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/content_provider.py` & `credsweeper-1.5.3/credsweeper/file_handler/text_content_provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,82 @@
-from abc import ABC, abstractmethod
-from typing import List, Optional
+import io
+import logging
+from pathlib import Path
+from typing import List, Optional, Union, Tuple, Generator
 
 from credsweeper.file_handler.analysis_target import AnalysisTarget
+from credsweeper.file_handler.content_provider import ContentProvider
 from credsweeper.utils import Util
 
+logger = logging.getLogger(__name__)
 
-class ContentProvider(ABC):
-    """Base class to provide access to analysis targets for scanned object."""
 
-    def __init__(
-            self,  #
-            file_path: Optional[str] = None,  #
-            file_type: Optional[str] = None,  #
-            info: Optional[str] = None) -> None:
-        """
-        Parameters:
-            file_path: optional string. Might be specified if you know the file name where data were taken from.
-            file_type: optional string. File extension e.g. ".java". It might be obtained from file_path if not given.
-            info: optional string. Any information to help understand how a credential was found.
+class TextContentProvider(ContentProvider):
+    """Provide access to analysis targets for full-text file scanning.
 
-        """
-        self.file_path: str = file_path
-        self.file_type: str = file_type if file_type is not None else Util.get_extension(file_path)
-        self.info: str = info
-
-    @abstractmethod
-    def get_analysis_target(self) -> List[AnalysisTarget]:
-        """Load and preprocess file diff data to scan.
+    Parameters:
+        file_path: string, path to file
 
-        Return:
-            row objects to analysing
-
-        """
-        raise NotImplementedError()
+    """
+
+    def __init__(self,
+                 file_path: Union[str, Path, Tuple[Union[str, Path], io.BytesIO]],
+                 file_type: Optional[str] = None,
+                 info: Optional[str] = None) -> None:
+        _path = str(file_path[0]) if isinstance(file_path, tuple) else str(file_path)
+        self.__io = file_path[1] if isinstance(file_path, tuple) else None
+        self.__data: Optional[bytes] = None
+        self.__lines: Optional[List[str]] = None
+        super().__init__(file_path=_path, file_type=file_type, info=info)
 
     @property
-    def file_path(self) -> str:
-        """file_path getter"""
-        return self.__file_path
-
-    @file_path.setter
-    def file_path(self, _file_path: str) -> None:
-        """file_path setter"""
-        self.__file_path = _file_path if _file_path else ""
+    def data(self) -> Optional[bytes]:
+        """data getter for TextContentProvider"""
+        if self.__data is None:
+            if isinstance(self.__io, io.BytesIO) and self.__io:
+                self.__data = self.__io.read()
+            else:
+                self.__data = Util.read_data(self.file_path)
+        return self.__data
 
-    @property
-    def file_type(self) -> str:
-        """file_type getter"""
-        return self.__file_type
-
-    @file_type.setter
-    def file_type(self, _file_type: str) -> None:
-        """file_type setter"""
-        self.__file_type = _file_type if _file_type else ""
+    @data.setter
+    def data(self, data: Optional[bytes]) -> None:
+        """data setter for TextContentProvider"""
+        self.__data = data
 
     @property
-    def info(self) -> str:
-        """info getter"""
-        return self.__info
-
-    @info.setter
-    def info(self, _info: str) -> None:
-        """info getter"""
-        self.__info = _info if _info else ""
+    def lines(self) -> Optional[List[str]]:
+        """lines getter for TextContentProvider"""
+        if self.__lines is None:
+            self.__lines = Util.decode_bytes(self.data)
+        return self.__lines if self.__lines is not None else []
+
+    @lines.setter
+    def lines(self, lines: Optional[List[str]]) -> None:
+        """lines setter for TextContentProvider"""
+        self.__lines = lines
 
-    @property
-    @abstractmethod
-    def data(self) -> Optional[bytes]:
-        """abstract data getter"""
-        raise NotImplementedError(__name__)
+    def yield_analysis_target(self, min_len: int) -> Generator[AnalysisTarget, None, None]:
+        """Load and preprocess file content to scan.
 
-    @data.setter
-    @abstractmethod
-    def data(self, data: Optional[bytes]) -> None:
-        """abstract data setter"""
-        raise NotImplementedError(__name__)
+        Args:
+            min_len: minimal line length to scan
+
+        Return:
+            list of analysis targets based on every row in file
+
+        """
+        lines: Optional[List[str]] = None
+        line_nums: Optional[List[int]] = None
+
+        if Util.get_extension(self.file_path) == ".xml":
+            try:
+                # append line ending for correct xml line numeration
+                xml_lines = [f"{line}\n" for line in self.lines]
+                lines, line_nums = Util.get_xml_from_lines(xml_lines)
+            except Exception as exc:
+                logger.error(f"Cannot parse to xml {exc}")
+
+        if lines is None:
+            lines = self.lines
 
-    def lines_to_targets(self, lines: List[str], line_nums: Optional[List[int]] = None) -> List[AnalysisTarget]:
-        """Creates list of targets with multiline concatenation"""
-        targets = []
-        if line_nums:
-            for line, line_num in zip(lines, line_nums):
-                target = AnalysisTarget(line, line_num, lines, self.file_path, self.file_type, self.info)
-                targets.append(target)
-        else:
-            for i, line in enumerate(lines):
-                target = AnalysisTarget(line, i + 1, lines, self.file_path, self.file_type, self.info)
-                targets.append(target)
-        return targets
+        return self.lines_to_targets(min_len, lines, line_nums)
```

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.5.3/credsweeper/file_handler/data_content_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 import json
 import logging
 import string
-from typing import List, Optional, Any
+from typing import List, Optional, Any, Generator
 
 import yaml
 from bs4 import BeautifulSoup
 
 from credsweeper.common.constants import DEFAULT_ENCODING
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.file_handler.content_provider import ContentProvider
@@ -220,15 +220,18 @@
                 validate=True)  #
         except Exception as exc:
             logger.debug("Cannot decoded as base64:%s %s", exc, self.data)
         else:
             return self.decoded is not None and 0 < len(self.decoded)
         return False
 
-    def get_analysis_target(self) -> List[AnalysisTarget]:
+    def yield_analysis_target(self, min_len: int) -> Generator[AnalysisTarget, None, None]:
         """Return nothing. The class provides only data storage.
 
+        Args:
+            min_len: minimal line length to scan
+
         Raise:
             NotImplementedError
 
         """
         raise NotImplementedError()
```

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.5.3/credsweeper/file_handler/diff_content_provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import List, Tuple
+from typing import List, Tuple, Generator
 
 from credsweeper.common.constants import DiffRowType
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.file_handler.content_provider import ContentProvider
 from credsweeper.utils import DiffRowData, Util, DiffDict
 
 logger = logging.getLogger(__name__)
@@ -55,42 +55,28 @@
             lines_data: data of all rows mentioned in diff file
 
         Return:
             tuple of line numbers with change type "self.change_type" and all file lines
             in original order(replaced all lines not mentioned in diff file with blank line)
 
         """
-        max_line_numbs = max(x.line_numb for x in lines_data) if lines_data else 0
-        # fix case when whatthepatch parses wrong patch - some exceptions are possibly
-        max_line_numbs = max(max_line_numbs, len(lines_data))
-        all_lines = [""] * max_line_numbs
         change_numbs = []
+        all_lines = []
         for line_data in lines_data:
-            if line_data.line_type.value.startswith(self.change_type.value):
-                all_lines[line_data.line_numb - 1] = line_data.line
             if line_data.line_type == self.change_type:
                 change_numbs.append(line_data.line_numb)
+                all_lines.append(line_data.line)
         return change_numbs, all_lines
 
-    def get_analysis_target(self) -> List[AnalysisTarget]:
+    def yield_analysis_target(self, min_len: int) -> Generator[AnalysisTarget, None, None]:
         """Preprocess file diff data to scan.
 
+        Args:
+            min_len: minimal line length to scan
+
         Return:
             list of analysis targets of every row of file diff corresponding to change type "self.change_type"
 
         """
         lines_data = Util.preprocess_file_diff(self.diff)
-        try:
-            change_numbs, all_lines = self.parse_lines_data(lines_data)
-            return [
-                AnalysisTarget(
-                    all_lines[l_numb - 1],  #
-                    l_numb,  #
-                    all_lines,  #
-                    self.file_path,  #
-                    self.file_type,  #
-                    self.change_type.value)  #
-                for l_numb in change_numbs
-            ]
-        except Exception as exc:
-            logger.error(f"Wrong diff {type(exc)} {exc}")
-        return []
+        change_numbs, all_lines = self.parse_lines_data(lines_data)
+        return self.lines_to_targets(min_len, all_lines, change_numbs)
```

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.5.3/credsweeper/file_handler/file_path_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,24 +123,26 @@
         Args:
             config: Config
             path: str - full path preferred
 
         Return:
             True when the file full path should be excluded according config
         """
-        path = path.replace('\\', '/').lower()
-        if config.not_allowed_path_pattern.match(path):
+        path = path.replace('\\', '/')
+        lower_path = path.lower()
+        if config.not_allowed_path_pattern.match(lower_path):
             return True
         for exclude_pattern in config.exclude_patterns:
-            if exclude_pattern.match(path):
+            if exclude_pattern.match(lower_path):
                 return True
         for exclude_path in config.exclude_paths:
+            # must be case-sensitive
             if exclude_path in path:
                 return True
-        file_extension = Util.get_extension(path, lower=False)
+        file_extension = Util.get_extension(lower_path, lower=False)
         if file_extension in config.exclude_extensions:
             return True
         if not config.depth and file_extension in config.exclude_containers:
             return True
         return False
 
     @staticmethod
```

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/files_provider.py` & `credsweeper-1.5.3/credsweeper/file_handler/files_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/patch_provider.py` & `credsweeper-1.5.3/credsweeper/file_handler/patch_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.5.3/credsweeper/file_handler/string_content_provider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Generator
 
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.file_handler.content_provider import ContentProvider
 
 
 class StringContentProvider(ContentProvider):
     """Provider performs scan simple text lines"""
@@ -33,18 +33,18 @@
         raise NotImplementedError(__name__)
 
     @data.setter
     def data(self, data: bytes) -> None:
         """data setter for StringContentProvider"""
         raise NotImplementedError(__name__)
 
-    def get_analysis_target(self) -> List[AnalysisTarget]:
+    def yield_analysis_target(self, min_len: int) -> Generator[AnalysisTarget, None, None]:
         """Return lines to scan.
 
+        Args:
+            min_len: minimal line length to scan
+
         Return:
             list of analysis targets based on every row in file
 
         """
-        return [
-            AnalysisTarget(line, line_number, self.lines, self.file_path, self.file_type, self.info)
-            for line_number, line in zip(self.line_numbers, self.lines)
-        ]
+        return self.lines_to_targets(min_len, self.lines, self.line_numbers)
```

### Comparing `credsweeper-1.5.2/credsweeper/file_handler/text_provider.py` & `credsweeper-1.5.3/credsweeper/file_handler/text_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/__init__.py` & `credsweeper-1.5.3/credsweeper/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/cred_card_number_check.py` & `credsweeper-1.5.3/credsweeper/filters/cred_card_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/filter.py` & `credsweeper-1.5.3/credsweeper/filters/filter.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/group/__init__.py` & `credsweeper-1.5.3/credsweeper/filters/group/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/group/group.py` & `credsweeper-1.5.3/credsweeper/filters/group/group.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,32 +31,33 @@
     def filters(self, filters: List[Filter]) -> None:
         """property setter"""
         self.__filters = filters
 
     @staticmethod
     def get_keyword_base_filters(config: Config) -> List[Filter]:
         """returns base filters"""
-        return [  #
+        filters = [  #
             SeparatorUnusualCheck(),
             ValueAllowlistCheck(),
             ValueArrayDictionaryCheck(),
             ValueBlocklistCheck(),
             ValueCamelCaseCheck(),
             ValueFilePathCheck(),
             ValueFirstWordCheck(),
             ValueLastWordCheck(),
             ValueLengthCheck(config),
             ValueMethodCheck(),
-            ValueNotAllowedPatternCheck(),
             ValueSimilarityCheck(),
             ValueStringTypeCheck(config),
             ValueTokenCheck(),
             VariableNotAllowedPatternCheck(),
-            ValuePatternCheck(config)
         ]
+        if not config.doc:
+            filters.extend([ValuePatternCheck(config), ValueNotAllowedPatternCheck()])
+        return filters
 
     @staticmethod
     def get_pattern_base_filters(config: Config) -> List[Filter]:
         """return base filters for pattern"""
         return [  #
             LineSpecificKeyCheck(),  #
             ValuePatternCheck(config),  #
```

### Comparing `credsweeper-1.5.2/credsweeper/filters/group/token_pattern.py` & `credsweeper-1.5.3/credsweeper/filters/group/token_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.5.3/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/group/weird_base36_token.py` & `credsweeper-1.5.3/credsweeper/filters/group/weird_base36_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/group/weird_base64_token.py` & `credsweeper-1.5.3/credsweeper/filters/group/weird_base64_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.5.3/credsweeper/filters/line_specific_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.5.3/credsweeper/filters/separator_unusual_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_allowlist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_array_dictionary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_base32_data_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_base32_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_base64_data_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_base64_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_blocklist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_camel_case_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_couple_keyword_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_couple_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_entropy_base32_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_entropy_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_entropy_base36_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_entropy_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_entropy_base64_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_entropy_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_file_path_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_first_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_grafana_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_grafana_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_json_web_token_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_json_web_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_last_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_length_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_method_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_method_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_not_part_encoded_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_not_part_encoded_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Optional
-
 import re
+from typing import Optional
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
@@ -30,15 +29,15 @@
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
 
         if line_data.line_num == target.line_num \
-                and line_data.line_len == target.line_len \
+                and len(line_data.line) == target.line_len \
                 and line_data.line == target.line \
                 and 0 < target.line_num <= target.lines_len \
                 and line_data.line == target.lines[target.line_num - 1]:
             # suppose, there is plain lines order
             if 1 < target.line_num:
                 result = ValueNotPartEncodedCheck._check_val(
                     target.lines[line_data.line_num - 2], ValueNotPartEncodedCheck.BASE64_ENCODED_DATA_PATTERN_BEFORE)
```

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_number_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_pem_pattern_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_pem_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_similarity_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_split_keyword_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_split_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_string_type_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_structured_token_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_structured_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_token_base32_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_token_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_token_base36_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_token_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_token_base64_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_token_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_token_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.5.3/credsweeper/filters/value_useless_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.5.3/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/logger/logger.py` & `credsweeper-1.5.3/credsweeper/logger/logger.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/ml_model/features.py` & `credsweeper-1.5.3/credsweeper/ml_model/features.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/ml_model/ml_model.onnx` & `credsweeper-1.5.3/credsweeper/ml_model/ml_model.onnx`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.5.3/credsweeper/ml_model/ml_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/ml_model/model_config.json` & `credsweeper-1.5.3/credsweeper/ml_model/model_config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/rules/config.yaml` & `credsweeper-1.5.3/credsweeper/rules/config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -2,965 +2,775 @@
   severity: info
   type: pattern
   values:
     - (?<!([0-9]\.|[=*+\/\-] |.[=*+\/\-]))((?<![0-9A-Za-z_=*+\-\/.])(?P<value>[0-9]{16})(?![0-9A-Za-z_=*+\-\/.]))(?!(\.[0-9]| [=*+\/\-]|.[=*+\/\-]))
   filter_type:
     - CreditCardNumberCheck
   min_line_len: 16
-  usage_list:
-    - src
+  doc_available: false
 
 - name: API
   severity: medium
   type: keyword
   values:
     - api
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 11
   required_substrings:
     - api
-  usage_list:
-    - src
+  doc_available: false
 
 - name: AWS Client ID
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>(ABIA|ACCA|AGPA|AIDA|AIPA|AKIA|ANPA|ANVA|AROA|APKA|ASCA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - A
   min_line_len: 20
-  usage_list:
-    - src
-    - doc
 
 - name: AWS Multi
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>(AKIA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
     - (?P<value>[0-9a-zA-Z/+]{40})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - AKIA
     - ASIA
   min_line_len: 20
-  usage_list:
-    - src
-    - doc
 
 - name: AWS MWS Key
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>amzn\.mws\.[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - amzn
   min_line_len: 30
-  usage_list:
-    - src
-    - doc
 
 - name: Credential
   severity: medium
   type: keyword
   values:
     - credential
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 18
   required_substrings:
     - credential
-  usage_list:
-    - src
+  doc_available: false
 
 - name: Dynatrace API Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>dt0[a-zA-Z]{1}[0-9]{2}\.[A-Z0-9]{24}\.[A-Z0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - dt0
   min_line_len: 90
-  usage_list:
-    - src
-    - doc
 
 - name: Facebook Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>EAAC[0-9A-Za-z]{27,})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - EAAC
   min_line_len: 31
-  usage_list:
-    - src
-    - doc
 
 - name: Github Old Token
   severity: high
   type: pattern
   values:
     - (?i)((git)[\w\-]*(token|key|api)[\w\-]*(\s)*(=|:|:=)(\s)*(["']?)(?P<value>[a-z|\d]{40})(["']?))
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - GithubTokenValidation
   required_substrings:
     - git
   min_line_len: 47
-  usage_list:
-    - src
-    - doc
 
 - name: Google API Key
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>AIza[0-9A-Za-z_-]{35})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   validations:
     - GoogleApiKeyValidation
   required_substrings:
     - AIza
   min_line_len: 39
-  usage_list:
-    - src
-    - doc
 
 - name: Google Multi
   severity: high
   type: pattern
   values:
     - (?P<value>[0-9]+\-[0-9A-Za-z_]{32}\.apps\.googleusercontent\.com)
     - (?<![0-9a-zA-Z_-])(?P<value>[0-9a-zA-Z_-]{24})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   validations:
     - GoogleMultiValidation
   required_substrings:
     - .apps.googleusercontent.com
   min_line_len: 40
-  usage_list:
-    - src
-    - doc
 
 - name: Google OAuth Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>ya29\.[0-9A-Za-z_-]{22,})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - ya29.
   min_line_len: 27
-  usage_list:
-    - src
-    - doc
 
 - name: Heroku API Key
   severity: high
   type: pattern
   values:
     - (?P<value>(?i)heroku(.{0,20})?[0-9a-f]{8}(-[0-9a-f]{4})+-[0-9a-f]{12})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - heroku
   min_line_len: 24
-  usage_list:
-    - src
-    - doc
 
 - name: Instagram Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>IGQVJ[\w]{100,})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - IGQVJ
   min_line_len: 105
-  usage_list:
-    - src
-    - doc
 
 - name: JSON Web Token
   severity: medium
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>eyJ[A-Za-z0-9=_-]{13,}(\.[A-Za-z0-9-_.+\/=]+)?)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - eyJ
   min_line_len: 16
-  usage_list:
-    - src
-    - doc
 
 - name: MailChimp API Key
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[0-9a-zA-Z]{32}-us[0-9]{1,2})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   validations:
     - MailChimpKeyValidation
   required_substrings:
     - -us
   min_line_len: 35
-  usage_list:
-    - src
-    - doc
 
 - name: MailGun API Key
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>key-[0-9a-zA-Z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - key-
   min_line_len: 36
-  usage_list:
-    - src
-    - doc
 
 - name: Password
   severity: medium
   type: keyword
   values:
-    - pass|pwd
+    - pass|pw(d|\b)
   filter_type: PasswordKeyword
   use_ml: true
   min_line_len: 10
   required_substrings:
     - pass
-    - pwd
-  usage_list:
-    - src
+    - pw
 
 - name: PayPal Braintree Access Token
   severity: high
   type: pattern
   values:
     - (?P<value>access_token\$production\$[0-9a-z]{16}\$[0-9a-z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   required_substrings:
     - access_token$production$
   min_line_len: 72
-  usage_list:
-    - src
-    - doc
 
 - name: PEM Private Key
   severity: high
   type: pem_key
   values:
     - (?P<value>-----BEGIN\s(?!ENCRYPTED|EC)[^-]*PRIVATE[^-]*KEY[^-]*-----(.+-----END[^-]+-----)?)
   filter_type:
     - LineSpecificKeyCheck
   min_line_len: 27
-  usage_list:
-    - src
-    - doc
 
 - name: Picatic API Key
   severity: high
   type: pattern
   values:
     - (?P<value>sk_live_[0-9a-z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   required_substrings:
     - sk_live_
   min_line_len: 40
-  usage_list:
-    - src
-    - doc
 
 - name: Secret
   severity: medium
   type: keyword
   values:
     - secret
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 14
   required_substrings:
     - secret
-  usage_list:
-    - src
+  doc_available: false
 
 - name: SendGrid API Key
   severity: high
   type: pattern
   values:
     - (?P<value>SG\.[\w_]{16,32}\.[\w_]{16,64})
   filter_type: GeneralPattern
   use_ml: false
   required_substrings:
     - SG.
   min_line_len: 34
-  usage_list:
-    - src
-    - doc
 
 - name: Shopify Token
   severity: high
   type: pattern
   values:
     - (?P<value>shp(at|ca|pa|ss)_[a-fA-F0-9]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   required_substrings:
     - shp
   min_line_len: 38
-  usage_list:
-    - src
-    - doc
 
 - name: Slack Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>xox[a|b|p|r|o|s]\-[-a-zA-Z0-9]{10,250})
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - SlackTokenValidation
   required_substrings:
     - xox
   min_line_len: 15
-  usage_list:
-    - src
-    - doc
 
 - name: Slack Webhook
   severity: high
   type: pattern
   values:
     - (?P<value>hooks\.slack\.com/services/T\w{8}/B\w{8}/\w{24})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - hooks.slack.com/services/T
   min_line_len: 61
-  usage_list:
-    - src
-    - doc
 
 - name: Stripe Standard API Key
   severity: high
   type: pattern
   values:
     - (?P<value>sk_live_[0-9a-zA-Z]{24})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - StripeApiKeyValidation
   required_substrings:
     - sk_live_
   min_line_len: 32
-  usage_list:
-    - src
-    - doc
 
 - name: Stripe Restricted API Key
   severity: high
   type: pattern
   values:
     - (?P<value>rk_live_[0-9a-zA-Z]{24})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - rk_live_
   min_line_len: 32
-  usage_list:
-    - src
-    - doc
 
 - name: Square Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>EAAA[0-9A-Za-z_-]{60})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - SquareAccessTokenValidation
   required_substrings:
     - EAAA
   min_line_len: 64
-  usage_list:
-    - src
-    - doc
 
 - name: Square Client ID
   severity: medium
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>sq0[a-z]{3}-[0-9A-Za-z_-]{22})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - SquareClientIdValidation
   required_substrings:
     - sq0
   min_line_len: 29
-  usage_list:
-    - src
-    - doc
 
 - name: Square OAuth Secret
   severity: high
   type: pattern
   values:
     - (?P<value>sq0csp-[0-9A-Za-z_-]{43})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   required_substrings:
     - sq0csp
   min_line_len: 50
-  usage_list:
-    - src
-    - doc
 
 - name: Token
   severity: medium
   type: keyword
   values:
     - token
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 13
   required_substrings:
     - token
-  usage_list:
-    - src
+  doc_available: false
 
 - name: Twilio API Key
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>SK[0-9a-fA-F]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - SK
   min_line_len: 34
-  usage_list:
-    - src
-    - doc
 
 - name: URL Credentials
   severity: high
   type: pattern
   values:
-    - //[^:]+(?P<separator>:)(?P<value>[^@]+)@
+    - ://[^:\s]+(?P<separator>:)(?P<value>[^@\s]+)@
   filter_type: UrlCredentialsGroup
   use_ml: true
   required_substrings:
-    - //
-  min_line_len: 6
-  usage_list:
-    - src
-    - doc
+    - ://
+  min_line_len: 10
+  doc_available: false
 
 - name: Auth
   severity: medium
   type: keyword
   values:
     - auth(?!or)
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 12
   required_substrings:
     - auth
-  usage_list:
-    - src
+  doc_available: false
 
 - name: Key
   severity: medium
   type: keyword
   values:
     - key(?!word)
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 11
   required_substrings:
     - key
-  usage_list:
-    - src
+  doc_available: false
 
 - name: Telegram Bot API Token
   severity: high
   type: pattern
   values:
     - (?P<value>[0-9]{8,10}:[0-9A-Za-z_-]{35})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   required_substrings:
     - :AA
   min_line_len: 45
-  usage_list:
-    - src
-    - doc
 
 - name: PyPi API Token
   severity: high
   type: pattern
   values:
     - (?P<value>pypi-[\w_\-]{150,})
   filter_type: GeneralPattern
   required_substrings:
     - pypi-
   min_line_len: 155
-  usage_list:
-    - src
-    - doc
 
 - name: Github Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>(ghr|gho|ghu|ghs)_[\w]{36,255})
   filter_type: GeneralPattern
   required_substrings:
     - gh
   min_line_len: 40
-  usage_list:
-    - src
-    - doc
 
 - name: Github Personal Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>ghp_[\w]{36,255})
   filter_type: GeneralPattern
   validations:
     - GithubTokenValidation
   required_substrings:
     - ghp_
   min_line_len: 40
-  usage_list:
-    - src
-    - doc
 
 - name: Github Fine-granted Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>github_pat_[0-9A-Za-z_]{80,255})
   filter_type: GeneralPattern
   validations:
     - GithubTokenValidation
   required_substrings:
     - github_pat_
   min_line_len: 90
-  usage_list:
-    - src
-    - doc
 
 - name: Firebase Domain
   severity: info
   type: pattern
   values:
     - (?P<value>[a-z0-9.-]+\.firebaseio\.com|[a-z0-9.-]+\.firebaseapp\.com)
   filter_type: GeneralPattern
   required_substrings:
     - .firebase
   min_line_len: 16
-  usage_list:
-    - src
-    - doc
 
 - name: AWS S3 Bucket
   severity: info
   type: pattern
   values:
     - (?P<value>[a-z0-9.-]+\.s3\.amazonaws\.com|[a-z0-9.-]+\.s3-website[.-](eu|ap|us|ca|sa|cn))
   filter_type: GeneralPattern
   required_substrings:
     - .s3-website
     - .s3.amazonaws.com
   min_line_len: 14
-  usage_list:
-    - src
-    - doc
 
 - name: Nonce
   severity: medium
   type: keyword
   values:
     - nonce
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 13
   required_substrings:
     - nonce
-  usage_list:
-    - src
+  doc_available: false
 
 - name: Salt
   severity: medium
   type: keyword
   values:
     - salt
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 12
   required_substrings:
     - salt
-  usage_list:
-    - src
+  doc_available: false
 
 - name: Certificate
   severity: medium
   type: keyword
   values:
     - cert
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 12
   required_substrings:
     - cert
-  usage_list:
-    - src
+  doc_available: false
 
 - name: Azure Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>eyJ[A-Za-z0-9_=-]{50,500}\.eyJ[A-Za-z0-9_=-]+\.[A-Za-z0-9_=-]+)
   filter_type:
     - ValueJsonWebTokenCheck
   required_substrings:
     - eyJ
   min_line_len: 148
-  usage_list:
-    - src
-    - doc
 
 - name: Azure Secret Value
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9_~.-]{3}8Q~[a-zA-Z0-9_~.-]{34})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 40
   required_substrings:
     - 8Q~
-  usage_list:
-    - src
-    - doc
 
 - name: Bitbucket App Password
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>ATBB[A-Za-z0-9]{24}[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 28
   required_substrings:
     - ATBB
-  usage_list:
-    - src
-    - doc
 
 - name: Bitbucket Repository Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>ATCTT3xFfGN0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 183
   required_substrings:
     - ATCTT3xFfGN0
-  usage_list:
-    - src
-    - doc
 
 - name: Bitbucket HTTP Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>BBDC-[NMO][ADgjQTwz][A-Za-z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 49
   required_substrings:
     - BBDC-
-  usage_list:
-    - src
-    - doc
 
 - name: Bitbucket Client ID
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9]{18}([a-zA-Z0-9]{14})?)([^0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 18
-  usage_list:
-    - src
-    - doc
 
 - name: Bitbucket Client Secret
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>([a-zA-Z0-9_-]{32}){1,2})([^0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 32
-  usage_list:
-    - src
-    - doc
 
 - name: Jira / Confluence PAT token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[NMO][ADgjQTwz][a-zA-Z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 44
   required_substrings:
     - M
     - N
     - O
-  usage_list:
-    - src
-    - doc
 
 - name: Atlassian Old PAT token
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9]{24})([^=0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 24
-  usage_list:
-    - src
-    - doc
 
 - name: Atlassian PAT token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>ATATT3xFfGF0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 191
   required_substrings:
     - ATATT3xFfGF0
-  usage_list:
-    - src
-    - doc
 
 - name: Digital Ocean PAT
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>dop_v1_[a-f0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 71
   required_substrings:
     - dop_v1_
-  usage_list:
-    - src
-    - doc
 
 - name: Digital Ocean OAuth Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>doo_v1_[a-f0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 71
   required_substrings:
     - doo_v1_
-  usage_list:
-    - src
-    - doc
 
 - name: Dropbox OAuth2 API Access Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>sl.[A-Za-z0-9_-]{135})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 138
   required_substrings:
     - sl.
-  usage_list:
-    - src
-    - doc
 
 - name: NuGet API key
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>oy2[a-z0-9]{43})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 46
   required_substrings:
     - oy2
-  usage_list:
-    - src
-    - doc
 
 - name: Gitlab PAT
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>glpat-[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 26
   required_substrings:
     - glpat-
-  usage_list:
-    - src
-    - doc
 
 - name: Gitlab Pipeline Trigger Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>glptt-[a-f0-9]{40})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 46
   required_substrings:
     - glptt-
-  usage_list:
-    - src
-    - doc
 
 - name: Gitlab Registration Runner Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>GR1348941[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 29
   required_substrings:
     - GR1348941
-  usage_list:
-    - src
-    - doc
 
 - name: Gitlab Registration Runner Token 2023
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>glrt-[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 25
   required_substrings:
     - glrt-
-  usage_list:
-    - src
-    - doc
 
 - name: Grafana Provisioned API Key
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>eyJ[a-zA-Z0-9=/-]{64,360})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueGrafanaCheck
   min_line_len: 67
   required_substrings:
     - eyJ
-  usage_list:
-    - src
-    - doc
 
 - name: Grafana Access Policy Token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>glc_eyJ[a-zA-Z0-9=/-]{80,360})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueGrafanaCheck
   min_line_len: 87
   required_substrings:
     - glc_eyJ
-  usage_list:
-    - src
-    - doc
 
 - name: Dropbox API secret (long term)
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?=[A-Za-z0-9]{64})(?P<value>[A-Za-z0-9]{10,12}[B-Za-z0-9]A{10,12}[B-Za-z0-9][A-Za-z0-9]{40,44})([^=0-9A-Za-z_/+-]|$)
   filter_type: []
   min_line_len: 43
   required_substrings:
     - AAAAAAAAAA
-  usage_list:
-    - src
-    - doc
 
 - name: Dropbox App secret
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-z0-9]{15})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase36Token
   min_line_len: 15
-  usage_list:
-    - src
-    - doc
 
 - name: Gitlab Incoming Email Token
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-z0-9]{24,25})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase36Token
   min_line_len: 24
-  usage_list:
-    - src
-    - doc
 
 - name: Gitlab Feed Token
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 20
-  usage_list:
-    - src
-    - doc
 
 - name: Jira 2FA
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[A-Z2-7]{16})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueCoupleKeywordCheck
     - ValuePatternCheck
     - ValueEntropyBase32Check
     - ValueBase32DataCheck
     - ValueTokenBase32Check
   min_line_len: 16
-  usage_list:
-    - src
-    - doc
+  doc_available: true
```

### Comparing `credsweeper-1.5.2/credsweeper/rules/rule.py` & `credsweeper-1.5.3/credsweeper/rules/rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,23 +41,24 @@
     MULTI_PATTERN = "multi_pattern"
     PEM_KEY_PATTERN = "pem_key_pattern"
 
     # mandatory fields
     NAME = "name"
     SEVERITY = "severity"
     TYPE = "type"
-    USAGE_LIST = "usage_list"
     VALUES = "values"
     FILTER_TYPE = "filter_type"
     MIN_LINE_LEN = "min_line_len"
 
     # auxiliary fields
     USE_ML = "use_ml"
     REQUIRED_SUBSTRINGS = "required_substrings"
+    REQUIRED_REGEX = "required_regex"
     VALIDATIONS = "validations"
+    DOC_AVAILABLE = "doc_available"  # True - by default
 
     def __init__(self, config: Config, rule_dict: Dict) -> None:
         self.config = config
         self._assert_rule_mandatory_fields(rule_dict)
         # mandatory fields
         self.__rule_name = str(rule_dict[Rule.NAME])
         if severity := Severity.get(rule_dict[Rule.SEVERITY]):
@@ -68,19 +69,26 @@
             self.__rule_type: RuleType = rule_type
         else:
             self._malformed_rule_error(rule_dict, Rule.TYPE)
         self.__patterns = Rule._get_patterns(self.rule_type, rule_dict[Rule.VALUES])
         # auxiliary fields
         self.__filters = self._get_filters(rule_dict.get(Rule.FILTER_TYPE))
         self.__pattern_type = Rule._get_pattern_type(self.rule_type, len(self.patterns))
+        if 2 < len(self.__patterns):
+            logger.warning(f"Rule {self.rule_name} has extra patterns. Only two patterns supported.")
         self.__use_ml = bool(rule_dict.get(Rule.USE_ML))
         self.__validations = self._get_validations(rule_dict.get(Rule.VALIDATIONS))
         self.__required_substrings = [i.strip().lower() for i in rule_dict.get(Rule.REQUIRED_SUBSTRINGS, [])]
+        self.__has_required_substrings = bool(self.__required_substrings)
+        required_regex = rule_dict.get(Rule.REQUIRED_REGEX)
+        if required_regex and not isinstance(required_regex, str):
+            self._malformed_rule_error(rule_dict, Rule.REQUIRED_REGEX)
+        self.__required_regex = re.compile(required_regex) if required_regex else None
         self.__min_line_len = int(rule_dict.get(Rule.MIN_LINE_LEN, MAX_LINE_LENGTH))
-        self.__usage_list: List[str] = rule_dict.get(Rule.USAGE_LIST, [])
+        self.__doc_available: bool = rule_dict.get(Rule.DOC_AVAILABLE, True)
 
     def _malformed_rule_error(self, rule_dict: Dict, field: str):
         raise ValueError(f"Malformed rule '{self.__rule_name}'."
                          f" field '{field}' has invalid value"
                          f" '{rule_dict.get(field)}'")
 
     @cached_property
@@ -238,28 +246,36 @@
         Args:
             rule_template: dictionary loaded from the config file
 
         Raises:
             ValueError if missing fields is present
 
         """
-        mandatory_fields = [
-            Rule.NAME, Rule.SEVERITY, Rule.TYPE, Rule.USAGE_LIST, Rule.VALUES, Rule.FILTER_TYPE, Rule.MIN_LINE_LEN
-        ]
+        mandatory_fields = [Rule.NAME, Rule.SEVERITY, Rule.TYPE, Rule.VALUES, Rule.FILTER_TYPE, Rule.MIN_LINE_LEN]
         missing_fields = [field for field in mandatory_fields if field not in rule_template]
         if len(missing_fields) > 0:
             raise ValueError(f"Malformed rule config file. Contain rule with missing fields: {missing_fields}.")
 
     @cached_property
     def required_substrings(self) -> List[str]:
         """required_substrings getter"""
         return self.__required_substrings
 
     @cached_property
+    def has_required_substrings(self) -> bool:
+        """has_required_substrings getter for speedup"""
+        return self.__has_required_substrings
+
+    @cached_property
+    def required_regex(self) -> Optional[re.Pattern]:
+        """required_regex getter"""
+        return self.__required_regex
+
+    @cached_property
     def min_line_len(self) -> int:
         """min_line_len getter"""
         return self.__min_line_len
 
     @cached_property
-    def usage_list(self) -> List[str]:
-        """usage_list getter"""
-        return self.__usage_list
+    def doc_available(self) -> bool:
+        """doc_available getter"""
+        return self.__doc_available
```

### Comparing `credsweeper-1.5.2/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.5.3/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,55 +35,56 @@
         assert rule.pattern_type == rule.MULTI_PATTERN, \
             "Rules provided to MultiPattern.run should have pattern_type equal to MULTI_PATTERN"
 
         candidate = cls._get_candidate(config, rule, target)
         if not candidate:
             return None
 
-        line_num_margin = 1
+        line_pos_margin = 1
 
-        while line_num_margin <= cls.MAX_SEARCH_MARGIN:
-            if 1 <= candidate.line_data_list[0].line_num - line_num_margin <= len(target.lines):
-                if cls._scan(config, candidate, -line_num_margin, target, rule):
+        while line_pos_margin <= cls.MAX_SEARCH_MARGIN:
+            candi_line_pos_backward = candidate.line_data_list[0].line_pos - line_pos_margin
+            if 0 <= candi_line_pos_backward < target.lines_len:
+                if cls._scan(config, candidate, candi_line_pos_backward, target, rule):
                     break
-            if candidate.line_data_list[0].line_num + line_num_margin <= len(target.lines):
-                if cls._scan(config, candidate, line_num_margin, target, rule):
+            candi_line_pos_forward = candidate.line_data_list[0].line_pos + line_pos_margin
+            if candi_line_pos_forward < target.lines_len:
+                if cls._scan(config, candidate, candi_line_pos_forward, target, rule):
                     break
-            line_num_margin += 1
+            line_pos_margin += 1
 
         # Check if found multi line
         if len(candidate.line_data_list) == 1:
             return None
 
         return candidate
 
     @classmethod
-    def _scan(cls, config: Config, candidate: Candidate, line_num_margin: int, target: AnalysisTarget,
+    def _scan(cls, config: Config, candidate: Candidate, candi_line_pos: int, target: AnalysisTarget,
               rule: Rule) -> bool:
         """Search for second part of multiline rule near the current line.
 
         Automatically update candidate with detected line if any.
 
         Args:
             config: dict, scanner configuration
             candidate: Current credential candidate detected in the line
-            line_num_margin: Number of lines around candidate to perform search
+            candi_line_pos: line position of lines around candidate to perform search
             target: Analysis target
             rule: Rule object to check current line. Should be a multi-pattern rule
 
         Return:
             Boolean. True if second part detected. False otherwise
 
         """
-        candi_line_num = candidate.line_data_list[0].line_num + line_num_margin
-        candi_line = target.lines[candi_line_num - 1]
-        if MAX_LINE_LENGTH < len(candi_line):
+        new_target = AnalysisTarget(candi_line_pos, target.lines, target.line_nums, target.descriptor)
+
+        if MAX_LINE_LENGTH < new_target.line_len:
             return False
-        # lines are not necessary - skip them
-        new_target = AnalysisTarget(candi_line, candi_line_num, [], target.file_path, target.file_type, target.info)
+
         line_data = cls.get_line_data(config=config, target=new_target, pattern=rule.patterns[1], filters=rule.filters)
 
         if line_data is None:
             return False
 
         candidate.add_line_data(line_data)
         return True
```

### Comparing `credsweeper-1.5.2/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.5.3/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,28 +72,26 @@
         Return:
             List of LineData with found PEM
 
         """
         line_data: List[LineData] = []
         key_data = ""
         # get line with -----BEGIN which may contain full key
-        first_line = LineData(config, target.line, target.line_num, target.file_path, target.file_type, target.info,
-                              rule.patterns[0])
+        first_line = LineData(config, target.line, target.line_pos, target.line_num, target.file_path, target.file_type,
+                              target.info, rule.patterns[0])
         line_data.append(first_line)
         # protection check for case when first line starts from 0
-        line_num = target.line_num if 0 < target.line_num else 1
-        finish_line = line_num + 200
-        for line in target.lines[line_num - 1:]:
-            if finish_line < line_num:
-                return []
-            if 1 != line_num and target.line_num != line_num:
-                _line = LineData(config, line, line_num, target.file_path, target.file_type, target.info,
-                                 cls.re_value_pem)
+        start_pos = target.line_pos if 0 <= target.line_pos else 0
+        finish_pos = min(start_pos + 200, target.lines_len)
+        for line_pos in range(start_pos, finish_pos):
+            line = target.lines[line_pos]
+            if target.line_pos != line_pos:
+                _line = LineData(config, line, line_pos, target.line_nums[line_pos], target.file_path, target.file_type,
+                                 target.info, cls.re_value_pem)
                 line_data.append(_line)
-            line_num += 1
             # replace escaped line ends with real and process them - PEM does not contain '\' sign
             sublines = line.replace("\\r", '\n').replace("\\n", '\n').splitlines()
             for subline in sublines:
                 if cls.is_leading_config_line(subline):
                     continue
                 elif PEM_END_PATTERN in subline:
                     # Check if entropy is high enough for base64 set with padding sign
```

### Comparing `credsweeper-1.5.2/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.5.3/credsweeper/scanner/scan_type/scan_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
             LineData object if pattern a line and filters do not remove current line. None otherwise
 
         """
         if not cls.is_pattern_detected_line(target.line, pattern):
             return None
         logger.debug("Valid line for pattern: %s in file: %s:%d in line: %s", pattern, target.file_path,
                      target.line_num, target.line)
-        line_data = LineData(config, target.line, target.line_num, target.file_path, target.file_type, target.info,
-                             pattern)
+        line_data = LineData(config, target.line, target.line_pos, target.line_num, target.file_path, target.file_type,
+                             target.info, pattern)
 
         if cls.filtering(config, target, line_data, filters):
             return None
         return line_data
 
     @classmethod
     def is_pattern_detected_line(cls, line: str, pattern: re.Pattern) -> bool:
```

### Comparing `credsweeper-1.5.2/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.5.3/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/secret/config.json` & `credsweeper-1.5.3/credsweeper/secret/config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/secret/log.yaml` & `credsweeper-1.5.3/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/utils/entropy_validator.py` & `credsweeper-1.5.3/credsweeper/utils/entropy_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/utils/util.py` & `credsweeper-1.5.3/credsweeper/utils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,24 +288,21 @@
             deleted_line_number: number of deleted line or None
             line: the text line
 
         Return:
             diff rows data with as list of row change type, line number, row content
 
         """
-        rows_data = []
-        if deleted_line_number is None:
+        rows_data: List[DiffRowData] = []
+        if isinstance(added_line_number, int):
             # indicates line was inserted
             rows_data.append(DiffRowData(DiffRowType.ADDED, added_line_number, line))
-        elif added_line_number is None:
+        if isinstance(deleted_line_number, int):
             # indicates line was removed
             rows_data.append(DiffRowData(DiffRowType.DELETED, deleted_line_number, line))
-        else:
-            rows_data.append(DiffRowData(DiffRowType.ADDED_ACCOMPANY, added_line_number, line))
-            rows_data.append(DiffRowData(DiffRowType.DELETED_ACCOMPANY, deleted_line_number, line))
         return rows_data
 
     @staticmethod
     def wrong_change(change: DiffDict) -> bool:
         """Returns True if the change is wrong"""
         for i in ["line", "new", "old"]:
             if i not in change:
```

### Comparing `credsweeper-1.5.2/credsweeper/validations/__init__.py` & `credsweeper-1.5.3/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/apply_validation.py` & `credsweeper-1.5.3/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/github_token_validation.py` & `credsweeper-1.5.3/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.5.3/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.5.3/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.5.3/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.5.3/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.5.3/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.5.3/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.5.3/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper/validations/validation.py` & `credsweeper-1.5.3/credsweeper/validations/validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/credsweeper.egg-info/PKG-INFO` & `credsweeper-1.5.3/credsweeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.5.2
+Version: 1.5.3
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.5.2/credsweeper.egg-info/SOURCES.txt` & `credsweeper-1.5.3/credsweeper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 credsweeper/deep_scanner/xml_scanner.py
 credsweeper/deep_scanner/zip_scanner.py
 credsweeper/file_handler/__init__.py
 credsweeper/file_handler/analysis_target.py
 credsweeper/file_handler/byte_content_provider.py
 credsweeper/file_handler/content_provider.py
 credsweeper/file_handler/data_content_provider.py
+credsweeper/file_handler/descriptor.py
 credsweeper/file_handler/diff_content_provider.py
 credsweeper/file_handler/file_path_extractor.py
 credsweeper/file_handler/files_provider.py
 credsweeper/file_handler/patch_provider.py
 credsweeper/file_handler/string_content_provider.py
 credsweeper/file_handler/struct_content_provider.py
 credsweeper/file_handler/text_content_provider.py
```

### Comparing `credsweeper-1.5.2/setup.py` & `credsweeper-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.2/tests/test_app.py` & `credsweeper-1.5.3/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import deepdiff
 import pytest
 
 from credsweeper.app import APP_PATH
 from credsweeper.utils import Util
 from tests import AZ_STRING, SAMPLES_POST_CRED_COUNT, SAMPLES_IN_DEEP_3, SAMPLES_PATH, \
-    TESTS_PATH, SAMPLES_CRED_COUNT
+    TESTS_PATH, SAMPLES_CRED_COUNT, SAMPLES_IN_DOC
 
 
 class TestApp(TestCase):
 
     @staticmethod
     def _m_credsweeper(args) -> Tuple[str, str]:
         proc = subprocess.Popen(
@@ -448,15 +448,15 @@
             _stdout, _stderr = self._m_credsweeper(
                 ["--path", tmp_dir, "--find-by-ext", "--save-json", json_filename, "--log", "silence"])
             self.assertTrue(os.path.exists(json_filename))
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
                 self.assertEqual(4, len(report), report)
                 for t in report:
-                    self.assertEqual(-1, t["line_data_list"][0]["line_num"])
+                    self.assertEqual(0, t["line_data_list"][0]["line_num"])
                     self.assertIn(str(t["line_data_list"][0]["path"][-4:]), [".pem", ".cer", ".csr", ".deR"])
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_find_by_ext_n(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             for f in [".pem", ".cer", ".csr", ".der", ".pfx", ".p12", ".key", ".jks"]:
@@ -603,15 +603,15 @@
             rules = Util.yaml_load(APP_PATH / "rules" / "config.yaml")
             rules_set = set([i["name"] for i in rules])
             missed = {  #
             }
             self.assertSetEqual(rules_set.difference(missed), report_set, f"\n{_stdout}")
             self.assertEqual(SAMPLES_POST_CRED_COUNT, len(report))
 
-            # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_rules_ml_n(self) -> None:
         # checks whether all rules have test samples which detected without ML
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             _stdout, _stderr = self._m_credsweeper([
                 "--log",
@@ -645,7 +645,16 @@
 
     def test_severity_n(self) -> None:
         _stdout, _stderr = self._m_credsweeper([  #
             "--log", "silence", "--ml_threshold", "0", "--severity", "critical", "--path",
             str(SAMPLES_PATH)
         ])
         self.assertNotIn("severity: medium", _stdout)
+
+    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+    def test_doc_n(self) -> None:
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            json_filename = os.path.join(tmp_dir, f"{__name__}.json")
+            _stdout, _stderr = self._m_credsweeper(["--doc", "--path", str(SAMPLES_PATH), "--save-json", json_filename])
+            report = Util.json_load(json_filename)
+            self.assertEqual(SAMPLES_IN_DOC, len(report))
```

### Comparing `credsweeper-1.5.2/tests/test_main.py` & `credsweeper-1.5.3/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -696,15 +696,16 @@
 
     def test_doc_p(self) -> None:
         content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "test.html"])
         cred_sweeper = CredSweeper(doc=True)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         expected_credential_lines = [
-            "508627689:AAEuLPKs-EhrjrYGnz60bnYNZqakf6HJxc0",
+            "508627689:AAEuLPKs-EhrjrYGnz60bnYNZqakf6HJxc0", 'password = "0dm1nk0"', 'password = "Cr3DeHTbIal"',
+            '"password" = "p@$$w0Rd42"'
         ]
         self.assertEqual(len(expected_credential_lines), len(found_credentials))
         for cred in found_credentials:
             self.assertEqual(1, len(cred.line_data_list))
             self.assertIn(cred.line_data_list[0].line, expected_credential_lines)
             expected_credential_lines.remove(cred.line_data_list[0].line)
         self.assertEqual(0, len(expected_credential_lines))
@@ -771,15 +772,15 @@
                     test_result = json.load(f)
                 prepare(test_result)
 
                 diff = deepdiff.DeepDiff(test_result, expected_result)
                 if diff:
                     # prints produced report to compare with present data in tests/data
                     print(f"\nThe produced report for {cfg['json_filename']}:\n{json.dumps(test_result)}", flush=True)
-                self.assertDictEqual({}, diff, cfg)
+                self.assertDictEqual(diff, {}, cfg)
                 self.assertEqual(cred_count, len(expected_result), cfg["json_filename"])
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     @pytest.mark.skipif(not os.getenv("BRUTEFORCEMAXEXTENSION4ML"),
                         reason="run the test only for renaming samples with maximal ml_probability")
     def test_samples_ml_p(self) -> None:
```

