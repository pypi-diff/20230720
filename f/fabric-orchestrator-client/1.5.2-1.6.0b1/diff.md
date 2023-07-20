# Comparing `tmp/fabric-orchestrator-client-1.5.2.tar.gz` & `tmp/fabric-orchestrator-client-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.5.2.tar", last modified: Mon Jul 17 20:55:45 2023, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.6.0b1.tar", last modified: Thu Jul 20 17:44:15 2023, max compression
```

## Comparing `fabric-orchestrator-client-1.5.2.tar` & `fabric-orchestrator-client-1.6.0b1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      793 2023-05-11 17:37:01.210207 fabric-orchestrator-client-1.5.2/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 17:37:01.210355 fabric-orchestrator-client-1.5.2/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-07-17 20:49:48.768205 fabric-orchestrator-client-1.5.2/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 17:37:01.210626 fabric-orchestrator-client-1.5.2/.travis.yml
--rw-r--r--   0        0        0      770 2023-05-11 17:37:01.210729 fabric-orchestrator-client-1.5.2/CODEGEN.md
--rw-r--r--   0        0        0     1071 2023-05-11 17:37:01.210862 fabric-orchestrator-client-1.5.2/LICENSE
--rw-r--r--   0        0        0       59 2023-05-11 17:37:01.210963 fabric-orchestrator-client-1.5.2/MANIFEST.in
--rw-r--r--   0        0        0     9867 2023-07-17 20:49:48.770096 fabric-orchestrator-client-1.5.2/README.md
--rw-r--r--   0        0        0      340 2023-07-17 20:49:48.770872 fabric-orchestrator-client-1.5.2/docs/Poa.md
--rw-r--r--   0        0        0      557 2023-07-17 20:49:48.771474 fabric-orchestrator-client-1.5.2/docs/PoaData.md
--rw-r--r--   0        0        0      376 2023-07-17 20:49:48.772151 fabric-orchestrator-client-1.5.2/docs/PoaPost.md
--rw-r--r--   0        0        0      430 2023-07-17 20:49:48.772876 fabric-orchestrator-client-1.5.2/docs/PoaPostData.md
--rw-r--r--   0        0        0      369 2023-07-17 20:49:48.773303 fabric-orchestrator-client-1.5.2/docs/PoaPostDataVcpuCpuMap.md
--rw-r--r--   0        0        0     6404 2023-07-17 20:49:48.774052 fabric-orchestrator-client-1.5.2/docs/PoasApi.md
--rw-r--r--   0        0        0     4263 2023-05-11 17:37:01.211350 fabric-orchestrator-client-1.5.2/docs/ResourcesApi.md
--rw-r--r--   0        0        0    20667 2023-07-17 20:49:48.775232 fabric-orchestrator-client-1.5.2/docs/SlicesApi.md
--rw-r--r--   0        0        0     4102 2023-07-17 20:49:48.776060 fabric-orchestrator-client-1.5.2/docs/SliversApi.md
--rw-r--r--   0        0        0      335 2023-05-11 17:37:01.211789 fabric-orchestrator-client-1.5.2/docs/Success.md
--rw-r--r--   0        0        0      352 2023-05-11 17:37:01.211912 fabric-orchestrator-client-1.5.2/docs/Version.md
--rw-r--r--   0        0        0       22 2023-07-17 20:55:28.031580 fabric-orchestrator-client-1.5.2/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:37:01.212158 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0    21840 2023-07-17 20:49:48.777773 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/orchestrator_proxy.py
--rw-r--r--   0        0        0     3557 2023-07-17 20:49:48.778938 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/__init__.py
--rw-r--r--   0        0        0      468 2023-07-17 20:49:48.779817 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0        0        0    13515 2023-07-17 20:49:48.780918 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/poas_api.py
--rw-r--r--   0        0        0     9597 2023-05-11 17:37:01.213024 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0        0        0    43978 2023-07-17 20:52:06.850318 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0        0        0     9260 2023-07-17 20:49:48.782141 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0        0        0     3748 2023-05-11 17:37:01.213724 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25272 2023-07-17 20:47:34.398882 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0        0        0     8240 2023-05-11 17:37:01.214372 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/configuration.py
--rw-r--r--   0        0        0     2978 2023-07-17 20:49:48.782449 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3427 2023-07-17 20:49:48.783245 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa.py
--rw-r--r--   0        0        0     6654 2023-07-17 20:49:48.784161 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_data.py
--rw-r--r--   0        0        0     4034 2023-07-17 20:49:48.785395 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post.py
--rw-r--r--   0        0        0     3878 2023-07-17 20:49:48.786219 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
--rw-r--r--   0        0        0     3648 2023-07-17 20:49:48.786798 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     3055 2023-05-11 17:37:01.214908 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0        0        0     3420 2023-05-11 17:37:01.215233 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0        0        0     8496 2023-05-11 17:37:01.215453 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0        0        0     3444 2023-07-17 20:49:48.787456 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0        0        0     3412 2023-05-11 17:37:01.215680 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0        0        0     3951 2023-07-17 20:49:48.788286 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slices_post.py
--rw-r--r--   0        0        0    10905 2023-07-17 20:49:48.789193 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0        0        0     3422 2023-05-11 17:37:01.216181 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0        0        0     4999 2023-05-11 17:37:01.216373 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3832 2023-05-11 17:37:01.216668 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     6211 2023-05-11 17:37:01.216937 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4253 2023-05-11 17:37:01.217164 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3163 2023-05-11 17:37:01.217341 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5771 2023-05-11 17:37:01.217534 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5063 2023-05-11 17:37:01.217713 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3870 2023-05-11 17:37:01.217919 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     4994 2023-05-11 17:37:01.218148 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3831 2023-05-11 17:37:01.218431 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4971 2023-05-11 17:37:01.218623 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3819 2023-05-11 17:37:01.218944 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5224 2023-05-11 17:37:01.219262 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3963 2023-05-11 17:37:01.219487 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3413 2023-05-11 17:37:01.219669 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0        0        0     3882 2023-05-11 17:37:01.219920 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    12988 2023-05-11 17:37:01.220174 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 17:37:01.220383 fabric-orchestrator-client-1.5.2/git_push.sh
--rw-r--r--   0        0        0     1024 2023-07-17 20:54:47.871007 fabric-orchestrator-client-1.5.2/pyproject.toml
--rw-r--r--   0        0        0       16 2023-07-17 20:49:48.791020 fabric-orchestrator-client-1.5.2/test/__init__.py
--rw-r--r--   0        0        0      809 2023-07-17 20:49:48.791882 fabric-orchestrator-client-1.5.2/test/test_poa.py
--rw-r--r--   0        0        0      843 2023-07-17 20:49:48.792642 fabric-orchestrator-client-1.5.2/test/test_poa_data.py
--rw-r--r--   0        0        0      843 2023-07-17 20:49:48.793127 fabric-orchestrator-client-1.5.2/test/test_poa_post.py
--rw-r--r--   0        0        0      877 2023-07-17 20:49:48.793692 fabric-orchestrator-client-1.5.2/test/test_poa_post_data.py
--rw-r--r--   0        0        0      963 2023-07-17 20:49:48.794485 fabric-orchestrator-client-1.5.2/test/test_poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     1157 2023-07-17 20:49:48.795260 fabric-orchestrator-client-1.5.2/test/test_poas_api.py
--rw-r--r--   0        0        0      896 2023-05-11 17:37:01.221224 fabric-orchestrator-client-1.5.2/test/test_resource.py
--rw-r--r--   0        0        0      950 2023-05-11 17:37:01.221397 fabric-orchestrator-client-1.5.2/test/test_resources.py
--rw-r--r--   0        0        0     1206 2023-05-11 17:37:01.221693 fabric-orchestrator-client-1.5.2/test/test_resources_api.py
--rw-r--r--   0        0        0      872 2023-05-11 17:37:01.221929 fabric-orchestrator-client-1.5.2/test/test_slice.py
--rw-r--r--   0        0        0      930 2023-05-11 17:37:01.222101 fabric-orchestrator-client-1.5.2/test/test_slice_details.py
--rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222270 fabric-orchestrator-client-1.5.2/test/test_slices.py
--rw-r--r--   0        0        0     2165 2023-07-17 20:49:48.796346 fabric-orchestrator-client-1.5.2/test/test_slices_api.py
--rw-r--r--   0        0        0      867 2023-07-17 20:49:48.797642 fabric-orchestrator-client-1.5.2/test/test_slices_post.py
--rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222608 fabric-orchestrator-client-1.5.2/test/test_sliver.py
--rw-r--r--   0        0        0      888 2023-05-11 17:37:01.222785 fabric-orchestrator-client-1.5.2/test/test_slivers.py
--rw-r--r--   0        0        0      974 2023-07-17 20:49:48.798816 fabric-orchestrator-client-1.5.2/test/test_slivers_api.py
--rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223296 fabric-orchestrator-client-1.5.2/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1032 2023-05-11 17:37:01.223607 fabric-orchestrator-client-1.5.2/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      996 2023-05-11 17:37:01.223847 fabric-orchestrator-client-1.5.2/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      972 2023-05-11 17:37:01.224081 fabric-orchestrator-client-1.5.2/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      988 2023-05-11 17:37:01.224292 fabric-orchestrator-client-1.5.2/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1038 2023-05-11 17:37:01.224535 fabric-orchestrator-client-1.5.2/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0     1002 2023-05-11 17:37:01.224771 fabric-orchestrator-client-1.5.2/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1052 2023-05-11 17:37:01.225030 fabric-orchestrator-client-1.5.2/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      978 2023-05-11 17:37:01.225269 fabric-orchestrator-client-1.5.2/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1028 2023-05-11 17:37:01.225554 fabric-orchestrator-client-1.5.2/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      972 2023-05-11 17:37:01.225840 fabric-orchestrator-client-1.5.2/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1022 2023-05-11 17:37:01.226137 fabric-orchestrator-client-1.5.2/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1062 2023-05-11 17:37:01.226327 fabric-orchestrator-client-1.5.2/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1112 2023-05-11 17:37:01.226547 fabric-orchestrator-client-1.5.2/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      888 2023-05-11 17:37:01.226964 fabric-orchestrator-client-1.5.2/test/test_version.py
--rw-r--r--   0        0        0      814 2023-05-11 17:37:01.227150 fabric-orchestrator-client-1.5.2/test/test_version_api.py
--rw-r--r--   0        0        0      922 2023-05-11 17:37:01.227332 fabric-orchestrator-client-1.5.2/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 17:37:01.227515 fabric-orchestrator-client-1.5.2/tox.ini
--rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      793 2023-07-20 16:57:55.683480 fabric-orchestrator-client-1.6.0b1/.gitignore
+-rw-r--r--   0        0        0     1030 2023-07-20 16:57:55.683782 fabric-orchestrator-client-1.6.0b1/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-07-20 17:37:23.319252 fabric-orchestrator-client-1.6.0b1/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-07-20 16:57:55.684203 fabric-orchestrator-client-1.6.0b1/.travis.yml
+-rw-r--r--   0        0        0      770 2023-07-20 16:57:55.684315 fabric-orchestrator-client-1.6.0b1/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2023-07-20 16:57:55.684446 fabric-orchestrator-client-1.6.0b1/LICENSE
+-rw-r--r--   0        0        0       59 2023-07-20 16:57:55.684550 fabric-orchestrator-client-1.6.0b1/MANIFEST.in
+-rw-r--r--   0        0        0     9867 2023-07-20 16:57:55.684688 fabric-orchestrator-client-1.6.0b1/README.md
+-rw-r--r--   0        0        0      340 2023-07-20 16:57:55.684865 fabric-orchestrator-client-1.6.0b1/docs/Poa.md
+-rw-r--r--   0        0        0      557 2023-07-20 16:57:55.685023 fabric-orchestrator-client-1.6.0b1/docs/PoaData.md
+-rw-r--r--   0        0        0      376 2023-07-20 16:57:55.685156 fabric-orchestrator-client-1.6.0b1/docs/PoaPost.md
+-rw-r--r--   0        0        0      472 2023-07-20 17:37:29.102056 fabric-orchestrator-client-1.6.0b1/docs/PoaPostData.md
+-rw-r--r--   0        0        0      369 2023-07-20 16:57:55.685376 fabric-orchestrator-client-1.6.0b1/docs/PoaPostDataVcpuCpuMap.md
+-rw-r--r--   0        0        0     6404 2023-07-20 16:57:55.685514 fabric-orchestrator-client-1.6.0b1/docs/PoasApi.md
+-rw-r--r--   0        0        0     4263 2023-07-20 16:57:55.685654 fabric-orchestrator-client-1.6.0b1/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    20667 2023-07-20 16:57:55.685813 fabric-orchestrator-client-1.6.0b1/docs/SlicesApi.md
+-rw-r--r--   0        0        0     4102 2023-07-20 16:57:55.685958 fabric-orchestrator-client-1.6.0b1/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2023-07-20 16:57:55.686145 fabric-orchestrator-client-1.6.0b1/docs/Success.md
+-rw-r--r--   0        0        0      352 2023-07-20 16:57:55.686293 fabric-orchestrator-client-1.6.0b1/docs/Version.md
+-rw-r--r--   0        0        0       24 2023-07-20 16:59:44.471092 fabric-orchestrator-client-1.6.0b1/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:57:55.686541 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    21942 2023-07-20 17:42:47.201620 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3557 2023-07-20 16:57:55.686919 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-20 16:57:55.687067 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0    13515 2023-07-20 16:57:55.687291 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/poas_api.py
+-rw-r--r--   0        0        0     9597 2023-07-20 16:57:55.687498 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    43978 2023-07-20 16:57:55.687852 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     9260 2023-07-20 16:57:55.688058 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2023-07-20 16:57:55.688305 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25272 2023-07-20 16:57:55.688514 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2023-07-20 16:57:55.688681 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2978 2023-07-20 16:57:55.688830 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3427 2023-07-20 16:57:55.689190 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa.py
+-rw-r--r--   0        0        0     6654 2023-07-20 16:57:55.689400 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_data.py
+-rw-r--r--   0        0        0     4057 2023-07-20 17:39:40.282831 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post.py
+-rw-r--r--   0        0        0     4469 2023-07-20 17:39:58.609765 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
+-rw-r--r--   0        0        0     3648 2023-07-20 16:57:55.690053 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     3055 2023-07-20 16:57:55.690298 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2023-07-20 16:57:55.690573 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     8496 2023-07-20 16:57:55.690977 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3444 2023-07-20 16:57:55.691422 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2023-07-20 16:57:55.691759 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0     3951 2023-07-20 16:57:55.691993 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slices_post.py
+-rw-r--r--   0        0        0    10905 2023-07-20 16:57:55.692233 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2023-07-20 16:57:55.692488 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2023-07-20 16:57:55.692698 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2023-07-20 16:57:55.692922 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2023-07-20 16:57:55.693156 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2023-07-20 16:57:55.693385 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2023-07-20 16:57:55.693582 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2023-07-20 16:57:55.693786 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2023-07-20 16:57:55.693960 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2023-07-20 16:57:55.694158 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2023-07-20 16:57:55.694424 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2023-07-20 16:57:55.694605 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2023-07-20 16:57:55.694784 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2023-07-20 16:57:55.695203 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2023-07-20 16:57:55.695486 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2023-07-20 16:57:55.695726 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2023-07-20 16:57:55.695941 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2023-07-20 16:57:55.696224 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12988 2023-07-20 16:57:55.696524 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-07-20 16:57:55.696710 fabric-orchestrator-client-1.6.0b1/git_push.sh
+-rw-r--r--   0        0        0     1024 2023-07-20 16:57:55.696907 fabric-orchestrator-client-1.6.0b1/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-07-20 16:57:55.697079 fabric-orchestrator-client-1.6.0b1/test/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-20 16:57:55.697378 fabric-orchestrator-client-1.6.0b1/test/test_poa.py
+-rw-r--r--   0        0        0      843 2023-07-20 16:57:55.697602 fabric-orchestrator-client-1.6.0b1/test/test_poa_data.py
+-rw-r--r--   0        0        0      843 2023-07-20 16:57:55.697806 fabric-orchestrator-client-1.6.0b1/test/test_poa_post.py
+-rw-r--r--   0        0        0      877 2023-07-20 16:57:55.697996 fabric-orchestrator-client-1.6.0b1/test/test_poa_post_data.py
+-rw-r--r--   0        0        0      963 2023-07-20 16:57:55.698208 fabric-orchestrator-client-1.6.0b1/test/test_poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1157 2023-07-20 16:57:55.698367 fabric-orchestrator-client-1.6.0b1/test/test_poas_api.py
+-rw-r--r--   0        0        0      896 2023-07-20 16:57:55.698574 fabric-orchestrator-client-1.6.0b1/test/test_resource.py
+-rw-r--r--   0        0        0      950 2023-07-20 16:57:55.698746 fabric-orchestrator-client-1.6.0b1/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2023-07-20 16:57:55.698949 fabric-orchestrator-client-1.6.0b1/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2023-07-20 16:57:55.699318 fabric-orchestrator-client-1.6.0b1/test/test_slice.py
+-rw-r--r--   0        0        0      930 2023-07-20 16:57:55.699499 fabric-orchestrator-client-1.6.0b1/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2023-07-20 16:57:55.699671 fabric-orchestrator-client-1.6.0b1/test/test_slices.py
+-rw-r--r--   0        0        0     2165 2023-07-20 16:57:55.699921 fabric-orchestrator-client-1.6.0b1/test/test_slices_api.py
+-rw-r--r--   0        0        0      867 2023-07-20 16:57:55.700175 fabric-orchestrator-client-1.6.0b1/test/test_slices_post.py
+-rw-r--r--   0        0        0      880 2023-07-20 16:57:55.700441 fabric-orchestrator-client-1.6.0b1/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2023-07-20 16:57:55.700646 fabric-orchestrator-client-1.6.0b1/test/test_slivers.py
+-rw-r--r--   0        0        0      974 2023-07-20 16:57:55.700829 fabric-orchestrator-client-1.6.0b1/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2023-07-20 16:57:55.701084 fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2023-07-20 16:57:55.701316 fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2023-07-20 16:57:55.701511 fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2023-07-20 16:57:55.701708 fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2023-07-20 16:57:55.701894 fabric-orchestrator-client-1.6.0b1/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2023-07-20 16:57:55.702089 fabric-orchestrator-client-1.6.0b1/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2023-07-20 16:57:55.702264 fabric-orchestrator-client-1.6.0b1/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2023-07-20 16:57:55.702486 fabric-orchestrator-client-1.6.0b1/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2023-07-20 16:57:55.702815 fabric-orchestrator-client-1.6.0b1/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2023-07-20 16:57:55.703064 fabric-orchestrator-client-1.6.0b1/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2023-07-20 16:57:55.703225 fabric-orchestrator-client-1.6.0b1/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2023-07-20 16:57:55.703377 fabric-orchestrator-client-1.6.0b1/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2023-07-20 16:57:55.703541 fabric-orchestrator-client-1.6.0b1/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2023-07-20 16:57:55.703700 fabric-orchestrator-client-1.6.0b1/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2023-07-20 16:57:55.703904 fabric-orchestrator-client-1.6.0b1/test/test_version.py
+-rw-r--r--   0        0        0      814 2023-07-20 16:57:55.704109 fabric-orchestrator-client-1.6.0b1/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2023-07-20 16:57:55.704281 fabric-orchestrator-client-1.6.0b1/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-07-20 16:57:55.704477 fabric-orchestrator-client-1.6.0b1/tox.ini
+-rw-r--r--   0        0        0    10818 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.6.0b1/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.5.2/.gitignore` & `fabric-orchestrator-client-1.6.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/.swagger-codegen-ignore` & `fabric-orchestrator-client-1.6.0b1/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/CODEGEN.md` & `fabric-orchestrator-client-1.6.0b1/CODEGEN.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/LICENSE` & `fabric-orchestrator-client-1.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/README.md` & `fabric-orchestrator-client-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/docs/PoaData.md` & `fabric-orchestrator-client-1.6.0b1/docs/PoaData.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/docs/PoasApi.md` & `fabric-orchestrator-client-1.6.0b1/docs/PoasApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/docs/ResourcesApi.md` & `fabric-orchestrator-client-1.6.0b1/docs/ResourcesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/docs/SlicesApi.md` & `fabric-orchestrator-client-1.6.0b1/docs/SlicesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/docs/SliversApi.md` & `fabric-orchestrator-client-1.6.0b1/docs/SliversApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,22 +463,23 @@
             self.slices_api.slices_renew_slice_id_post(slice_id=slice_id, lease_end_time=new_lease_end_time)
 
             return Status.OK, None
         except Exception as e:
             return Status.FAILURE, e
 
     def poa(self, *, token: str, sliver_id: str, operation: str, vcpu_cpu_map: List[Dict[str, str]] = None,
-            node_set: List[str] = None) -> Tuple[Status, Union[Exception, List[PoaData]]]:
+            node_set: List[str] = None, keys: List[str]) -> Tuple[Status, Union[Exception, List[PoaData]]]:
         """
         Modify a slice
         @param token fabric token
         @param sliver_id Sliver Id
         @param operation POA operation
         @param vcpu_cpu_map vCPU to physical CPU Map
         @param node_set List of Numa nodes
+        @param keys list of keys to add/remove
         @return Tuple containing Status and Exception/Json containing poa info created
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         if sliver_id is None:
             return Status.INVALID_ARGUMENTS, \
@@ -489,14 +490,15 @@
             self.__set_tokens(token=token)
 
             body = PoaPost(operation=operation)
             if vcpu_cpu_map is not None or node_set is not None:
                 post_data = PoaPostData()
                 post_data.vcpu_cpu_map = vcpu_cpu_map
                 post_data.node_set = node_set
+                post_data.keys = keys
                 body.data = post_data
 
             poa_data = self.poas_api.poas_create_sliver_id_post(sliver_id=sliver_id, body=body)
 
             return Status.OK, poa_data.data if poa_data.data is not None else None
         except Exception as e:
             return Status.FAILURE, e
```

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/poas_api.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_data.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
         :param operation: The operation of this PoaPost.  # noqa: E501
         :type: str
         """
         if operation is None:
             raise ValueError("Invalid value for `operation`, must not be `None`")  # noqa: E501
-        allowed_values = ["cpuinfo", "numainfo", "cpupin", "numatune", "reboot"]  # noqa: E501
+        allowed_values = ["cpuinfo", "numainfo", "cpupin", "numatune", "reboot", "addkey", "removekey"]  # noqa: E501
         if operation not in allowed_values:
             raise ValueError(
                 "Invalid value for `operation` ({0}), must be one of {1}"  # noqa: E501
                 .format(operation, allowed_values)
             )
 
         self._operation = operation
```

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,31 +25,36 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'vcpu_cpu_map': 'list[PoaPostDataVcpuCpuMap]',
-        'node_set': 'list[str]'
+        'node_set': 'list[str]',
+        'keys': 'list[str]'
     }
 
     attribute_map = {
         'vcpu_cpu_map': 'vcpu_cpu_map',
-        'node_set': 'node_set'
+        'node_set': 'node_set',
+        'keys': 'keys'
     }
 
-    def __init__(self, vcpu_cpu_map=None, node_set=None):  # noqa: E501
+    def __init__(self, vcpu_cpu_map=None, node_set=None, keys=None):  # noqa: E501
         """PoaPostData - a model defined in Swagger"""  # noqa: E501
         self._vcpu_cpu_map = None
         self._node_set = None
+        self._keys = None
         self.discriminator = None
         if vcpu_cpu_map is not None:
             self.vcpu_cpu_map = vcpu_cpu_map
         if node_set is not None:
             self.node_set = node_set
+        if keys is not None:
+            self.keys = keys
 
     @property
     def vcpu_cpu_map(self):
         """Gets the vcpu_cpu_map of this PoaPostData.  # noqa: E501
 
 
         :return: The vcpu_cpu_map of this PoaPostData.  # noqa: E501
@@ -85,14 +90,35 @@
 
         :param node_set: The node_set of this PoaPostData.  # noqa: E501
         :type: list[str]
         """
 
         self._node_set = node_set
 
+    @property
+    def keys(self):
+        """Gets the keys of this PoaPostData.  # noqa: E501
+
+
+        :return: The keys of this PoaPostData.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._keys
+
+    @keys.setter
+    def keys(self, keys):
+        """Sets the keys of this PoaPostData.
+
+
+        :param keys: The keys of this PoaPostData.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._keys = keys
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slices_post.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/git_push.sh` & `fabric-orchestrator-client-1.6.0b1/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/pyproject.toml` & `fabric-orchestrator-client-1.6.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_poa.py` & `fabric-orchestrator-client-1.6.0b1/test/test_poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_poa_data.py` & `fabric-orchestrator-client-1.6.0b1/test/test_poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_poa_post.py` & `fabric-orchestrator-client-1.6.0b1/test/test_poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_poa_post_data.py` & `fabric-orchestrator-client-1.6.0b1/test/test_poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.6.0b1/test/test_poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_poas_api.py` & `fabric-orchestrator-client-1.6.0b1/test/test_poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_resource.py` & `fabric-orchestrator-client-1.6.0b1/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_resources.py` & `fabric-orchestrator-client-1.6.0b1/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_resources_api.py` & `fabric-orchestrator-client-1.6.0b1/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_slice.py` & `fabric-orchestrator-client-1.6.0b1/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_slice_details.py` & `fabric-orchestrator-client-1.6.0b1/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_slices.py` & `fabric-orchestrator-client-1.6.0b1/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_slices_api.py` & `fabric-orchestrator-client-1.6.0b1/test/test_slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_slices_post.py` & `fabric-orchestrator-client-1.6.0b1/test/test_slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_sliver.py` & `fabric-orchestrator-client-1.6.0b1/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_slivers.py` & `fabric-orchestrator-client-1.6.0b1/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_slivers_api.py` & `fabric-orchestrator-client-1.6.0b1/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.6.0b1/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_version.py` & `fabric-orchestrator-client-1.6.0b1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_version_api.py` & `fabric-orchestrator-client-1.6.0b1/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/test/test_version_data.py` & `fabric-orchestrator-client-1.6.0b1/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.2/PKG-INFO` & `fabric-orchestrator-client-1.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-orchestrator-client
-Version: 1.5.2
+Version: 1.6.0b1
 Summary: Fabric Orchestrator API
 Keywords: Swagger,Fabric Orchestrator API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

