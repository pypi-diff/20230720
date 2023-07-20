# Comparing `tmp/types-boto-2.49.8.tar.gz` & `tmp/types-boto-2.49.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-boto-2.49.8.tar", last modified: Wed Mar  9 18:21:32 2022, max compression
+gzip compressed data, was "types-boto-2.49.9.tar", last modified: Thu Mar 10 01:15:35 2022, max compression
```

## Comparing `types-boto-2.49.8.tar` & `types-boto-2.49.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:21:32.733060 types-boto-2.49.8/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-03-09 18:21:32.000000 types-boto-2.49.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-09 18:21:32.000000 types-boto-2.49.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-03-09 18:21:32.733060 types-boto-2.49.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:21:32.729060 types-boto-2.49.8/boto-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-09 18:21:32.000000 types-boto-2.49.8/boto-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     6849 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4179 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/auth_handler.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5549 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/connection.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:21:32.729060 types-boto-2.49.8/boto-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/ec2/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:21:32.729060 types-boto-2.49.8/boto-stubs/elb/
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4532 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:21:32.729060 types-boto-2.49.8/boto-stubs/kms/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/kms/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/kms/layer1.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/regioninfo.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:21:32.733060 types-boto-2.49.8/boto-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/acl.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8383 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/bucket.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/bucketlistresultset.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/bucketlogging.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/cors.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/deletemarker.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8037 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/key.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/keyfile.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/lifecycle.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/multidelete.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/multipart.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/prefix.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/tagging.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/user.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/s3/website.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5648 2022-03-09 18:21:05.000000 types-boto-2.49.8/boto-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-09 18:21:32.733060 types-boto-2.49.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-03-09 18:21:32.000000 types-boto-2.49.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:21:32.733060 types-boto-2.49.8/types_boto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-03-09 18:21:32.000000 types-boto-2.49.8/types_boto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-03-09 18:21:32.000000 types-boto-2.49.8/types_boto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-09 18:21:32.000000 types-boto-2.49.8/types_boto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-09 18:21:32.000000 types-boto-2.49.8/types_boto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-09 18:21:32.000000 types-boto-2.49.8/types_boto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 01:15:35.258960 types-boto-2.49.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      828 2022-03-10 01:15:33.000000 types-boto-2.49.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-10 01:15:33.000000 types-boto-2.49.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-03-10 01:15:35.258960 types-boto-2.49.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 01:15:35.258960 types-boto-2.49.9/boto-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-10 01:15:33.000000 types-boto-2.49.9/boto-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     6841 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4179 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/auth_handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5549 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/connection.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 01:15:35.258960 types-boto-2.49.9/boto-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/ec2/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 01:15:35.258960 types-boto-2.49.9/boto-stubs/elb/
+-rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4532 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 01:15:35.258960 types-boto-2.49.9/boto-stubs/kms/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/kms/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/kms/layer1.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/regioninfo.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 01:15:35.258960 types-boto-2.49.9/boto-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/acl.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8250 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/bucket.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/bucketlistresultset.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/bucketlogging.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4653 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/cors.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/deletemarker.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7958 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/key.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/keyfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/lifecycle.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/multidelete.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/multipart.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/prefix.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/tagging.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/s3/website.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5686 2022-03-10 01:15:25.000000 types-boto-2.49.9/boto-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-10 01:15:35.258960 types-boto-2.49.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-03-10 01:15:33.000000 types-boto-2.49.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 01:15:35.258960 types-boto-2.49.9/types_boto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-03-10 01:15:35.000000 types-boto-2.49.9/types_boto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-03-10 01:15:35.000000 types-boto-2.49.9/types_boto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-10 01:15:35.000000 types-boto-2.49.9/types_boto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-10 01:15:35.000000 types-boto-2.49.9/types_boto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-10 01:15:35.000000 types-boto-2.49.9/types_boto.egg-info/top_level.txt
```

### Comparing `types-boto-2.49.8/CHANGELOG.md` & `types-boto-2.49.9/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.49.9 (2022-03-10)
+
+Modernize syntax in various stubs (#7469)
+
+Use `str` and `contextlib.AbstractContextManager` instead of `typing.Text` and `typing.ContextManager`.
+
 ## 2.49.8 (2022-03-09)
 
 Remove Python 2 support from some third-party distributions (#7466)
 
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
 
 ## 2.49.7 (2022-01-30)
```

### Comparing `types-boto-2.49.8/PKG-INFO` & `types-boto-2.49.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-boto
-Version: 2.49.8
+Version: 2.49.9
 Summary: Typing stubs for boto
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boto.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `boto` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `boto`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/boto. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `c3907ab26b1c75bc19163aa828d1197ae8640127`.
+This package was generated from typeshed commit `9a1f5fb06cc9ca4938ba78301664a79e1718f8fb`.
```

### Comparing `types-boto-2.49.8/boto-stubs/__init__.pyi` & `types-boto-2.49.9/boto-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Text
+from typing import Any
 
 from .s3.connection import S3Connection
 
 Version: Any
 UserAgent: Any
 config: Any
 BUCKET_NAME_RE: Any
@@ -19,15 +19,15 @@
 
 log: Any
 perflog: Any
 
 def set_file_logger(name, filepath, level: Any = ..., format_string: Any | None = ...): ...
 def set_stream_logger(name, level: Any = ..., format_string: Any | None = ...): ...
 def connect_sqs(aws_access_key_id: Any | None = ..., aws_secret_access_key: Any | None = ..., **kwargs): ...
-def connect_s3(aws_access_key_id: Text | None = ..., aws_secret_access_key: Text | None = ..., **kwargs) -> S3Connection: ...
+def connect_s3(aws_access_key_id: str | None = ..., aws_secret_access_key: str | None = ..., **kwargs) -> S3Connection: ...
 def connect_gs(gs_access_key_id: Any | None = ..., gs_secret_access_key: Any | None = ..., **kwargs): ...
 def connect_ec2(aws_access_key_id: Any | None = ..., aws_secret_access_key: Any | None = ..., **kwargs): ...
 def connect_elb(aws_access_key_id: Any | None = ..., aws_secret_access_key: Any | None = ..., **kwargs): ...
 def connect_autoscale(aws_access_key_id: Any | None = ..., aws_secret_access_key: Any | None = ..., **kwargs): ...
 def connect_cloudwatch(aws_access_key_id: Any | None = ..., aws_secret_access_key: Any | None = ..., **kwargs): ...
 def connect_sdb(aws_access_key_id: Any | None = ..., aws_secret_access_key: Any | None = ..., **kwargs): ...
 def connect_fps(aws_access_key_id: Any | None = ..., aws_secret_access_key: Any | None = ..., **kwargs): ...
```

### Comparing `types-boto-2.49.8/boto-stubs/auth.pyi` & `types-boto-2.49.9/boto-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/connection.pyi` & `types-boto-2.49.9/boto-stubs/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/elb/__init__.pyi` & `types-boto-2.49.9/boto-stubs/elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/exception.pyi` & `types-boto-2.49.9/boto-stubs/exception.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/kms/exceptions.pyi` & `types-boto-2.49.9/boto-stubs/kms/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/kms/layer1.pyi` & `types-boto-2.49.9/boto-stubs/kms/layer1.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/regioninfo.pyi` & `types-boto-2.49.9/boto-stubs/regioninfo.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/s3/acl.pyi` & `types-boto-2.49.9/boto-stubs/s3/acl.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Any, Text
+from typing import Any
 
 from .connection import S3Connection
 from .user import User
 
 CannedACLStrings: list[str]
 
 class Policy:
     parent: Any
     namespace: Any
     acl: ACL
     def __init__(self, parent: Any | None = ...) -> None: ...
     owner: User
-    def startElement(self, name: Text, attrs: dict[str, Any], connection: S3Connection) -> None | User | ACL: ...
-    def endElement(self, name: Text, value: Any, connection: S3Connection) -> None: ...
+    def startElement(self, name: str, attrs: dict[str, Any], connection: S3Connection) -> None | User | ACL: ...
+    def endElement(self, name: str, value: Any, connection: S3Connection) -> None: ...
     def to_xml(self) -> str: ...
 
 class ACL:
     policy: Policy
     grants: list[Grant]
     def __init__(self, policy: Policy | None = ...) -> None: ...
     def add_grant(self, grant: Grant) -> None: ...
-    def add_email_grant(self, permission: Text, email_address: Text) -> None: ...
-    def add_user_grant(self, permission: Text, user_id: Text, display_name: Text | None = ...) -> None: ...
+    def add_email_grant(self, permission: str, email_address: str) -> None: ...
+    def add_user_grant(self, permission: str, user_id: str, display_name: str | None = ...) -> None: ...
     def startElement(self, name, attrs, connection): ...
-    def endElement(self, name: Text, value: Any, connection: S3Connection) -> None: ...
+    def endElement(self, name: str, value: Any, connection: S3Connection) -> None: ...
     def to_xml(self) -> str: ...
 
 class Grant:
-    NameSpace: Text
-    permission: Text
-    id: Text
-    display_name: Text
-    uri: Text
-    email_address: Text
-    type: Text
+    NameSpace: str
+    permission: str
+    id: str
+    display_name: str
+    uri: str
+    email_address: str
+    type: str
     def __init__(
         self,
-        permission: Text | None = ...,
-        type: Text | None = ...,
-        id: Text | None = ...,
-        display_name: Text | None = ...,
-        uri: Text | None = ...,
-        email_address: Text | None = ...,
+        permission: str | None = ...,
+        type: str | None = ...,
+        id: str | None = ...,
+        display_name: str | None = ...,
+        uri: str | None = ...,
+        email_address: str | None = ...,
     ) -> None: ...
     def startElement(self, name, attrs, connection): ...
-    def endElement(self, name: Text, value: Any, connection: S3Connection) -> None: ...
+    def endElement(self, name: str, value: Any, connection: S3Connection) -> None: ...
     def to_xml(self) -> str: ...
```

### Comparing `types-boto-2.49.8/boto-stubs/s3/bucket.pyi` & `types-boto-2.49.9/boto-stubs/s3/key.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,178 +1,231 @@
-from typing import Any, Text
+from typing import Any, Callable, overload
 
-from .bucketlistresultset import BucketListResultSet
-from .connection import S3Connection
-from .key import Key
-
-class S3WebsiteEndpointTranslate:
-    trans_region: dict[str, str]
-    @classmethod
-    def translate_region(cls, reg: Text) -> str: ...
-
-S3Permissions: list[str]
-
-class Bucket:
-    LoggingGroup: str
-    BucketPaymentBody: str
-    VersioningBody: str
-    VersionRE: str
-    MFADeleteRE: str
-    name: Text
-    connection: S3Connection
-    key_class: type[Key]
-    def __init__(self, connection: S3Connection | None = ..., name: Text | None = ..., key_class: type[Key] = ...) -> None: ...
+class Key:
+    DefaultContentType: str
+    RestoreBody: str
+    BufferSize: Any
+    base_user_settable_fields: Any
+    base_fields: Any
+    bucket: Any
+    name: str
+    metadata: Any
+    cache_control: Any
+    content_type: Any
+    content_encoding: Any
+    content_disposition: Any
+    content_language: Any
+    filename: Any
+    etag: Any
+    is_latest: bool
+    last_modified: Any
+    owner: Any
+    path: Any
+    resp: Any
+    mode: Any
+    size: Any
+    version_id: Any
+    source_version_id: Any
+    delete_marker: bool
+    encrypted: Any
+    ongoing_restore: Any
+    expiry_date: Any
+    local_hashes: Any
+    def __init__(self, bucket: Any | None = ..., name: Any | None = ...) -> None: ...
     def __iter__(self): ...
-    def __contains__(self, key_name) -> bool: ...
+    @property
+    def provider(self): ...
+    key: Any
+    md5: Any
+    base64md5: Any
+    storage_class: Any
+    def get_md5_from_hexdigest(self, md5_hexdigest): ...
+    def handle_encryption_headers(self, resp): ...
+    def handle_version_headers(self, resp, force: bool = ...): ...
+    def handle_restore_headers(self, response): ...
+    def handle_addl_headers(self, headers): ...
+    def open_read(
+        self,
+        headers: dict[str, str] | None = ...,
+        query_args: str = ...,
+        override_num_retries: Any | None = ...,
+        response_headers: dict[str, str] | None = ...,
+    ): ...
+    def open_write(self, headers: dict[str, str] | None = ..., override_num_retries: Any | None = ...): ...
+    def open(
+        self,
+        mode: str = ...,
+        headers: dict[str, str] | None = ...,
+        query_args: Any | None = ...,
+        override_num_retries: Any | None = ...,
+    ): ...
+    closed: bool
+    def close(self, fast: bool = ...): ...
+    def next(self): ...
+    __next__: Any
+    def read(self, size: int = ...): ...
+    def change_storage_class(self, new_storage_class, dst_bucket: Any | None = ..., validate_dst_bucket: bool = ...): ...
+    def copy(
+        self,
+        dst_bucket,
+        dst_key,
+        metadata: Any | None = ...,
+        reduced_redundancy: bool = ...,
+        preserve_acl: bool = ...,
+        encrypt_key: bool = ...,
+        validate_dst_bucket: bool = ...,
+    ): ...
     def startElement(self, name, attrs, connection): ...
-    creation_date: Any
     def endElement(self, name, value, connection): ...
-    def set_key_class(self, key_class): ...
-    def lookup(self, key_name, headers: dict[Text, Text] | None = ...): ...
-    def get_key(
-        self,
-        key_name,
-        headers: dict[Text, Text] | None = ...,
-        version_id: Any | None = ...,
-        response_headers: dict[Text, Text] | None = ...,
-        validate: bool = ...,
-    ) -> Key: ...
-    def list(
-        self,
-        prefix: Text = ...,
-        delimiter: Text = ...,
-        marker: Text = ...,
-        headers: dict[Text, Text] | None = ...,
-        encoding_type: Any | None = ...,
-    ) -> BucketListResultSet: ...
-    def list_versions(
-        self,
-        prefix: str = ...,
-        delimiter: str = ...,
-        key_marker: str = ...,
-        version_id_marker: str = ...,
-        headers: dict[Text, Text] | None = ...,
-        encoding_type: Text | None = ...,
-    ) -> BucketListResultSet: ...
-    def list_multipart_uploads(
-        self,
-        key_marker: str = ...,
-        upload_id_marker: str = ...,
-        headers: dict[Text, Text] | None = ...,
-        encoding_type: Any | None = ...,
-    ): ...
-    def validate_kwarg_names(self, kwargs, names): ...
-    def get_all_keys(self, headers: dict[Text, Text] | None = ..., **params): ...
-    def get_all_versions(self, headers: dict[Text, Text] | None = ..., **params): ...
-    def validate_get_all_versions_params(self, params): ...
-    def get_all_multipart_uploads(self, headers: dict[Text, Text] | None = ..., **params): ...
-    def new_key(self, key_name: Any | None = ...): ...
+    def exists(self, headers: dict[str, str] | None = ...): ...
+    def delete(self, headers: dict[str, str] | None = ...): ...
+    def get_metadata(self, name): ...
+    def set_metadata(self, name, value): ...
+    def update_metadata(self, d): ...
+    def set_acl(self, acl_str, headers: dict[str, str] | None = ...): ...
+    def get_acl(self, headers: dict[str, str] | None = ...): ...
+    def get_xml_acl(self, headers: dict[str, str] | None = ...): ...
+    def set_xml_acl(self, acl_str, headers: dict[str, str] | None = ...): ...
+    def set_canned_acl(self, acl_str, headers: dict[str, str] | None = ...): ...
+    def get_redirect(self): ...
+    def set_redirect(self, redirect_location, headers: dict[str, str] | None = ...): ...
+    def make_public(self, headers: dict[str, str] | None = ...): ...
     def generate_url(
         self,
         expires_in,
         method: str = ...,
-        headers: dict[Text, Text] | None = ...,
+        headers: dict[str, str] | None = ...,
+        query_auth: bool = ...,
         force_http: bool = ...,
-        response_headers: dict[Text, Text] | None = ...,
+        response_headers: dict[str, str] | None = ...,
         expires_in_absolute: bool = ...,
-    ): ...
-    def delete_keys(self, keys, quiet: bool = ..., mfa_token: Any | None = ..., headers: dict[Text, Text] | None = ...): ...
-    def delete_key(
-        self, key_name, headers: dict[Text, Text] | None = ..., version_id: Any | None = ..., mfa_token: Any | None = ...
-    ): ...
-    def copy_key(
-        self,
-        new_key_name,
-        src_bucket_name,
-        src_key_name,
-        metadata: Any | None = ...,
-        src_version_id: Any | None = ...,
-        storage_class: str = ...,
-        preserve_acl: bool = ...,
+        version_id: Any | None = ...,
+        policy: Any | None = ...,
+        reduced_redundancy: bool = ...,
         encrypt_key: bool = ...,
-        headers: dict[Text, Text] | None = ...,
+    ): ...
+    def send_file(
+        self,
+        fp,
+        headers: dict[str, str] | None = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
         query_args: Any | None = ...,
+        chunked_transfer: bool = ...,
+        size: Any | None = ...,
     ): ...
-    def set_canned_acl(
-        self, acl_str, key_name: str = ..., headers: dict[Text, Text] | None = ..., version_id: Any | None = ...
+    def should_retry(self, response, chunked_transfer: bool = ...): ...
+    def compute_md5(self, fp, size: Any | None = ...): ...
+    def set_contents_from_stream(
+        self,
+        fp,
+        headers: dict[str, str] | None = ...,
+        replace: bool = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
+        policy: Any | None = ...,
+        reduced_redundancy: bool = ...,
+        query_args: Any | None = ...,
+        size: Any | None = ...,
     ): ...
-    def get_xml_acl(self, key_name: str = ..., headers: dict[Text, Text] | None = ..., version_id: Any | None = ...): ...
-    def set_xml_acl(
+    def set_contents_from_file(
         self,
-        acl_str,
-        key_name: str = ...,
-        headers: dict[Text, Text] | None = ...,
-        version_id: Any | None = ...,
-        query_args: str = ...,
+        fp,
+        headers: dict[str, str] | None = ...,
+        replace: bool = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
+        policy: Any | None = ...,
+        md5: Any | None = ...,
+        reduced_redundancy: bool = ...,
+        query_args: Any | None = ...,
+        encrypt_key: bool = ...,
+        size: Any | None = ...,
+        rewind: bool = ...,
     ): ...
-    def set_acl(self, acl_or_str, key_name: str = ..., headers: dict[Text, Text] | None = ..., version_id: Any | None = ...): ...
-    def get_acl(self, key_name: str = ..., headers: dict[Text, Text] | None = ..., version_id: Any | None = ...): ...
-    def set_subresource(
-        self, subresource, value, key_name: str = ..., headers: dict[Text, Text] | None = ..., version_id: Any | None = ...
-    ): ...
-    def get_subresource(
-        self, subresource, key_name: str = ..., headers: dict[Text, Text] | None = ..., version_id: Any | None = ...
-    ): ...
-    def make_public(self, recursive: bool = ..., headers: dict[Text, Text] | None = ...): ...
-    def add_email_grant(self, permission, email_address, recursive: bool = ..., headers: dict[Text, Text] | None = ...): ...
-    def add_user_grant(
-        self, permission, user_id, recursive: bool = ..., headers: dict[Text, Text] | None = ..., display_name: Any | None = ...
-    ): ...
-    def list_grants(self, headers: dict[Text, Text] | None = ...): ...
-    def get_location(self): ...
-    def set_xml_logging(self, logging_str, headers: dict[Text, Text] | None = ...): ...
-    def enable_logging(
-        self, target_bucket, target_prefix: str = ..., grants: Any | None = ..., headers: dict[Text, Text] | None = ...
-    ): ...
-    def disable_logging(self, headers: dict[Text, Text] | None = ...): ...
-    def get_logging_status(self, headers: dict[Text, Text] | None = ...): ...
-    def set_as_logging_target(self, headers: dict[Text, Text] | None = ...): ...
-    def get_request_payment(self, headers: dict[Text, Text] | None = ...): ...
-    def set_request_payment(self, payer: str = ..., headers: dict[Text, Text] | None = ...): ...
-    def configure_versioning(
-        self, versioning, mfa_delete: bool = ..., mfa_token: Any | None = ..., headers: dict[Text, Text] | None = ...
-    ): ...
-    def get_versioning_status(self, headers: dict[Text, Text] | None = ...): ...
-    def configure_lifecycle(self, lifecycle_config, headers: dict[Text, Text] | None = ...): ...
-    def get_lifecycle_config(self, headers: dict[Text, Text] | None = ...): ...
-    def delete_lifecycle_configuration(self, headers: dict[Text, Text] | None = ...): ...
-    def configure_website(
-        self,
-        suffix: Any | None = ...,
-        error_key: Any | None = ...,
-        redirect_all_requests_to: Any | None = ...,
-        routing_rules: Any | None = ...,
-        headers: dict[Text, Text] | None = ...,
-    ): ...
-    def set_website_configuration(self, config, headers: dict[Text, Text] | None = ...): ...
-    def set_website_configuration_xml(self, xml, headers: dict[Text, Text] | None = ...): ...
-    def get_website_configuration(self, headers: dict[Text, Text] | None = ...): ...
-    def get_website_configuration_obj(self, headers: dict[Text, Text] | None = ...): ...
-    def get_website_configuration_with_xml(self, headers: dict[Text, Text] | None = ...): ...
-    def get_website_configuration_xml(self, headers: dict[Text, Text] | None = ...): ...
-    def delete_website_configuration(self, headers: dict[Text, Text] | None = ...): ...
-    def get_website_endpoint(self): ...
-    def get_policy(self, headers: dict[Text, Text] | None = ...): ...
-    def set_policy(self, policy, headers: dict[Text, Text] | None = ...): ...
-    def delete_policy(self, headers: dict[Text, Text] | None = ...): ...
-    def set_cors_xml(self, cors_xml, headers: dict[Text, Text] | None = ...): ...
-    def set_cors(self, cors_config, headers: dict[Text, Text] | None = ...): ...
-    def get_cors_xml(self, headers: dict[Text, Text] | None = ...): ...
-    def get_cors(self, headers: dict[Text, Text] | None = ...): ...
-    def delete_cors(self, headers: dict[Text, Text] | None = ...): ...
-    def initiate_multipart_upload(
+    def set_contents_from_filename(
         self,
-        key_name,
-        headers: dict[Text, Text] | None = ...,
+        filename,
+        headers: dict[str, str] | None = ...,
+        replace: bool = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
+        policy: Any | None = ...,
+        md5: Any | None = ...,
         reduced_redundancy: bool = ...,
-        metadata: Any | None = ...,
         encrypt_key: bool = ...,
+    ): ...
+    def set_contents_from_string(
+        self,
+        string_data: str | bytes,
+        headers: dict[str, str] | None = ...,
+        replace: bool = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
         policy: Any | None = ...,
+        md5: Any | None = ...,
+        reduced_redundancy: bool = ...,
+        encrypt_key: bool = ...,
+    ) -> None: ...
+    def get_file(
+        self,
+        fp,
+        headers: dict[str, str] | None = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
+        torrent: bool = ...,
+        version_id: Any | None = ...,
+        override_num_retries: Any | None = ...,
+        response_headers: dict[str, str] | None = ...,
+    ): ...
+    def get_torrent_file(
+        self, fp, headers: dict[str, str] | None = ..., cb: Callable[[int, int], Any] | None = ..., num_cb: int = ...
+    ): ...
+    def get_contents_to_file(
+        self,
+        fp,
+        headers: dict[str, str] | None = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
+        torrent: bool = ...,
+        version_id: Any | None = ...,
+        res_download_handler: Any | None = ...,
+        response_headers: dict[str, str] | None = ...,
     ): ...
-    def complete_multipart_upload(self, key_name, upload_id, xml_body, headers: dict[Text, Text] | None = ...): ...
-    def cancel_multipart_upload(self, key_name, upload_id, headers: dict[Text, Text] | None = ...): ...
-    def delete(self, headers: dict[Text, Text] | None = ...): ...
-    def get_tags(self): ...
-    def get_xml_tags(self): ...
-    def set_xml_tags(self, tag_str, headers: dict[Text, Text] | None = ..., query_args: str = ...): ...
-    def set_tags(self, tags, headers: dict[Text, Text] | None = ...): ...
-    def delete_tags(self, headers: dict[Text, Text] | None = ...): ...
+    def get_contents_to_filename(
+        self,
+        filename,
+        headers: dict[str, str] | None = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
+        torrent: bool = ...,
+        version_id: Any | None = ...,
+        res_download_handler: Any | None = ...,
+        response_headers: dict[str, str] | None = ...,
+    ): ...
+    @overload
+    def get_contents_as_string(
+        self,
+        headers: dict[str, str] | None = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
+        torrent: bool = ...,
+        version_id: Any | None = ...,
+        response_headers: dict[str, str] | None = ...,
+        encoding: None = ...,
+    ) -> bytes: ...
+    @overload
+    def get_contents_as_string(
+        self,
+        headers: dict[str, str] | None = ...,
+        cb: Callable[[int, int], Any] | None = ...,
+        num_cb: int = ...,
+        torrent: bool = ...,
+        version_id: Any | None = ...,
+        response_headers: dict[str, str] | None = ...,
+        *,
+        encoding: str,
+    ) -> str: ...
+    def add_email_grant(self, permission, email_address, headers: dict[str, str] | None = ...): ...
+    def add_user_grant(self, permission, user_id, headers: dict[str, str] | None = ..., display_name: Any | None = ...): ...
+    def set_remote_metadata(self, metadata_plus, metadata_minus, preserve_acl, headers: dict[str, str] | None = ...): ...
+    def restore(self, days, headers: dict[str, str] | None = ...): ...
```

### Comparing `types-boto-2.49.8/boto-stubs/s3/bucketlistresultset.pyi` & `types-boto-2.49.9/boto-stubs/s3/bucketlistresultset.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/s3/connection.pyi` & `types-boto-2.49.9/boto-stubs/s3/connection.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Text
+from typing import Any
 
 from boto.connection import AWSAuthConnection
 from boto.exception import BotoClientError
 
 from .bucket import Bucket
 
 def check_lowercase_bucketname(n): ...
@@ -93,36 +93,34 @@
     ): ...
     def generate_url_sigv4(
         self,
         expires_in,
         method,
         bucket: str = ...,
         key: str = ...,
-        headers: dict[Text, Text] | None = ...,
+        headers: dict[str, str] | None = ...,
         force_http: bool = ...,
-        response_headers: dict[Text, Text] | None = ...,
+        response_headers: dict[str, str] | None = ...,
         version_id: Any | None = ...,
         iso_date: Any | None = ...,
     ): ...
     def generate_url(
         self,
         expires_in,
         method,
         bucket: str = ...,
         key: str = ...,
-        headers: dict[Text, Text] | None = ...,
+        headers: dict[str, str] | None = ...,
         query_auth: bool = ...,
         force_http: bool = ...,
-        response_headers: dict[Text, Text] | None = ...,
+        response_headers: dict[str, str] | None = ...,
         expires_in_absolute: bool = ...,
         version_id: Any | None = ...,
     ): ...
-    def get_all_buckets(self, headers: dict[Text, Text] | None = ...): ...
-    def get_canonical_user_id(self, headers: dict[Text, Text] | None = ...): ...
-    def get_bucket(self, bucket_name: Text, validate: bool = ..., headers: dict[Text, Text] | None = ...) -> Bucket: ...
-    def head_bucket(self, bucket_name, headers: dict[Text, Text] | None = ...): ...
-    def lookup(self, bucket_name, validate: bool = ..., headers: dict[Text, Text] | None = ...): ...
-    def create_bucket(
-        self, bucket_name, headers: dict[Text, Text] | None = ..., location: Any = ..., policy: Any | None = ...
-    ): ...
-    def delete_bucket(self, bucket, headers: dict[Text, Text] | None = ...): ...
+    def get_all_buckets(self, headers: dict[str, str] | None = ...): ...
+    def get_canonical_user_id(self, headers: dict[str, str] | None = ...): ...
+    def get_bucket(self, bucket_name: str, validate: bool = ..., headers: dict[str, str] | None = ...) -> Bucket: ...
+    def head_bucket(self, bucket_name, headers: dict[str, str] | None = ...): ...
+    def lookup(self, bucket_name, validate: bool = ..., headers: dict[str, str] | None = ...): ...
+    def create_bucket(self, bucket_name, headers: dict[str, str] | None = ..., location: Any = ..., policy: Any | None = ...): ...
+    def delete_bucket(self, bucket, headers: dict[str, str] | None = ...): ...
     def make_request(self, method, bucket: str = ..., key: str = ..., headers: Any | None = ..., data: str = ..., query_args: Any | None = ..., sender: Any | None = ..., override_num_retries: Any | None = ..., retry_handler: Any | None = ..., *args, **kwargs): ...  # type: ignore # https://github.com/python/mypy/issues/1237
```

### Comparing `types-boto-2.49.8/boto-stubs/s3/cors.pyi` & `types-boto-2.49.9/boto-stubs/s3/cors.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/s3/keyfile.pyi` & `types-boto-2.49.9/boto-stubs/s3/keyfile.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/s3/lifecycle.pyi` & `types-boto-2.49.9/boto-stubs/s3/lifecycle.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/s3/multidelete.pyi` & `types-boto-2.49.9/boto-stubs/s3/multidelete.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/s3/multipart.pyi` & `types-boto-2.49.9/boto-stubs/s3/multipart.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/s3/tagging.pyi` & `types-boto-2.49.9/boto-stubs/s3/tagging.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/s3/website.pyi` & `types-boto-2.49.9/boto-stubs/s3/website.pyi`

 * *Files identical despite different names*

### Comparing `types-boto-2.49.8/boto-stubs/utils.pyi` & `types-boto-2.49.9/boto-stubs/utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import logging.handlers
 import subprocess
 import sys
 import time
-from typing import IO, Any, Callable, ContextManager, Iterable, Mapping, Sequence, TypeVar
+from contextlib import AbstractContextManager
+from typing import IO, Any, Callable, Iterable, Mapping, Sequence, TypeVar
 
 import boto.connection
 
 _KT = TypeVar("_KT")
 _VT = TypeVar("_VT")
 
 if sys.version_info >= (3,):
@@ -64,15 +65,15 @@
 ) -> Mapping[str, str]: ...
 
 ISO8601: str
 ISO8601_MS: str
 RFC1123: str
 LOCALE_LOCK: _LockType
 
-def setlocale(name: str | tuple[str, str]) -> ContextManager[str]: ...
+def setlocale(name: str | tuple[str, str]) -> AbstractContextManager[str]: ...
 def get_ts(ts: time.struct_time | None = ...) -> str: ...
 def parse_ts(ts: str) -> datetime.datetime: ...
 def find_class(module_name: str, class_name: str | None = ...) -> type[Any] | None: ...
 def update_dme(username: str, password: str, dme_id: str, ip_address: str) -> str: ...
 def fetch_file(
     uri: str, file: IO[str] | None = ..., username: str | None = ..., password: str | None = ...
 ) -> IO[str] | None: ...
```

### Comparing `types-boto-2.49.8/setup.py` & `types-boto-2.49.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `boto` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `boto`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/boto. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `c3907ab26b1c75bc19163aa828d1197ae8640127`.
+This package was generated from typeshed commit `9a1f5fb06cc9ca4938ba78301664a79e1718f8fb`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.49.8",
+      version="2.49.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boto.md",
```

### Comparing `types-boto-2.49.8/types_boto.egg-info/PKG-INFO` & `types-boto-2.49.9/types_boto.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-boto
-Version: 2.49.8
+Version: 2.49.9
 Summary: Typing stubs for boto
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boto.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `boto` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `boto`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/boto. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `c3907ab26b1c75bc19163aa828d1197ae8640127`.
+This package was generated from typeshed commit `9a1f5fb06cc9ca4938ba78301664a79e1718f8fb`.
```

### Comparing `types-boto-2.49.8/types_boto.egg-info/SOURCES.txt` & `types-boto-2.49.9/types_boto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

