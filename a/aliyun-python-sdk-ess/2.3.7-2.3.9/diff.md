# Comparing `tmp/aliyun-python-sdk-ess-2.3.7.tar.gz` & `tmp/aliyun-python-sdk-ess-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ess-2.3.7.tar", last modified: Thu Feb  9 02:52:10 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ess-2.3.9.tar", last modified: Wed Jul 12 08:09:14 2023, max compression
```

## Comparing `aliyun-python-sdk-ess-2.3.7.tar` & `aliyun-python-sdk-ess-2.3.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/
--rw-r--r--   0 root         (0) root         (0)      575 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyun_python_sdk_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyun_python_sdk_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5162 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyun_python_sdk_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyun_python_sdk_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyun_python_sdk_ess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyun_python_sdk_ess.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3033 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/
--rw-r--r--   0 root         (0) root         (0)     3061 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachAlbServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2577 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachDBInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3321 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachLoadBalancersRequest.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3738 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachVServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2333 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2837 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CompleteLifecycleActionRequest.py
--rw-r--r--   0 root         (0) root         (0)     6140 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateAlarmRequest.py
--rw-r--r--   0 root         (0) root         (0)    33751 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateEciScalingConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3506 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateLifecycleHookRequest.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateNotificationConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)    20126 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateScalingConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)    15264 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateScalingGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     6992 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateScalingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateScheduledTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2188 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeactivateScalingConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteAlarmRequest.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteEciScalingConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteLifecycleHookRequest.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteNotificationConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteScalingConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2315 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteScalingGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2108 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteScalingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteScheduledTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3200 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeAlarmsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3457 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeEciScalingConfigurationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeLifecycleActionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeLifecycleHooksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeLimitationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1945 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeNotificationConfigurationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeNotificationTypesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3231 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingActivitiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingActivityDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     3451 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingConfigurationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     8195 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4106 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4043 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3644 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScheduledTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachAlbServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2577 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachDBInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3282 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachLoadBalancersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachVServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DisableAlarmRequest.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DisableScalingGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/EnableAlarmRequest.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/EnableScalingGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/EnterStandbyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2944 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ExecuteScalingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ExitStandbyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2253 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ListTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2771 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ListTagValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     6122 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyAlarmRequest.py
--rw-r--r--   0 root         (0) root         (0)    34056 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyEciScalingConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyLifecycleHookRequest.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyNotificationConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)    19218 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyScalingConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     9161 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyScalingGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     6982 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyScalingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     5104 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyScheduledTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2333 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/RebalanceInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/RecordLifecycleActionHeartbeatRequest.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/RemoveInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ResumeProcessesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3020 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ScaleWithAdjustmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/SetGroupDeletionProtectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/SetInstanceHealthRequest.py
--rw-r--r--   0 root         (0) root         (0)     2444 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/SetInstancesProtectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/SuspendProcessesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2724 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/VerifyAuthenticationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/VerifyUserRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-02-09 02:52:10.000000 aliyun-python-sdk-ess-2.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyun_python_sdk_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyun_python_sdk_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5162 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyun_python_sdk_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyun_python_sdk_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyun_python_sdk_ess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyun_python_sdk_ess.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/
+-rw-r--r--   0 root         (0) root         (0)     3061 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachAlbServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachDBInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3380 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachLoadBalancersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3738 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachVServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CompleteLifecycleActionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateAlarmRequest.py
+-rw-r--r--   0 root         (0) root         (0)    33951 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateEciScalingConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3506 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateLifecycleHookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateNotificationConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)    20417 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateScalingConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)    15884 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateScalingGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7586 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateScalingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateScheduledTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeactivateScalingConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteAlarmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteEciScalingConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteLifecycleHookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteNotificationConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteScalingConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteScalingGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteScalingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteScheduledTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeAlarmsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeEciScalingConfigurationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeLifecycleActionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeLifecycleHooksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeLimitationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeNotificationConfigurationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeNotificationTypesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3231 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingActivitiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingActivityDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingConfigurationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8195 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4106 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4043 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScheduledTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachAlbServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachDBInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachLoadBalancersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachVServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DisableAlarmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DisableScalingGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/EnableAlarmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/EnableScalingGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/EnterStandbyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ExecuteScalingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ExitStandbyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ListTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ListTagValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6122 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyAlarmRequest.py
+-rw-r--r--   0 root         (0) root         (0)    34256 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyEciScalingConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyLifecycleHookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyNotificationConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)    19509 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyScalingConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     9161 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyScalingGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7576 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyScalingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5104 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyScheduledTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/RebalanceInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/RecordLifecycleActionHeartbeatRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/RemoveInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ResumeProcessesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ScaleWithAdjustmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/SetGroupDeletionProtectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/SetInstanceHealthRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/SetInstancesProtectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/SuspendProcessesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/VerifyAuthenticationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/VerifyUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-07-12 08:09:14.000000 aliyun-python-sdk-ess-2.3.9/setup.py
```

### Comparing `aliyun-python-sdk-ess-2.3.7/LICENSE` & `aliyun-python-sdk-ess-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/PKG-INFO` & `aliyun-python-sdk-ess-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ess
-Version: 2.3.7
+Version: 2.3.9
 Summary: The ess module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ess
```

### Comparing `aliyun-python-sdk-ess-2.3.7/README.rst` & `aliyun-python-sdk-ess-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyun_python_sdk_ess.egg-info/PKG-INFO` & `aliyun-python-sdk-ess-2.3.9/aliyun_python_sdk_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ess
-Version: 2.3.7
+Version: 2.3.9
 Summary: The ess module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ess
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyun_python_sdk_ess.egg-info/SOURCES.txt` & `aliyun-python-sdk-ess-2.3.9/aliyun_python_sdk_ess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/endpoint.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachAlbServerGroupsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachAlbServerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachDBInstancesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachDBInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachInstancesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachLoadBalancersRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachLoadBalancersRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkess.endpoint import endpoint_data
 
-class AttachLoadBalancersRequest(RpcRequest):
+class DetachLoadBalancersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Ess', '2014-08-28', 'AttachLoadBalancers','ess')
+		RpcRequest.__init__(self, 'Ess', '2014-08-28', 'DetachLoadBalancers','ess')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,19 +37,14 @@
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_ScalingGroupId(self): # String
 		return self.get_query_params().get('ScalingGroupId')
 
 	def set_ScalingGroupId(self, ScalingGroupId):  # String
 		self.add_query_param('ScalingGroupId', ScalingGroupId)
-	def get_ForceAttach(self): # Boolean
-		return self.get_query_params().get('ForceAttach')
-
-	def set_ForceAttach(self, ForceAttach):  # Boolean
-		self.add_query_param('ForceAttach', ForceAttach)
 	def get_LoadBalancers(self): # RepeatList
 		return self.get_query_params().get('LoadBalancer')
 
 	def set_LoadBalancers(self, LoadBalancer):  # RepeatList
 		for depth1 in range(len(LoadBalancer)):
 			self.add_query_param('LoadBalancer.' + str(depth1 + 1), LoadBalancer[depth1])
 	def get_ResourceOwnerAccount(self): # String
@@ -63,7 +58,12 @@
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_Async(self): # Boolean
 		return self.get_query_params().get('Async')
 
 	def set_Async(self, _Async):  # Boolean
 		self.add_query_param('Async', _Async)
+	def get_ForceDetach(self): # Boolean
+		return self.get_query_params().get('ForceDetach')
+
+	def set_ForceDetach(self, ForceDetach):  # Boolean
+		self.add_query_param('ForceDetach', ForceDetach)
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachServerGroupsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachServerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/AttachVServerGroupsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachVServerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ChangeResourceGroupRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ChangeResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CompleteLifecycleActionRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CompleteLifecycleActionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateAlarmRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateAlarmRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateEciScalingConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateEciScalingConfigurationRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,16 @@
 	def get_Volumes(self): # RepeatList
 		return self.get_query_params().get('Volume')
 
 	def set_Volumes(self, Volume):  # RepeatList
 		for depth1 in range(len(Volume)):
 			if Volume[depth1].get('DiskVolume.FsType') is not None:
 				self.add_query_param('Volume.' + str(depth1 + 1) + '.DiskVolume.FsType', Volume[depth1].get('DiskVolume.FsType'))
+			if Volume[depth1].get('EmptyDirVolume.SizeLimit') is not None:
+				self.add_query_param('Volume.' + str(depth1 + 1) + '.EmptyDirVolume.SizeLimit', Volume[depth1].get('EmptyDirVolume.SizeLimit'))
 			if Volume[depth1].get('NFSVolume.Path') is not None:
 				self.add_query_param('Volume.' + str(depth1 + 1) + '.NFSVolume.Path', Volume[depth1].get('NFSVolume.Path'))
 			if Volume[depth1].get('DiskVolume.DiskId') is not None:
 				self.add_query_param('Volume.' + str(depth1 + 1) + '.DiskVolume.DiskId', Volume[depth1].get('DiskVolume.DiskId'))
 			if Volume[depth1].get('FlexVolume.FsType') is not None:
 				self.add_query_param('Volume.' + str(depth1 + 1) + '.FlexVolume.FsType', Volume[depth1].get('FlexVolume.FsType'))
 			if Volume[depth1].get('Type') is not None:
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateLifecycleHookRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateLifecycleHookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateNotificationConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateNotificationConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateScalingConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateScalingConfigurationRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,19 @@
 	def set_SystemDiskAutoSnapshotPolicyId(self, SystemDiskAutoSnapshotPolicyId):  # String
 		self.add_query_param('SystemDisk.AutoSnapshotPolicyId', SystemDiskAutoSnapshotPolicyId)
 	def get_PrivatePoolOptionsId(self): # String
 		return self.get_query_params().get('PrivatePoolOptions.Id')
 
 	def set_PrivatePoolOptionsId(self, PrivatePoolOptionsId):  # String
 		self.add_query_param('PrivatePoolOptions.Id', PrivatePoolOptionsId)
+	def get_ImageOptionsLoginAsNonRoot(self): # Boolean
+		return self.get_query_params().get('ImageOptions.LoginAsNonRoot')
+
+	def set_ImageOptionsLoginAsNonRoot(self, ImageOptionsLoginAsNonRoot):  # Boolean
+		self.add_query_param('ImageOptions.LoginAsNonRoot', ImageOptionsLoginAsNonRoot)
 	def get_Ipv6AddressCount(self): # Integer
 		return self.get_query_params().get('Ipv6AddressCount')
 
 	def set_Ipv6AddressCount(self, Ipv6AddressCount):  # Integer
 		self.add_query_param('Ipv6AddressCount', Ipv6AddressCount)
 	def get_Cpu(self): # Integer
 		return self.get_query_params().get('Cpu')
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateScalingGroupRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateScalingGroupRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,23 @@
 	def set_LoadBalancerIds(self, LoadBalancerIds):  # String
 		self.add_query_param('LoadBalancerIds', LoadBalancerIds)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
+	def get_LoadBalancerConfigs(self): # RepeatList
+		return self.get_query_params().get('LoadBalancerConfig')
+
+	def set_LoadBalancerConfigs(self, LoadBalancerConfig):  # RepeatList
+		for depth1 in range(len(LoadBalancerConfig)):
+			if LoadBalancerConfig[depth1].get('LoadBalancerId') is not None:
+				self.add_query_param('LoadBalancerConfig.' + str(depth1 + 1) + '.LoadBalancerId', LoadBalancerConfig[depth1].get('LoadBalancerId'))
+			if LoadBalancerConfig[depth1].get('Weight') is not None:
+				self.add_query_param('LoadBalancerConfig.' + str(depth1 + 1) + '.Weight', LoadBalancerConfig[depth1].get('Weight'))
 	def get_OnDemandBaseCapacity(self): # Integer
 		return self.get_query_params().get('OnDemandBaseCapacity')
 
 	def set_OnDemandBaseCapacity(self, OnDemandBaseCapacity):  # Integer
 		self.add_query_param('OnDemandBaseCapacity', OnDemandBaseCapacity)
 	def get_OnDemandPercentageAboveBaseCapacity(self): # Integer
 		return self.get_query_params().get('OnDemandPercentageAboveBaseCapacity')
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateScalingRuleRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateScalingRuleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,23 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_AlarmDimensions(self): # RepeatList
+		return self.get_query_params().get('AlarmDimension')
+
+	def set_AlarmDimensions(self, AlarmDimension):  # RepeatList
+		for depth1 in range(len(AlarmDimension)):
+			if AlarmDimension[depth1].get('DimensionValue') is not None:
+				self.add_query_param('AlarmDimension.' + str(depth1 + 1) + '.DimensionValue', AlarmDimension[depth1].get('DimensionValue'))
+			if AlarmDimension[depth1].get('DimensionKey') is not None:
+				self.add_query_param('AlarmDimension.' + str(depth1 + 1) + '.DimensionKey', AlarmDimension[depth1].get('DimensionKey'))
 	def get_StepAdjustments(self): # RepeatList
 		return self.get_query_params().get('StepAdjustment')
 
 	def set_StepAdjustments(self, StepAdjustment):  # RepeatList
 		for depth1 in range(len(StepAdjustment)):
 			if StepAdjustment[depth1].get('MetricIntervalUpperBound') is not None:
 				self.add_query_param('StepAdjustment.' + str(depth1 + 1) + '.MetricIntervalUpperBound', StepAdjustment[depth1].get('MetricIntervalUpperBound'))
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/CreateScheduledTaskRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/CreateScheduledTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeactivateScalingConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeactivateScalingConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteAlarmRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteAlarmRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteEciScalingConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteEciScalingConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteLifecycleHookRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteLifecycleHookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteNotificationConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteNotificationConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteScalingConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteScalingConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteScalingGroupRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteScalingGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteScalingRuleRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteScalingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DeleteScheduledTaskRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DeleteScheduledTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeAlarmsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeAlarmsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeEciScalingConfigurationsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeEciScalingConfigurationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeLifecycleActionsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeLifecycleActionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeLifecycleHooksRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeLifecycleHooksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeLimitationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeLimitationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeNotificationConfigurationsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeNotificationConfigurationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeNotificationTypesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeNotificationTypesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeRegionsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingActivitiesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingActivitiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingActivityDetailRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingActivityDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingConfigurationsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingConfigurationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingGroupsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingInstancesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScalingRulesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScalingRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DescribeScheduledTasksRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DescribeScheduledTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachAlbServerGroupsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachAlbServerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachDBInstancesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachDBInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachInstancesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachLoadBalancersRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/AttachLoadBalancersRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkess.endpoint import endpoint_data
 
-class DetachLoadBalancersRequest(RpcRequest):
+class AttachLoadBalancersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Ess', '2014-08-28', 'DetachLoadBalancers','ess')
+		RpcRequest.__init__(self, 'Ess', '2014-08-28', 'AttachLoadBalancers','ess')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,14 +37,28 @@
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_ScalingGroupId(self): # String
 		return self.get_query_params().get('ScalingGroupId')
 
 	def set_ScalingGroupId(self, ScalingGroupId):  # String
 		self.add_query_param('ScalingGroupId', ScalingGroupId)
+	def get_ForceAttach(self): # Boolean
+		return self.get_query_params().get('ForceAttach')
+
+	def set_ForceAttach(self, ForceAttach):  # Boolean
+		self.add_query_param('ForceAttach', ForceAttach)
+	def get_LoadBalancerConfigs(self): # RepeatList
+		return self.get_query_params().get('LoadBalancerConfig')
+
+	def set_LoadBalancerConfigs(self, LoadBalancerConfig):  # RepeatList
+		for depth1 in range(len(LoadBalancerConfig)):
+			if LoadBalancerConfig[depth1].get('LoadBalancerId') is not None:
+				self.add_query_param('LoadBalancerConfig.' + str(depth1 + 1) + '.LoadBalancerId', LoadBalancerConfig[depth1].get('LoadBalancerId'))
+			if LoadBalancerConfig[depth1].get('Weight') is not None:
+				self.add_query_param('LoadBalancerConfig.' + str(depth1 + 1) + '.Weight', LoadBalancerConfig[depth1].get('Weight'))
 	def get_LoadBalancers(self): # RepeatList
 		return self.get_query_params().get('LoadBalancer')
 
 	def set_LoadBalancers(self, LoadBalancer):  # RepeatList
 		for depth1 in range(len(LoadBalancer)):
 			self.add_query_param('LoadBalancer.' + str(depth1 + 1), LoadBalancer[depth1])
 	def get_ResourceOwnerAccount(self): # String
@@ -58,12 +72,7 @@
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_Async(self): # Boolean
 		return self.get_query_params().get('Async')
 
 	def set_Async(self, _Async):  # Boolean
 		self.add_query_param('Async', _Async)
-	def get_ForceDetach(self): # Boolean
-		return self.get_query_params().get('ForceDetach')
-
-	def set_ForceDetach(self, ForceDetach):  # Boolean
-		self.add_query_param('ForceDetach', ForceDetach)
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachServerGroupsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachServerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DetachVServerGroupsRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DetachVServerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DisableAlarmRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DisableAlarmRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/DisableScalingGroupRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/DisableScalingGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/EnableAlarmRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/EnableAlarmRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/EnableScalingGroupRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/EnableScalingGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/EnterStandbyRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/EnterStandbyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ExecuteScalingRuleRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ExecuteScalingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ExitStandbyRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ExitStandbyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ListTagKeysRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ListTagKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ListTagResourcesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ListTagValuesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ListTagValuesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyAlarmRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyAlarmRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyEciScalingConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyEciScalingConfigurationRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,16 @@
 	def get_Volumes(self): # RepeatList
 		return self.get_query_params().get('Volume')
 
 	def set_Volumes(self, Volume):  # RepeatList
 		for depth1 in range(len(Volume)):
 			if Volume[depth1].get('DiskVolume.FsType') is not None:
 				self.add_query_param('Volume.' + str(depth1 + 1) + '.DiskVolume.FsType', Volume[depth1].get('DiskVolume.FsType'))
+			if Volume[depth1].get('EmptyDirVolume.SizeLimit') is not None:
+				self.add_query_param('Volume.' + str(depth1 + 1) + '.EmptyDirVolume.SizeLimit', Volume[depth1].get('EmptyDirVolume.SizeLimit'))
 			if Volume[depth1].get('NFSVolume.Path') is not None:
 				self.add_query_param('Volume.' + str(depth1 + 1) + '.NFSVolume.Path', Volume[depth1].get('NFSVolume.Path'))
 			if Volume[depth1].get('DiskVolume.DiskId') is not None:
 				self.add_query_param('Volume.' + str(depth1 + 1) + '.DiskVolume.DiskId', Volume[depth1].get('DiskVolume.DiskId'))
 			if Volume[depth1].get('FlexVolume.FsType') is not None:
 				self.add_query_param('Volume.' + str(depth1 + 1) + '.FlexVolume.FsType', Volume[depth1].get('FlexVolume.FsType'))
 			if Volume[depth1].get('Type') is not None:
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyLifecycleHookRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyLifecycleHookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyNotificationConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyNotificationConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyScalingConfigurationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyScalingConfigurationRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,19 @@
 	def set_SystemDiskAutoSnapshotPolicyId(self, SystemDiskAutoSnapshotPolicyId):  # String
 		self.add_query_param('SystemDisk.AutoSnapshotPolicyId', SystemDiskAutoSnapshotPolicyId)
 	def get_PrivatePoolOptionsId(self): # String
 		return self.get_query_params().get('PrivatePoolOptions.Id')
 
 	def set_PrivatePoolOptionsId(self, PrivatePoolOptionsId):  # String
 		self.add_query_param('PrivatePoolOptions.Id', PrivatePoolOptionsId)
+	def get_ImageOptionsLoginAsNonRoot(self): # Boolean
+		return self.get_query_params().get('ImageOptions.LoginAsNonRoot')
+
+	def set_ImageOptionsLoginAsNonRoot(self, ImageOptionsLoginAsNonRoot):  # Boolean
+		self.add_query_param('ImageOptions.LoginAsNonRoot', ImageOptionsLoginAsNonRoot)
 	def get_Ipv6AddressCount(self): # Integer
 		return self.get_query_params().get('Ipv6AddressCount')
 
 	def set_Ipv6AddressCount(self, Ipv6AddressCount):  # Integer
 		self.add_query_param('Ipv6AddressCount', Ipv6AddressCount)
 	def get_Cpu(self): # Integer
 		return self.get_query_params().get('Cpu')
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyScalingGroupRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyScalingGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyScalingRuleRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyScalingRuleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,23 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AlarmDimensions(self): # RepeatList
+		return self.get_query_params().get('AlarmDimension')
+
+	def set_AlarmDimensions(self, AlarmDimension):  # RepeatList
+		for depth1 in range(len(AlarmDimension)):
+			if AlarmDimension[depth1].get('DimensionValue') is not None:
+				self.add_query_param('AlarmDimension.' + str(depth1 + 1) + '.DimensionValue', AlarmDimension[depth1].get('DimensionValue'))
+			if AlarmDimension[depth1].get('DimensionKey') is not None:
+				self.add_query_param('AlarmDimension.' + str(depth1 + 1) + '.DimensionKey', AlarmDimension[depth1].get('DimensionKey'))
 	def get_StepAdjustments(self): # RepeatList
 		return self.get_query_params().get('StepAdjustment')
 
 	def set_StepAdjustments(self, StepAdjustment):  # RepeatList
 		for depth1 in range(len(StepAdjustment)):
 			if StepAdjustment[depth1].get('MetricIntervalUpperBound') is not None:
 				self.add_query_param('StepAdjustment.' + str(depth1 + 1) + '.MetricIntervalUpperBound', StepAdjustment[depth1].get('MetricIntervalUpperBound'))
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ModifyScheduledTaskRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ModifyScheduledTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/RebalanceInstancesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/RebalanceInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/RecordLifecycleActionHeartbeatRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/RecordLifecycleActionHeartbeatRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/RemoveInstancesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/RemoveInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ResumeProcessesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ResumeProcessesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/ScaleWithAdjustmentRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/ScaleWithAdjustmentRequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,34 +27,39 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AdjustmentValue(self): # Integer
-		return self.get_query_params().get('AdjustmentValue')
-
-	def set_AdjustmentValue(self, AdjustmentValue):  # Integer
-		self.add_query_param('AdjustmentValue', AdjustmentValue)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
-	def get_ResourceOwnerAccount(self): # String
-		return self.get_query_params().get('ResourceOwnerAccount')
-
-	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
-		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_ScalingGroupId(self): # String
 		return self.get_query_params().get('ScalingGroupId')
 
 	def set_ScalingGroupId(self, ScalingGroupId):  # String
 		self.add_query_param('ScalingGroupId', ScalingGroupId)
+	def get_SyncActivity(self): # Boolean
+		return self.get_query_params().get('SyncActivity')
+
+	def set_SyncActivity(self, SyncActivity):  # Boolean
+		self.add_query_param('SyncActivity', SyncActivity)
+	def get_AdjustmentValue(self): # Integer
+		return self.get_query_params().get('AdjustmentValue')
+
+	def set_AdjustmentValue(self, AdjustmentValue):  # Integer
+		self.add_query_param('AdjustmentValue', AdjustmentValue)
+	def get_ResourceOwnerAccount(self): # String
+		return self.get_query_params().get('ResourceOwnerAccount')
+
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_AdjustmentType(self): # String
 		return self.get_query_params().get('AdjustmentType')
 
 	def set_AdjustmentType(self, AdjustmentType):  # String
 		self.add_query_param('AdjustmentType', AdjustmentType)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
@@ -62,12 +67,7 @@
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_MinAdjustmentMagnitude(self): # Integer
 		return self.get_query_params().get('MinAdjustmentMagnitude')
 
 	def set_MinAdjustmentMagnitude(self, MinAdjustmentMagnitude):  # Integer
 		self.add_query_param('MinAdjustmentMagnitude', MinAdjustmentMagnitude)
-	def get_SyncActivity(self): # Boolean
-		return self.get_query_params().get('SyncActivity')
-
-	def set_SyncActivity(self, SyncActivity):  # Boolean
-		self.add_query_param('SyncActivity', SyncActivity)
```

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/SetGroupDeletionProtectionRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/SetGroupDeletionProtectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/SetInstanceHealthRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/SetInstanceHealthRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/SetInstancesProtectionRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/SetInstancesProtectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/SuspendProcessesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/SuspendProcessesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/TagResourcesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/UntagResourcesRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/VerifyAuthenticationRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/VerifyAuthenticationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/aliyunsdkess/request/v20140828/VerifyUserRequest.py` & `aliyun-python-sdk-ess-2.3.9/aliyunsdkess/request/v20140828/VerifyUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ess-2.3.7/setup.py` & `aliyun-python-sdk-ess-2.3.9/setup.py`

 * *Files identical despite different names*

