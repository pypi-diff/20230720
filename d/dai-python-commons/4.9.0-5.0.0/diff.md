# Comparing `tmp/dai_python_commons-4.9.0.tar.gz` & `tmp/dai_python_commons-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dai_python_commons-4.9.0.tar", max compression
+gzip compressed data, was "dai_python_commons-5.0.0.tar", max compression
```

## Comparing `dai_python_commons-4.9.0.tar` & `dai_python_commons-5.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      108 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/__init__.py
--rw-r--r--   0        0        0     1372 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/cloudwatch_utils.py
--rw-r--r--   0        0        0     4383 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/dai_error.py
--rw-r--r--   0        0        0     2390 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/event_bridge.py
--rw-r--r--   0        0        0     5269 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/glue_utils.py
--rw-r--r--   0        0        0     1660 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/logging_utils.py
--rw-r--r--   0        0        0    10203 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/parquet_utils.py
--rw-r--r--   0        0        0    23860 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/s3_event_object_copy.py
--rw-r--r--   0        0        0     7285 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/s3_utils.py
--rw-r--r--   0        0        0     2391 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/time_utils.py
--rw-r--r--   0        0        0      782 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/pyproject.toml
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 dai_python_commons-4.9.0/setup.py
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 dai_python_commons-4.9.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/__init__.py
+-rw-r--r--   0        0        0     1521 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/cdk_utils.py
+-rw-r--r--   0        0        0     1372 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/cloudwatch_utils.py
+-rw-r--r--   0        0        0     4421 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/dai_error.py
+-rw-r--r--   0        0        0     2390 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/event_bridge.py
+-rw-r--r--   0        0        0     5314 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/glue_utils.py
+-rw-r--r--   0        0        0     1742 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/logging_utils.py
+-rw-r--r--   0        0        0    10471 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/parquet_utils.py
+-rw-r--r--   0        0        0    24224 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/s3_event_object_copy.py
+-rw-r--r--   0        0        0     7973 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/s3_utils.py
+-rw-r--r--   0        0        0     2391 2023-07-20 06:25:07.178630 dai_python_commons-5.0.0/dai_python_commons/time_utils.py
+-rw-r--r--   0        0        0      995 2023-07-20 06:25:07.182630 dai_python_commons-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 dai_python_commons-5.0.0/setup.py
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 dai_python_commons-5.0.0/PKG-INFO
```

### Comparing `dai_python_commons-4.9.0/dai_python_commons/cloudwatch_utils.py` & `dai_python_commons-5.0.0/dai_python_commons/cloudwatch_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.9.0/dai_python_commons/dai_error.py` & `dai_python_commons-5.0.0/dai_python_commons/dai_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module defines the exceptions used throughout this package
 """
 from dataclasses import dataclass
+from typing import Optional
 
 
 @dataclass
 class S3BucketLocation:
     """
     Class that contains information about objects location in s3.
 
@@ -53,15 +54,15 @@
 
         return ret_str
 
 
 class DaiS3DeleteObjectError(DaiS3Error):
     """Class for exceptions related to deleting objects in S3."""
 
-    def __init__(self, s3_bucket: str, error_infos: list, message: str = None):  # pylint: disable=super-init-not-called
+    def __init__(self, s3_bucket: str, error_infos: list, message: Optional[str] = None):  # pylint: disable=super-init-not-called
         self.bucket = s3_bucket
         self.error_infos = error_infos
         self.message = message
 
     def __repr__(self):
         ret_str = f"Bucket: {self.bucket}, Error info: {self.error_infos}"
         if self.message:
```

### Comparing `dai_python_commons-4.9.0/dai_python_commons/event_bridge.py` & `dai_python_commons-5.0.0/dai_python_commons/event_bridge.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.9.0/dai_python_commons/glue_utils.py` & `dai_python_commons-5.0.0/dai_python_commons/glue_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Functionality to fetch/modify info in glue database"""
+from __future__ import annotations
 from typing import List, Dict
 
 import boto3
 import awswrangler as wr
 import loguru
 
 from dai_python_commons.dai_error import DaiGlueError
 
 
-class GlueUtils:  # pylint: disable=too-few-public-methods
+class GlueUtils:  # pylint: disable=too-few-public-methods,no-member
     """Used to fetch/modify info in glue database
 
     FUNCTIONS
         get_columns_info :func:`~dai_python_commons.GlueUtils.get_columns_info`
         get_partitions :func:`~dai_python_commons.GlueUtils.get_partitions`
         add_partitions :func:`~dai_python_commons.GlueUtils.add_partitions`
     """
@@ -36,15 +37,15 @@
         return columns_info
 
     @staticmethod
     def get_partitions(
         glue_client,
         database_name: str,
         table_name: str,
-        logger: loguru.logger,
+        logger: loguru.Logger,
         max_results=100,
     ) -> list:
         """
         Get information about all the partitions of the given table
         :param glue_client: Glue boto3 client with the region set
         :param database_name: Name of the database
         :param table_name: Name of the table
@@ -83,15 +84,15 @@
         return all_partitions
 
     @staticmethod
     def add_partitions(
         session,
         database_name: str,
         table_name: str,
-        logger: loguru.logger,
+        logger: loguru.Logger,
         partitions2add: List[Dict[str, str]],
     ) -> None:
         """
         Add new partitions to a glue table
         :param session: Boto3 session
         :param database_name: Name of the database
         :param table_name: Name of the table
```

### Comparing `dai_python_commons-4.9.0/dai_python_commons/logging_utils.py` & `dai_python_commons-5.0.0/dai_python_commons/logging_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Functions for logging"""
+from __future__ import annotations
+
 import itertools
 import json
 import sys
 from typing import Any, Dict
 
+import loguru
 from loguru import logger
 from loguru._better_exceptions import ExceptionFormatter
 from loguru._handler import Message
 
 
-class LoggingUtils:  # pylint: disable=too-few-public-methods
+class LoggingUtils:  # pylint: disable=too-few-public-methods,no-member
     """
     Class that provides useful functions for logging
     """
 
     exception_formatter = ExceptionFormatter()
 
     @staticmethod
-    def get_logger(name: str, level: str = "INFO") -> logger:
+    def get_logger(name: str, level: str = "INFO") -> loguru.Logger:
         """Returns a logger object"""
         logger.remove()
         logger.configure(extra={"name": name})
-        logger.add(LoggingUtils._sink, level=level)
+        logger.add(LoggingUtils._sink, level=level) # type: ignore
 
         return logger
 
     @staticmethod
     def _sink(message: Message) -> None:
         simplified = LoggingUtils._formatter(message.record)
         print(json.dumps(simplified), file=sys.stderr)
```

### Comparing `dai_python_commons-4.9.0/dai_python_commons/parquet_utils.py` & `dai_python_commons-5.0.0/dai_python_commons/parquet_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Functionality to modify parquet files in an S3 bucket"""
+from __future__ import annotations
+
 import gc
 from dataclasses import dataclass
 from typing import Optional
+from aiobotocore.session import AioSession
 
 import boto3
 import loguru
 import pyarrow.parquet as pq
 import s3fs
 
 from dai_python_commons.s3_utils import S3Utils
@@ -41,20 +44,21 @@
     total_files_size: int = 1024 * 1024 * 1024   # 1GB
 
 
 class ParquetUtils:
     """
     Class that provides functionality for manipulating parquet files
     """
+    # pylint: disable=no-member
     VALID_COMPRESSION_TYPES = {'NONE', 'SNAPPY', 'GZIP', 'BROTLI', 'LZ4', 'ZSTD'}
 
     @staticmethod
     def s3_merge_files_in_place(boto3_session: boto3.Session,
                                 parquet_file_location: ParquetFileLocation,
-                                logger: loguru.logger,
+                                logger: loguru.Logger,
                                 compression: Optional[str] = "SNAPPY",
                                 keep_source_files: bool = False) -> int:
         """
          Merge many small parquet files into one larger parquet file. In place.
 
         :param boto3_session: Boto3 session
         :param parquet_file_location: s3 bucket and prefix location where parquet files will be merged
@@ -63,20 +67,22 @@
         :param keep_source_files: True to keep the source files, False to delete them.
         :return:
         """
         data_path = f"s3://{parquet_file_location.source_bucket}/{parquet_file_location.source_prefix}"
         logger.info(f"Merging files from {data_path} to {data_path}, compression: {compression}")
 
         # this is a bit of hack, one should probably find a better way to do this
-        botoc_session = boto3_session._session  # pylint: disable=protected-access
-        f_s = s3fs.S3FileSystem(session=botoc_session)
-        botoc_s3_client = botoc_session.create_client("s3")
+        botoc_session = boto3_session._session # pylint: disable=protected-access
+        aio_session = AioSession(session_vars=botoc_session.session_var_map)
+        f_s = s3fs.S3FileSystem(session=aio_session)
+
+        boto_s3_client = boto3_session.client("s3")
         num_rows = 0
 
-        file_paths_iter = S3Utils.iter_file_paths_in_prefix(boto_s3_client=botoc_s3_client,
+        file_paths_iter = S3Utils.iter_file_paths_in_prefix(boto_s3_client=boto_s3_client,
                                                   bucket_name=parquet_file_location.source_bucket,
                                                   prefix=parquet_file_location.source_prefix,
                                                   logger=logger,
                                                   max_size=parquet_file_location.total_files_size)
         for file_paths in file_paths_iter:
             if len(file_paths) <2:
                 logger.info(f"file paths is less than 2 files, no reason to merge: {file_paths}")
@@ -91,21 +97,21 @@
             # The type in the interface is wrong, source code does handle the None
             pq_table = pq.read_table(full_s3_paths, filesystem=f_s, partitioning=None)  # type: ignore
             num_rows += pq_table.num_rows
             logger.debug(f"Shape of the table {pq_table.shape}")
 
             logger.debug(f"Writing to the destination {data_path}")
             try:
-                pq.write_to_dataset(pq_table, data_path, filesystem=f_s, compression=compression, flavor="spark")
+                pq.write_to_dataset(pq_table, data_path, filesystem=f_s, compression=compression)
                 logger.info(f"Done merging, {pq_table.num_rows} rows were written at {data_path}")
                 if not keep_source_files:
                     logger.info('Removing source files')
                     logger.debug(f'Removing these files {file_paths}')
                     S3Utils.delete_objects(
-                        boto_s3_client=botoc_s3_client,
+                        boto_s3_client=boto_s3_client,
                         bucket_name=parquet_file_location.source_bucket,
                         to_delete=file_paths,
                         logger=logger
                     )
             except Exception:
                 logger.exception(f'Caught error when trying to merge parquet files: {file_paths}')
                 raise
@@ -117,15 +123,15 @@
         if num_rows == 0:
             logger.warning(f"No files found at {data_path}, nothing to merge")
 
         return num_rows
 
     @staticmethod
     def s3_merge_files(boto3_session: boto3.Session, parquet_file_location: ParquetFileLocation,
-                       logger: loguru.logger) -> int:
+                       logger: loguru.Logger) -> int:
         """
         Merge many small parquet files into one larger parquet file. From source to destination.
         Exception will be raised if source is equals to destination.
 
         :param boto3_session: Boto3 session
         :param parquet_file_location: ParquetFileLocation contains info about the files location in the s3 bucket
         :param logger: The logger
@@ -155,26 +161,28 @@
             return 0
 
         if remove_files_at_destination:
             ParquetUtils._remove_files(parquet_file_location, destination_data_path, logger, s3_client)
 
         logger.debug(f"Reading data from {source_data_path}")
         # this is a bit of hack, one should probably find a better way to do this
-        f_s = s3fs.S3FileSystem(session=boto3_session._session)  # pylint: disable=protected-access
+        botoc_session = boto3_session._session  # pylint: disable=protected-access
+        aio_session = AioSession(session_vars=botoc_session.session_var_map) # type: ignore
+        f_s = s3fs.S3FileSystem(session=aio_session)
         full_s3_paths = [f's3://{source_bucket}/{file_path["Key"]}' for file_path in file_paths]
-        pq_table = pq.read_table(full_s3_paths, filesystem=f_s, partitioning=None)
+        pq_table = pq.read_table(full_s3_paths, filesystem=f_s, partitioning=None) # type: ignore
         logger.debug(f"Shape of the table {pq_table.shape}")
 
         try:
             logger.debug(f"Writing to the destination {destination_data_path}")
             pq.write_to_dataset(pq_table,
                                 destination_data_path,
                                 filesystem=f_s,
-                                compression=parquet_file_location.compression,
-                                flavor="spark")
+                                compression=parquet_file_location.compression
+            )
 
             logger.info(f"Done merging, {pq_table.num_rows} rows were written at {destination_data_path}")
             if not parquet_file_location.keep_source_files:
                 logger.info('Removing source files')
                 logger.debug(f'Removing these files {file_paths}')
                 S3Utils.delete_objects(
                     boto_s3_client=s3_client,
```

### Comparing `dai_python_commons-4.9.0/dai_python_commons/s3_event_object_copy.py` & `dai_python_commons-5.0.0/dai_python_commons/s3_event_object_copy.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,34 +6,35 @@
 from enum import Enum, auto
 from io import BytesIO
 from typing import Any, Dict, Optional
 from urllib.parse import unquote_plus
 from zipfile import BadZipFile, ZipFile
 
 from botocore.exceptions import ClientError
+from mypy_boto3_s3.service_resource import S3ServiceResource as S3Resource
+from mypy_boto3_s3.type_defs import CopyObjectOutputTypeDef, CopySourceTypeDef, ObjectTypeDef
 
 import dai_python_commons.dai_error as dai_error
-from dai_python_commons.dai_error import DaiError
-from dai_python_commons.dai_error import S3BucketLocation
-from dai_python_commons.s3_utils import S3Utils
+from dai_python_commons.dai_error import DaiError, S3BucketLocation
 from dai_python_commons.event_bridge import EventBridgeS3Event
+from dai_python_commons.s3_utils import S3Utils
 
 
 class ObjectEqualityStrategy(Enum):
     ETAG = auto()
     SIZE = auto()
 
 
 class S3EventObjectCopy:
     """
     Class that provides functionality to copy objects that triggered an S3 event from one bucket to another
     Useful in lambda functions that have an S3 trigger on PUT operations
     """
 
-    def __init__(self, s3_resource, logger, destination_bucket: str, source_prefix_to_replace: str,
+    def __init__(self, s3_resource: S3Resource, logger, destination_bucket: str, source_prefix_to_replace: str,
                  destination_prefix_replacement: str, unzip_file: bool, filename_prefix: str = '',
                  remove_processed: bool = False,
                  object_equality_strategy: ObjectEqualityStrategy = ObjectEqualityStrategy.ETAG):
         """
         :param s3_resource: Boto3 resource for S3
         :param logger: The logger
         :param destination_bucket: The name of the destination bucket
@@ -64,15 +65,15 @@
         self.object_equality_strategy = object_equality_strategy
         if self.remove_processed and self.unzip_file:
             raise dai_error.IncorrectInputValueError(
                 {"unzip_file": unzip_file, "remove_unprocessed": remove_processed},
                 "The remove_unprocessed option is not supported together with unzip_file.")
 
     @staticmethod
-    def service_exception(response: dict) -> bool:
+    def service_exception(response: CopyObjectOutputTypeDef) -> bool:
         """
         Given a response from a boto3 S3 client command, check if a service error occurred
 
         :param response: Response from an S3 client request
         :return: True if an error occurred, False otherwise
         """
         if "Error" in response:
@@ -94,56 +95,59 @@
         :return: The value of field_name in the_dict or None if the field is not found in the dictionary
         """
         if the_dict and field_name in the_dict:
             return the_dict[field_name]
 
         return None
 
-    def are_equal(self, object1_info: dict, object2_info: dict) -> bool:
+    def are_equal(self, object1_info: ObjectTypeDef, object2_info: ObjectTypeDef) -> bool:
+        """
+        compares 2 responses from listing s2 objects and asserts on their equality
+        """
         if self.object_equality_strategy is ObjectEqualityStrategy.ETAG:
             return S3EventObjectCopy.are_etags_identical(object1_info, object2_info)
         elif self.object_equality_strategy is ObjectEqualityStrategy.SIZE:
             return S3EventObjectCopy.are_objects_same_size(object1_info, object2_info)
         else:
             raise ValueError(f"Unknown object equality strategy: {self.object_equality_strategy}")
 
     @staticmethod
-    def are_etags_identical(object1_info: dict, object2_info: dict) -> bool:
+    def are_etags_identical(object1_info: ObjectTypeDef, object2_info: ObjectTypeDef) -> bool:
         """
         Given two dictionaries as returned by S3 method list_objects_v2, check if their ETags are identical
 
         :param object1_info: Dictionary as returned by list_objects_v2
         :param object2_info: Dictionary as returned by list_objects_v2
         :return: True if the ETags are identical, False otherwise
         """
-        etag1 = S3EventObjectCopy.extract_field_from_dict(object1_info, "ETag")
-        etag2 = S3EventObjectCopy.extract_field_from_dict(object2_info, "ETag")
+        etag1 = object1_info.get("ETag")
+        etag2 = object2_info.get("ETag")
         if not etag1 or not etag2 or etag1 != etag2:
             return False
 
         return True
 
     @staticmethod
-    def are_objects_same_size(object1_info: dict, object2_info: dict) -> bool:
+    def are_objects_same_size(object1_info: ObjectTypeDef, object2_info: ObjectTypeDef) -> bool:
         """
         Given two dictionaries as returned by S3 method list_objects_v2, check if they are the same size
 
         :param object1_info: Dictionary as returned by list_objects_v2
         :param object2_info: Dictionary as returned by list_objects_v2
         :return: True if the objects have the same size, False otherwise
         """
-        size1 = S3EventObjectCopy.extract_field_from_dict(object1_info, "Size")
-        size2 = S3EventObjectCopy.extract_field_from_dict(object2_info, "Size")
+        size1 = object1_info.get("Size")
+        size2 = object2_info.get("Size")
         if size1 is None or size2 is None:
             return False
 
         return size1 == size2
 
     @staticmethod
-    def get_object_lock_retain_until_date(tag_dict: Dict[str, any]) -> Optional[datetime.datetime]:
+    def get_object_lock_retain_until_date(tag_dict: Optional[Dict[str, Any]]) -> Optional[datetime.datetime]:
         """
         Calculates the object lock retain until date based on the *retention_time* tag value
 
         :param tag_dict: dict that may contain the *retention_time* key
         :return: the "retain until date" or None if no *retention_time* can be found in *destination_tags*
         """
 
@@ -178,15 +182,15 @@
             new_filename = self._append_filename_prefix(filename)
             destination_prefix = os.path.join(destination_prefix_wo_filename, new_filename)
             # upload the object
             self.logger.debug(f"{filename} -> {destination_prefix}")
             self.s3_client.upload_fileobj(zip_file.open(filename), Bucket=self.destination_bucket,
                                           Key=destination_prefix)
 
-    def _get_object_info(self, bucket: str, prefix: str) -> Dict[str, Any]:
+    def _get_object_info(self, bucket: str, prefix: str) -> Optional[ObjectTypeDef]:
         """
         Return metadata information about an object stored in S3
 
         :param bucket: name of the bucket
         :param prefix: prefix of the object
         :return: A dictionary as returned by list_objects_v2, or None if the object doesn't exist
         """
@@ -199,16 +203,16 @@
         # The boto3 exception mechanisms seems pretty badly documented so I use Exception to be on the safe side
         except Exception as the_exception:
             self.logger.warning(
                 f"Unable to get information about object {bucket}/{prefix}, error: {the_exception}")
 
         return result
 
-    def _remove_processed_object(self, source_bucket: str, source_prefix: str, source_object_info: Dict[str, Any],
-                                 destination_object_info: Dict[str, Any]) -> bool:
+    def _remove_processed_object(self, source_bucket: str, source_prefix: str, source_object_info: ObjectTypeDef,
+                                 destination_object_info: ObjectTypeDef) -> bool:
         """
         Removes an object that has been processed. It only removes the object if the source and destination etags
         match
 
         :param source_bucket: The name of the source bucket
         :param source_prefix: The key of the object
         :param source_object_info: Metadata information about the source object as returned by boto3 list_objects_v2
@@ -224,15 +228,15 @@
         if not self.are_equal(source_object_info, destination_object_info):
             self.logger.warning(f"Source and destination objects do not match, the processed object "
                                 f"{source_object} will not be removed")
             return False
 
         # delete the processed file
         try:
-            _response = self.s3_client.delete_object(Bucket=source_bucket, Key=source_prefix)
+            self.s3_client.delete_object(Bucket=source_bucket, Key=source_prefix)
         except Exception as the_exception:
             self.logger.opt(exception=True).warning(f"Unable to remove {source_object}, error: {the_exception}")
             return False
         else:
             self.logger.debug(f"Object {source_object} was deleted")
             return True
 
@@ -267,43 +271,43 @@
         :return: the filename with prefix added, if filename prefix configured, else same as given filename
         """
         if self.filename_prefix:
             filename = f'{self.filename_prefix}_{filename}'
 
         return filename
 
-    def _get_tagging_str(self, tag_dict: Dict[str, any]) -> str:
+    def _get_tagging_str(self, tag_dict: Optional[Dict[str, Any]]) -> str:
         """
         :param tag_dict: Dictionary giving tag_name, tag_value
         :return: A string that can be used by boto3 copy commands to tag objects
         """
         return urllib.parse.urlencode(tag_dict) if tag_dict else ""
 
     def _copy_using_unmanaged_transfer(self,
                                        source_bucket_name: str,
                                        source_object: str,
-                                       copy_source_object: Dict[str, any],
-                                       object_info: Dict[str, Any],
+                                       copy_source_object: CopySourceTypeDef,
+                                       object_info: ObjectTypeDef,
                                        destination_prefix: str,
-                                       destination_tags: Dict[str, any]):
+                                       destination_tags: Optional[Dict[str, Any]]):
         """
         Uses client.copy_object to copy an object from one location to another.
 
         :param source_bucket_name: The name of the source bucket
         :param source_object: Key of the object to be copied
         :param copy_source_object: Dict containing information about the source bucket and key
         :param object_info: Dictionary as returned by list_objects_v2
         :param destination_prefix: The destination prefix
         :param destination_tags: Tags that should be set on the object in the request.
         :return:
         """
         tagging = self._get_tagging_str(destination_tags)
 
         object_lock_arguments = {}
-        if S3Utils.is_raw_bucket(self.destination_bucket):
+        if S3Utils.is_raw_bucket(self.destination_bucket) and destination_tags:
             if destination_tags.get("retention_type") in ["shall", "may"]:
                 object_lock_arguments = {
                     "ObjectLockMode": "GOVERNANCE",
                     "ObjectLockRetainUntilDate": self.get_object_lock_retain_until_date(destination_tags)
                 }
             elif destination_tags.get("retention_type") == "preserve":
                 # 52000 weeks are ~1000 years
@@ -324,38 +328,40 @@
                                               source_object,
                                               self.destination_bucket,
                                               destination_prefix)
         if S3EventObjectCopy.service_exception(response):
             raise dai_error.DaiS3CopyObjectError(s3_bucket_location)
         if self.remove_processed:
             destination_object_info = self._get_object_info(self.destination_bucket, destination_prefix)
+            if not destination_object_info:
+                return
             self._remove_processed_object(source_bucket=source_bucket_name, source_prefix=source_object,
                                           source_object_info=object_info,
                                           destination_object_info=destination_object_info)
 
     def _copy_using_managed_transfer(self,
-                                     copy_source_object: Dict[str, any],
+                                     copy_source_object: CopySourceTypeDef,
                                      destination_prefix: str,
                                      content_length: Optional[int],
-                                     destination_tags: Dict[str, any]):
+                                     destination_tags: Optional[Dict[str, Any]]):
         """
         Uses client.copy to copy an object from one location to another. This copy is a so called managed transfer.
 
         client.copy docs:
 
                 "This is a managed transfer which will perform a multipart copy in multiple threads if necessary."
 
         :param copy_source_object: Dict containing information about the source bucket and key
         :param destination_prefix: The destination prefix
         :param content_length: The size of the object
         :param destination_tags: Tags that should be set on the object in the request.
         :return:
         """
-        s3_bucket_location = S3BucketLocation(copy_source_object.get("Bucket"),
-                                              copy_source_object.get("Key"),
+        s3_bucket_location = S3BucketLocation(copy_source_object.get("Bucket", ""),
+                                              copy_source_object.get("Key", ""),
                                               self.destination_bucket,
                                               destination_prefix)
 
         if S3Utils.is_raw_bucket(self.destination_bucket):
             raise dai_error.DaiS3CopyObjectError(
                 s3_bucket_location,
                 message="Can't copy object due to destination bucket requiring "
@@ -379,39 +385,40 @@
                                     "{source_bucket_name}/{source_object} ")
             elif content_length is not None and content_length > 4.9e9:
                 self.logger.warning("Removal of processed objects for large objects (>= 5Gb) not supported "
                                     "unable to remove {source_bucket_name}/{source_object} ")
             else:
                 raise dai_error.DaiS3Error(f"Don't know how to remove processed: {copy_source_object}")
 
-    def _copy_one_object(self, source_bucket_name: str, source_object: str, destination_tags: Dict[str, any] = None):
+    def _copy_one_object(self, source_bucket_name: str, source_object: str, destination_tags: Optional[Dict[str, Any]] = None):
         """
         Copies one object to the destination bucket
 
         :param source_bucket_name: Name of the bucket
         :param source_object: Key of the object to be copied
+        :param destination_tags: Tags to append to destination file
         :return: Nothing
         :raises dai_error.DaiS3CopyObjectError if the copy_object operation fails
         """
 
         self.logger.debug(f"Processing {source_bucket_name}/{source_object} ")
         # if needed, unzip the file in memory then copy
         if self.unzip_file:
             destination_prefix_wo_filename = self._get_destination_prefix(source_object, exclude_filename=True)
             self._unzip_and_copy(source_bucket_name, source_object, destination_prefix_wo_filename)
         else:
             # copy the file without unzipping
-            copy_source_object = {'Bucket': source_bucket_name, 'Key': source_object}
+            copy_source_object = CopySourceTypeDef(Bucket=source_bucket_name, Key=source_object)
             destination_prefix = self._get_destination_prefix(source_object, exclude_filename=False)
 
             self.logger.debug(f"{source_bucket_name}/{source_object} -> {self.destination_bucket}/{destination_prefix}")
 
             object_info = self._get_object_info(source_bucket_name, source_object)
             if object_info is not None:
-                content_length = S3EventObjectCopy.extract_field_from_dict(object_info, "Size")
+                content_length = object_info.get("Size")
                 # use different methods depending on object size
                 if not self.remove_processed or content_length is None or content_length > 4.9e9:
                     self._copy_using_managed_transfer(content_length=content_length,
                                                       copy_source_object=copy_source_object,
                                                       destination_prefix=destination_prefix,
                                                       destination_tags=destination_tags)
                 else:
@@ -421,15 +428,15 @@
                                                         source_object=source_object, destination_tags=destination_tags)
             else:
                 self.logger.warning(
                     f"The object {source_bucket_name}/{source_object} does not exist, perhaps it was already copied?")
 
         self.logger.debug(f"Finished processing {source_bucket_name}/{source_object} ")
 
-    def copy_objects_s3_event(self, event: Dict[str, Any], destination_tags: Dict[str, any] = None) -> int:
+    def copy_objects_s3_event(self, event: Dict[str, Any], destination_tags: Optional[Dict[str, Any]] = None) -> int:
         """
         Copy the object(s) that triggered an S3 event to a destination bucket.
 
         :param event: The event that triggered the function
         :param destination_tags: The tags that should be added to the object in the destination
         :return: the number of objects copied
         """
@@ -450,15 +457,15 @@
                 num_records_copied += 1
             except (BadZipFile, ClientError) as e:
                 self.logger.exception(f"Caught exception: {e}")
                 raise
 
         return num_records_copied
 
-    def copy_objects_event_bridge_s3_event(self, event: EventBridgeS3Event, destination_tags: Dict[str, any] = None) -> int:
+    def copy_objects_event_bridge_s3_event(self, event: EventBridgeS3Event, destination_tags: Optional[Dict[str, Any]] = None):
         source_bucket_name = event.s3_bucket
         # needed to handle special characters
         source_key = unquote_plus(event.s3_key)
 
         self.logger.info(f"Copying object s3://{source_bucket_name}/{source_key} to bucket {self.destination_bucket}")
 
         if source_bucket_name == self.destination_bucket:
```

### Comparing `dai_python_commons-4.9.0/dai_python_commons/s3_utils.py` & `dai_python_commons-5.0.0/dai_python_commons/s3_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 """Useful functions for s3 buckets"""
-import re
+from __future__ import annotations
+
 import datetime
-from typing import Any, Dict, Iterable, List
+import re
+from typing import Iterable, List
 
-import botocore.client
 import loguru
+from botocore.response import StreamingBody
+from mypy_boto3_s3.client import S3Client
+from mypy_boto3_s3.type_defs import DeleteTypeDef, ObjectIdentifierTypeDef
 
 from dai_python_commons import dai_error
 
+# pylint: disable=no-member
 
 class S3Utils:
     """
     Class provides functions to modify s3 buckets
     """
 
     RAW_BUCKET_PATTERN = re.compile(r"se-sl-tf-dai-[^-]*-data-raw")
 
     @staticmethod
     def delete_objects_by_prefix(
-        boto_s3_client: botocore.client,
+        boto_s3_client: S3Client,
         bucket_name: str,
         prefix: str,
-        logger: loguru.logger,
+        logger: loguru.Logger,
     ) -> int:
         """
         Deletes all objects with given prefix from a bucket
 
         :param boto_s3_client: S3 client to be used
         :param bucket_name: Name of the bucket
         :param prefix: Prefix of objects that should be removed
@@ -38,30 +43,30 @@
         page_iterator = paginator.paginate(Bucket=bucket_name, Prefix=prefix)
 
         # gather all objects to be deleted
         to_delete = []
         for item in page_iterator.search("Contents"):
             if not item:
                 break
-            to_delete.append(dict(Key=item["Key"]))
+            to_delete.append({"Key": item["Key"]})
 
         # delete the objects
         return S3Utils.delete_objects(
             boto_s3_client=boto_s3_client,
             bucket_name=bucket_name,
             to_delete=to_delete,
             logger=logger,
         )
 
     @staticmethod
     def delete_objects(
-        boto_s3_client: botocore.client,
+        boto_s3_client: S3Client,
         bucket_name: str,
-        to_delete: List[Dict[str, str]],
-        logger: loguru.logger,
+        to_delete: List[ObjectIdentifierTypeDef],
+        logger: loguru.Logger,
     ) -> int:
         """
         Deletes the specified objects in `to_delete` and returns the number of deleted objects.
 
         `to_delete` should be in the following format:
 
             [
@@ -76,15 +81,15 @@
         :param logger: The logger
         :return: Number of objects deleted
         """
 
         start_index = 0
         while start_index < len(to_delete):
             end_index = min(len(to_delete), start_index + 1000)
-            batch_to_delete = {"Objects": to_delete[start_index:end_index]}
+            batch_to_delete = DeleteTypeDef( Objects=to_delete[start_index:end_index] )
             logger.debug(f"Deleting {batch_to_delete}")
             response = boto_s3_client.delete_objects(
                 Bucket=bucket_name, Delete=batch_to_delete
             )
 
             # If something went wrong raise an error
             if "Errors" in response and len(response["Errors"]) > 0:
@@ -96,20 +101,20 @@
 
         logger.info(f"Number of objects deleted: {len(to_delete)}")
 
         return len(to_delete)
 
     @staticmethod
     def iter_file_paths_in_prefix(
-        boto_s3_client: botocore.client,
+        boto_s3_client: S3Client,
         bucket_name: str,
         prefix: str,
-        logger: loguru.logger,
+        logger: loguru.Logger,
         max_size: int,
-    ) -> Iterable[List[Dict[str, Any]]]:
+    ) -> Iterable[List[ObjectIdentifierTypeDef]]:
         """
         Returns a Iterable over lists of dicts representing file paths in the format:
 
             [
                 {
                     'Key': 'prefix'
                 }
@@ -152,19 +157,19 @@
 
         logger.debug(f'In "{bucket_name}/{prefix}" yields last results: {prefixes}')
 
         yield prefixes
 
     @staticmethod
     def file_paths_in_prefix(
-        boto_s3_client: botocore.client,
+        boto_s3_client: S3Client,
         bucket_name: str,
         prefix: str,
-        logger: loguru.logger,
-    ) -> List[Dict[str, str]]:
+        logger: loguru.Logger,
+    ) -> List[ObjectIdentifierTypeDef]:
         """
         Returns a list of dicts representing file paths in the format:
 
             [
                 {
                     'Key': 'prefix'
                 }
@@ -193,30 +198,45 @@
     @staticmethod
     def is_raw_bucket(bucket_name: str) -> bool:
         """Checks that bucket_name matches RAW_BUCKET_PATTERN regex"""
         return S3Utils.RAW_BUCKET_PATTERN.match(bucket_name) is not None
 
     @staticmethod
     def get_last_modified(
-        boto_s3_client: botocore.client,
+        boto_s3_client: S3Client,
         bucket_name: str,
         key: str,
-        logger: loguru.logger,
+        logger: loguru.Logger,
     ) -> datetime.datetime:
         """
         Gets the last modified stamp for a object stored in s3
 
         :param boto_s3_client: Boto3 s3 client
         :param bucket_name: Name of s3 bucket
         :param key: Object key
         :param logger: Logger object
         :return: Last modified value
         """
         response = boto_s3_client.head_object(Bucket=bucket_name, Key=key)
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
-            error_info = response.get("Error", "")
+            error_info = response.get("Error", {})
             logger.error(
                 f"Unable to obtain LastModified for s3://{bucket_name}/{key}. Error info: {error_info}"
             )
-            raise Exception(error_info.get("Message", ""))
+            raise Exception(error_info.get("Message", ""))  # pylint:  disable=broad-exception-raised
 
         return response["LastModified"]
+
+    @staticmethod
+    def read_s3_file(s3_client: S3Client, bucket_name: str, key: str) -> StreamingBody:
+        """
+        Get content of an S3 object
+
+        :param s3_client: Boto3 s3 client
+        :param bucket_name: Name of s3 bucket
+        :param key: Object key
+        :return: Http response body
+        """
+        response = s3_client.get_object(Bucket=bucket_name, Key=key)
+        content = response["Body"]
+
+        return content
```

### Comparing `dai_python_commons-4.9.0/dai_python_commons/time_utils.py` & `dai_python_commons-5.0.0/dai_python_commons/time_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.9.0/pyproject.toml` & `dai_python_commons-5.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 [tool.poetry]
 name = "dai-python-commons"
-version = "4.9.0"
+version = "5.0.0"
 description = "Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration."
 authors = []
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-loguru = "^0.6.0"
-boto3 = "^1.18.31"
-pyarrow = { version = "3.0.0", optional = true }
-s3fs = { version = "0.4.2", optional = true }
-awswrangler = { version = "2.18.0", optional = true }
-cryptography = { version = "38.0.1", optional = true }
+python = "~3.11"
+loguru = "^0.7.0"
+boto3 = "^1.26.0"
+pyarrow = { version = "12.0.0", optional = true }
+s3fs = { version = "2023.6.0", optional = true }
+awswrangler = { version = "3.2.1", optional = true }
+boto3-stubs = { version = "^1.26.0", extras = ["s3", "glue"] }
+cryptography = { version = "41.0.2", optional = true }
+aiobotocore = { version="2.5.2", optional=true }
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-moto = "^1.3"
-pylint = "^2.13.5"
+pytest = "7.4"
+moto = { version = "4.1.13", extras = ["s3", "glue"] }
+pylint = "2.17.4"
 
 
 [tool.poetry.extras]
-data-consolidation = ["s3fs", "pyarrow"]
+data-consolidation = ["s3fs", "pyarrow", "aiobotocore"]
 glue = ["awswrangler", "cryptography"]
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+pythonpath = ["."]
```

### Comparing `dai_python_commons-4.9.0/setup.py` & `dai_python_commons-5.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,32 +4,36 @@
 packages = \
 ['dai_python_commons']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.18.31,<2.0.0', 'loguru>=0.6.0,<0.7.0']
+['boto3-stubs[glue,s3]>=1.26.0,<2.0.0',
+ 'boto3>=1.26.0,<2.0.0',
+ 'loguru>=0.7.0,<0.8.0']
 
 extras_require = \
-{'data-consolidation': ['pyarrow==3.0.0', 's3fs==0.4.2'],
- 'glue': ['awswrangler==2.18.0', 'cryptography==38.0.1']}
+{'data-consolidation': ['pyarrow==12.0.0',
+                        's3fs==2023.6.0',
+                        'aiobotocore==2.5.2'],
+ 'glue': ['awswrangler==3.2.1', 'cryptography==41.0.2']}
 
 setup_kwargs = {
     'name': 'dai-python-commons',
-    'version': '4.9.0',
+    'version': '5.0.0',
     'description': 'Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration.',
     'long_description': 'None',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.11,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

