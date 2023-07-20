# Comparing `tmp/types-aws-xray-sdk-2.8.5.tar.gz` & `tmp/types-aws-xray-sdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aws-xray-sdk-2.8.5.tar", last modified: Sat Apr 16 15:19:07 2022, max compression
+gzip compressed data, was "types-aws-xray-sdk-2.9.0.tar", last modified: Sun Jun 26 15:18:03 2022, max compression
```

## Comparing `types-aws-xray-sdk-2.8.5.tar` & `types-aws-xray-sdk-2.9.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.970226 types-aws-xray-sdk-2.8.5/
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-04-16 15:19:07.000000 types-aws-xray-sdk-2.8.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-16 15:19:07.000000 types-aws-xray-sdk-2.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-04-16 15:19:07.970226 types-aws-xray-sdk-2.8.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.954226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-16 15:19:07.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.954226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/async_context.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/async_recorder.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/context.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/daemon_config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.954226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/emitters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/emitters/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/emitters/udp_emitter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.958226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/exceptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/exceptions/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/lambda_launcher.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.958226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/default_dynamic_naming.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/dummy_entities.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/entity.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/facade_segment.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/http.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/noop_traceid.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/segment.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/subsegment.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/throwable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/trace_header.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/traceid.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/patcher.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.962226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/plugins/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/plugins/ec2_plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/plugins/ecs_plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/plugins/elasticbeanstalk_plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/plugins/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5357 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/recorder.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.962226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/connector.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.966226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/local/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/local/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/local/reservoir.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/local/sampler.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/local/sampling_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/reservoir.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/rule_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/rule_poller.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/sampler.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/sampling_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/target_poller.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.966226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/streaming/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/streaming/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/streaming/default_streaming.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.966226 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/utils/atomic_counter.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/utils/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/utils/conversion.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/utils/search_pattern.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/utils/stacktrace.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/sdk_config.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-16 15:18:33.000000 types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-16 15:19:07.970226 types-aws-xray-sdk-2.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-04-16 15:19:07.000000 types-aws-xray-sdk-2.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:19:07.970226 types-aws-xray-sdk-2.8.5/types_aws_xray_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-04-16 15:19:07.000000 types-aws-xray-sdk-2.8.5/types_aws_xray_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-04-16 15:19:07.000000 types-aws-xray-sdk-2.8.5/types_aws_xray_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-16 15:19:07.000000 types-aws-xray-sdk-2.8.5/types_aws_xray_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-16 15:19:07.000000 types-aws-xray-sdk-2.8.5/types_aws_xray_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.492822 types-aws-xray-sdk-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-06-26 15:18:02.000000 types-aws-xray-sdk-2.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-26 15:18:02.000000 types-aws-xray-sdk-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-26 15:18:03.492822 types-aws-xray-sdk-2.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.484822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-26 15:18:02.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.484822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/async_context.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/async_recorder.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/daemon_config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.484822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/emitters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/emitters/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/emitters/udp_emitter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.484822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/exceptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/exceptions/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/lambda_launcher.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.488822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/default_dynamic_naming.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/dummy_entities.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/entity.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/facade_segment.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/noop_traceid.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/segment.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/subsegment.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/throwable.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/trace_header.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/traceid.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/patcher.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.488822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/plugins/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/plugins/ec2_plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/plugins/ecs_plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/plugins/elasticbeanstalk_plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/plugins/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5323 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/recorder.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.488822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/connector.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.488822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/local/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/local/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/local/reservoir.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/local/sampler.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/local/sampling_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/reservoir.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/rule_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/rule_poller.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/sampler.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/sampling_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/target_poller.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.488822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/streaming/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/streaming/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/streaming/default_streaming.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.488822 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/utils/atomic_counter.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/utils/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/utils/conversion.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/utils/search_pattern.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/utils/stacktrace.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/sdk_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-26 15:17:49.000000 types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-26 15:18:03.492822 types-aws-xray-sdk-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-06-26 15:18:02.000000 types-aws-xray-sdk-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 15:18:03.488822 types-aws-xray-sdk-2.9.0/types_aws_xray_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-26 15:18:03.000000 types-aws-xray-sdk-2.9.0/types_aws_xray_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-06-26 15:18:03.000000 types-aws-xray-sdk-2.9.0/types_aws_xray_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-26 15:18:03.000000 types-aws-xray-sdk-2.9.0/types_aws_xray_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-26 15:18:03.000000 types-aws-xray-sdk-2.9.0/types_aws_xray_sdk.egg-info/top_level.txt
```

### Comparing `types-aws-xray-sdk-2.8.5/PKG-INFO` & `types-aws-xray-sdk-2.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: types-aws-xray-sdk
-Version: 2.8.5
+Version: 2.9.0
 Summary: Typing stubs for aws-xray-sdk
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aws-xray-sdk.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for aws-xray-sdk
 
 This is a PEP 561 type stub package for the `aws-xray-sdk` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `aws-xray-sdk`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/aws-xray-sdk. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `7a3eb5a4818664d7619ea6ec664c280d0a64c7ee`.
+This package was generated from typeshed commit `d23d213d7eaf51692348fcd0773b95b00dcd0dd8`.
```

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/async_recorder.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/async_recorder.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/context.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/context.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/emitters/udp_emitter.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/emitters/udp_emitter.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/lambda_launcher.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/lambda_launcher.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/dummy_entities.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/dummy_entities.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/entity.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/entity.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/facade_segment.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/facade_segment.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/segment.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/segment.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/subsegment.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/subsegment.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/models/trace_header.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/models/trace_header.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/recorder.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/recorder.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 )
 from .lambda_launcher import check_in_lambda as check_in_lambda
 from .models.default_dynamic_naming import DefaultDynamicNaming as DefaultDynamicNaming
 from .models.dummy_entities import DummySegment as DummySegment, DummySubsegment as DummySubsegment
 from .models.segment import Segment as Segment, SegmentContextManager as SegmentContextManager
 from .models.subsegment import Subsegment as Subsegment, SubsegmentContextManager as SubsegmentContextManager
 from .plugins.utils import get_plugin_modules as get_plugin_modules
-from .sampling.local.sampler import LocalSampler as LocalSampler
-from .sampling.sampler import DefaultSampler as DefaultSampler
+from .sampling.local.sampler import LocalSampler
+from .sampling.sampler import DefaultSampler
 from .streaming.default_streaming import DefaultStreaming as DefaultStreaming
 from .utils import stacktrace as stacktrace
 from .utils.compat import string_types as string_types
 
 log: Logger
 TRACING_NAME_KEY: str
 DAEMON_ADDR_KEY: str
```

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/connector.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/connector.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/local/sampling_rule.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/local/sampling_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/sampler.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/sampler.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/aws_xray_sdk-stubs/core/sampling/sampling_rule.pyi` & `types-aws-xray-sdk-2.9.0/aws_xray_sdk-stubs/core/sampling/sampling_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-aws-xray-sdk-2.8.5/setup.py` & `types-aws-xray-sdk-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `aws-xray-sdk` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `aws-xray-sdk`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/aws-xray-sdk. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `7a3eb5a4818664d7619ea6ec664c280d0a64c7ee`.
+This package was generated from typeshed commit `d23d213d7eaf51692348fcd0773b95b00dcd0dd8`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.8.5",
+      version="2.9.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aws-xray-sdk.md",
@@ -29,10 +29,11 @@
       },
       install_requires=[],
       packages=['aws_xray_sdk-stubs'],
       package_data={'aws_xray_sdk-stubs': ['__init__.pyi', 'core/__init__.pyi', 'core/async_context.pyi', 'core/async_recorder.pyi', 'core/context.pyi', 'core/daemon_config.pyi', 'core/emitters/__init__.pyi', 'core/emitters/udp_emitter.pyi', 'core/exceptions/__init__.pyi', 'core/exceptions/exceptions.pyi', 'core/lambda_launcher.pyi', 'core/models/__init__.pyi', 'core/models/default_dynamic_naming.pyi', 'core/models/dummy_entities.pyi', 'core/models/entity.pyi', 'core/models/facade_segment.pyi', 'core/models/http.pyi', 'core/models/noop_traceid.pyi', 'core/models/segment.pyi', 'core/models/subsegment.pyi', 'core/models/throwable.pyi', 'core/models/trace_header.pyi', 'core/models/traceid.pyi', 'core/patcher.pyi', 'core/plugins/__init__.pyi', 'core/plugins/ec2_plugin.pyi', 'core/plugins/ecs_plugin.pyi', 'core/plugins/elasticbeanstalk_plugin.pyi', 'core/plugins/utils.pyi', 'core/recorder.pyi', 'core/sampling/__init__.pyi', 'core/sampling/connector.pyi', 'core/sampling/local/__init__.pyi', 'core/sampling/local/reservoir.pyi', 'core/sampling/local/sampler.pyi', 'core/sampling/local/sampling_rule.pyi', 'core/sampling/reservoir.pyi', 'core/sampling/rule_cache.pyi', 'core/sampling/rule_poller.pyi', 'core/sampling/sampler.pyi', 'core/sampling/sampling_rule.pyi', 'core/sampling/target_poller.pyi', 'core/streaming/__init__.pyi', 'core/streaming/default_streaming.pyi', 'core/utils/__init__.pyi', 'core/utils/atomic_counter.pyi', 'core/utils/compat.pyi', 'core/utils/conversion.pyi', 'core/utils/search_pattern.pyi', 'core/utils/stacktrace.pyi', 'sdk_config.pyi', 'version.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
+          "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-aws-xray-sdk-2.8.5/types_aws_xray_sdk.egg-info/PKG-INFO` & `types-aws-xray-sdk-2.9.0/types_aws_xray_sdk.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: types-aws-xray-sdk
-Version: 2.8.5
+Version: 2.9.0
 Summary: Typing stubs for aws-xray-sdk
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aws-xray-sdk.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for aws-xray-sdk
 
 This is a PEP 561 type stub package for the `aws-xray-sdk` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `aws-xray-sdk`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/aws-xray-sdk. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `7a3eb5a4818664d7619ea6ec664c280d0a64c7ee`.
+This package was generated from typeshed commit `d23d213d7eaf51692348fcd0773b95b00dcd0dd8`.
```

### Comparing `types-aws-xray-sdk-2.8.5/types_aws_xray_sdk.egg-info/SOURCES.txt` & `types-aws-xray-sdk-2.9.0/types_aws_xray_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

