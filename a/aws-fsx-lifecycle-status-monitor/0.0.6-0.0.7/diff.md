# Comparing `tmp/aws-fsx-lifecycle-status-monitor-0.0.6.tar.gz` & `tmp/aws-fsx-lifecycle-status-monitor-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-fsx-lifecycle-status-monitor-0.0.6.tar", last modified: Thu Jul 20 08:10:19 2023, max compression
+gzip compressed data, was "aws-fsx-lifecycle-status-monitor-0.0.7.tar", last modified: Thu Jul 20 17:39:45 2023, max compression
```

## Comparing `aws-fsx-lifecycle-status-monitor-0.0.6.tar` & `aws-fsx-lifecycle-status-monitor-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   452431 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/_jsii/aws_fsx_lifecycle_status_monitor@0.0.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   452790 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.6/LICENSE` & `aws-fsx-lifecycle-status-monitor-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.6/PKG-INFO` & `aws-fsx-lifecycle-status-monitor-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aws-fsx-lifecycle-status-monitor
-Version: 0.0.6
-Summary: aws_fsx_lifecycle_status_monitor
+Version: 0.0.7
+Summary: aws-fsx-lifecycle-status-monitor
 Home-page: https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.6/setup.py` & `aws-fsx-lifecycle-status-monitor-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-fsx-lifecycle-status-monitor",
-    "version": "0.0.6",
-    "description": "aws_fsx_lifecycle_status_monitor",
+    "version": "0.0.7",
+    "description": "aws-fsx-lifecycle-status-monitor",
     "license": "Apache-2.0",
     "url": "https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_fsx_lifecycle_status_monitor",
         "aws_fsx_lifecycle_status_monitor._jsii"
     ],
     "package_data": {
         "aws_fsx_lifecycle_status_monitor._jsii": [
-            "aws_fsx_lifecycle_status_monitor@0.0.6.jsii.tgz"
+            "aws-fsx-lifecycle-status-monitor@0.0.7.jsii.tgz"
         ],
         "aws_fsx_lifecycle_status_monitor": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/__init__.py` & `aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import aws_cdk.aws_sns as _aws_cdk_aws_sns_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
 class FsxLifecycleStatusMonitor(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
-    jsii_type="aws_fsx_lifecycle_status_monitor.FsxLifecycleStatusMonitor",
+    jsii_type="aws-fsx-lifecycle-status-monitor.FsxLifecycleStatusMonitor",
 ):
     '''
     :stability: experimental
     '''
 
     def __init__(
         self,
@@ -61,15 +61,15 @@
         :param id: - unique id.
         :param schedule: (experimental) The schedule for the FSx Lifecycle Status Monitor.
 
         :stability: experimental
         :memberof: FsxLifecycleStatusMonitor - class instance
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0bea38a9f9d3a7ccb22620e56835a7b5cbf0ec89beae2d61e0ea183098f5416c)
+            type_hints = typing.get_type_hints(_typecheckingstub__b81cd38fb38b316d1be164277c3405c07340ac222fdb134c62c28d69a33d4354)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = FsxLifecycleStatusMonitorProps(schedule=schedule)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="createIamPolicy")
@@ -115,66 +115,66 @@
         :stability: experimental
         '''
         return typing.cast(_aws_cdk_aws_lambda_ceddda9d.Function, jsii.get(self, "fn"))
 
     @fn.setter
     def fn(self, value: _aws_cdk_aws_lambda_ceddda9d.Function) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f5b694d5a48779fe78e91dc649a27c8dd309970cb1029cc68a6db3312ca2dd0a)
+            type_hints = typing.get_type_hints(_typecheckingstub__a8b4032180c59ac1c1c0df56b2db93e26a474dc0966a18b6fe0df00ea86e84e8)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "fn", value)
 
     @builtins.property
     @jsii.member(jsii_name="policy")
     def policy(self) -> _aws_cdk_aws_iam_ceddda9d.Policy:
         '''
         :stability: experimental
         '''
         return typing.cast(_aws_cdk_aws_iam_ceddda9d.Policy, jsii.get(self, "policy"))
 
     @policy.setter
     def policy(self, value: _aws_cdk_aws_iam_ceddda9d.Policy) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f0817232f0cba7b0115bdd3fefb7ac5b03061a704e15a06fa2d7fb3439519644)
+            type_hints = typing.get_type_hints(_typecheckingstub__02a1148af1bfc2f0583587e22e7db7e7e8748ffaba4d54835e19a8bf66b5b136)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policy", value)
 
     @builtins.property
     @jsii.member(jsii_name="rule")
     def rule(self) -> _aws_cdk_aws_events_ceddda9d.Rule:
         '''
         :stability: experimental
         '''
         return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.get(self, "rule"))
 
     @rule.setter
     def rule(self, value: _aws_cdk_aws_events_ceddda9d.Rule) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1307118b507bd5fe4ac4e20cfeb79870f16bba9b44d219f4a6506f94baf6b71e)
+            type_hints = typing.get_type_hints(_typecheckingstub__23c10cd73da7a12439f1a5d36cb378b2bb0455726c883157646552ce5281d1cf)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "rule", value)
 
     @builtins.property
     @jsii.member(jsii_name="topic")
     def topic(self) -> _aws_cdk_aws_sns_ceddda9d.Topic:
         '''
         :stability: experimental
         '''
         return typing.cast(_aws_cdk_aws_sns_ceddda9d.Topic, jsii.get(self, "topic"))
 
     @topic.setter
     def topic(self, value: _aws_cdk_aws_sns_ceddda9d.Topic) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5fdedb79384d0423e054048b7b549d7ea785a9973c1ddc97237c3d96599983dd)
+            type_hints = typing.get_type_hints(_typecheckingstub__2c8971392deb4f782b22feab8db090bb4d67e2fb89e84bbd0ac0da200604a66c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topic", value)
 
 
 @jsii.data_type(
-    jsii_type="aws_fsx_lifecycle_status_monitor.FsxLifecycleStatusMonitorProps",
+    jsii_type="aws-fsx-lifecycle-status-monitor.FsxLifecycleStatusMonitorProps",
     jsii_struct_bases=[],
     name_mapping={"schedule": "schedule"},
 )
 class FsxLifecycleStatusMonitorProps:
     def __init__(
         self,
         *,
@@ -185,15 +185,15 @@
         :param schedule: (experimental) The schedule for the FSx Lifecycle Status Monitor.
 
         :stability: experimental
         :export: true
         :interface: FsxLifecycleStatusMonitorProps
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__be461e59cf3d96e472a6b442ffba1268fe66c6514c192dd611bc338a68ef6483)
+            type_hints = typing.get_type_hints(_typecheckingstub__ed85d95b85def793f715df77d38ad651d2df87abc06c2ddb33b2e3ec9da39b8b)
             check_type(argname="argument schedule", value=schedule, expected_type=type_hints["schedule"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if schedule is not None:
             self._values["schedule"] = schedule
 
     @builtins.property
     def schedule(self) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule]:
@@ -225,46 +225,46 @@
 __all__ = [
     "FsxLifecycleStatusMonitor",
     "FsxLifecycleStatusMonitorProps",
 ]
 
 publication.publish()
 
-def _typecheckingstub__0bea38a9f9d3a7ccb22620e56835a7b5cbf0ec89beae2d61e0ea183098f5416c(
+def _typecheckingstub__b81cd38fb38b316d1be164277c3405c07340ac222fdb134c62c28d69a33d4354(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     schedule: typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f5b694d5a48779fe78e91dc649a27c8dd309970cb1029cc68a6db3312ca2dd0a(
+def _typecheckingstub__a8b4032180c59ac1c1c0df56b2db93e26a474dc0966a18b6fe0df00ea86e84e8(
     value: _aws_cdk_aws_lambda_ceddda9d.Function,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f0817232f0cba7b0115bdd3fefb7ac5b03061a704e15a06fa2d7fb3439519644(
+def _typecheckingstub__02a1148af1bfc2f0583587e22e7db7e7e8748ffaba4d54835e19a8bf66b5b136(
     value: _aws_cdk_aws_iam_ceddda9d.Policy,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1307118b507bd5fe4ac4e20cfeb79870f16bba9b44d219f4a6506f94baf6b71e(
+def _typecheckingstub__23c10cd73da7a12439f1a5d36cb378b2bb0455726c883157646552ce5281d1cf(
     value: _aws_cdk_aws_events_ceddda9d.Rule,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__5fdedb79384d0423e054048b7b549d7ea785a9973c1ddc97237c3d96599983dd(
+def _typecheckingstub__2c8971392deb4f782b22feab8db090bb4d67e2fb89e84bbd0ac0da200604a66c(
     value: _aws_cdk_aws_sns_ceddda9d.Topic,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__be461e59cf3d96e472a6b442ffba1268fe66c6514c192dd611bc338a68ef6483(
+def _typecheckingstub__ed85d95b85def793f715df77d38ad651d2df87abc06c2ddb33b2e3ec9da39b8b(
     *,
     schedule: typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO` & `aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aws-fsx-lifecycle-status-monitor
-Version: 0.0.6
-Summary: aws_fsx_lifecycle_status_monitor
+Version: 0.0.7
+Summary: aws-fsx-lifecycle-status-monitor
 Home-page: https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt` & `aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_fsx_lifecycle_status_monitor/py.typed
 src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
 src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
 src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
-src/aws_fsx_lifecycle_status_monitor/_jsii/aws_fsx_lifecycle_status_monitor@0.0.6.jsii.tgz
+src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.7.jsii.tgz
```

