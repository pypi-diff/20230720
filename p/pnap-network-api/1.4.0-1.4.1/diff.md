# Comparing `tmp/pnap-network-api-1.4.0.tar.gz` & `tmp/pnap-network-api-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-network-api-1.4.0.tar", last modified: Tue Apr 25 13:57:58 2023, max compression
+gzip compressed data, was "dist/pnap-network-api-1.4.1.tar", last modified: Thu Jul 20 10:04:56 2023, max compression
```

## Comparing `pnap-network-api-1.4.0.tar` & `pnap-network-api-1.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     9947 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9947 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1561 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/api/
--rw-r--r--   0 runner    (1001) docker     (122)    39925 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/api/public_networks_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28150 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/api/private_networks_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    15039 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/apis/
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    83362 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/model/
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12773 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network_modify.py
--rw-r--r--   0 runner    (1001) docker     (122)    12582 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network_membership.py
--rw-r--r--   0 runner    (1001) docker     (122)    14730 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/private_network_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    16462 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/private_network.py
--rw-r--r--   0 runner    (1001) docker     (122)    12570 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (122)    15699 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    12941 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/network_membership.py
--rw-r--r--   0 runner    (1001) docker     (122)    12257 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (122)    13310 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/private_network_modify.py
--rw-r--r--   0 runner    (1001) docker     (122)    12530 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/private_network_server.py
--rw-r--r--   0 runner    (1001) docker     (122)    17325 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    40261 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)    12570 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12773 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/public_network_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13310 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/private_network_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14730 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/private_network_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15699 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/public_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12530 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/private_network_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12941 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/network_membership.py
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16462 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12257 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/public_network_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12582 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/public_network_membership.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model/public_network_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40261 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)    39925 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/api/public_networks_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28150 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/api/private_networks_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15039 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83362 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17325 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1561 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/pnap_network_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-20 10:04:42.000000 pnap-network-api-1.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9947 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9947 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-20 10:04:56.000000 pnap-network-api-1.4.1/pnap_network_api.egg-info/SOURCES.txt
```

### Comparing `pnap-network-api-1.4.0/PKG-INFO` & `pnap-network-api-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-network-api
-Version: 1.4.0
+Version: 1.4.1
 Summary: Networks API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-network-api Version: 1.4.0 Summary: Networks
+Metadata-Version: 2.1 Name: pnap-network-api Version: 1.4.1 Summary: Networks
 API Home-page: https://phoenixnap.com/bare-metal-cloud Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com License: Apache 2.0 Project-URL:
 Repository, https://github.com/phoenixnap/python-sdk-bmc Description: # pnap-
 network-api Create, list, edit and delete public/private networks with the
 Network API. Use public networks to place multiple servers on the same network
 or VLAN. Assign new servers with IP addresses from the same CIDR range. Use
 private networks to avoid unnecessary egress data charges. Model your networks
```

### Comparing `pnap-network-api-1.4.0/README.md` & `pnap-network-api-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api.egg-info/PKG-INFO` & `pnap-network-api-1.4.1/pnap_network_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-network-api
-Version: 1.4.0
+Version: 1.4.1
 Summary: Networks API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-network-api Version: 1.4.0 Summary: Networks
+Metadata-Version: 2.1 Name: pnap-network-api Version: 1.4.1 Summary: Networks
 API Home-page: https://phoenixnap.com/bare-metal-cloud Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com License: Apache 2.0 Project-URL:
 Repository, https://github.com/phoenixnap/python-sdk-bmc Description: # pnap-
 network-api Create, list, edit and delete public/private networks with the
 Network API. Use public networks to place multiple servers on the same network
 or VLAN. Assign new servers with IP addresses from the same CIDR range. Use
 private networks to avoid unnecessary egress data charges. Model your networks
```

### Comparing `pnap-network-api-1.4.0/pnap_network_api.egg-info/SOURCES.txt` & `pnap-network-api-1.4.1/pnap_network_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/models/__init__.py` & `pnap-network-api-1.4.1/pnap_network_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/__init__.py` & `pnap-network-api-1.4.1/pnap_network_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/api/public_networks_api.py` & `pnap-network-api-1.4.1/pnap_network_api/api/public_networks_api.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/api/private_networks_api.py` & `pnap-network-api-1.4.1/pnap_network_api/api/private_networks_api.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/rest.py` & `pnap-network-api-1.4.1/pnap_network_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/apis/__init__.py` & `pnap-network-api-1.4.1/pnap_network_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model_utils.py` & `pnap-network-api-1.4.1/pnap_network_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/exceptions.py` & `pnap-network-api-1.4.1/pnap_network_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/public_network_modify.py` & `pnap-network-api-1.4.1/pnap_network_api/model/public_network_modify.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/public_network_membership.py` & `pnap-network-api-1.4.1/pnap_network_api/model/public_network_membership.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/private_network_create.py` & `pnap-network-api-1.4.1/pnap_network_api/model/private_network_create.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/private_network.py` & `pnap-network-api-1.4.1/pnap_network_api/model/private_network.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/error.py` & `pnap-network-api-1.4.1/pnap_network_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/public_network.py` & `pnap-network-api-1.4.1/pnap_network_api/model/public_network.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/public_network_create.py` & `pnap-network-api-1.4.1/pnap_network_api/model/public_network_create.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/network_membership.py` & `pnap-network-api-1.4.1/pnap_network_api/model/network_membership.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/public_network_ip_block.py` & `pnap-network-api-1.4.1/pnap_network_api/model/public_network_ip_block.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/private_network_modify.py` & `pnap-network-api-1.4.1/pnap_network_api/model/private_network_modify.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/model/private_network_server.py` & `pnap-network-api-1.4.1/pnap_network_api/model/private_network_server.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/configuration.py` & `pnap-network-api-1.4.1/pnap_network_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/pnap_network_api/api_client.py` & `pnap-network-api-1.4.1/pnap_network_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.4.0/setup.py` & `pnap-network-api-1.4.1/setup.py`

 * *Files identical despite different names*

