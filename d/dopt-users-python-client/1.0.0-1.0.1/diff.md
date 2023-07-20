# Comparing `tmp/dopt_users_python_client-1.0.0.tar.gz` & `tmp/dopt_users_python_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dopt_users_python_client-1.0.0.tar", max compression
+gzip compressed data, was "dopt_users_python_client-1.0.1.tar", max compression
```

## Comparing `dopt_users_python_client-1.0.0.tar` & `dopt_users_python_client-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1583 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/README.md
--rw-r--r--   0        0        0      383 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1654 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/__init__.py
--rw-r--r--   0        0        0      989 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/client.py
--rw-r--r--   0        0        0      348 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      155 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/environment.py
--rw-r--r--   0        0        0      292 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/errors/__init__.py
--rw-r--r--   0        0        0      330 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/errors/bad_request_error.py
--rw-r--r--   0        0        0      346 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/errors/internal_server_error.py
--rw-r--r--   0        0        0      337 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/py.typed
--rw-r--r--   0        0        0      124 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/resources/groups/__init__.py
--rw-r--r--   0        0        0     3925 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/resources/users/__init__.py
--rw-r--r--   0        0        0     7590 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/resources/users/client.py
--rw-r--r--   0        0        0     2090 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/__init__.py
--rw-r--r--   0        0        0      888 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/bad_request_error_response_body.py
--rw-r--r--   0        0        0      676 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/bad_request_error_response_body_code.py
--rw-r--r--   0        0        0      225 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_batch_request_body.py
--rw-r--r--   0        0        0     1080 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_batch_request_body_item.py
--rw-r--r--   0        0        0      912 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_batch_request_body_item_groups_item.py
--rw-r--r--   0        0        0      762 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_batch_response_body.py
--rw-r--r--   0        0        0      131 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_request_body.py
--rw-r--r--   0        0        0      761 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_request_params.py
--rw-r--r--   0        0        0      372 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_segment_request_body.py
--rw-r--r--   0        0        0     1203 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_segment_request_body_identify_segment_request_body.py
--rw-r--r--   0        0        0      764 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_segment_response_body.py
--rw-r--r--   0        0        0      907 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/identify_user_request_body_groups_item.py
--rw-r--r--   0        0        0      854 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/internal_server_error_response_body.py
--rw-r--r--   0        0        0      842 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/not_found_error_response_body.py
--rw-r--r--   0        0        0      956 2023-07-19 00:13:00.921433 dopt_users_python_client-1.0.0/src/dopt/types/segment_common.py
--rw-r--r--   0        0        0     1163 2023-07-19 00:13:00.925433 dopt_users_python_client-1.0.0/src/dopt/types/segment_group.py
--rw-r--r--   0        0        0     1031 2023-07-19 00:13:00.929433 dopt_users_python_client-1.0.0/src/dopt/types/segment_identify.py
--rw-r--r--   0        0        0      847 2023-07-19 00:13:00.929433 dopt_users_python_client-1.0.0/src/dopt/types/timeout_error_response_body.py
--rw-r--r--   0        0        0      849 2023-07-19 00:13:00.929433 dopt_users_python_client-1.0.0/src/dopt/types/unauthorized_error_response_body.py
--rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 dopt_users_python_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1583 2023-07-20 16:33:54.076676 dopt_users_python_client-1.0.1/README.md
+-rw-r--r--   0        0        0      383 2023-07-20 16:33:54.076676 dopt_users_python_client-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1654 2023-07-20 16:33:54.076676 dopt_users_python_client-1.0.1/src/dopt/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-20 16:33:54.076676 dopt_users_python_client-1.0.1/src/dopt/client.py
+-rw-r--r--   0        0        0      348 2023-07-20 16:33:54.076676 dopt_users_python_client-1.0.1/src/dopt/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-20 16:33:54.076676 dopt_users_python_client-1.0.1/src/dopt/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      155 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/environment.py
+-rw-r--r--   0        0        0      292 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/errors/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/errors/bad_request_error.py
+-rw-r--r--   0        0        0      346 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/errors/internal_server_error.py
+-rw-r--r--   0        0        0      337 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/py.typed
+-rw-r--r--   0        0        0      124 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/resources/groups/__init__.py
+-rw-r--r--   0        0        0     3925 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/resources/users/__init__.py
+-rw-r--r--   0        0        0     7590 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/resources/users/client.py
+-rw-r--r--   0        0        0     2090 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/__init__.py
+-rw-r--r--   0        0        0      888 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/bad_request_error_response_body.py
+-rw-r--r--   0        0        0      676 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/bad_request_error_response_body_code.py
+-rw-r--r--   0        0        0      225 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_batch_request_body.py
+-rw-r--r--   0        0        0     1080 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_batch_request_body_item.py
+-rw-r--r--   0        0        0      912 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_batch_request_body_item_groups_item.py
+-rw-r--r--   0        0        0      762 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_batch_response_body.py
+-rw-r--r--   0        0        0      131 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_request_body.py
+-rw-r--r--   0        0        0      761 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_request_params.py
+-rw-r--r--   0        0        0      372 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_segment_request_body.py
+-rw-r--r--   0        0        0     1203 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_segment_request_body_identify_segment_request_body.py
+-rw-r--r--   0        0        0      764 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_segment_response_body.py
+-rw-r--r--   0        0        0      907 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/identify_user_request_body_groups_item.py
+-rw-r--r--   0        0        0      854 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/internal_server_error_response_body.py
+-rw-r--r--   0        0        0      842 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/not_found_error_response_body.py
+-rw-r--r--   0        0        0      956 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/segment_common.py
+-rw-r--r--   0        0        0     1163 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/segment_group.py
+-rw-r--r--   0        0        0     1031 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/segment_identify.py
+-rw-r--r--   0        0        0      847 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/timeout_error_response_body.py
+-rw-r--r--   0        0        0      849 2023-07-20 16:33:54.080676 dopt_users_python_client-1.0.1/src/dopt/types/unauthorized_error_response_body.py
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 dopt_users_python_client-1.0.1/PKG-INFO
```

### Comparing `dopt_users_python_client-1.0.0/README.md` & `dopt_users_python_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/__init__.py` & `dopt_users_python_client-1.0.1/src/dopt/__init__.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/client.py` & `dopt_users_python_client-1.0.1/src/dopt/client.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/core/datetime_utils.py` & `dopt_users_python_client-1.0.1/src/dopt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/core/jsonable_encoder.py` & `dopt_users_python_client-1.0.1/src/dopt/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/resources/groups/client.py` & `dopt_users_python_client-1.0.1/src/dopt/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/resources/users/client.py` & `dopt_users_python_client-1.0.1/src/dopt/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/__init__.py` & `dopt_users_python_client-1.0.1/src/dopt/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/bad_request_error_response_body.py` & `dopt_users_python_client-1.0.1/src/dopt/types/bad_request_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/bad_request_error_response_body_code.py` & `dopt_users_python_client-1.0.1/src/dopt/types/bad_request_error_response_body_code.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/identify_batch_request_body_item.py` & `dopt_users_python_client-1.0.1/src/dopt/types/identify_batch_request_body_item.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/identify_batch_request_body_item_groups_item.py` & `dopt_users_python_client-1.0.1/src/dopt/types/identify_batch_request_body_item_groups_item.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/identify_batch_response_body.py` & `dopt_users_python_client-1.0.1/src/dopt/types/identify_batch_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/identify_request_params.py` & `dopt_users_python_client-1.0.1/src/dopt/types/identify_request_params.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/identify_segment_request_body_identify_segment_request_body.py` & `dopt_users_python_client-1.0.1/src/dopt/types/identify_segment_request_body_identify_segment_request_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/identify_segment_response_body.py` & `dopt_users_python_client-1.0.1/src/dopt/types/identify_segment_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/identify_user_request_body_groups_item.py` & `dopt_users_python_client-1.0.1/src/dopt/types/identify_user_request_body_groups_item.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/internal_server_error_response_body.py` & `dopt_users_python_client-1.0.1/src/dopt/types/internal_server_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/not_found_error_response_body.py` & `dopt_users_python_client-1.0.1/src/dopt/types/not_found_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/segment_common.py` & `dopt_users_python_client-1.0.1/src/dopt/types/segment_common.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/segment_group.py` & `dopt_users_python_client-1.0.1/src/dopt/types/segment_group.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/segment_identify.py` & `dopt_users_python_client-1.0.1/src/dopt/types/segment_identify.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/timeout_error_response_body.py` & `dopt_users_python_client-1.0.1/src/dopt/types/timeout_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/src/dopt/types/unauthorized_error_response_body.py` & `dopt_users_python_client-1.0.1/src/dopt/types/unauthorized_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.0/PKG-INFO` & `dopt_users_python_client-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopt-users-python-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

