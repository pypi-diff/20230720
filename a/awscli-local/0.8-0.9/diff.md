# Comparing `tmp/awscli-local-0.8.tar.gz` & `tmp/awscli-local-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awscli-local-0.8.tar", last modified: Sun Aug 23 17:57:15 2020, max compression
+gzip compressed data, was "dist/awscli-local-0.9.tar", last modified: Thu Oct  1 20:20:48 2020, max compression
```

## Comparing `awscli-local-0.8.tar` & `awscli-local-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-08-23 17:57:15.342623 awscli-local-0.8/
--rw-r--r--   0 whummer    (502) staff       (20)      837 2020-08-23 17:57:15.342231 awscli-local-0.8/PKG-INFO
--rw-r--r--   0 whummer    (502) staff       (20)     1767 2020-08-23 17:56:48.000000 awscli-local-0.8/README.md
-drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-08-23 17:57:15.321772 awscli-local-0.8/awscli_local.egg-info/
--rw-r--r--   0 whummer    (502) staff       (20)      837 2020-08-23 17:57:15.000000 awscli-local-0.8/awscli_local.egg-info/PKG-INFO
--rw-r--r--   0 whummer    (502) staff       (20)      227 2020-08-23 17:57:15.000000 awscli-local-0.8/awscli_local.egg-info/SOURCES.txt
--rw-r--r--   0 whummer    (502) staff       (20)        1 2020-08-23 17:57:15.000000 awscli-local-0.8/awscli_local.egg-info/dependency_links.txt
--rw-r--r--   0 whummer    (502) staff       (20)       25 2020-08-23 17:57:15.000000 awscli-local-0.8/awscli_local.egg-info/requires.txt
--rw-r--r--   0 whummer    (502) staff       (20)        1 2020-08-23 17:57:15.000000 awscli-local-0.8/awscli_local.egg-info/top_level.txt
-drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-08-23 17:57:15.335510 awscli-local-0.8/bin/
--rwxr-xr-x   0 whummer    (502) staff       (20)     6862 2020-08-23 17:55:57.000000 awscli-local-0.8/bin/awslocal
--rw-r--r--   0 whummer    (502) staff       (20)       36 2020-07-20 11:06:25.000000 awscli-local-0.8/bin/awslocal.bat
--rw-r--r--   0 whummer    (502) staff       (20)       38 2020-08-23 17:57:15.342751 awscli-local-0.8/setup.cfg
--rwxr-xr-x   0 whummer    (502) staff       (20)     1184 2020-08-23 17:55:10.000000 awscli-local-0.8/setup.py
+drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-10-01 20:20:48.496584 awscli-local-0.9/
+-rw-r--r--   0 whummer    (502) staff       (20)      837 2020-10-01 20:20:48.496226 awscli-local-0.9/PKG-INFO
+-rw-r--r--   0 whummer    (502) staff       (20)     1921 2020-10-01 20:20:36.000000 awscli-local-0.9/README.md
+drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-10-01 20:20:48.474951 awscli-local-0.9/awscli_local.egg-info/
+-rw-r--r--   0 whummer    (502) staff       (20)      837 2020-10-01 20:20:48.000000 awscli-local-0.9/awscli_local.egg-info/PKG-INFO
+-rw-r--r--   0 whummer    (502) staff       (20)      227 2020-10-01 20:20:48.000000 awscli-local-0.9/awscli_local.egg-info/SOURCES.txt
+-rw-r--r--   0 whummer    (502) staff       (20)        1 2020-10-01 20:20:48.000000 awscli-local-0.9/awscli_local.egg-info/dependency_links.txt
+-rw-r--r--   0 whummer    (502) staff       (20)       25 2020-10-01 20:20:48.000000 awscli-local-0.9/awscli_local.egg-info/requires.txt
+-rw-r--r--   0 whummer    (502) staff       (20)        1 2020-10-01 20:20:48.000000 awscli-local-0.9/awscli_local.egg-info/top_level.txt
+drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-10-01 20:20:48.489162 awscli-local-0.9/bin/
+-rwxr-xr-x   0 whummer    (502) staff       (20)     7195 2020-10-01 20:20:36.000000 awscli-local-0.9/bin/awslocal
+-rw-r--r--   0 whummer    (502) staff       (20)       36 2020-07-20 11:06:25.000000 awscli-local-0.9/bin/awslocal.bat
+-rw-r--r--   0 whummer    (502) staff       (20)       38 2020-10-01 20:20:48.496684 awscli-local-0.9/setup.cfg
+-rwxr-xr-x   0 whummer    (502) staff       (20)     1184 2020-10-01 20:20:36.000000 awscli-local-0.9/setup.py
```

### Comparing `awscli-local-0.8/PKG-INFO` & `awscli-local-0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: awscli-local
-Version: 0.8
+Version: 0.9
 Summary: Thin wrapper around the "aws" command line interface for use with LocalStack
 Home-page: https://github.com/localstack/awscli-local
 Author: Waldemar Hummer
 Author-email: waldemar.hummer@gmail.com
 License: Apache License 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `awscli-local-0.8/README.md` & `awscli-local-0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -36,17 +36,19 @@
 
 You can use the following environment variables for configuration:
 
 * `LOCALSTACK_HOST`: Set the hostname for the localstack instance. Useful when you have
 localstack is bound to another interface (i.e. docker-machine).
 * `USE_SSL`: Whether to use `https` endpoint URLs (required if LocalStack has been started
 with `USE_SSL=true` enabled). Defaults to `false`.
+* `DEFAULT_REGION`: Set the default region. Overrides `AWS_DEFAULT_REGION` environment varible.
 
 ## Change Log
 
+* v0.9: Support for `DEFAULT_REGION` environment variable
 * v0.8: Switch to using edge port for all service endpoints by default
 * v0.7: Apply runtime patch to aws-cli to enable `--s3-endpoint-url` CloudFormation parameter
 * v0.6: Start `aws` CLI command in-memory instead of calling external process
 * v0.5: Support piping binary files to stdout; add .bat file for Windows
 * v0.4: Minor fix for Python 3 compatibility
 * v0.3: Add support for additional service endpoints
 * v0.2: Enable SSL connections; refactor code
```

### Comparing `awscli-local-0.8/awscli_local.egg-info/PKG-INFO` & `awscli-local-0.9/awscli_local.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: awscli-local
-Version: 0.8
+Version: 0.9
 Summary: Thin wrapper around the "aws" command line interface for use with LocalStack
 Home-page: https://github.com/localstack/awscli-local
 Author: Waldemar Hummer
 Author-email: waldemar.hummer@gmail.com
 License: Apache License 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `awscli-local-0.8/bin/awslocal` & `awscli-local-0.9/bin/awslocal`

 * *Files 5% similar despite different names*

```diff
@@ -84,16 +84,23 @@
 
 def prepare_environment():
 
     # prepare env vars
     env_dict = os.environ.copy()
     env_dict['PYTHONWARNINGS'] = os.environ.get(
         'PYTHONWARNINGS', 'ignore:Unverified HTTPS request')
-    env_dict['AWS_DEFAULT_REGION'] = os.environ.get(
-        'AWS_DEFAULT_REGION', 'us-east-1')
+    if os.environ.get('DEFAULT_REGION'):
+        if os.environ.get('AWS_DEFAULT_REGION'):
+            msg = 'Environment variable "AWS_DEFAULT_REGION" will be overwritten by "DEFAULT_REGION"'
+            print('INFO: %s' % msg)
+        env_dict['AWS_DEFAULT_REGION'] = os.environ.get(
+            'DEFAULT_REGION')
+    else:
+        env_dict['AWS_DEFAULT_REGION'] = os.environ.get(
+            'AWS_DEFAULT_REGION', 'us-east-1')
     env_dict['AWS_ACCESS_KEY_ID'] = os.environ.get(
         'AWS_ACCESS_KEY_ID', '_not_needed_locally_')
     env_dict['AWS_SECRET_ACCESS_KEY'] = os.environ.get(
         'AWS_SECRET_ACCESS_KEY', '_not_needed_locally_')
 
     # update environment variables in the current process
     os.environ.update(env_dict)
```

### Comparing `awscli-local-0.8/setup.py` & `awscli-local-0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 if __name__ == '__main__':
 
     setup(
         name='awscli-local',
-        version='0.8',
+        version='0.9',
         description='Thin wrapper around the "aws" command line interface for use with LocalStack',
         author='Waldemar Hummer',
         author_email='waldemar.hummer@gmail.com',
         url='https://github.com/localstack/awscli-local',
         packages=[],
         scripts=['bin/awslocal', 'bin/awslocal.bat'],
         package_data={},
```

