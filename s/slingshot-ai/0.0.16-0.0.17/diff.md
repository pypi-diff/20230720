# Comparing `tmp/slingshot_ai-0.0.16.tar.gz` & `tmp/slingshot_ai-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slingshot_ai-0.0.16.tar", max compression
+gzip compressed data, was "slingshot_ai-0.0.17.tar", max compression
```

## Comparing `slingshot_ai-0.0.16.tar` & `slingshot_ai-0.0.17.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      831 2023-07-12 16:16:00.198753 slingshot_ai-0.0.16/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.16/src/slingshot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.16/src/slingshot/cli/__init__.py
--rw-r--r--   0        0        0    17378 2023-07-12 16:07:14.032130 slingshot_ai-0.0.16/src/slingshot/cli/add.py
--rw-r--r--   0        0        0     2125 2023-07-12 13:35:06.558558 slingshot_ai-0.0.16/src/slingshot/cli/apply.py
--rw-r--r--   0        0        0     6431 2023-07-12 16:07:14.032400 slingshot_ai-0.0.16/src/slingshot/cli/apps.py
--rw-r--r--   0        0        0     5916 2023-06-20 21:48:49.557285 slingshot_ai-0.0.16/src/slingshot/cli/artifact.py
--rw-r--r--   0        0        0     5263 2023-06-27 15:26:50.737721 slingshot_ai-0.0.16/src/slingshot/cli/auth.py
--rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.16/src/slingshot/cli/code.py
--rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.16/src/slingshot/cli/config/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.16/src/slingshot/cli/config/py.typed
--rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.16/src/slingshot/cli/config/sentry_setup.py
--rw-r--r--   0        0        0    13774 2023-06-27 15:26:50.739279 slingshot_ai-0.0.16/src/slingshot/cli/config/slingshot_cli.py
--rw-r--r--   0        0        0     1234 2023-06-08 13:51:24.735333 slingshot_ai-0.0.16/src/slingshot/cli/dev.py
--rw-r--r--   0        0        0     1123 2023-07-03 01:17:17.281267 slingshot_ai-0.0.16/src/slingshot/cli/environment.py
--rw-r--r--   0        0        0     5323 2023-07-05 13:59:49.265273 slingshot_ai-0.0.16/src/slingshot/cli/inference.py
--rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.16/src/slingshot/cli/logs.py
--rw-r--r--   0        0        0     1951 2023-07-03 17:32:15.325020 slingshot_ai-0.0.16/src/slingshot/cli/machine.py
--rw-r--r--   0        0        0     2759 2023-07-04 04:36:55.756325 slingshot_ai-0.0.16/src/slingshot/cli/main.py
--rw-r--r--   0        0        0     3011 2023-07-12 16:07:14.032658 slingshot_ai-0.0.16/src/slingshot/cli/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.16/src/slingshot/cli/py.typed
--rw-r--r--   0        0        0     8920 2023-07-07 20:43:45.117337 slingshot_ai-0.0.16/src/slingshot/cli/run.py
--rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.16/src/slingshot/cli/secret.py
--rw-r--r--   0        0        0     3845 2023-07-04 04:36:55.756967 slingshot_ai-0.0.16/src/slingshot/cli/session.py
--rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.16/src/slingshot/cli/shared/__init__.py
--rw-r--r--   0        0        0     6260 2023-06-20 21:48:49.557743 slingshot_ai-0.0.16/src/slingshot/cli/shared/code_sync.py
--rw-r--r--   0        0        0     7036 2023-07-12 16:07:14.033096 slingshot_ai-0.0.16/src/slingshot/cli/shared/prompt.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.16/src/slingshot/cli/shared/py.typed
--rw-r--r--   0        0        0      191 2023-06-08 13:51:24.738326 slingshot_ai-0.0.16/src/slingshot/cli/shared/settings.py
--rw-r--r--   0        0        0     6504 2023-07-12 16:07:14.033408 slingshot_ai-0.0.16/src/slingshot/cli/shared/utils.py
--rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.16/src/slingshot/cli/volume.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.16/src/slingshot/code/__init__.py
--rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.16/src/slingshot/code/annotation.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.16/src/slingshot/code/py.typed
--rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.16/src/slingshot/inference_model/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.16/src/slingshot/inference_model/inference_model.py
--rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.16/src/slingshot/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.16/src/slingshot/schemas/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.16/src/slingshot/schemas/generated/py.typed
--rw-r--r--   0        0        0    26727 2023-07-12 16:07:23.000000 slingshot_ai-0.0.16/src/slingshot/schemas/generated/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.16/src/slingshot/schemas/py.typed
--rw-r--r--   0        0        0    10181 2023-06-27 15:26:50.747432 slingshot_ai-0.0.16/src/slingshot/schemas/schema_extensions.py
--rw-r--r--   0        0        0    15216 2023-07-12 16:07:14.034110 slingshot_ai-0.0.16/src/slingshot/schemas/slingshot-schema.config.json
--rw-r--r--   0        0        0    19713 2023-07-12 16:07:14.034438 slingshot_ai-0.0.16/src/slingshot/schemas/slingshot_schema.py
--rw-r--r--   0        0        0      125 2023-07-06 14:31:59.119085 slingshot_ai-0.0.16/src/slingshot/sdk/__init__.py
--rw-r--r--   0        0        0    45791 2023-07-12 16:07:14.034882 slingshot_ai-0.0.16/src/slingshot/sdk/apply.py
--rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.16/src/slingshot/sdk/auth.py
--rw-r--r--   0        0        0     2073 2023-06-27 15:26:50.749266 slingshot_ai-0.0.16/src/slingshot/sdk/config.py
--rw-r--r--   0        0        0     1856 2023-06-14 17:13:24.234357 slingshot_ai-0.0.16/src/slingshot/sdk/config_utils.py
--rw-r--r--   0        0        0     2372 2023-07-06 15:25:20.145323 slingshot_ai-0.0.16/src/slingshot/sdk/data_collector.py
--rw-r--r--   0        0        0     5334 2023-06-08 13:51:24.743481 slingshot_ai-0.0.16/src/slingshot/sdk/errors.py
--rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-08 13:51:24.743943 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/base_graphql.py
--rw-r--r--   0        0        0    18365 2023-07-12 16:07:14.035297 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/fragments.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/py.typed
--rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/__init__.py
--rw-r--r--   0        0        0     5265 2023-07-06 15:15:48.339951 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/apps.py
--rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/deployment.py
--rw-r--r--   0        0        0     3671 2023-06-08 13:51:24.745123 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/environment.py
--rw-r--r--   0        0        0     5247 2023-06-27 15:26:50.751307 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/py.typed
--rw-r--r--   0        0        0     2416 2023-07-07 20:43:45.118845 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/run.py
--rw-r--r--   0        0        0     3578 2023-06-08 13:51:24.745899 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/storage.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.16/src/slingshot/sdk/py.typed
--rw-r--r--   0        0        0    48311 2023-07-12 16:07:14.035714 slingshot_ai-0.0.16/src/slingshot/sdk/slingshot_api.py
--rw-r--r--   0        0        0    51951 2023-07-12 16:07:14.036162 slingshot_ai-0.0.16/src/slingshot/sdk/slingshot_sdk.py
--rw-r--r--   0        0        0     5420 2023-06-08 13:51:24.747044 slingshot_ai-0.0.16/src/slingshot/sdk/sync.py
--rw-r--r--   0        0        0     2862 2023-06-08 13:51:24.747244 slingshot_ai-0.0.16/src/slingshot/sdk/upload_download_utils.py
--rw-r--r--   0        0        0     2876 2023-06-14 14:56:40.739250 slingshot_ai-0.0.16/src/slingshot/sdk/utils.py
--rw-r--r--   0        0        0     4361 2023-07-05 13:59:49.269504 slingshot_ai-0.0.16/src/slingshot/sdk/web_path_util.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.16/src/slingshot/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.16/src/slingshot/shared/py.typed
--rw-r--r--   0        0        0     6753 2023-07-12 16:07:14.036481 slingshot_ai-0.0.16/src/slingshot/shared/utils.py
--rw-r--r--   0        0        0       23 2023-07-12 17:47:47.333786 slingshot_ai-0.0.16/src/slingshot/slingshot_version.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.16/src/slingshot/templates/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-28 22:37:34.391674 slingshot_ai-0.0.16/src/slingshot/templates/inference_template.py
--rw-r--r--   0        0        0     1090 2023-06-08 13:51:24.748859 slingshot_ai-0.0.16/src/slingshot/templates/label_studio_data_export_template.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.16/src/slingshot/templates/py.typed
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 slingshot_ai-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0      831 2023-07-20 17:43:37.505854 slingshot_ai-0.0.17/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.17/src/slingshot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.17/src/slingshot/cli/__init__.py
+-rw-r--r--   0        0        0    17378 2023-07-19 17:55:36.034054 slingshot_ai-0.0.17/src/slingshot/cli/add.py
+-rw-r--r--   0        0        0     1982 2023-07-13 15:57:24.531070 slingshot_ai-0.0.17/src/slingshot/cli/apply.py
+-rw-r--r--   0        0        0     6431 2023-07-12 21:00:50.132623 slingshot_ai-0.0.17/src/slingshot/cli/apps.py
+-rw-r--r--   0        0        0     5916 2023-06-20 21:48:49.557285 slingshot_ai-0.0.17/src/slingshot/cli/artifact.py
+-rw-r--r--   0        0        0     5263 2023-06-27 15:26:50.737721 slingshot_ai-0.0.17/src/slingshot/cli/auth.py
+-rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.17/src/slingshot/cli/code.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.17/src/slingshot/cli/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.17/src/slingshot/cli/config/py.typed
+-rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.17/src/slingshot/cli/config/sentry_setup.py
+-rw-r--r--   0        0        0    13774 2023-06-27 15:26:50.739279 slingshot_ai-0.0.17/src/slingshot/cli/config/slingshot_cli.py
+-rw-r--r--   0        0        0     1234 2023-06-08 13:51:24.735333 slingshot_ai-0.0.17/src/slingshot/cli/dev.py
+-rw-r--r--   0        0        0     1123 2023-07-03 01:17:17.281267 slingshot_ai-0.0.17/src/slingshot/cli/environment.py
+-rw-r--r--   0        0        0     5323 2023-07-05 13:59:49.265273 slingshot_ai-0.0.17/src/slingshot/cli/inference.py
+-rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.17/src/slingshot/cli/logs.py
+-rw-r--r--   0        0        0     1951 2023-07-03 17:32:15.325020 slingshot_ai-0.0.17/src/slingshot/cli/machine.py
+-rw-r--r--   0        0        0     2759 2023-07-04 04:36:55.756325 slingshot_ai-0.0.17/src/slingshot/cli/main.py
+-rw-r--r--   0        0        0     3011 2023-07-12 21:00:50.133568 slingshot_ai-0.0.17/src/slingshot/cli/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.17/src/slingshot/cli/py.typed
+-rw-r--r--   0        0        0     8920 2023-07-07 20:43:45.117337 slingshot_ai-0.0.17/src/slingshot/cli/run.py
+-rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.17/src/slingshot/cli/secret.py
+-rw-r--r--   0        0        0     3845 2023-07-04 04:36:55.756967 slingshot_ai-0.0.17/src/slingshot/cli/session.py
+-rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.17/src/slingshot/cli/shared/__init__.py
+-rw-r--r--   0        0        0     6260 2023-06-20 21:48:49.557743 slingshot_ai-0.0.17/src/slingshot/cli/shared/code_sync.py
+-rw-r--r--   0        0        0     7036 2023-07-12 21:00:50.134070 slingshot_ai-0.0.17/src/slingshot/cli/shared/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.17/src/slingshot/cli/shared/py.typed
+-rw-r--r--   0        0        0      191 2023-06-08 13:51:24.738326 slingshot_ai-0.0.17/src/slingshot/cli/shared/settings.py
+-rw-r--r--   0        0        0     6183 2023-07-18 01:03:50.455195 slingshot_ai-0.0.17/src/slingshot/cli/shared/utils.py
+-rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.17/src/slingshot/cli/volume.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.17/src/slingshot/code/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.17/src/slingshot/code/annotation.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.17/src/slingshot/code/py.typed
+-rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.17/src/slingshot/inference_model/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.17/src/slingshot/inference_model/inference_model.py
+-rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.17/src/slingshot/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.17/src/slingshot/schemas/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.17/src/slingshot/schemas/generated/py.typed
+-rw-r--r--   0        0        0    26686 2023-07-20 17:22:15.000000 slingshot_ai-0.0.17/src/slingshot/schemas/generated/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.17/src/slingshot/schemas/py.typed
+-rw-r--r--   0        0        0    10181 2023-06-27 15:26:50.747432 slingshot_ai-0.0.17/src/slingshot/schemas/schema_extensions.py
+-rw-r--r--   0        0        0    15314 2023-07-19 17:55:36.035248 slingshot_ai-0.0.17/src/slingshot/schemas/slingshot-schema.config.json
+-rw-r--r--   0        0        0    19863 2023-07-19 17:55:36.035584 slingshot_ai-0.0.17/src/slingshot/schemas/slingshot_schema.py
+-rw-r--r--   0        0        0      125 2023-07-06 14:31:59.119085 slingshot_ai-0.0.17/src/slingshot/sdk/__init__.py
+-rw-r--r--   0        0        0    48950 2023-07-19 17:56:27.919660 slingshot_ai-0.0.17/src/slingshot/sdk/apply.py
+-rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.17/src/slingshot/sdk/auth.py
+-rw-r--r--   0        0        0     2073 2023-06-27 15:26:50.749266 slingshot_ai-0.0.17/src/slingshot/sdk/config.py
+-rw-r--r--   0        0        0     2007 2023-07-13 02:14:29.104748 slingshot_ai-0.0.17/src/slingshot/sdk/config_utils.py
+-rw-r--r--   0        0        0     2372 2023-07-06 15:25:20.145323 slingshot_ai-0.0.17/src/slingshot/sdk/data_collector.py
+-rw-r--r--   0        0        0     5394 2023-07-19 17:56:27.920088 slingshot_ai-0.0.17/src/slingshot/sdk/errors.py
+-rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-08 13:51:24.743943 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/base_graphql.py
+-rw-r--r--   0        0        0    18486 2023-07-14 18:10:49.055701 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/fragments.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/py.typed
+-rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/__init__.py
+-rw-r--r--   0        0        0     5265 2023-07-06 15:15:48.339951 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/apps.py
+-rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/deployment.py
+-rw-r--r--   0        0        0     3671 2023-06-08 13:51:24.745123 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/environment.py
+-rw-r--r--   0        0        0     5247 2023-06-27 15:26:50.751307 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/py.typed
+-rw-r--r--   0        0        0     2416 2023-07-07 20:43:45.118845 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/run.py
+-rw-r--r--   0        0        0     3578 2023-06-08 13:51:24.745899 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/storage.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.17/src/slingshot/sdk/py.typed
+-rw-r--r--   0        0        0    48581 2023-07-19 17:56:27.920680 slingshot_ai-0.0.17/src/slingshot/sdk/slingshot_api.py
+-rw-r--r--   0        0        0    52327 2023-07-20 13:33:03.423585 slingshot_ai-0.0.17/src/slingshot/sdk/slingshot_sdk.py
+-rw-r--r--   0        0        0     7010 2023-07-18 16:49:57.082909 slingshot_ai-0.0.17/src/slingshot/sdk/sync.py
+-rw-r--r--   0        0        0     2862 2023-06-08 13:51:24.747244 slingshot_ai-0.0.17/src/slingshot/sdk/upload_download_utils.py
+-rw-r--r--   0        0        0     4149 2023-07-13 15:57:24.533800 slingshot_ai-0.0.17/src/slingshot/sdk/utils.py
+-rw-r--r--   0        0        0     4361 2023-07-05 13:59:49.269504 slingshot_ai-0.0.17/src/slingshot/sdk/web_path_util.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.17/src/slingshot/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.17/src/slingshot/shared/py.typed
+-rw-r--r--   0        0        0     6753 2023-07-12 21:00:50.142218 slingshot_ai-0.0.17/src/slingshot/shared/utils.py
+-rw-r--r--   0        0        0       23 2023-07-20 17:44:29.983945 slingshot_ai-0.0.17/src/slingshot/slingshot_version.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.17/src/slingshot/templates/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-28 22:37:34.391674 slingshot_ai-0.0.17/src/slingshot/templates/inference_template.py
+-rw-r--r--   0        0        0     1090 2023-06-08 13:51:24.748859 slingshot_ai-0.0.17/src/slingshot/templates/label_studio_data_export_template.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.17/src/slingshot/templates/py.typed
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 slingshot_ai-0.0.17/PKG-INFO
```

### Comparing `slingshot_ai-0.0.16/pyproject.toml` & `slingshot_ai-0.0.17/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "slingshot-ai"
-version = "0.0.16"
+version = "0.0.17"
 
 [tool.poetry]
 name = "slingshot-ai"
-version = "0.0.16"
+version = "0.0.17"
 description = ""
 authors = ["Slingshot AI <service-account@slingshot.xyz>"]
 packages = [ { include = "slingshot", from = "src" } ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "~=3.8.1"
@@ -18,15 +18,15 @@
 requests = "~=2.28.1"
 sh = "~=1.14.3"
 pyyaml = "~=6.0"
 "ruamel.yaml" = "~=0.17.0"
 simple-term-menu = "~=1.6.0"
 deepdiff = "~=6.3.0"
 fastapi = "~=0.88.0"
-uvicorn = {extras = ["standard"], version = "~=0.18.0"}
+uvicorn = {extras = ["standard"], version = "~=0.22.0"}
 tqdm = "~=4.63.0"
 sentry-sdk = "~=1.16.0"
 backoff = "~=2.0.0"
 openai = "~=0.27.8"
 
 [tool.poetry.scripts]
 slingshot = "slingshot.cli.main:app"
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/add.py` & `slingshot_ai-0.0.17/src/slingshot/cli/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     alphanumeric_hyphen_underscore = re.sub(r"[^a-z0-9-_]", "", single_hyphen)
     return alphanumeric_hyphen_underscore
 
 
 async def _create_project(sdk: SlingshotSDK) -> str:
     new_id = None
     display_name = typer.prompt("Enter a name for your project")
-    project_id_default = _display_name_to_id(display_name) + "-" + uuid.uuid4().hex[:5]
+    project_id_default = _display_name_to_id(display_name) + "-" + uuid.uuid4().hex[:4]
     while True:
         # Replace multiple spaces with a single space and spaces with hyphens
         new_id = new_id or typer.prompt(
             "Enter a slug for your project (unique ID used for URLs)", default=project_id_default
         )
         try:
             project_response = await sdk.create_project(new_id, display_name=display_name)
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/apply.py` & `slingshot_ai-0.0.17/src/slingshot/cli/apply.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 async def pull(
     *, sdk: SlingshotSDK, y: bool = typer.Option(False, "--yes", "-y", help="Skip confirmation and apply changes")
 ) -> None:
     """Pull the slingshot.yaml file to the current project
 
     Pulls the slingshot.yaml file in the current directory to the project on Slingshot
     """
-    any_changes_applied = await sdk.apply_to_local(force=y)
-    if not any_changes_applied:
-        console.print("No changes pulled")
-    else:
-        console.print("Changes pulled successfully")
+    await sdk.apply_to_local(force=y, print_logs=True)
 
 
 @app.command(name="plan", requires_project=True, top_level=True, requires_auth=True, hidden=True)
 async def plan(*, sdk: SlingshotSDK) -> None:
     """Plan what changes would be applied by the slingshot.yaml file, but don't apply them"""
     manifest = load_slingshot_project_config()
     remote_manifest = await remote_project_manifest(sdk)
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/apps.py` & `slingshot_ai-0.0.17/src/slingshot/cli/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/artifact.py` & `slingshot_ai-0.0.17/src/slingshot/cli/artifact.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/auth.py` & `slingshot_ai-0.0.17/src/slingshot/cli/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/code.py` & `slingshot_ai-0.0.17/src/slingshot/cli/code.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/config/sentry_setup.py` & `slingshot_ai-0.0.17/src/slingshot/cli/config/sentry_setup.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/config/slingshot_cli.py` & `slingshot_ai-0.0.17/src/slingshot/cli/config/slingshot_cli.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/dev.py` & `slingshot_ai-0.0.17/src/slingshot/cli/dev.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/environment.py` & `slingshot_ai-0.0.17/src/slingshot/cli/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/inference.py` & `slingshot_ai-0.0.17/src/slingshot/cli/inference.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/logs.py` & `slingshot_ai-0.0.17/src/slingshot/cli/logs.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/machine.py` & `slingshot_ai-0.0.17/src/slingshot/cli/machine.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/main.py` & `slingshot_ai-0.0.17/src/slingshot/cli/main.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/project.py` & `slingshot_ai-0.0.17/src/slingshot/cli/project.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/run.py` & `slingshot_ai-0.0.17/src/slingshot/cli/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/secret.py` & `slingshot_ai-0.0.17/src/slingshot/cli/secret.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/session.py` & `slingshot_ai-0.0.17/src/slingshot/cli/session.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/shared/code_sync.py` & `slingshot_ai-0.0.17/src/slingshot/cli/shared/code_sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/shared/prompt.py` & `slingshot_ai-0.0.17/src/slingshot/cli/shared/prompt.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/shared/utils.py` & `slingshot_ai-0.0.17/src/slingshot/cli/shared/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,44 +25,39 @@
     return logline.log
 
 
 def merge_loglines(loglines: list[schemas.LogLine]) -> str:
     return "\n".join(format_logline(logline) for logline in loglines)
 
 
-async def follow_run_logs_until_done(sdk: SlingshotSDK, run_id: str) -> schemas.JobStatus:
+async def follow_run_logs_until_done(sdk: SlingshotSDK, run_id: str) -> None:
     task_logs = asyncio.create_task(sdk.print_logs(run_id=run_id, follow=True))
     task_status = asyncio.create_task(_wait_for_run_finished(sdk=sdk, run_id=run_id))
     done, pending = await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
     for task in pending:
         task.cancel()
 
-    # If task_status was cancelled or raised an exception, handle it
-    if task_status.cancelled():
-        raise SlingshotException("Something went wrong following logs")
-    elif (exception := task_status.exception()) is not None:
-        raise exception
-
-    return task_status.result()
+    await asyncio.gather(*pending)
 
 
 async def follow_app_logs_until_ready(sdk: SlingshotSDK, app_spec_id: str) -> schemas.AppInstanceStatus:
     task_logs = asyncio.create_task(sdk.print_logs(app_spec_id=app_spec_id, follow=True))
     task_status = asyncio.create_task(_wait_for_app_ready(sdk=sdk, app_spec_id=app_spec_id))
     done, pending = await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
     for task in pending:
         task.cancel()
 
-    # If task_status was cancelled or raised an exception, handle it
-    if task_status.cancelled():
-        raise SlingshotException("Something went wrong following logs")
-    elif (exception := task_status.exception()) is not None:
-        raise exception
+    status = None
+    try:
+        await asyncio.gather(*pending)
+        status = await task_status
+    except asyncio.CancelledError:
+        pass
 
-    return task_status.result()
+    return status or await follow_app_logs_until_ready(sdk=sdk, app_spec_id=app_spec_id)
 
 
 def datetime_to_human_readable(dt: datetime) -> str:
     """Assumes UTC datetime and converts to local time in the format of: Mar 2, 2021 1:30AM EST"""
     date_str = dt.strftime('%b %d, %Y %I:%M:%S %p')
     return f'{date_str} UTC'
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/cli/volume.py` & `slingshot_ai-0.0.17/src/slingshot/cli/volume.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/inference_model/inference_model.py` & `slingshot_ai-0.0.17/src/slingshot/inference_model/inference_model.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/schemas/generated/schemas.py` & `slingshot_ai-0.0.17/src/slingshot/schemas/generated/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     project_id: constr(
         regex=r'^[A-Za-z][A-Za-z0-9_-]*$', min_length=4, max_length=50
     ) = Field(
         ...,
         description='This is the unique name to be associated with your new project',
         title='Project ID',
     )
-    display_name: constr(min_length=4, max_length=20) = Field(
+    display_name: constr(min_length=4, max_length=50) = Field(
         ...,
         description='An optional name for your project that will be shown in the UI',
         title='Display Name',
     )
 
 
 class BodyPredictByName(BaseModel):
@@ -520,15 +520,14 @@
 
 class BoolResponse(BaseModel):
     data: Optional[bool] = Field(None, title='Data')
     error: Optional[SlingshotLogicalError] = None
 
 
 class CreateAppBody(BaseModel):
-    name: str = Field(..., title='Name')
     command: Optional[str] = Field(None, title='Command')
     exec_env_spec_id: str = Field(..., title='Exec Env Spec Id')
     machine_size: MachineSize
     attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     mounts: List[
         Union[
             DownloadByNameMountSpecRequest,
@@ -538,14 +537,15 @@
         ]
     ] = Field(..., title='Mounts')
     config_variables: Optional[Dict[str, Any]] = Field(None, title='Config Variables')
     app_port: Optional[int] = Field(None, title='App Port')
     batch_size: Optional[PositiveInt] = Field(None, title='Batch Size')
     batch_interval: Optional[PositiveInt] = Field(None, title='Batch Interval')
     soft_concurrency: Optional[PositiveInt] = Field(None, title='Soft Concurrency')
+    name: constr(regex=r'^[A-Za-z][A-Za-z0-9_-]*$') = Field(..., title='Name')
     app_type: AppType
     app_sub_type: Optional[AppSubType] = None
 
 
 class CreateEnvironmentSpecResponse(BaseModel):
     data: Optional[List[Union[ExecutionEnvironmentSpecId, bool]]] = Field(
         None, max_items=2, min_items=2, title='Data'
@@ -575,15 +575,17 @@
 
 class EvaluationTestSetResultIdResponse(BaseModel):
     data: Optional[EvaluationTestSetResultId] = None
     error: Optional[SlingshotLogicalError] = None
 
 
 class ExecutionEnvironmentSpecRequestBody(BaseModel):
-    name: str = Field(..., description='Name of the environment.', title='Name')
+    name: constr(regex=r'^[A-Za-z][A-Za-z0-9_-]*$') = Field(
+        ..., description='Name of the environment.', title='Name'
+    )
     python_packages: List[RequestedRequirement] = Field(
         ...,
         description='List of Python packages to install in the environment.',
         title='Python packages',
     )
     apt_packages: List[RequestedAptPackage] = Field(
         ...,
@@ -717,35 +719,35 @@
             DownloadByNameMountSpecRequest,
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
     exec_env_id: str = Field(..., title='Exec Env Id')
-    cmd: str = Field(..., description='Command to run', title='Cmd')
     attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: Optional[str] = Field(None, title='Source Code Id')
     app_port: Optional[int] = Field(None, title='App Port')
+    cmd: Optional[str] = Field(None, title='Cmd')
 
 
 class StartDeploymentBody(BaseModel):
     machine_size: MachineSize
     config_variables: Optional[Dict[str, Any]] = Field(None, title='Config Variables')
     mounts: List[
         Union[
             DownloadByNameMountSpecRequest,
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
     exec_env_id: str = Field(..., title='Exec Env Id')
-    cmd: str = Field(..., description='Command to run', title='Cmd')
     attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: str = Field(..., title='Source Code Id')
+    cmd: str = Field(..., title='Cmd')
     batch_size: Optional[PositiveInt] = Field(None, title='Batch Size')
     batch_interval: Optional[PositiveInt] = Field(None, title='Batch Interval')
 
 
 class StartRunBody(BaseModel):
     machine_size: MachineSize
     config_variables: Optional[Dict[str, Any]] = Field(None, title='Config Variables')
@@ -754,21 +756,20 @@
             DownloadByNameMountSpecRequest,
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
     exec_env_id: str = Field(..., title='Exec Env Id')
-    cmd: str = Field(..., description='Command to run', title='Cmd')
     attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: str = Field(..., title='Source Code Id')
+    cmd: str = Field(..., title='Cmd')
 
 
 class UpdateAppBody(BaseModel):
-    name: Optional[str] = Field(None, title='Name')
     command: Optional[str] = Field(None, title='Command')
     exec_env_spec_id: str = Field(..., title='Exec Env Spec Id')
     machine_size: MachineSize
     attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     mounts: List[
         Union[
             DownloadByNameMountSpecRequest,
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/schemas/schema_extensions.py` & `slingshot_ai-0.0.17/src/slingshot/schemas/schema_extensions.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/schemas/slingshot-schema.config.json` & `slingshot_ai-0.0.17/src/slingshot/schemas/slingshot-schema.config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999877025462963%*

 * *Differences: {"'definitions'": "{'SlingshotCustomAppSpec': {'properties': {'name': {'pattern': "*

 * *                  "'^[A-Za-z][A-Za-z0-9_-]*$'}}}, 'SessionAppSpec': {'properties': {'name': "*

 * *                  "{'pattern': '^[A-Za-z][A-Za-z0-9_-]*$'}}}}"}*

```diff
@@ -329,14 +329,15 @@
                         ]
                     },
                     "title": "Mounts",
                     "type": "array"
                 },
                 "name": {
                     "description": "The name of the app.",
+                    "pattern": "^[A-Za-z][A-Za-z0-9_-]*$",
                     "title": "Name",
                     "type": "string"
                 },
                 "num_gpu": {
                     "default": 0,
                     "description": "The number of GPUs to use.",
                     "title": "Number of GPUs",
@@ -415,14 +416,15 @@
                         ]
                     },
                     "title": "Mounts",
                     "type": "array"
                 },
                 "name": {
                     "description": "The name of the app.",
+                    "pattern": "^[A-Za-z][A-Za-z0-9_-]*$",
                     "title": "Name",
                     "type": "string"
                 },
                 "num_gpu": {
                     "default": 0,
                     "description": "The number of GPUs to use.",
                     "title": "Number of GPUs",
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/schemas/slingshot_schema.py` & `slingshot_ai-0.0.17/src/slingshot/schemas/slingshot_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 PATH_TO_FILE = "slingshot_client/src/slingshot/schemas"
 FILENAME = "slingshot-schema.config.json"
 FILE_LOCATION = "/".join([REPO, "blob/main", PATH_TO_FILE, FILENAME])
 PATH_FIELD = Field(
     ..., title="Path", description="The path to mount into the environment.", regex=r"/mnt/(?!slingshot).+"
 )
 MODE_FIELD = Field(..., title="Mode", description="The mode to use for the mount.")
+ALPHANUMERIC_UNDERSCORE_HYPHEN_RE = "^[A-Za-z][A-Za-z0-9_-]*$"  # This should match the regex on the backend
 
 
 class BaseMountSpec(BaseModel):
     mode: str = Field(..., title="Mode", description="The mode to use for the mount.")
     path: str = Field(
         ..., title="Path", description="The path to mount into the environment.", regex=r"/mnt/(?!slingshot).+"
     )
@@ -204,15 +205,15 @@
         for req in existing:
             if req not in current:
                 diff.append(f"  [red]-[/red] {req.name}")
         return diff
 
 
 class SlingshotAbstractAppSpec(BaseModel, ABC):
-    name: str = Field(..., title="Name", description="The name of the app.")
+    name: str = Field(..., title="Name", description="The name of the app.", regex=ALPHANUMERIC_UNDERSCORE_HYPHEN_RE)
     environment: str = Field(..., title="Environment", description="The name of the execution environment.")
     machine_type: schemas.MachineType = Field(
         schemas.MachineType.CPU_SMALL, title="Machine size", description="The machine size to be used."
     )
     num_gpu: int = Field(0, title="Number of GPUs", description="The number of GPUs to use.")
     config_variables: dict[str, Any] = Field(
         default_factory=dict, title="Arguments", description="Optional user defined arguments to pass to the app."
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/apply.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/apply.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 
 import json
 import re
 from enum import Enum
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union
 
+import sentry_sdk
 import typer
 from deepdiff import DeepDiff
 from pydantic import parse_obj_as
 
 from slingshot import schemas
-from slingshot.cli.shared import prompt_confirm, prompt_for_single_choice
+from slingshot.cli.shared import create_empty_project_manifest, prompt_confirm, prompt_for_single_choice
 from slingshot.schemas import ProjectManifest
 from slingshot.sdk import config
+from slingshot.sdk.config import client_settings
 from slingshot.sdk.errors import SlingshotException
 from slingshot.sdk.graphql import fragments
-from slingshot.sdk.utils import console, edit_slingshot_yaml
+from slingshot.sdk.utils import console, edit_slingshot_yaml, recursive_enum_to_str
 from slingshot.shared.utils import (
+    SlingshotFileNotFoundException,
     get_data_or_raise,
     load_slingshot_project_config,
     machine_size_to_machine_type_gpu_count,
     machine_type_gpu_count_to_machine_size,
 )
 
 if TYPE_CHECKING:
@@ -337,15 +340,18 @@
             app_port=app_spec.port if hasattr(app_spec, "port") else None,
             batch_size=app_spec.batch_size if hasattr(app_spec, "batch_size") else None,
             batch_interval=app_spec.batch_interval if hasattr(app_spec, "batch_interval") else None,
         )
         console.print("✅ ")
 
     async def delete_app_spec(self, app_spec: fragments.AppSpec) -> None:
-        console.print(f"Deleting app '{app_spec.app_spec_name}'...", end="")
+        console.print(
+            f"Deleting {app_spec.friendly_app_type} '{app_spec.app_spec_name}' from the remote project manifest...",
+            end="",
+        )
         await self._sdk.delete_app(app_spec_id=app_spec.app_spec_id)
         console.print("✅ ")
 
     async def run(
         self,
         project_manifest: schemas.ProjectManifest,
         env_spec_plan: EnvSpecPlan,
@@ -375,65 +381,77 @@
         The last pushed manifest is used as the base of the initial diff. If there is no last-pushed manifest,
         the base is an empty manifest so that all remote changes are computed in the plan and can be applied.
         Then, the local slingshot.yaml applied using the resulting diff. If there are conflicts, the user is
         prompted to override either the local or remote changes.
 
         Returns True if there were changes, False otherwise.
         """
-        current_manifest = load_slingshot_project_config()  # Reload local, in case it was changed
+        try:
+            current_manifest = load_slingshot_project_config()  # Reload local, in case it was changed
+        except SlingshotFileNotFoundException:
+            create_empty_project_manifest(client_settings.slingshot_config_path)
+
+            # Try again.
+            current_manifest = load_slingshot_project_config()  # Reload local, which is now an empty manifest.
+
         last_pushed_manifest = config.project_config.last_pushed_manifest
         is_last_pushed_manifest_empty = last_pushed_manifest is None
 
         diff_base = last_pushed_manifest or ProjectManifest()
         if isinstance(diff_base, ProjectManifest):
             diff_base = diff_base.dict()
 
         if not remote_manifest:
             remote_manifest = await remote_project_manifest(self._sdk)
 
-        diff = DeepDiff(diff_base, remote_manifest.dict(), ignore_order=True)
+        diff = DeepDiff(diff_base, recursive_enum_to_str(remote_manifest.dict()), ignore_order=True)
+        local_diff = DeepDiff(diff_base, recursive_enum_to_str(current_manifest.dict()), ignore_order=True)
         if not diff:
             logger.debug("No remote changes detected")
             return False
 
-        console.print("[red]Conflict detected[/red]. Changes found on the remote since your last push:")
-        diff_formatted = diff_to_str(diff, remote_manifest)
-        diff_formatted = "\n".join([f"  [yellow]*[/yellow] {line}" for line in diff_formatted.split('\n')])
-        console.print(diff_formatted)
         if not validate_if_changes_can_be_applied(diff, current_manifest=current_manifest):
+            console.print("[red]Conflict detected[/red]. Changes found on the remote since your last push:")
+            console.print(diff_to_str(diff, remote_manifest))
+            console.print("Changes found on the local copy since your last push:")
+            console.print(diff_to_str(local_diff, current_manifest))
             return await prompt_override_local_remote(diff=diff, remote_manifest=remote_manifest, force=force)
 
-        console.print("[yellow]Conflict resolution[/yellow]: ", end="")
-        if not (
-            force
-            or prompt_confirm("Do you want to apply the above changes to your local slingshot.yaml?", default=True)
-        ):
-            return False
+        console.print("Changes found on the remote since your last push:")
+        console.print(diff_to_str(diff, remote_manifest))
 
         try:
-            apply_to_local(diff, remote_manifest)
+            apply_diff_to_manifest(diff, remote_manifest)
             # If the last pushed manifest was empty, we should set it to the remote manifest to avoid showing conflicts
             if is_last_pushed_manifest_empty:
                 config.project_config.last_pushed_manifest = remote_manifest
             else:
                 config.project_config.last_pushed_manifest = load_slingshot_project_config()
             return True
         except Exception as e:
             # If the validation succeeded but apply fails nonetheless, we should still prompt the user
+            sentry_sdk.capture_exception(e)
+            console.print("[red]An error occurred...[/red] Changes found on the remote since your last push:")
+            console.print(diff_to_str(diff, remote_manifest))
+            console.print("Changes found on the local copy since your last push:")
+            console.print(diff_to_str(local_diff, current_manifest))
             return await prompt_override_local_remote(diff=diff, remote_manifest=remote_manifest, force=force)
 
     async def plan_prompt_apply(
         self, *, force: bool, and_wait: bool = False
     ) -> tuple[bool, list[fragments.ExecutionEnvironmentSpec]]:
         """
         Plan, prompt and apply changes to the remote environment.
 
         If force is true, the changes will be applied without prompting. If it's a string, then only the matching
         environment spec (by ID) will be awaited.
 
+        Detects if there are conflicts with the remote. If there are, then we stop applying and instead begin the pull
+        flow.
+
         Returns (True, x) if any changes were applied, False otherwise. X is the list of any environment specs created
         or updated.
         """
         # We use a "last-pushed-manifest" as a merge base to determine what changes to apply.
         #  There are three cases to keep in mind:
         #  - No last-pushed-manifest and no remote manifest: it's a new project -- can safely apply the diff and push
         #  - No last-pushed-manifest and remote manifest: it's a new copy of a project -- user should pull first
@@ -445,24 +463,21 @@
             last_pushed_manifest = ProjectManifest()
         if isinstance(last_pushed_manifest, ProjectManifest):
             last_pushed_manifest = last_pushed_manifest.dict()
 
         remote_manifest = await remote_project_manifest(self._sdk)
         remote_diff = DeepDiff(last_pushed_manifest, remote_manifest.dict(), ignore_order=True)
         if is_last_pushed_manifest_empty and len(remote_diff.keys()) > 0 and not force:
-            raise SlingshotException(
-                "You have unmerged remote changes. Run 'slingshot pull' and then try apply again. To ignore this "
-                "error and force-apply, run 'slingshot apply -y'."
-            )
+            any_changes_applied = await self._sdk.apply_to_local(force=False, print_logs=True)
+            return any_changes_applied, []
 
         current_manifest = load_slingshot_project_config()
         if not (force or validate_if_changes_can_be_applied(remote_diff, current_manifest=current_manifest)):
-            raise SlingshotException(
-                "Cannot apply changes because local and remote changes conflict. Run 'slingshot pull' then try again."
-            )
+            any_changes_applied = await self._sdk.apply_to_local(force=False, print_logs=True)
+            return any_changes_applied, []
 
         any_changes_applied = False
         if not force:
             any_changes_applied = await self.apply_to_local(remote_manifest)
 
         manifest = load_slingshot_project_config()  # Reload local, in case it was changed
         env_spec_plan, app_spec_plan = await self.plan(config=manifest)
@@ -477,25 +492,45 @@
             logger.debug("No changes detected ✅ ")
             return any_changes_applied, []
 
 
 async def prompt_override_local_remote(
     diff: DeepDiff, remote_manifest: schemas.ProjectManifest, *, force: bool
 ) -> bool:
+    """
+    Returns True if changes were applied, and False otherwise.
+    """
     unable_to_synchronise_message = (
         f"[yellow]Conflict resolution[/yellow]: Unable to synchronise remote changes to your local slingshot.yaml."
     )
     console.print(unable_to_synchronise_message)
-    if not force and (
-        prompt_for_single_choice("Do you want to use the local or remote version?", ["local", "remote"], default=0) == 0
-    ):
-        config.project_config.last_pushed_manifest = load_slingshot_project_config()
-        return False
+    if not force:
+        prompt_result = prompt_for_single_choice(
+            "Do you want to use the local or remote version?", ["local", "remote", "resolve manually"], default=0
+        )
+        if prompt_result == 0:
+            config.project_config.last_pushed_manifest = load_slingshot_project_config()
+            console.print(
+                "[bold]Ignored[/bold] the remote changes. To override the remote manifest with your local "
+                "'slingshot.yaml', run 'slingshot apply -f'."
+            )
+            return False
+        elif prompt_result == 2:
+            with edit_slingshot_yaml(raise_if_absent=False, filename=".slingshot.remote.yaml") as slingshot_yaml:
+                slingshot_yaml.clear()
+                slingshot_yaml.update(remote_manifest.dict())
+
+            console.print(
+                "[bold]Manual resolution:[/bold] A copy of the remote slingshot manifest has been saved to "
+                "'.slingshot.remote.yaml'. Please resolve the conflicts manually in 'slingshot.yaml' and then "
+                "force-apply your local resolution with 'slingshot apply -f'."
+            )
+            return False
 
-    apply_to_local(diff, remote_manifest, force=True)
+    apply_diff_to_manifest(diff, remote_manifest, force=True)
     config.project_config.last_pushed_manifest = load_slingshot_project_config()
     return True
 
 
 def apply_diff(local_slingshot_yaml: dict[str, Any], diff: DeepDiff, remote_manifest: schemas.ProjectManifest) -> None:
     """Applies a diff to the local slingshot.yaml, using the remote manifest as a reference."""
     for key_path, value in diff.get("values_changed", {}).items():
@@ -529,19 +564,30 @@
         for k in keys[:-1]:
             d = d[k]  # type: ignore[index]
         # insert
         assert isinstance(d, list)
         if isinstance(value, dict):
             value = {k: v if not isinstance(v, Enum) else v.value for k, v in value.items()}
         d.insert(keys[-1], value)
-    for key_path, value in diff.get("iterable_item_removed", {}).items():
-        keys = parse_keys(key_path)
+
+    # If the user deletes two values from a list, then we must delete them in reverse order, both to eliminate an
+    #  out-of-bounds error, and also to delete the correct value.
+    # For purposes of sorting, first parse the keys of each item in the list, then sort by the last key, before
+    #  iterating and deleting the matching items.
+    diff_iterable_item_removed_with_sorted_parsed_keys = sorted(
+        [(parse_keys(key), value) for key, value in diff.get("iterable_item_removed", {}).items()],
+        # Mypy doesn't know that the last key is always an int, so we ignore the type error on unary - over str | int.
+        key=lambda x: -x[0][-1],  # type: ignore
+    )
+    for keys, value in diff_iterable_item_removed_with_sorted_parsed_keys:
         d = local_slingshot_yaml
+        # Walk to the last/inner node, which is the inner list, i.e. python_packages.
         for k in keys[:-1]:
             d = d[k]  # type: ignore[index]
+
         del d[keys[-1]]  # type: ignore[arg-type]
 
 
 def parse_keys(key_path: str) -> list[Union[str, int]]:
     """
     >>> parse_keys("root['key1']['key2']")
     ['key1', 'key2']
@@ -587,45 +633,53 @@
         else:
             key_path = f"deployment {rest_fields_str}".rstrip()
     return key_path
 
 
 def diff_to_str(diff: DeepDiff, reference: schemas.ProjectManifest) -> str:
     """Converts a diff to a human-readable string."""
-    lines = []
+    changes = []
+    additions = []
+    removals = []
+    other = []
     for key_path, value in diff.get("values_changed", {}).items():
         key_path = _key_path_to_str(key_path, reference)
-        lines.append(f"{key_path} changed from '{value['old_value']}' to '{value['new_value']}'")
+        changes.append(f"{key_path} changed from '{value['old_value']}' to '{value['new_value']}'")
     for key_path in diff.get("dictionary_item_added", []):
         key_path = _key_path_to_str(key_path, reference)
-        lines.append(f"{key_path} added")
+        additions.append(key_path)
     for key_path in diff.get("dictionary_item_removed", []):
         key_path = _key_path_to_str(key_path, reference)
-        lines.append(f"{key_path} removed")
+        removals.append(key_path)
     for key_path, value in diff.get("iterable_item_added", {}).items():
         key_path = _key_path_to_str(key_path, reference)
-        if isinstance(value, dict) and 'name' in value:
-            value = value['name']
-        lines.append(f"{key_path} added: \"{value}\"")
+        additions.append(key_path)
     for key_path, value in diff.get("iterable_item_removed", {}).items():
         key_path = _key_path_to_str(key_path, reference)
         if isinstance(value, dict) and 'name' in value:
             value = value['name']
 
-        lines.append(f"{key_path} removed (was \"{value}\")")
+        removals.append(f"{key_path} '{value}'")
     if set(diff.keys()) - {
         "values_changed",
         "dictionary_item_added",
         "dictionary_item_removed",
         "iterable_item_added",
         "iterable_item_removed",
     }:
-        lines.append("Other changes detected, please see the diff below:")
-        lines.append(str(diff))
-    return "\n".join(lines)
+        other.append(str(diff))
+
+    other_prefix = (
+        "\n    [yellow]Other changes detected:[/yellow]\n" if other and not (changes or additions or removals) else ""
+    )
+    change_lines = "\n".join([f" [blue](~)[/blue] {change}" for change in changes]) + "\n" if changes else ""
+    addition_lines = "\n".join([f" [green](+)[/green] {add}" for add in additions]) + "\n" if additions else ""
+    removal_lines = "\n".join([f" [red](-)[/red] {removal}" for removal in removals]) + "\n" if removals else ""
+    other_lines = "\n".join([f" [yellow](!)[/yellow] {item}" for item in other]) + "\n" if other else ""
+    return f"{change_lines}{addition_lines}{removal_lines}{other_prefix}{other_lines}"
 
 
 def validate_if_changes_can_be_applied(diff: DeepDiff, current_manifest: schemas.ProjectManifest) -> bool:
     """
     Validates if the changes to reference manifest can be applied to current manifest.
     This is useful to fail early if we can't merge in the changes from the diff.
     """
@@ -725,22 +779,23 @@
             return False
         if not current_root[key] == value:
             logger.debug(f"Cannot remove an iterable item that doesn't match the value to be removed: {value}")
             return False
     return True
 
 
-def apply_to_local(diff: DeepDiff, reference_manifest: schemas.ProjectManifest, force: bool = False) -> None:
+def apply_diff_to_manifest(diff: DeepDiff, reference_manifest: schemas.ProjectManifest, force: bool = False) -> None:
     """
     Apply a diff to the local slingshot.yaml file.
-    If force, just use the reference manifest - completely ignore the local slingshot.yaml file.
+    If `force`, just use the reference manifest - completely ignore the local slingshot.yaml file.
     """
     if force:
         diff = DeepDiff(load_slingshot_project_config().dict(), reference_manifest.dict(), ignore_order=True)
-    with edit_slingshot_yaml(raise_if_absent=True) as slingshot_yaml:
+
+    with edit_slingshot_yaml(raise_if_absent=False) as slingshot_yaml:
         apply_diff(slingshot_yaml, diff, reference_manifest)
 
 
 def _get_app_type(spec: schemas.SlingshotAbstractAppSpec) -> schemas.AppType:
     if isinstance(spec, schemas.RunSpec):
         return schemas.AppType.RUN
     elif isinstance(spec, schemas.DeploymentSpec):
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/auth.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/config.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/config.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/config_utils.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/config_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,19 @@
     try:
         return json.loads(settings_json_file.read_text())
     except json.JSONDecodeError as e:
         return {}
 
 
 class BaseJSONSettings(BaseSettings):
+    """
+    Base class for settings that are saved to a JSON file.
+    Whenever an attribute is set, the settings are saved to the JSON file.
+    """
+
     class Config:
         @classmethod
         def customise_sources(cls, init_settings: Any, env_settings: Any, file_secret_settings: Any) -> tuple[Any, ...]:
             return init_settings, _json_config_settings_source, env_settings, file_secret_settings
 
         extra: Extra = Extra.allow
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/data_collector.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/errors.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,18 @@
         console.print(
             f'[bold][red]Could not connect to {self._url}[/bold][/red]\n'
             'If the host is not correct, you can reconfigure the backend url by running '
             '"slingshot be [backend]".'
         )
 
 
+class SlingshotBackoffError(SlingshotException):
+    pass
+
+
 class SlingshotCodeNotFound(SlingshotException):
     def __init__(self) -> None:
         super().__init__(f"No source code found.")
 
     def rich_show(self, console: Console, verbose: bool = False) -> None:
         console.print("[red]Error:[/red] No source code found for your project. Please run 'slingshot push'.")
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/base_graphql.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/base_graphql.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/fragments.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,14 +461,18 @@
 
     @property
     def deployment_status(self) -> schemas.AppInstanceStatus | None:
         if self.deployments:
             return self.deployments[0].deployment_status
         return None
 
+    @property
+    def friendly_app_type(self) -> str:
+        return (self.app_sub_type or self.app_type).value.lower()
+
 
 class AppInstance(BaseGraphQLEntity):
     _depends_on = [AppSpec]
     _fragment = """
         fragment AppInstance on AppInstances {
             appInstanceId
             appInstanceStatus
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/apps.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/deployment.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/deployment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/environment.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/project.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/project.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/run.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/storage.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/storage.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/slingshot_api.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/slingshot_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from pydantic import BaseModel, ValidationError, parse_obj_as
 
 from .. import schemas
 from ..schemas import AuthTokenUnion, Hyperparameter, MachineSize
 from ..shared.utils import get_data_or_raise
 from . import config
 from .errors import (
+    SlingshotBackoffError,
     SlingshotClientHttpException,
     SlingshotConnectionError,
     SlingshotException,
     SlingshotJWSInvalidSignature,
     SlingshotJWTExpiredError,
     SlingshotUnauthenticatedError,
 )
@@ -97,14 +98,15 @@
     async def _maybe_setup(self) -> None:
         if self._is_setup:
             return
         if self._auto_setup_hook is None:
             return
         await self._auto_setup_hook()
 
+    @backoff.on_exception(backoff.expo, (SlingshotBackoffError,), max_tries=3)
     async def make_request(
         self,
         url: str,
         *,
         method: str,
         response_model: Type[T] | None,
         params: ParamsType | None = None,
@@ -135,14 +137,16 @@
                     headers=headers,
                     timeout=int(timeout.total_seconds()),
                     max_redirects=0,
                 ) as resp:
                     logger.debug(f"Got response from '{url}': {resp.status}")
                     if 400 <= resp.status <= 600:
                         exception = await SlingshotClientHttpException.from_response(resp)
+                        if resp.status == 503 or resp.status == 429:
+                            raise SlingshotBackoffError(f"Service unavailable: {resp.status}")
                         if 500 <= resp.status <= 600:
                             if self._slingshot_url != config.global_config.slingshot_local_url:
                                 sentry_sdk.capture_exception(exception)
                         raise exception
                     if response_model == aiohttp.ClientResponse:
                         return resp
                     elif response_model is None:
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/slingshot_sdk.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/slingshot_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,17 +229,29 @@
         """
         Apply the YAML configuration in the current directory to the current project.
 
         Returns True if any changes were applied, False otherwise.
         """
         return await ApplyService(self).plan_prompt_apply(and_wait=and_wait, force=force)
 
-    async def apply_to_local(self, force: bool = False) -> bool:
-        """Apply the YAML configuration from the remote project to the current project"""
-        return await ApplyService(self).apply_to_local(None, force=force)
+    async def apply_to_local(self, force: bool = False, print_logs: bool = False) -> bool:
+        """
+        Apply the YAML configuration from the remote project to the current project.
+
+        Returns True if any changes were applied.
+        """
+        any_changes_applied = await ApplyService(self).apply_to_local(None, force=force)
+
+        if print_logs:
+            if not any_changes_applied:
+                console.print("No changes pulled")
+            else:
+                console.print("Changes pulled to your local 'slingshot.yaml'.")
+
+        return any_changes_applied
 
     """
     Source code SDK methods
     """
 
     async def push_code(
         self, code_dir: str | None = None, description: Optional[str] = None, and_print: bool = False
@@ -280,15 +292,15 @@
         self, url_response: schemas.BlobArtifactSignedURL, *, save_path: str | None, prompt_overwrite: bool = False
     ) -> str:
         signed_url = url_response.signed_url
         if save_path:
             download_filepath = save_path
         else:
             blob_name = url_response.blob_artifact_name
-            file_path = url_response.file_path
+            file_path = url_response.blob_filename
             download_filepath = f"{blob_name}/{file_path}"
 
         # Check if file already exists for overwriting
         while prompt_overwrite and os.path.exists(download_filepath):
             # Prompt the user to overwrite the file
             overwrite = typer.confirm(f"File {download_filepath} already exists. Do you wish to overwrite?")
             if overwrite:
@@ -378,20 +390,20 @@
         blob_artifact = await self._api.get_blob_artifact_by_id(blob_artifact_id=blob_artifact_id)
         assert blob_artifact, "Blob artifact not found"
         return blob_artifact
 
     @experimental
     async def upsert_dataset_artifact(self, upsert: schemas.Upsert | Path, dataset_tag: str) -> fragments.BlobArtifact:
         """
-        Apply an upsert to the latest dataset matching the given tag for the current project that outputs.
-        All upserted datasets will be a single file called `dataset.jsonl`.
+        Apply an upsert to the latest dataset matching the given tag.
+
+        All upsert datasets need to contain a file called `dataset.jsonl` in the root of the artifact.
 
-        If there is an existing dataset with the given tag, then the upsert will be applied to it. An error will occur
-        if the existing dataset is not a single file called `dataset.jsonl`. Otherwise, a new dataset will be created
-        with the given tag, that only contains the upsert data.
+        If there is an existing dataset with the given tag, then the upsert will be applied to it.
+        Otherwise, a new dataset will be created with the given tag that only contains the upsert data.
         """
         project_id = await self._get_current_project_id_or_raise()
         if isinstance(upsert, schemas.Upsert):
             with tempfile.TemporaryDirectory() as tmpdir:
                 upsert_filename = Path(tmpdir) / f"upsert-{uuid.uuid4().hex[:8]}.json"
                 with open(upsert_filename, "w") as f:
                     json.dump(json.loads(upsert.json()), f)
@@ -649,17 +661,18 @@
         project_id = await self._get_current_project_id_or_raise()
         app_spec = await self._api.get_app_spec_by_name(app_spec_name=app_name, project_id=project_id)
         if not app_spec:
             raise SlingshotException(f"Could not find app with name {app_name}")
 
         if not source_code_id:
             source_code = await self._api.get_latest_source_codes_for_project(project_id=project_id)
-            if not source_code:
+            # Custom plugins don't need to have source code
+            if not source_code and app_spec.app_sub_type is None:
                 raise SlingshotCodeNotFound()
-            source_code_id = source_code.source_code_id
+            source_code_id = source_code.source_code_id if source_code else None
 
         resp = await self._api.start_app(app_spec=app_spec, source_code_id=source_code_id, project_id=project_id)
         data = get_data_or_raise(resp)
         app_instance = await self._api.get_app_instance(app_instance_id=data.app_instance_id, project_id=project_id)
         if not app_instance:
             raise SlingshotException(f"Could not find app instance")
         return app_instance
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/sync.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/sync.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,80 +6,119 @@
 from contextlib import contextmanager
 from io import BytesIO
 from logging import getLogger
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Generator, Optional
 
+import sh  # type: ignore
 import typer
+from sh import CommandNotFound, ErrorReturnCode
 
 from slingshot import schemas
 from slingshot.sdk.errors import SlingshotException
 from slingshot.sdk.utils import bytes_to_str, console, md5_hash
 from slingshot.shared.utils import get_data_or_raise
 
 if typing.TYPE_CHECKING:
     from slingshot.sdk import SlingshotSDK
 
 logger = getLogger(__name__)
 app = typer.Typer()
 
 ROOT_SUFFIX_TO_IGNORE = ["__pycache__", ".egg-info", ".slingshot"]
-FILES_TO_IGNORE = [".DS_Store", "slingshot.yaml"]
 
-# 100kb = 100_000 bytes
-MAX_FILESIZE = 100_000
+MAX_FILESIZE = 100_000  # 100KiB in bytes
 
-# 10mb = 10_000_000 bytes
-MAX_TOTAL_SIZE = 10_000_000
+MAX_FILESIZE_LARGE = 1_000_000  # 1MiB in bytes
+
+MAX_TOTAL_SIZE = 10_000_000  # 10MiB in bytes
 
 MAX_NUM_FILES = 1000
 
 
 def should_skip_root(root: str) -> bool:
     return any(root.endswith(suffix) for suffix in ROOT_SUFFIX_TO_IGNORE)
 
 
 def _zip_artifact_recursive(quiet: bool) -> bytes:
     """
-    Zip the files in the current working directory, recursively. This does not exclude files that are gitignored.
-    TODO: [nice to have] Do a better job at ignoring stuff (e.g. via git)
+    Zip the files in the current working directory, recursively. Excludes files based on size and git metadata:
+      - Ignored files are skipped unless they're committed, in which case they're limited at MAX_FILESIZE
+      - Files that are neither ignored nor committed are included, limited at MAX_FILESIZE
+      - Otherwise, files are limited at MAX_FILESIZE_LARGE
     """
     with BytesIO() as zip_io:
         with zipfile.ZipFile(zip_io, "w") as zf:
-            for root, dirs, files in os.walk("."):
-                if should_skip_root(root):
-                    continue
-                # Check if the directory has more than MAX_NUM_FILES files
-                if len(files) > MAX_NUM_FILES:
-                    console.print(
-                        f"Sync directory has too many files: '{root}' ⚠️. Skipping this directory.", style="yellow"
-                    )
-                    continue
-                for file in files:
-                    if file in FILES_TO_IGNORE:
-                        continue
-                    # Check size of file
-                    file_path = os.path.join(root, file)
-                    size = os.path.getsize(file_path)
-                    if size > MAX_FILESIZE:
-                        relative_path = os.path.relpath(file_path)
-                        if not quiet:
-                            console.print(
-                                f"Skipping '{relative_path}' because it is too large ({bytes_to_str(size)}) ⚠️",
-                                style="yellow",
-                            )
-                        continue
-                    zf.write(file_path)
+            try:
+                _zip_with_git_ls(quiet, zf)
+            except (CommandNotFound, ErrorReturnCode):
+                _zip_legacy(quiet, zf)
+
         bytes_ = zip_io.getvalue()
         if len(bytes_) > MAX_TOTAL_SIZE:
             raise SlingshotException(f"Sync directory is too large ({len(bytes_)} bytes) ⚠️. ")
         return bytes_
 
 
+def _zip_legacy(quiet: bool, zf: zipfile.ZipFile) -> None:
+    if not quiet:
+        console.print("[yellow]Using legacy code push strategy[/yellow]. (Make sure 'git' is on your PATH to resolve.)")
+
+    for root, dirs, files in os.walk("."):
+        if should_skip_root(root):
+            continue
+        if len(files) > MAX_NUM_FILES:
+            console.print(f"Sync directory has too many files: '{root}' ⚠️. Skipping this directory.", style="yellow")
+            continue
+        for file in files:
+            file_path = os.path.join(root, file)
+            size = os.path.getsize(file_path)
+            if size > MAX_FILESIZE:
+                relative_path = os.path.relpath(file_path)
+                if not quiet:
+                    console.print(
+                        f"Skipping '{relative_path}' because it is too large ({bytes_to_str(size)}) ⚠️", style="yellow"
+                    )
+                continue
+            zf.write(file_path)
+
+
+def _zip_with_git_ls(quiet: bool, zf: zipfile.ZipFile) -> None:
+    tracked_files = set(Path(path) for path in sh.git("ls-files").splitlines())
+    untracked_files = set(Path(path) for path in sh.git("ls-files", "-o", "--exclude-standard").splitlines())
+    for root, dirs, files in os.walk("."):
+        if should_skip_root(root):
+            continue
+
+        for file in files:
+            file_path = Path(os.path.join(root, file))
+            size = os.path.getsize(file_path)
+            if file_path in tracked_files:
+                if size > MAX_FILESIZE_LARGE:
+                    relative_path = os.path.relpath(file_path)
+                    if not quiet:
+                        console.print(
+                            f"Skipping '{relative_path}' because it is too large ({bytes_to_str(size)}) ⚠️",
+                            style="yellow",
+                        )
+                    continue
+                zf.write(file_path)
+            elif file_path in untracked_files:
+                if size > MAX_FILESIZE:
+                    relative_path = os.path.relpath(file_path)
+                    if not quiet:
+                        console.print(
+                            f"Skipping '{relative_path}' because it is too large ({bytes_to_str(size)}) ⚠️",
+                            style="yellow",
+                        )
+                    continue
+                zf.write(file_path)
+
+
 async def sync_code(
     sdk: SlingshotSDK, path: Path, description: Optional[str]
 ) -> tuple[schemas.UploadedSourceCode, bool]:
     logger.debug(f"Zipping up {path}...")
     zip_bytes = zip_code_artifact(path)
 
     # Check if the code is already uploaded
@@ -111,15 +150,14 @@
     return uploaded_source_code_resp, True
 
 
 def zip_code_artifact(root: Path, *, quiet: bool = False) -> bytes:
     """Zip the files in the current working directory, recursively. If the working directory is within a
     git repository, zip only the files that are in the directory and in the repository."""
     with enter_route(root):
-        os.chdir(root)
         logger.debug(f"Zipping up {root.absolute()}...")
         return _zip_artifact_recursive(quiet)
 
 
 @contextmanager
 def enter_route(path: Path) -> Generator[None, None, None]:
     """
```

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/upload_download_utils.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/upload_download_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/sdk/web_path_util.py` & `slingshot_ai-0.0.17/src/slingshot/sdk/web_path_util.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/shared/utils.py` & `slingshot_ai-0.0.17/src/slingshot/shared/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/templates/inference_template.py` & `slingshot_ai-0.0.17/src/slingshot/templates/inference_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/src/slingshot/templates/label_studio_data_export_template.py` & `slingshot_ai-0.0.17/src/slingshot/templates/label_studio_data_export_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.16/PKG-INFO` & `slingshot_ai-0.0.17/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slingshot-ai
-Version: 0.0.16
+Version: 0.0.17
 Summary: 
 Author: Slingshot AI
 Author-email: service-account@slingshot.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,8 +19,8 @@
 Requires-Dist: ruamel.yaml (>=0.17.0,<0.18.0)
 Requires-Dist: sentry-sdk (>=1.16.0,<1.17.0)
 Requires-Dist: sh (>=1.14.3,<1.15.0)
 Requires-Dist: simple-term-menu (>=1.6.0,<1.7.0)
 Requires-Dist: tqdm (>=4.63.0,<4.64.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: urllib3 (>=1.26.11,<1.27.0)
-Requires-Dist: uvicorn[standard] (>=0.18.0,<0.19.0)
+Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0)
```

