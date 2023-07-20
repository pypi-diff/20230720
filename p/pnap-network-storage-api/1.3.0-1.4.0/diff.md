# Comparing `tmp/pnap-network-storage-api-1.3.0.tar.gz` & `tmp/pnap-network-storage-api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-network-storage-api-1.3.0.tar", last modified: Tue Apr 25 13:58:00 2023, max compression
+gzip compressed data, was "dist/pnap-network-storage-api-1.4.0.tar", last modified: Thu Jul 20 10:04:58 2023, max compression
```

## Comparing `pnap-network-storage-api-1.3.0.tar` & `pnap-network-storage-api-1.4.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10208 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/api/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    55925 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/api/storage_networks_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    14678 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/apis/
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    83001 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/
--rw-r--r--   0 runner    (1001) docker     (122)    12938 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    12087 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    12723 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/status.py
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13696 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    12920 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)    12938 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    12217 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (122)    13390 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_volume_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    12026 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    14739 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume.py
--rw-r--r--   0 runner    (1001) docker     (122)    13559 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    14298 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network.py
--rw-r--r--   0 runner    (1001) docker     (122)    12087 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    12333 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    16994 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    39932 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10208 2023-04-25 13:57:59.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:57:59.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-25 13:57:59.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:57:59.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)    12938 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/nfs_permissions_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13186 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/tag_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12217 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12938 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/nfs_permissions_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12026 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12087 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/permissions_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15130 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/volume.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14007 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/storage_network_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12087 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/permissions_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12920 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/nfs_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12975 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/tag_assignment_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12333 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/storage_network_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13696 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/volume_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14543 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/volume_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14191 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/storage_network_volume_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14298 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/storage_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12723 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39932 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)    62396 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/api/storage_networks_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14678 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83001 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16994 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8728 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-07-20 10:04:42.000000 pnap-network-storage-api-1.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10722 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    10722 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-20 10:04:58.000000 pnap-network-storage-api-1.4.0/pnap_network_storage_api.egg-info/SOURCES.txt
```

### Comparing `pnap-network-storage-api-1.3.0/PKG-INFO` & `pnap-network-storage-api-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-network-storage-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Network Storage API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-storage-api
@@ -65,14 +65,15 @@
         import pnap_network_storage_api
         from pprint import pprint
         from pnap_network_storage_api.api import storage_networks_api
         from pnap_network_storage_api.model.error import Error
         from pnap_network_storage_api.model.storage_network import StorageNetwork
         from pnap_network_storage_api.model.storage_network_create import StorageNetworkCreate
         from pnap_network_storage_api.model.storage_network_update import StorageNetworkUpdate
+        from pnap_network_storage_api.model.tag_assignment_request import TagAssignmentRequest
         from pnap_network_storage_api.model.volume import Volume
         from pnap_network_storage_api.model.volume_create import VolumeCreate
         from pnap_network_storage_api.model.volume_update import VolumeUpdate
         # Defining the host is optional and defaults to https://api.phoenixnap.com/network-storage/v1
         # See configuration.py for a list of all supported configuration parameters.
         configuration = pnap_network_storage_api.Configuration(
             host = "https://api.phoenixnap.com/network-storage/v1"
@@ -134,14 +135,15 @@
         *StorageNetworksApi* | [**storage_networks_id_patch**](docs/StorageNetworksApi.md#storage_networks_id_patch) | **PATCH** /storage-networks/{storageNetworkId} | Update storage network details.
         *StorageNetworksApi* | [**storage_networks_post**](docs/StorageNetworksApi.md#storage_networks_post) | **POST** /storage-networks | Create a storage network and volume.
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_get**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_get) | **GET** /storage-networks/{storageNetworkId}/volumes | Display one or more volumes belonging to a storage network.
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_post**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_post) | **POST** /storage-networks/{storageNetworkId}/volumes | Create a volume belonging to a storage network.
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_delete**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_delete) | **DELETE** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Delete a Storage Network&#39;s Volume
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_get**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_get) | **GET** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Get a storage network&#39;s volume details.
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch) | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a storage network&#39;s volume details.
+        *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_tags_put**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_tags_put) | **PUT** /storage-networks/{storageNetworkId}/volumes/{volumeId}/tags | Overwrites tags assigned for the volume.
         
         
         ## Documentation For Models
         
          - [Error](docs/Error.md)
          - [NfsPermissions](docs/NfsPermissions.md)
          - [NfsPermissionsCreate](docs/NfsPermissionsCreate.md)
@@ -150,14 +152,16 @@
          - [PermissionsCreate](docs/PermissionsCreate.md)
          - [PermissionsUpdate](docs/PermissionsUpdate.md)
          - [Status](docs/Status.md)
          - [StorageNetwork](docs/StorageNetwork.md)
          - [StorageNetworkCreate](docs/StorageNetworkCreate.md)
          - [StorageNetworkUpdate](docs/StorageNetworkUpdate.md)
          - [StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md)
+         - [TagAssignment](docs/TagAssignment.md)
+         - [TagAssignmentRequest](docs/TagAssignmentRequest.md)
          - [Volume](docs/Volume.md)
          - [VolumeCreate](docs/VolumeCreate.md)
          - [VolumeUpdate](docs/VolumeUpdate.md)
         
         
         ## Documentation For Authorization
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-network-storage-api Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: pnap-network-storage-api Version: 1.4.0 Summary:
 Network Storage API Home-page: https://phoenixnap.com/bare-metal-cloud Author:
 PhoenixNAP Team Author-email: support@phoenixnap.com License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-storage-api Create, list, edit, and delete storage
 networks with the Network Storage API. Use storage networks to expand storage
 capacity on a private network.
  Knowledge base articles to help you can be found here
@@ -21,50 +21,51 @@
 procedure](#installation--usage) and then run the following: ```python import
 time import pnap_network_storage_api from pprint import pprint from
 pnap_network_storage_api.api import storage_networks_api from
 pnap_network_storage_api.model.error import Error from
 pnap_network_storage_api.model.storage_network import StorageNetwork from
 pnap_network_storage_api.model.storage_network_create import
 StorageNetworkCreate from pnap_network_storage_api.model.storage_network_update
-import StorageNetworkUpdate from pnap_network_storage_api.model.volume import
-Volume from pnap_network_storage_api.model.volume_create import VolumeCreate
-from pnap_network_storage_api.model.volume_update import VolumeUpdate #
-Defining the host is optional and defaults to https://api.phoenixnap.com/
-network-storage/v1 # See configuration.py for a list of all supported
-configuration parameters. configuration =
+import StorageNetworkUpdate from
+pnap_network_storage_api.model.tag_assignment_request import
+TagAssignmentRequest from pnap_network_storage_api.model.volume import Volume
+from pnap_network_storage_api.model.volume_create import VolumeCreate from
+pnap_network_storage_api.model.volume_update import VolumeUpdate # Defining the
+host is optional and defaults to https://api.phoenixnap.com/network-storage/v1
+# See configuration.py for a list of all supported configuration parameters.
+configuration = pnap_network_storage_api.Configuration( host = "https://
+api.phoenixnap.com/network-storage/v1" ) # The client must configure the
+authentication and authorization parameters # in accordance with the API server
+security policy. # Examples for each auth method are provided below, use the
+example that # satisfies your auth use case. # Configure OAuth2 access token
+for authorization: OAuth2 configuration =
 pnap_network_storage_api.Configuration( host = "https://api.phoenixnap.com/
-network-storage/v1" ) # The client must configure the authentication and
-authorization parameters # in accordance with the API server security policy. #
-Examples for each auth method are provided below, use the example that #
-satisfies your auth use case. # Configure OAuth2 access token for
-authorization: OAuth2 configuration = pnap_network_storage_api.Configuration
-( host = "https://api.phoenixnap.com/network-storage/v1" )
-configuration.access_token = 'YOUR_ACCESS_TOKEN' # Enter a context with an
-instance of the API client with pnap_network_storage_api.ApiClient
-(configuration) as api_client: # Create an instance of the API class
-api_instance = storage_networks_api.StorageNetworksApi(api_client) location =
-"PHX" # str | If present will filter the result by the given location.
-(optional) try: # List all storage networks. api_response =
-api_instance.storage_networks_get(location=location) pprint(api_response)
-except pnap_network_storage_api.ApiException as e: print("Exception when
-calling StorageNetworksApi->storage_networks_get: %s\n" % e) ``` To generate a
-token using the [python-keycloak](https://pypi.org/project/python-keycloak/
-) library: ```python from keycloak import KeycloakOpenID clientId =
-"YOUR_CLIENT_ID" clientSecret = "YOUR_CLIENT_SECRET" serverUrl = "https://
-auth.phoenixnap.com/auth/" realmName = "BMC" grantType = "client_credentials"
-keycloakOpenId = KeycloakOpenID(server_url=serverUrl, realm_name=realmName,
-client_id=clientId, client_secret_key=clientSecret) ACCESS_TOKEN =
-keycloakOpenId.token(grant_type=grantType)['access_token'] ``` ## Documentation
-for API Endpoints All URIs are relative to *https://api.phoenixnap.com/network-
-storage/v1* Class | Method | HTTP request | Description ------------ | --------
------ | ------------- | ------------- *StorageNetworksApi* |
-[**storage_networks_get**](docs/StorageNetworksApi.md#storage_networks_get) |
-**GET** /storage-networks | List all storage networks. *StorageNetworksApi* |
-[**storage_networks_id_delete**](docs/
-StorageNetworksApi.md#storage_networks_id_delete) | **DELETE** /storage-
+network-storage/v1" ) configuration.access_token = 'YOUR_ACCESS_TOKEN' # Enter
+a context with an instance of the API client with
+pnap_network_storage_api.ApiClient(configuration) as api_client: # Create an
+instance of the API class api_instance =
+storage_networks_api.StorageNetworksApi(api_client) location = "PHX" # str | If
+present will filter the result by the given location. (optional) try: # List
+all storage networks. api_response = api_instance.storage_networks_get
+(location=location) pprint(api_response) except
+pnap_network_storage_api.ApiException as e: print("Exception when calling
+StorageNetworksApi->storage_networks_get: %s\n" % e) ``` To generate a token
+using the [python-keycloak](https://pypi.org/project/python-keycloak/) library:
+```python from keycloak import KeycloakOpenID clientId = "YOUR_CLIENT_ID"
+clientSecret = "YOUR_CLIENT_SECRET" serverUrl = "https://auth.phoenixnap.com/
+auth/" realmName = "BMC" grantType = "client_credentials" keycloakOpenId =
+KeycloakOpenID(server_url=serverUrl, realm_name=realmName, client_id=clientId,
+client_secret_key=clientSecret) ACCESS_TOKEN = keycloakOpenId.token
+(grant_type=grantType)['access_token'] ``` ## Documentation for API Endpoints
+All URIs are relative to *https://api.phoenixnap.com/network-storage/v1* Class
+| Method | HTTP request | Description ------------ | ------------- | ----------
+--- | ------------- *StorageNetworksApi* | [**storage_networks_get**](docs/
+StorageNetworksApi.md#storage_networks_get) | **GET** /storage-networks | List
+all storage networks. *StorageNetworksApi* | [**storage_networks_id_delete**]
+(docs/StorageNetworksApi.md#storage_networks_id_delete) | **DELETE** /storage-
 networks/{storageNetworkId} | Delete a storage network and its volume.
 *StorageNetworksApi* | [**storage_networks_id_get**](docs/
 StorageNetworksApi.md#storage_networks_id_get) | **GET** /storage-networks/
 {storageNetworkId} | Get storage network details. *StorageNetworksApi* |
 [**storage_networks_id_patch**](docs/
 StorageNetworksApi.md#storage_networks_id_patch) | **PATCH** /storage-networks/
 {storageNetworkId} | Update storage network details. *StorageNetworksApi* |
@@ -85,33 +86,39 @@
 [**storage_networks_storage_network_id_volumes_volume_id_get**](docs/
 StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_get)
 | **GET** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Get a
 storage network's volume details. *StorageNetworksApi* |
 [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/
 StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch)
 | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a
-storage network's volume details. ## Documentation For Models - [Error](docs/
-Error.md) - [NfsPermissions](docs/NfsPermissions.md) - [NfsPermissionsCreate]
-(docs/NfsPermissionsCreate.md) - [NfsPermissionsUpdate](docs/
-NfsPermissionsUpdate.md) - [Permissions](docs/Permissions.md) -
+storage network's volume details. *StorageNetworksApi* |
+[**storage_networks_storage_network_id_volumes_volume_id_tags_put**](docs/
+StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_tags_put)
+| **PUT** /storage-networks/{storageNetworkId}/volumes/{volumeId}/tags |
+Overwrites tags assigned for the volume. ## Documentation For Models - [Error]
+(docs/Error.md) - [NfsPermissions](docs/NfsPermissions.md) -
+[NfsPermissionsCreate](docs/NfsPermissionsCreate.md) - [NfsPermissionsUpdate]
+(docs/NfsPermissionsUpdate.md) - [Permissions](docs/Permissions.md) -
 [PermissionsCreate](docs/PermissionsCreate.md) - [PermissionsUpdate](docs/
 PermissionsUpdate.md) - [Status](docs/Status.md) - [StorageNetwork](docs/
 StorageNetwork.md) - [StorageNetworkCreate](docs/StorageNetworkCreate.md) -
 [StorageNetworkUpdate](docs/StorageNetworkUpdate.md) -
-[StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md) - [Volume]
-(docs/Volume.md) - [VolumeCreate](docs/VolumeCreate.md) - [VolumeUpdate](docs/
-VolumeUpdate.md) ## Documentation For Authorization ## OAuth2 - **Type**: OAuth
-- **Flow**: application - **Authorization URL**: - **Scopes**: -
-**networkstorage**: Grants full access to Network Storage API. -
-**networkstorage.read**: Grants read only access to Network Storage API. ##
-Author support@phoenixnap.com ## Notes for Large OpenAPI documents If the
-OpenAPI document is large, imports in pnap_network_storage_api.apis and
-pnap_network_storage_api.models may fail with a RecursionError indicating the
-maximum recursion limit has been exceeded. In that case, there are a couple of
-solutions: Solution 1: Use specific imports for apis and models like: - `from
-pnap_network_storage_api.api.default_api import DefaultApi` - `from
-pnap_network_storage_api.model.pet import Pet` Solution 2: Before importing the
-package, adjust the maximum recursion limit as shown below: ``` import sys
-sys.setrecursionlimit(1500) import pnap_network_storage_api from
-pnap_network_storage_api.apis import * from pnap_network_storage_api.models
-import * ``` Keywords: OpenAPI,OpenAPI-Generator,Network Storage API Platform:
-UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/markdown
+[StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md) -
+[TagAssignment](docs/TagAssignment.md) - [TagAssignmentRequest](docs/
+TagAssignmentRequest.md) - [Volume](docs/Volume.md) - [VolumeCreate](docs/
+VolumeCreate.md) - [VolumeUpdate](docs/VolumeUpdate.md) ## Documentation For
+Authorization ## OAuth2 - **Type**: OAuth - **Flow**: application -
+**Authorization URL**: - **Scopes**: - **networkstorage**: Grants full access
+to Network Storage API. - **networkstorage.read**: Grants read only access to
+Network Storage API. ## Author support@phoenixnap.com ## Notes for Large
+OpenAPI documents If the OpenAPI document is large, imports in
+pnap_network_storage_api.apis and pnap_network_storage_api.models may fail with
+a RecursionError indicating the maximum recursion limit has been exceeded. In
+that case, there are a couple of solutions: Solution 1: Use specific imports
+for apis and models like: - `from pnap_network_storage_api.api.default_api
+import DefaultApi` - `from pnap_network_storage_api.model.pet import Pet`
+Solution 2: Before importing the package, adjust the maximum recursion limit as
+shown below: ``` import sys sys.setrecursionlimit(1500) import
+pnap_network_storage_api from pnap_network_storage_api.apis import * from
+pnap_network_storage_api.models import * ``` Keywords: OpenAPI,OpenAPI-
+Generator,Network Storage API Platform: UNKNOWN Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `pnap-network-storage-api-1.3.0/README.md` & `pnap-network-storage-api-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 import pnap_network_storage_api
 from pprint import pprint
 from pnap_network_storage_api.api import storage_networks_api
 from pnap_network_storage_api.model.error import Error
 from pnap_network_storage_api.model.storage_network import StorageNetwork
 from pnap_network_storage_api.model.storage_network_create import StorageNetworkCreate
 from pnap_network_storage_api.model.storage_network_update import StorageNetworkUpdate
+from pnap_network_storage_api.model.tag_assignment_request import TagAssignmentRequest
 from pnap_network_storage_api.model.volume import Volume
 from pnap_network_storage_api.model.volume_create import VolumeCreate
 from pnap_network_storage_api.model.volume_update import VolumeUpdate
 # Defining the host is optional and defaults to https://api.phoenixnap.com/network-storage/v1
 # See configuration.py for a list of all supported configuration parameters.
 configuration = pnap_network_storage_api.Configuration(
     host = "https://api.phoenixnap.com/network-storage/v1"
@@ -125,14 +126,15 @@
 *StorageNetworksApi* | [**storage_networks_id_patch**](docs/StorageNetworksApi.md#storage_networks_id_patch) | **PATCH** /storage-networks/{storageNetworkId} | Update storage network details.
 *StorageNetworksApi* | [**storage_networks_post**](docs/StorageNetworksApi.md#storage_networks_post) | **POST** /storage-networks | Create a storage network and volume.
 *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_get**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_get) | **GET** /storage-networks/{storageNetworkId}/volumes | Display one or more volumes belonging to a storage network.
 *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_post**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_post) | **POST** /storage-networks/{storageNetworkId}/volumes | Create a volume belonging to a storage network.
 *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_delete**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_delete) | **DELETE** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Delete a Storage Network&#39;s Volume
 *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_get**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_get) | **GET** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Get a storage network&#39;s volume details.
 *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch) | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a storage network&#39;s volume details.
+*StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_tags_put**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_tags_put) | **PUT** /storage-networks/{storageNetworkId}/volumes/{volumeId}/tags | Overwrites tags assigned for the volume.
 
 
 ## Documentation For Models
 
  - [Error](docs/Error.md)
  - [NfsPermissions](docs/NfsPermissions.md)
  - [NfsPermissionsCreate](docs/NfsPermissionsCreate.md)
@@ -141,14 +143,16 @@
  - [PermissionsCreate](docs/PermissionsCreate.md)
  - [PermissionsUpdate](docs/PermissionsUpdate.md)
  - [Status](docs/Status.md)
  - [StorageNetwork](docs/StorageNetwork.md)
  - [StorageNetworkCreate](docs/StorageNetworkCreate.md)
  - [StorageNetworkUpdate](docs/StorageNetworkUpdate.md)
  - [StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md)
+ - [TagAssignment](docs/TagAssignment.md)
+ - [TagAssignmentRequest](docs/TagAssignmentRequest.md)
  - [Volume](docs/Volume.md)
  - [VolumeCreate](docs/VolumeCreate.md)
  - [VolumeUpdate](docs/VolumeUpdate.md)
 
 
 ## Documentation For Authorization
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/models/__init__.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,10 +17,12 @@
 from pnap_network_storage_api.model.permissions_create import PermissionsCreate
 from pnap_network_storage_api.model.permissions_update import PermissionsUpdate
 from pnap_network_storage_api.model.status import Status
 from pnap_network_storage_api.model.storage_network import StorageNetwork
 from pnap_network_storage_api.model.storage_network_create import StorageNetworkCreate
 from pnap_network_storage_api.model.storage_network_update import StorageNetworkUpdate
 from pnap_network_storage_api.model.storage_network_volume_create import StorageNetworkVolumeCreate
+from pnap_network_storage_api.model.tag_assignment import TagAssignment
+from pnap_network_storage_api.model.tag_assignment_request import TagAssignmentRequest
 from pnap_network_storage_api.model.volume import Volume
 from pnap_network_storage_api.model.volume_create import VolumeCreate
 from pnap_network_storage_api.model.volume_update import VolumeUpdate
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/__init__.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/api/storage_networks_api.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/api/storage_networks_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     none_type,
     validate_and_convert_types
 )
 from pnap_network_storage_api.model.error import Error
 from pnap_network_storage_api.model.storage_network import StorageNetwork
 from pnap_network_storage_api.model.storage_network_create import StorageNetworkCreate
 from pnap_network_storage_api.model.storage_network_update import StorageNetworkUpdate
+from pnap_network_storage_api.model.tag_assignment_request import TagAssignmentRequest
 from pnap_network_storage_api.model.volume import Volume
 from pnap_network_storage_api.model.volume_create import VolumeCreate
 from pnap_network_storage_api.model.volume_update import VolumeUpdate
 
 
 class StorageNetworksApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -310,14 +311,15 @@
                 'operation_id': 'storage_networks_storage_network_id_volumes_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'storage_network_id',
+                    'tag',
                 ],
                 'required': [
                     'storage_network_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -329,22 +331,27 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'storage_network_id':
                         (str,),
+                    'tag':
+                        ([str],),
                 },
                 'attribute_map': {
                     'storage_network_id': 'storageNetworkId',
+                    'tag': 'tag',
                 },
                 'location_map': {
                     'storage_network_id': 'path',
+                    'tag': 'query',
                 },
                 'collection_format_map': {
+                    'tag': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
@@ -581,14 +588,77 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.storage_networks_storage_network_id_volumes_volume_id_tags_put_endpoint = _Endpoint(
+            settings={
+                'response_type': (Volume,),
+                'auth': [
+                    'OAuth2'
+                ],
+                'endpoint_path': '/storage-networks/{storageNetworkId}/volumes/{volumeId}/tags',
+                'operation_id': 'storage_networks_storage_network_id_volumes_volume_id_tags_put',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'storage_network_id',
+                    'volume_id',
+                    'tag_assignment_request',
+                ],
+                'required': [
+                    'storage_network_id',
+                    'volume_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'storage_network_id':
+                        (str,),
+                    'volume_id':
+                        (str,),
+                    'tag_assignment_request':
+                        ([TagAssignmentRequest],),
+                },
+                'attribute_map': {
+                    'storage_network_id': 'storageNetworkId',
+                    'volume_id': 'volumeId',
+                },
+                'location_map': {
+                    'storage_network_id': 'path',
+                    'volume_id': 'path',
+                    'tag_assignment_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
 
     def storage_networks_get(
         self,
         **kwargs
     ):
         """List all storage networks.  # noqa: E501
 
@@ -1008,14 +1078,15 @@
         >>> thread = api.storage_networks_storage_network_id_volumes_get(storage_network_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             storage_network_id (str): ID of storage network.
 
         Keyword Args:
+            tag ([str]): A list of query parameters related to tags in the form of tagName.tagValue. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1419,7 +1490,95 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['storage_network_id'] = \
             storage_network_id
         kwargs['volume_id'] = \
             volume_id
         return self.storage_networks_storage_network_id_volumes_volume_id_patch_endpoint.call_with_http_info(**kwargs)
 
+    def storage_networks_storage_network_id_volumes_volume_id_tags_put(
+        self,
+        storage_network_id,
+        volume_id,
+        **kwargs
+    ):
+        """Overwrites tags assigned for the volume.  # noqa: E501
+
+        Overwrites tags assigned for the volume.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.storage_networks_storage_network_id_volumes_volume_id_tags_put(storage_network_id, volume_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            storage_network_id (str): ID of storage network.
+            volume_id (str): ID of volume.
+
+        Keyword Args:
+            tag_assignment_request ([TagAssignmentRequest]): Tags to assign to the volume.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Volume
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['storage_network_id'] = \
+            storage_network_id
+        kwargs['volume_id'] = \
+            volume_id
+        return self.storage_networks_storage_network_id_volumes_volume_id_tags_put_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/rest.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/apis/__init__.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model_utils.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/exceptions.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions_update.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/nfs_permissions_update.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions_update.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/permissions_update.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/status.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/status.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume_update.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/volume_update.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/nfs_permissions.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions_create.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/nfs_permissions_create.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/error.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_volume_create.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/storage_network_update.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pnap_network_storage_api.exceptions import ApiAttributeError
 
 
 
-class StorageNetworkVolumeCreate(ModelNormal):
+class StorageNetworkUpdate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -59,27 +59,17 @@
     }
 
     validations = {
         ('name',): {
             'max_length': 100,
             'min_length': 1,
         },
-        ('capacity_in_gb',): {
-            'inclusive_minimum': 1000,
-        },
         ('description',): {
             'max_length': 250,
         },
-        ('path_suffix',): {
-            'max_length': 27,
-            'min_length': 0,
-            'regex': {
-                'pattern': r'^(\/[\w-]+)+$|^$',  # noqa: E501
-            },
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -96,44 +86,36 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
-            'capacity_in_gb': (int,),  # noqa: E501
             'description': (str,),  # noqa: E501
-            'path_suffix': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
-        'capacity_in_gb': 'capacityInGb',  # noqa: E501
         'description': 'description',  # noqa: E501
-        'path_suffix': 'pathSuffix',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, capacity_in_gb, *args, **kwargs):  # noqa: E501
-        """StorageNetworkVolumeCreate - a model defined in OpenAPI
-
-        Args:
-            name (str): Volume friendly name.
-            capacity_in_gb (int): Capacity of Volume in GB. Currently only whole numbers and multiples of 1000GB are supported.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """StorageNetworkUpdate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -158,16 +140,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str): Volume description.. [optional]  # noqa: E501
-            path_suffix (str): Last part of volume's path.. [optional]  # noqa: E501
+            name (str): Storage network friendly name.. [optional]  # noqa: E501
+            description (str): Storage network description.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,16 +173,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.capacity_in_gb = capacity_in_gb
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -213,20 +193,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, capacity_in_gb, *args, **kwargs):  # noqa: E501
-        """StorageNetworkVolumeCreate - a model defined in OpenAPI
-
-        Args:
-            name (str): Volume friendly name.
-            capacity_in_gb (int): Capacity of Volume in GB. Currently only whole numbers and multiples of 1000GB are supported.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """StorageNetworkUpdate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -251,16 +227,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str): Volume description.. [optional]  # noqa: E501
-            path_suffix (str): Last part of volume's path.. [optional]  # noqa: E501
+            name (str): Storage network friendly name.. [optional]  # noqa: E501
+            description (str): Storage network description.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -282,16 +258,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.capacity_in_gb = capacity_in_gb
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/permissions.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume_create.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/volume_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     OpenApiModel
 )
 from pnap_network_storage_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from pnap_network_storage_api.model.permissions_create import PermissionsCreate
+    from pnap_network_storage_api.model.tag_assignment_request import TagAssignmentRequest
     globals()['PermissionsCreate'] = PermissionsCreate
+    globals()['TagAssignmentRequest'] = TagAssignmentRequest
 
 
 class VolumeCreate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -106,27 +108,29 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'capacity_in_gb': (int,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'path_suffix': (str,),  # noqa: E501
             'permissions': (PermissionsCreate,),  # noqa: E501
+            'tags': ([TagAssignmentRequest],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'capacity_in_gb': 'capacityInGb',  # noqa: E501
         'description': 'description',  # noqa: E501
         'path_suffix': 'pathSuffix',  # noqa: E501
         'permissions': 'permissions',  # noqa: E501
+        'tags': 'tags',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -169,14 +173,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): Volume description.. [optional]  # noqa: E501
             path_suffix (str): Last part of volume's path.. [optional]  # noqa: E501
             permissions (PermissionsCreate): [optional]  # noqa: E501
+            tags ([TagAssignmentRequest]): Tags to set to the resource. To create a new tag or list all the existing tags that you can use, refer to [Tags API](https://developers.phoenixnap.com/docs/tags/1/overview).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -263,14 +268,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): Volume description.. [optional]  # noqa: E501
             path_suffix (str): Last part of volume's path.. [optional]  # noqa: E501
             permissions (PermissionsCreate): [optional]  # noqa: E501
+            tags ([TagAssignmentRequest]): Tags to set to the resource. To create a new tag or list all the existing tags that you can use, refer to [Tags API](https://developers.phoenixnap.com/docs/tags/1/overview).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 )
 from pnap_network_storage_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from pnap_network_storage_api.model.permissions import Permissions
     from pnap_network_storage_api.model.status import Status
+    from pnap_network_storage_api.model.tag_assignment import TagAssignment
     globals()['Permissions'] = Permissions
     globals()['Status'] = Status
+    globals()['TagAssignment'] = TagAssignment
 
 
 class Volume(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -97,14 +99,15 @@
             'path_suffix': (str,),  # noqa: E501
             'capacity_in_gb': (int,),  # noqa: E501
             'used_capacity_in_gb': (int,),  # noqa: E501
             'protocol': (str,),  # noqa: E501
             'status': (Status,),  # noqa: E501
             'created_on': (datetime,),  # noqa: E501
             'permissions': (Permissions,),  # noqa: E501
+            'tags': ([TagAssignment],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -116,14 +119,15 @@
         'path_suffix': 'pathSuffix',  # noqa: E501
         'capacity_in_gb': 'capacityInGb',  # noqa: E501
         'used_capacity_in_gb': 'usedCapacityInGb',  # noqa: E501
         'protocol': 'protocol',  # noqa: E501
         'status': 'status',  # noqa: E501
         'created_on': 'createdOn',  # noqa: E501
         'permissions': 'permissions',  # noqa: E501
+        'tags': 'tags',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -170,14 +174,15 @@
             path_suffix (str): Last part of volume's path.. [optional]  # noqa: E501
             capacity_in_gb (int): Maximum capacity in GB.. [optional]  # noqa: E501
             used_capacity_in_gb (int): Used capacity in GB, updated periodically.. [optional]  # noqa: E501
             protocol (str): File system protocol. Currently this field should be set to `NFS`.. [optional]  # noqa: E501
             status (Status): [optional]  # noqa: E501
             created_on (datetime): [optional]  # noqa: E501
             permissions (Permissions): [optional]  # noqa: E501
+            tags ([TagAssignment]): The tags assigned if any.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -266,14 +271,15 @@
             path_suffix (str): Last part of volume's path.. [optional]  # noqa: E501
             capacity_in_gb (int): Maximum capacity in GB.. [optional]  # noqa: E501
             used_capacity_in_gb (int): Used capacity in GB, updated periodically.. [optional]  # noqa: E501
             protocol (str): File system protocol. Currently this field should be set to `NFS`.. [optional]  # noqa: E501
             status (Status): [optional]  # noqa: E501
             created_on (datetime): [optional]  # noqa: E501
             permissions (Permissions): [optional]  # noqa: E501
+            tags ([TagAssignment]): The tags assigned if any.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_create.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/storage_network_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         ('volumes',): {
             'max_items': 1,
             'min_items': 1,
         },
         ('description',): {
             'max_length': 250,
         },
+        ('client_vlan',): {
+            'inclusive_maximum': 4094,
+            'inclusive_minimum': 2,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -99,26 +103,28 @@
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'location': (str,),  # noqa: E501
             'volumes': ([StorageNetworkVolumeCreate],),  # noqa: E501
             'description': (str,),  # noqa: E501
+            'client_vlan': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'location': 'location',  # noqa: E501
         'volumes': 'volumes',  # noqa: E501
         'description': 'description',  # noqa: E501
+        'client_vlan': 'clientVlan',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -160,14 +166,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): Storage network description.. [optional]  # noqa: E501
+            client_vlan (int): Custom Client VLAN that the Storage Network will be set to.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -254,14 +261,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): Storage network description.. [optional]  # noqa: E501
+            client_vlan (int): Custom Client VLAN that the Storage Network will be set to.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/storage_network.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions_create.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/permissions_create.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_update.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/model/tag_assignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pnap_network_storage_api.exceptions import ApiAttributeError
 
 
 
-class StorageNetworkUpdate(ModelNormal):
+class TagAssignment(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,24 +52,21 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('created_by',): {
+            'USER': "USER",
+            'SYSTEM': "SYSTEM",
+        },
     }
 
     validations = {
-        ('name',): {
-            'max_length': 100,
-            'min_length': 1,
-        },
-        ('description',): {
-            'max_length': 250,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -85,37 +82,48 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
+            'is_billing_tag': (bool,),  # noqa: E501
+            'value': (str,),  # noqa: E501
+            'created_by': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'description': 'description',  # noqa: E501
+        'is_billing_tag': 'isBillingTag',  # noqa: E501
+        'value': 'value',  # noqa: E501
+        'created_by': 'createdBy',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StorageNetworkUpdate - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, is_billing_tag, *args, **kwargs):  # noqa: E501
+        """TagAssignment - a model defined in OpenAPI
+
+        Args:
+            id (str): The unique id of the tag.
+            name (str): The name of the tag.
+            is_billing_tag (bool): Whether or not to show the tag as part of billing and invoices
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,16 +148,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): Storage network friendly name.. [optional]  # noqa: E501
-            description (str): Storage network description.. [optional]  # noqa: E501
+            value (str): The value of the tag assigned to the resource.. [optional]  # noqa: E501
+            created_by (str): Who the tag was created by.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -173,14 +181,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.name = name
+        self.is_billing_tag = is_billing_tag
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,16 +204,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """StorageNetworkUpdate - a model defined in OpenAPI
+    def __init__(self, id, name, is_billing_tag, *args, **kwargs):  # noqa: E501
+        """TagAssignment - a model defined in OpenAPI
+
+        Args:
+            id (str): The unique id of the tag.
+            name (str): The name of the tag.
+            is_billing_tag (bool): Whether or not to show the tag as part of billing and invoices
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,16 +243,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): Storage network friendly name.. [optional]  # noqa: E501
-            description (str): Storage network description.. [optional]  # noqa: E501
+            value (str): The value of the tag assigned to the resource.. [optional]  # noqa: E501
+            created_by (str): Who the tag was created by.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,14 +274,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.name = name
+        self.is_billing_tag = is_billing_tag
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/configuration.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api/api_client.py` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/PKG-INFO` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-network-storage-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Network Storage API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-storage-api
@@ -65,14 +65,15 @@
         import pnap_network_storage_api
         from pprint import pprint
         from pnap_network_storage_api.api import storage_networks_api
         from pnap_network_storage_api.model.error import Error
         from pnap_network_storage_api.model.storage_network import StorageNetwork
         from pnap_network_storage_api.model.storage_network_create import StorageNetworkCreate
         from pnap_network_storage_api.model.storage_network_update import StorageNetworkUpdate
+        from pnap_network_storage_api.model.tag_assignment_request import TagAssignmentRequest
         from pnap_network_storage_api.model.volume import Volume
         from pnap_network_storage_api.model.volume_create import VolumeCreate
         from pnap_network_storage_api.model.volume_update import VolumeUpdate
         # Defining the host is optional and defaults to https://api.phoenixnap.com/network-storage/v1
         # See configuration.py for a list of all supported configuration parameters.
         configuration = pnap_network_storage_api.Configuration(
             host = "https://api.phoenixnap.com/network-storage/v1"
@@ -134,14 +135,15 @@
         *StorageNetworksApi* | [**storage_networks_id_patch**](docs/StorageNetworksApi.md#storage_networks_id_patch) | **PATCH** /storage-networks/{storageNetworkId} | Update storage network details.
         *StorageNetworksApi* | [**storage_networks_post**](docs/StorageNetworksApi.md#storage_networks_post) | **POST** /storage-networks | Create a storage network and volume.
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_get**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_get) | **GET** /storage-networks/{storageNetworkId}/volumes | Display one or more volumes belonging to a storage network.
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_post**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_post) | **POST** /storage-networks/{storageNetworkId}/volumes | Create a volume belonging to a storage network.
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_delete**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_delete) | **DELETE** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Delete a Storage Network&#39;s Volume
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_get**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_get) | **GET** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Get a storage network&#39;s volume details.
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch) | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a storage network&#39;s volume details.
+        *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_tags_put**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_tags_put) | **PUT** /storage-networks/{storageNetworkId}/volumes/{volumeId}/tags | Overwrites tags assigned for the volume.
         
         
         ## Documentation For Models
         
          - [Error](docs/Error.md)
          - [NfsPermissions](docs/NfsPermissions.md)
          - [NfsPermissionsCreate](docs/NfsPermissionsCreate.md)
@@ -150,14 +152,16 @@
          - [PermissionsCreate](docs/PermissionsCreate.md)
          - [PermissionsUpdate](docs/PermissionsUpdate.md)
          - [Status](docs/Status.md)
          - [StorageNetwork](docs/StorageNetwork.md)
          - [StorageNetworkCreate](docs/StorageNetworkCreate.md)
          - [StorageNetworkUpdate](docs/StorageNetworkUpdate.md)
          - [StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md)
+         - [TagAssignment](docs/TagAssignment.md)
+         - [TagAssignmentRequest](docs/TagAssignmentRequest.md)
          - [Volume](docs/Volume.md)
          - [VolumeCreate](docs/VolumeCreate.md)
          - [VolumeUpdate](docs/VolumeUpdate.md)
         
         
         ## Documentation For Authorization
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-network-storage-api Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: pnap-network-storage-api Version: 1.4.0 Summary:
 Network Storage API Home-page: https://phoenixnap.com/bare-metal-cloud Author:
 PhoenixNAP Team Author-email: support@phoenixnap.com License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-storage-api Create, list, edit, and delete storage
 networks with the Network Storage API. Use storage networks to expand storage
 capacity on a private network.
  Knowledge base articles to help you can be found here
@@ -21,50 +21,51 @@
 procedure](#installation--usage) and then run the following: ```python import
 time import pnap_network_storage_api from pprint import pprint from
 pnap_network_storage_api.api import storage_networks_api from
 pnap_network_storage_api.model.error import Error from
 pnap_network_storage_api.model.storage_network import StorageNetwork from
 pnap_network_storage_api.model.storage_network_create import
 StorageNetworkCreate from pnap_network_storage_api.model.storage_network_update
-import StorageNetworkUpdate from pnap_network_storage_api.model.volume import
-Volume from pnap_network_storage_api.model.volume_create import VolumeCreate
-from pnap_network_storage_api.model.volume_update import VolumeUpdate #
-Defining the host is optional and defaults to https://api.phoenixnap.com/
-network-storage/v1 # See configuration.py for a list of all supported
-configuration parameters. configuration =
+import StorageNetworkUpdate from
+pnap_network_storage_api.model.tag_assignment_request import
+TagAssignmentRequest from pnap_network_storage_api.model.volume import Volume
+from pnap_network_storage_api.model.volume_create import VolumeCreate from
+pnap_network_storage_api.model.volume_update import VolumeUpdate # Defining the
+host is optional and defaults to https://api.phoenixnap.com/network-storage/v1
+# See configuration.py for a list of all supported configuration parameters.
+configuration = pnap_network_storage_api.Configuration( host = "https://
+api.phoenixnap.com/network-storage/v1" ) # The client must configure the
+authentication and authorization parameters # in accordance with the API server
+security policy. # Examples for each auth method are provided below, use the
+example that # satisfies your auth use case. # Configure OAuth2 access token
+for authorization: OAuth2 configuration =
 pnap_network_storage_api.Configuration( host = "https://api.phoenixnap.com/
-network-storage/v1" ) # The client must configure the authentication and
-authorization parameters # in accordance with the API server security policy. #
-Examples for each auth method are provided below, use the example that #
-satisfies your auth use case. # Configure OAuth2 access token for
-authorization: OAuth2 configuration = pnap_network_storage_api.Configuration
-( host = "https://api.phoenixnap.com/network-storage/v1" )
-configuration.access_token = 'YOUR_ACCESS_TOKEN' # Enter a context with an
-instance of the API client with pnap_network_storage_api.ApiClient
-(configuration) as api_client: # Create an instance of the API class
-api_instance = storage_networks_api.StorageNetworksApi(api_client) location =
-"PHX" # str | If present will filter the result by the given location.
-(optional) try: # List all storage networks. api_response =
-api_instance.storage_networks_get(location=location) pprint(api_response)
-except pnap_network_storage_api.ApiException as e: print("Exception when
-calling StorageNetworksApi->storage_networks_get: %s\n" % e) ``` To generate a
-token using the [python-keycloak](https://pypi.org/project/python-keycloak/
-) library: ```python from keycloak import KeycloakOpenID clientId =
-"YOUR_CLIENT_ID" clientSecret = "YOUR_CLIENT_SECRET" serverUrl = "https://
-auth.phoenixnap.com/auth/" realmName = "BMC" grantType = "client_credentials"
-keycloakOpenId = KeycloakOpenID(server_url=serverUrl, realm_name=realmName,
-client_id=clientId, client_secret_key=clientSecret) ACCESS_TOKEN =
-keycloakOpenId.token(grant_type=grantType)['access_token'] ``` ## Documentation
-for API Endpoints All URIs are relative to *https://api.phoenixnap.com/network-
-storage/v1* Class | Method | HTTP request | Description ------------ | --------
------ | ------------- | ------------- *StorageNetworksApi* |
-[**storage_networks_get**](docs/StorageNetworksApi.md#storage_networks_get) |
-**GET** /storage-networks | List all storage networks. *StorageNetworksApi* |
-[**storage_networks_id_delete**](docs/
-StorageNetworksApi.md#storage_networks_id_delete) | **DELETE** /storage-
+network-storage/v1" ) configuration.access_token = 'YOUR_ACCESS_TOKEN' # Enter
+a context with an instance of the API client with
+pnap_network_storage_api.ApiClient(configuration) as api_client: # Create an
+instance of the API class api_instance =
+storage_networks_api.StorageNetworksApi(api_client) location = "PHX" # str | If
+present will filter the result by the given location. (optional) try: # List
+all storage networks. api_response = api_instance.storage_networks_get
+(location=location) pprint(api_response) except
+pnap_network_storage_api.ApiException as e: print("Exception when calling
+StorageNetworksApi->storage_networks_get: %s\n" % e) ``` To generate a token
+using the [python-keycloak](https://pypi.org/project/python-keycloak/) library:
+```python from keycloak import KeycloakOpenID clientId = "YOUR_CLIENT_ID"
+clientSecret = "YOUR_CLIENT_SECRET" serverUrl = "https://auth.phoenixnap.com/
+auth/" realmName = "BMC" grantType = "client_credentials" keycloakOpenId =
+KeycloakOpenID(server_url=serverUrl, realm_name=realmName, client_id=clientId,
+client_secret_key=clientSecret) ACCESS_TOKEN = keycloakOpenId.token
+(grant_type=grantType)['access_token'] ``` ## Documentation for API Endpoints
+All URIs are relative to *https://api.phoenixnap.com/network-storage/v1* Class
+| Method | HTTP request | Description ------------ | ------------- | ----------
+--- | ------------- *StorageNetworksApi* | [**storage_networks_get**](docs/
+StorageNetworksApi.md#storage_networks_get) | **GET** /storage-networks | List
+all storage networks. *StorageNetworksApi* | [**storage_networks_id_delete**]
+(docs/StorageNetworksApi.md#storage_networks_id_delete) | **DELETE** /storage-
 networks/{storageNetworkId} | Delete a storage network and its volume.
 *StorageNetworksApi* | [**storage_networks_id_get**](docs/
 StorageNetworksApi.md#storage_networks_id_get) | **GET** /storage-networks/
 {storageNetworkId} | Get storage network details. *StorageNetworksApi* |
 [**storage_networks_id_patch**](docs/
 StorageNetworksApi.md#storage_networks_id_patch) | **PATCH** /storage-networks/
 {storageNetworkId} | Update storage network details. *StorageNetworksApi* |
@@ -85,33 +86,39 @@
 [**storage_networks_storage_network_id_volumes_volume_id_get**](docs/
 StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_get)
 | **GET** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Get a
 storage network's volume details. *StorageNetworksApi* |
 [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/
 StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch)
 | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a
-storage network's volume details. ## Documentation For Models - [Error](docs/
-Error.md) - [NfsPermissions](docs/NfsPermissions.md) - [NfsPermissionsCreate]
-(docs/NfsPermissionsCreate.md) - [NfsPermissionsUpdate](docs/
-NfsPermissionsUpdate.md) - [Permissions](docs/Permissions.md) -
+storage network's volume details. *StorageNetworksApi* |
+[**storage_networks_storage_network_id_volumes_volume_id_tags_put**](docs/
+StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_tags_put)
+| **PUT** /storage-networks/{storageNetworkId}/volumes/{volumeId}/tags |
+Overwrites tags assigned for the volume. ## Documentation For Models - [Error]
+(docs/Error.md) - [NfsPermissions](docs/NfsPermissions.md) -
+[NfsPermissionsCreate](docs/NfsPermissionsCreate.md) - [NfsPermissionsUpdate]
+(docs/NfsPermissionsUpdate.md) - [Permissions](docs/Permissions.md) -
 [PermissionsCreate](docs/PermissionsCreate.md) - [PermissionsUpdate](docs/
 PermissionsUpdate.md) - [Status](docs/Status.md) - [StorageNetwork](docs/
 StorageNetwork.md) - [StorageNetworkCreate](docs/StorageNetworkCreate.md) -
 [StorageNetworkUpdate](docs/StorageNetworkUpdate.md) -
-[StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md) - [Volume]
-(docs/Volume.md) - [VolumeCreate](docs/VolumeCreate.md) - [VolumeUpdate](docs/
-VolumeUpdate.md) ## Documentation For Authorization ## OAuth2 - **Type**: OAuth
-- **Flow**: application - **Authorization URL**: - **Scopes**: -
-**networkstorage**: Grants full access to Network Storage API. -
-**networkstorage.read**: Grants read only access to Network Storage API. ##
-Author support@phoenixnap.com ## Notes for Large OpenAPI documents If the
-OpenAPI document is large, imports in pnap_network_storage_api.apis and
-pnap_network_storage_api.models may fail with a RecursionError indicating the
-maximum recursion limit has been exceeded. In that case, there are a couple of
-solutions: Solution 1: Use specific imports for apis and models like: - `from
-pnap_network_storage_api.api.default_api import DefaultApi` - `from
-pnap_network_storage_api.model.pet import Pet` Solution 2: Before importing the
-package, adjust the maximum recursion limit as shown below: ``` import sys
-sys.setrecursionlimit(1500) import pnap_network_storage_api from
-pnap_network_storage_api.apis import * from pnap_network_storage_api.models
-import * ``` Keywords: OpenAPI,OpenAPI-Generator,Network Storage API Platform:
-UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/markdown
+[StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md) -
+[TagAssignment](docs/TagAssignment.md) - [TagAssignmentRequest](docs/
+TagAssignmentRequest.md) - [Volume](docs/Volume.md) - [VolumeCreate](docs/
+VolumeCreate.md) - [VolumeUpdate](docs/VolumeUpdate.md) ## Documentation For
+Authorization ## OAuth2 - **Type**: OAuth - **Flow**: application -
+**Authorization URL**: - **Scopes**: - **networkstorage**: Grants full access
+to Network Storage API. - **networkstorage.read**: Grants read only access to
+Network Storage API. ## Author support@phoenixnap.com ## Notes for Large
+OpenAPI documents If the OpenAPI document is large, imports in
+pnap_network_storage_api.apis and pnap_network_storage_api.models may fail with
+a RecursionError indicating the maximum recursion limit has been exceeded. In
+that case, there are a couple of solutions: Solution 1: Use specific imports
+for apis and models like: - `from pnap_network_storage_api.api.default_api
+import DefaultApi` - `from pnap_network_storage_api.model.pet import Pet`
+Solution 2: Before importing the package, adjust the maximum recursion limit as
+shown below: ``` import sys sys.setrecursionlimit(1500) import
+pnap_network_storage_api from pnap_network_storage_api.apis import * from
+pnap_network_storage_api.models import * ``` Keywords: OpenAPI,OpenAPI-
+Generator,Network Storage API Platform: UNKNOWN Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/SOURCES.txt` & `pnap-network-storage-api-1.4.0/pnap_network_storage_api.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,11 +24,13 @@
 pnap_network_storage_api/model/permissions_create.py
 pnap_network_storage_api/model/permissions_update.py
 pnap_network_storage_api/model/status.py
 pnap_network_storage_api/model/storage_network.py
 pnap_network_storage_api/model/storage_network_create.py
 pnap_network_storage_api/model/storage_network_update.py
 pnap_network_storage_api/model/storage_network_volume_create.py
+pnap_network_storage_api/model/tag_assignment.py
+pnap_network_storage_api/model/tag_assignment_request.py
 pnap_network_storage_api/model/volume.py
 pnap_network_storage_api/model/volume_create.py
 pnap_network_storage_api/model/volume_update.py
 pnap_network_storage_api/models/__init__.py
```

### Comparing `pnap-network-storage-api-1.3.0/setup.py` & `pnap-network-storage-api-1.4.0/setup.py`

 * *Files identical despite different names*

