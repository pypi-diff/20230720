# Comparing `tmp/DigiCore-1.0.9.tar.gz` & `tmp/DigiCore-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DigiCore-1.0.9.tar", last modified: Thu Jul 20 06:32:54 2023, max compression
+gzip compressed data, was "dist\DigiCore-1.1.0.tar", last modified: Thu Jul 20 09:08:39 2023, max compression
```

## Comparing `DigiCore-1.0.9.tar` & `DigiCore-1.1.0.tar`

### file list

```diff
@@ -1,63 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.798747 DigiCore-1.0.9/
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.597261 DigiCore-1.0.9/DigiCore.egg-info/
--rw-rw-rw-   0        0        0     4014 2023-07-20 06:32:54.000000 DigiCore-1.0.9/DigiCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1534 2023-07-20 06:32:54.000000 DigiCore-1.0.9/DigiCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 06:32:54.000000 DigiCore-1.0.9/DigiCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      585 2023-07-20 06:32:54.000000 DigiCore-1.0.9/DigiCore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       97 2023-07-20 06:32:54.000000 DigiCore-1.0.9/DigiCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 06:32:54.000000 DigiCore-1.0.9/DigiCore.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     4014 2023-07-20 06:32:54.797747 DigiCore-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.598001 DigiCore-1.0.9/alibabacloud_dingtalk/
--rw-rw-rw-   0        0        0       22 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_dingtalk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.603207 DigiCore-1.0.9/alibabacloud_dingtalk/yida_1_0/
--rw-rw-rw-   0        0        0       23 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-rw-rw-   0        0        0   474192 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_dingtalk/yida_1_0/client.py
--rw-rw-rw-   0        0        0   707743 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_dingtalk/yida_1_0/models.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.609212 DigiCore-1.0.9/alibabacloud_tea_openapi/
--rw-rw-rw-   0        0        0       23 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_tea_openapi/__init__.py
--rw-rw-rw-   0        0        0   102955 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_tea_openapi/client.py
--rw-rw-rw-   0        0        0    14699 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_tea_openapi/models.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.612575 DigiCore-1.0.9/alibabacloud_tea_util/
--rw-rw-rw-   0        0        0       24 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_tea_util/__init__.py
--rw-rw-rw-   0        0        0    13526 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_tea_util/client.py
--rw-rw-rw-   0        0        0     5687 2023-07-20 06:23:17.000000 DigiCore-1.0.9/alibabacloud_tea_util/models.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.665773 DigiCore-1.0.9/digiCore/
--rw-rw-rw-   0        0        0     1382 2023-07-05 07:14:07.000000 DigiCore-1.0.9/digiCore/__init__.py
--rw-rw-rw-   0        0        0     3056 2023-07-05 06:47:32.000000 DigiCore-1.0.9/digiCore/db_init.py
--rw-rw-rw-   0        0        0     4914 2023-07-20 06:23:17.000000 DigiCore-1.0.9/digiCore/dsd_kafka.py
--rw-rw-rw-   0        0        0     3450 2023-07-05 06:47:32.000000 DigiCore-1.0.9/digiCore/dsd_mongodb.py
--rw-rw-rw-   0        0        0     6853 2023-07-05 06:45:24.000000 DigiCore-1.0.9/digiCore/dsd_mysql.py
--rw-rw-rw-   0        0        0     5667 2023-07-20 06:23:17.000000 DigiCore-1.0.9/digiCore/dsd_redis.py
--rw-rw-rw-   0        0        0     4539 2023-07-20 06:23:17.000000 DigiCore-1.0.9/digiCore/lingxing_api_scheduler.py
--rw-rw-rw-   0        0        0     3558 2023-07-05 06:47:32.000000 DigiCore-1.0.9/digiCore/model.py
--rw-rw-rw-   0        0        0     3227 2023-07-20 06:23:17.000000 DigiCore-1.0.9/digiCore/read_yida_table.py
--rw-rw-rw-   0        0        0     3739 2023-07-05 06:45:24.000000 DigiCore-1.0.9/digiCore/send_to_group.py
--rw-rw-rw-   0        0        0     6413 2023-07-20 06:23:17.000000 DigiCore-1.0.9/digiCore/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.685748 DigiCore-1.0.9/k3cloud_webapi_sdk/
--rw-rw-rw-   0        0        0       29 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.702966 DigiCore-1.0.9/k3cloud_webapi_sdk/const/
--rw-rw-rw-   0        0        0       16 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/const/__init__.py
--rw-rw-rw-   0        0        0      418 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/const/const_define.py
--rw-rw-rw-   0        0        0      500 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/const/header_param.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.715983 DigiCore-1.0.9/k3cloud_webapi_sdk/core/
--rw-rw-rw-   0        0        0       15 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/core/__init__.py
--rw-rw-rw-   0        0        0     8162 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/core/webapi_client.py
--rw-rw-rw-   0        0        0     7910 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/main.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.762057 DigiCore-1.0.9/k3cloud_webapi_sdk/model/
--rw-rw-rw-   0        0        0       16 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/model/__init__.py
--rw-rw-rw-   0        0        0      433 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/model/api_config.py
--rw-rw-rw-   0        0        0     1109 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/model/cookie.py
--rw-rw-rw-   0        0        0      327 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/model/cookie_store.py
--rw-rw-rw-   0        0        0      411 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/model/identity.py
--rw-rw-rw-   0        0        0      197 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/model/query_param.py
--rw-rw-rw-   0        0        0     4385 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:32:54.796747 DigiCore-1.0.9/k3cloud_webapi_sdk/util/
--rw-rw-rw-   0        0        0       15 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/util/base64_util.py
--rw-rw-rw-   0        0        0     2671 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/util/config_util.py
--rw-rw-rw-   0        0        0     1654 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/util/encode_util.py
--rw-rw-rw-   0        0        0      420 2023-07-05 06:45:24.000000 DigiCore-1.0.9/k3cloud_webapi_sdk/util/hmac_util.py
--rw-rw-rw-   0        0        0       42 2023-07-20 06:32:54.798747 DigiCore-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     3015 2023-07-20 06:27:42.000000 DigiCore-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.764164 DigiCore-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.660105 DigiCore-1.1.0/DigiCore.egg-info/
+-rw-rw-rw-   0        0        0     4014 2023-07-20 09:08:39.000000 DigiCore-1.1.0/DigiCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2408 2023-07-20 09:08:39.000000 DigiCore-1.1.0/DigiCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 09:08:39.000000 DigiCore-1.1.0/DigiCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      585 2023-07-20 09:08:39.000000 DigiCore-1.1.0/DigiCore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      228 2023-07-20 09:08:39.000000 DigiCore-1.1.0/DigiCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 09:08:39.000000 DigiCore-1.1.0/DigiCore.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4014 2023-07-20 09:08:39.764164 DigiCore-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.669733 DigiCore-1.1.0/Tea/
+-rw-rw-rw-   0        0        0       23 2023-07-20 09:06:20.000000 DigiCore-1.1.0/Tea/__init__.py
+-rw-rw-rw-   0        0        0    10185 2023-07-20 09:06:20.000000 DigiCore-1.1.0/Tea/core.py
+-rw-rw-rw-   0        0        0     1546 2023-07-20 09:06:20.000000 DigiCore-1.1.0/Tea/exceptions.py
+-rw-rw-rw-   0        0        0     1595 2023-07-20 09:06:20.000000 DigiCore-1.1.0/Tea/model.py
+-rw-rw-rw-   0        0        0      878 2023-07-20 09:06:20.000000 DigiCore-1.1.0/Tea/request.py
+-rw-rw-rw-   0        0        0      157 2023-07-20 09:06:20.000000 DigiCore-1.1.0/Tea/response.py
+-rw-rw-rw-   0        0        0      892 2023-07-20 09:06:20.000000 DigiCore-1.1.0/Tea/stream.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.677740 DigiCore-1.1.0/alibabacloud_credentials/
+-rw-rw-rw-   0        0        0       23 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/__init__.py
+-rw-rw-rw-   0        0        0     3597 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/client.py
+-rw-rw-rw-   0        0        0    14926 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/credentials.py
+-rw-rw-rw-   0        0        0      199 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/exceptions.py
+-rw-rw-rw-   0        0        0     6494 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/models.py
+-rw-rw-rw-   0        0        0    28952 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/providers.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.683987 DigiCore-1.1.0/alibabacloud_credentials/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/utils/__init__.py
+-rw-rw-rw-   0        0        0      960 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/utils/auth_constant.py
+-rw-rw-rw-   0        0        0     1055 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/utils/auth_util.py
+-rw-rw-rw-   0        0        0     1377 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_credentials/utils/parameter_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.684851 DigiCore-1.1.0/alibabacloud_dingtalk/
+-rw-rw-rw-   0        0        0       22 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_dingtalk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.691243 DigiCore-1.1.0/alibabacloud_dingtalk/yida_1_0/
+-rw-rw-rw-   0        0        0       23 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-rw-rw-   0        0        0   474192 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-rw-rw-   0        0        0   707743 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_dingtalk/yida_1_0/models.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.695728 DigiCore-1.1.0/alibabacloud_gateway_dingtalk/
+-rw-rw-rw-   0        0        0       23 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_gateway_dingtalk/__init__.py
+-rw-rw-rw-   0        0        0     6749 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_gateway_dingtalk/client.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.700142 DigiCore-1.1.0/alibabacloud_gateway_spi/
+-rw-rw-rw-   0        0        0       23 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_gateway_spi/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_gateway_spi/client.py
+-rw-rw-rw-   0        0        0    12462 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_gateway_spi/models.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.703318 DigiCore-1.1.0/alibabacloud_openapi_util/
+-rw-rw-rw-   0        0        0       23 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_openapi_util/__init__.py
+-rw-rw-rw-   0        0        0    14673 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_openapi_util/client.py
+-rw-rw-rw-   0        0        0     4463 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_openapi_util/sm3.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.709287 DigiCore-1.1.0/alibabacloud_tea_openapi/
+-rw-rw-rw-   0        0        0       23 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_tea_openapi/__init__.py
+-rw-rw-rw-   0        0        0   102955 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_tea_openapi/client.py
+-rw-rw-rw-   0        0        0    14699 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_tea_openapi/models.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.713990 DigiCore-1.1.0/alibabacloud_tea_util/
+-rw-rw-rw-   0        0        0       24 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_tea_util/__init__.py
+-rw-rw-rw-   0        0        0    13526 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_tea_util/client.py
+-rw-rw-rw-   0        0        0     5687 2023-07-20 06:23:17.000000 DigiCore-1.1.0/alibabacloud_tea_util/models.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.716138 DigiCore-1.1.0/alibabacloud_tea_xml/
+-rw-rw-rw-   0        0        0       23 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_tea_xml/__init__.py
+-rw-rw-rw-   0        0        0     3170 2023-07-20 09:06:20.000000 DigiCore-1.1.0/alibabacloud_tea_xml/client.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.733151 DigiCore-1.1.0/digiCore/
+-rw-rw-rw-   0        0        0     1382 2023-07-05 07:14:07.000000 DigiCore-1.1.0/digiCore/__init__.py
+-rw-rw-rw-   0        0        0     3056 2023-07-05 06:47:32.000000 DigiCore-1.1.0/digiCore/db_init.py
+-rw-rw-rw-   0        0        0     4914 2023-07-20 06:23:17.000000 DigiCore-1.1.0/digiCore/dsd_kafka.py
+-rw-rw-rw-   0        0        0     3450 2023-07-05 06:47:32.000000 DigiCore-1.1.0/digiCore/dsd_mongodb.py
+-rw-rw-rw-   0        0        0     6853 2023-07-05 06:45:24.000000 DigiCore-1.1.0/digiCore/dsd_mysql.py
+-rw-rw-rw-   0        0        0     5667 2023-07-20 06:23:17.000000 DigiCore-1.1.0/digiCore/dsd_redis.py
+-rw-rw-rw-   0        0        0     4539 2023-07-20 06:23:17.000000 DigiCore-1.1.0/digiCore/lingxing_api_scheduler.py
+-rw-rw-rw-   0        0        0     3558 2023-07-05 06:47:32.000000 DigiCore-1.1.0/digiCore/model.py
+-rw-rw-rw-   0        0        0     3227 2023-07-20 06:23:17.000000 DigiCore-1.1.0/digiCore/read_yida_table.py
+-rw-rw-rw-   0        0        0     3739 2023-07-05 06:45:24.000000 DigiCore-1.1.0/digiCore/send_to_group.py
+-rw-rw-rw-   0        0        0     6413 2023-07-20 06:23:17.000000 DigiCore-1.1.0/digiCore/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.738140 DigiCore-1.1.0/k3cloud_webapi_sdk/
+-rw-rw-rw-   0        0        0       29 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.742230 DigiCore-1.1.0/k3cloud_webapi_sdk/const/
+-rw-rw-rw-   0        0        0       16 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/const/const_define.py
+-rw-rw-rw-   0        0        0      500 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/const/header_param.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.745237 DigiCore-1.1.0/k3cloud_webapi_sdk/core/
+-rw-rw-rw-   0        0        0       15 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/core/__init__.py
+-rw-rw-rw-   0        0        0     8162 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/core/webapi_client.py
+-rw-rw-rw-   0        0        0     7910 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/main.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.754521 DigiCore-1.1.0/k3cloud_webapi_sdk/model/
+-rw-rw-rw-   0        0        0       16 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/model/api_config.py
+-rw-rw-rw-   0        0        0     1109 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/model/cookie.py
+-rw-rw-rw-   0        0        0      327 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/model/cookie_store.py
+-rw-rw-rw-   0        0        0      411 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/model/identity.py
+-rw-rw-rw-   0        0        0      197 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/model/query_param.py
+-rw-rw-rw-   0        0        0     4385 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:08:39.762163 DigiCore-1.1.0/k3cloud_webapi_sdk/util/
+-rw-rw-rw-   0        0        0       15 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/util/base64_util.py
+-rw-rw-rw-   0        0        0     2671 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/util/config_util.py
+-rw-rw-rw-   0        0        0     1654 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/util/encode_util.py
+-rw-rw-rw-   0        0        0      420 2023-07-05 06:45:24.000000 DigiCore-1.1.0/k3cloud_webapi_sdk/util/hmac_util.py
+-rw-rw-rw-   0        0        0       42 2023-07-20 09:08:39.764164 DigiCore-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3015 2023-07-20 09:06:54.000000 DigiCore-1.1.0/setup.py
```

### Comparing `DigiCore-1.0.9/DigiCore.egg-info/PKG-INFO` & `DigiCore-1.1.0/DigiCore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.9
+Version: 1.1.0
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.9/DigiCore.egg-info/requires.txt` & `DigiCore-1.1.0/DigiCore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/LICENSE` & `DigiCore-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/PKG-INFO` & `DigiCore-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.9
+Version: 1.1.0
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.9/README.md` & `DigiCore-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/alibabacloud_dingtalk/yida_1_0/client.py` & `DigiCore-1.1.0/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/alibabacloud_dingtalk/yida_1_0/models.py` & `DigiCore-1.1.0/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/alibabacloud_tea_openapi/client.py` & `DigiCore-1.1.0/alibabacloud_tea_openapi/client.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/alibabacloud_tea_openapi/models.py` & `DigiCore-1.1.0/alibabacloud_tea_openapi/models.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/alibabacloud_tea_util/client.py` & `DigiCore-1.1.0/alibabacloud_tea_util/client.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/alibabacloud_tea_util/models.py` & `DigiCore-1.1.0/alibabacloud_tea_util/models.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/__init__.py` & `DigiCore-1.1.0/digiCore/__init__.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/db_init.py` & `DigiCore-1.1.0/digiCore/db_init.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/dsd_kafka.py` & `DigiCore-1.1.0/digiCore/dsd_kafka.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/dsd_mongodb.py` & `DigiCore-1.1.0/digiCore/dsd_mongodb.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/dsd_mysql.py` & `DigiCore-1.1.0/digiCore/dsd_mysql.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/dsd_redis.py` & `DigiCore-1.1.0/digiCore/dsd_redis.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/lingxing_api_scheduler.py` & `DigiCore-1.1.0/digiCore/lingxing_api_scheduler.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/model.py` & `DigiCore-1.1.0/digiCore/model.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/read_yida_table.py` & `DigiCore-1.1.0/digiCore/read_yida_table.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/send_to_group.py` & `DigiCore-1.1.0/digiCore/send_to_group.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/digiCore/utils.py` & `DigiCore-1.1.0/digiCore/utils.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/k3cloud_webapi_sdk/core/webapi_client.py` & `DigiCore-1.1.0/k3cloud_webapi_sdk/core/webapi_client.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/k3cloud_webapi_sdk/main.py` & `DigiCore-1.1.0/k3cloud_webapi_sdk/main.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/k3cloud_webapi_sdk/model/cookie.py` & `DigiCore-1.1.0/k3cloud_webapi_sdk/model/cookie.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/k3cloud_webapi_sdk/sample.py` & `DigiCore-1.1.0/k3cloud_webapi_sdk/sample.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/k3cloud_webapi_sdk/util/base64_util.py` & `DigiCore-1.1.0/k3cloud_webapi_sdk/util/base64_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/k3cloud_webapi_sdk/util/config_util.py` & `DigiCore-1.1.0/k3cloud_webapi_sdk/util/config_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/k3cloud_webapi_sdk/util/encode_util.py` & `DigiCore-1.1.0/k3cloud_webapi_sdk/util/encode_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.9/setup.py` & `DigiCore-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 "tzdata>=2023.3",
 "urllib3>=2.0.2",
 "win32-setctime>=1.1.0"
 ]
 
 setup(
     name="DigiCore",
-    version="1.0.9",
+    version="1.1.0",
     description="DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。",
     long_description=README,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
```

