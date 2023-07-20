# Comparing `tmp/pnap-bmc-api-1.4.0.tar.gz` & `tmp/pnap-bmc-api-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-bmc-api-1.4.0.tar", last modified: Tue Apr 25 13:58:03 2023, max compression
+gzip compressed data, was "dist/pnap-bmc-api-1.5.0.tar", last modified: Thu Jul 20 10:04:52 2023, max compression
```

## Comparing `pnap-bmc-api-1.4.0.tar` & `pnap-bmc-api-1.5.0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)    13973 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11725 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13973 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/models/
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16527 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/quotas_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    26456 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/ssh_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (122)   121100 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/servers_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    14821 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/apis/
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    83144 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5619 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/
--rw-r--r--   0 runner    (1001) docker     (122)    13546 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/ip_blocks_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    12425 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/delete_ssh_key_result.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12348 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (122)    12238 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py
--rw-r--r--   0 runner    (1001) docker     (122)    12549 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_network_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    13614 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_reset.py
--rw-r--r--   0 runner    (1001) docker     (122)    13603 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map_esxi.py
--rw-r--r--   0 runner    (1001) docker     (122)    13530 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_netris_softgate.py
--rw-r--r--   0 runner    (1001) docker     (122)    14631 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota.py
--rw-r--r--   0 runner    (1001) docker     (122)    12904 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/reset_result.py
--rw-r--r--   0 runner    (1001) docker     (122)    12373 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/delete_result.py
--rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_cloud_init.py
--rw-r--r--   0 runner    (1001) docker     (122)    12862 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    16770 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    14632 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_private_network.py
--rw-r--r--   0 runner    (1001) docker     (122)    14601 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/private_network_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    14408 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/network_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/public_network_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    14037 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (122)    12299 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/relinquish_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (122)    13480 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_netris_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)    12525 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_patch.py
--rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map.py
--rw-r--r--   0 runner    (1001) docker     (122)    13317 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/tag_assignment.py
--rw-r--r--   0 runner    (1001) docker     (122)    24169 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    13616 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map_proxmox.py
--rw-r--r--   0 runner    (1001) docker     (122)    12675 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    12085 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/action_result.py
--rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_windows.py
--rw-r--r--   0 runner    (1001) docker     (122)    15012 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request_details.py
--rw-r--r--   0 runner    (1001) docker     (122)    13106 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/tag_assignment_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    12438 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    12411 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (122)    12450 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_reserve.py
--rw-r--r--   0 runner    (1001) docker     (122)    20659 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    13558 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_public_network.py
--rw-r--r--   0 runner    (1001) docker     (122)    17089 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    39978 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11863 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14127 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14127 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)    13317 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/tag_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13546 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/ip_blocks_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12348 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13616 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_map_proxmox.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14631 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/quota.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24803 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12675 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/ssh_key_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13558 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_public_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/public_network_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12750 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/storage_configuration_root_partition.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_cloud_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12450 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_reserve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_windows.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13880 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_netris_softgate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14633 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12361 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/storage_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13603 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_map_esxi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16770 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14037 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14408 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/network_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12373 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/delete_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12085 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/action_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13106 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/tag_assignment_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13614 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_reset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12525 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_patch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12299 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/relinquish_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15158 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/quota_edit_limit_request_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14617 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/private_network_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12425 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/delete_ssh_key_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12411 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12862 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/ssh_key_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12549 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_network_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21427 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12238 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12584 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/quota_edit_limit_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13486 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_netris_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12904 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model/reset_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39978 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5619 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)   121100 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/api/servers_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26456 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/api/ssh_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16527 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/api/quotas_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14821 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83144 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17089 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:04:52.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     3064 2023-07-20 10:04:41.000000 pnap-bmc-api-1.5.0/pnap_bmc_api/models/__init__.py
```

### Comparing `pnap-bmc-api-1.4.0/PKG-INFO` & `pnap-bmc-api-1.5.0/pnap_bmc_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-bmc-api
-Version: 1.4.0
+Version: 1.5.0
 Summary: Bare Metal Cloud API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-bmc-api
@@ -188,14 +188,16 @@
          - [ServerPrivateNetwork](docs/ServerPrivateNetwork.md)
          - [ServerPublicNetwork](docs/ServerPublicNetwork.md)
          - [ServerReserve](docs/ServerReserve.md)
          - [ServerReset](docs/ServerReset.md)
          - [SshKey](docs/SshKey.md)
          - [SshKeyCreate](docs/SshKeyCreate.md)
          - [SshKeyUpdate](docs/SshKeyUpdate.md)
+         - [StorageConfiguration](docs/StorageConfiguration.md)
+         - [StorageConfigurationRootPartition](docs/StorageConfigurationRootPartition.md)
          - [TagAssignment](docs/TagAssignment.md)
          - [TagAssignmentRequest](docs/TagAssignmentRequest.md)
         
         
         ## Documentation For Authorization
```

### Comparing `pnap-bmc-api-1.4.0/README.md` & `pnap-bmc-api-1.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,16 @@
  - [ServerPrivateNetwork](docs/ServerPrivateNetwork.md)
  - [ServerPublicNetwork](docs/ServerPublicNetwork.md)
  - [ServerReserve](docs/ServerReserve.md)
  - [ServerReset](docs/ServerReset.md)
  - [SshKey](docs/SshKey.md)
  - [SshKeyCreate](docs/SshKeyCreate.md)
  - [SshKeyUpdate](docs/SshKeyUpdate.md)
+ - [StorageConfiguration](docs/StorageConfiguration.md)
+ - [StorageConfigurationRootPartition](docs/StorageConfigurationRootPartition.md)
  - [TagAssignment](docs/TagAssignment.md)
  - [TagAssignmentRequest](docs/TagAssignmentRequest.md)
 
 
 ## Documentation For Authorization
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/PKG-INFO` & `pnap-bmc-api-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-bmc-api
-Version: 1.4.0
+Version: 1.5.0
 Summary: Bare Metal Cloud API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-bmc-api
@@ -188,14 +188,16 @@
          - [ServerPrivateNetwork](docs/ServerPrivateNetwork.md)
          - [ServerPublicNetwork](docs/ServerPublicNetwork.md)
          - [ServerReserve](docs/ServerReserve.md)
          - [ServerReset](docs/ServerReset.md)
          - [SshKey](docs/SshKey.md)
          - [SshKeyCreate](docs/SshKeyCreate.md)
          - [SshKeyUpdate](docs/SshKeyUpdate.md)
+         - [StorageConfiguration](docs/StorageConfiguration.md)
+         - [StorageConfigurationRootPartition](docs/StorageConfigurationRootPartition.md)
          - [TagAssignment](docs/TagAssignment.md)
          - [TagAssignmentRequest](docs/TagAssignmentRequest.md)
         
         
         ## Documentation For Authorization
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/SOURCES.txt` & `pnap-bmc-api-1.5.0/pnap_bmc_api.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -48,10 +48,12 @@
 pnap_bmc_api/model/server_private_network.py
 pnap_bmc_api/model/server_public_network.py
 pnap_bmc_api/model/server_reserve.py
 pnap_bmc_api/model/server_reset.py
 pnap_bmc_api/model/ssh_key.py
 pnap_bmc_api/model/ssh_key_create.py
 pnap_bmc_api/model/ssh_key_update.py
+pnap_bmc_api/model/storage_configuration.py
+pnap_bmc_api/model/storage_configuration_root_partition.py
 pnap_bmc_api/model/tag_assignment.py
 pnap_bmc_api/model/tag_assignment_request.py
 pnap_bmc_api/models/__init__.py
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/models/__init__.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,9 +39,11 @@
 from pnap_bmc_api.model.server_private_network import ServerPrivateNetwork
 from pnap_bmc_api.model.server_public_network import ServerPublicNetwork
 from pnap_bmc_api.model.server_reserve import ServerReserve
 from pnap_bmc_api.model.server_reset import ServerReset
 from pnap_bmc_api.model.ssh_key import SshKey
 from pnap_bmc_api.model.ssh_key_create import SshKeyCreate
 from pnap_bmc_api.model.ssh_key_update import SshKeyUpdate
+from pnap_bmc_api.model.storage_configuration import StorageConfiguration
+from pnap_bmc_api.model.storage_configuration_root_partition import StorageConfigurationRootPartition
 from pnap_bmc_api.model.tag_assignment import TagAssignment
 from pnap_bmc_api.model.tag_assignment_request import TagAssignmentRequest
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/__init__.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/api/quotas_api.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/api/quotas_api.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/api/ssh_keys_api.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/api/ssh_keys_api.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/api/servers_api.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/api/servers_api.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/rest.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/apis/__init__.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model_utils.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/exceptions.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/ip_blocks_configuration.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/ip_blocks_configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/delete_ssh_key_result.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/delete_ssh_key_result.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/error.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_network_update.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_network_update.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_reset.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_reset.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map_esxi.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_map_esxi.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_netris_softgate.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_netris_softgate.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,25 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('controller_address',): {
+            'max_length': 253,
+            'regex': {
+                'pattern': r'^(?!-)[\w\-]{1,63}(?<!-)(\.(?!-)[\w\-]{1,63}(?<!-))*$',  # noqa: E501
+            },
+        },
+        ('controller_auth_key',): {
+            'regex': {
+                'pattern': r'^\S+$',  # noqa: E501
+            },
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/quota.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/reset_result.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/reset_result.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/delete_result.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/delete_result.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_cloud_init.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_cloud_init.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key_create.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/ssh_key_create.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_private_network.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_private_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """
 
     allowed_values = {
     }
 
     validations = {
         ('ips',): {
-            'max_items': 10,
+            'max_items': 256,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/private_network_configuration.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/private_network_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gateway_address (str): Deprecated in favour of a common gateway address across all networks available under NetworkConfiguration.<br> The address of the gateway assigned / to assign to the server.<br> When used as part of request body, IP address has to be part of private network assigned to this server.<br> Gateway address also has to be assigned on an already deployed resource unless the `force` query parameter is true.. [optional]  # noqa: E501
-            configuration_type (str): (Write-only) Determines the approach for configuring private network(s) for the server being provisioned. Currently this field should be set to `USE_OR_CREATE_DEFAULT` or `USER_DEFINED`.. [optional] if omitted the server will use the default value of "USE_OR_CREATE_DEFAULT"  # noqa: E501
+            configuration_type (str): (Write-only) Determines the approach for configuring private network(s) for the server being provisioned. Currently this field should be set to `USE_OR_CREATE_DEFAULT`, `USER_DEFINED` or `NONE`.. [optional] if omitted the server will use the default value of "USE_OR_CREATE_DEFAULT"  # noqa: E501
             private_networks ([ServerPrivateNetwork]): The list of private networks this server is member of. When this field is part of request body, it'll be used to specify the private networks to assign to this server upon provisioning. Used alongside the `USER_DEFINED` configurationType.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -230,15 +230,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gateway_address (str): Deprecated in favour of a common gateway address across all networks available under NetworkConfiguration.<br> The address of the gateway assigned / to assign to the server.<br> When used as part of request body, IP address has to be part of private network assigned to this server.<br> Gateway address also has to be assigned on an already deployed resource unless the `force` query parameter is true.. [optional]  # noqa: E501
-            configuration_type (str): (Write-only) Determines the approach for configuring private network(s) for the server being provisioned. Currently this field should be set to `USE_OR_CREATE_DEFAULT` or `USER_DEFINED`.. [optional] if omitted the server will use the default value of "USE_OR_CREATE_DEFAULT"  # noqa: E501
+            configuration_type (str): (Write-only) Determines the approach for configuring private network(s) for the server being provisioned. Currently this field should be set to `USE_OR_CREATE_DEFAULT`, `USER_DEFINED` or `NONE`.. [optional] if omitted the server will use the default value of "USE_OR_CREATE_DEFAULT"  # noqa: E501
             private_networks ([ServerPrivateNetwork]): The list of private networks this server is member of. When this field is part of request body, it'll be used to specify the private networks to assign to this server upon provisioning. Used alongside the `USER_DEFINED` configurationType.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/network_configuration.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/network_configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/public_network_configuration.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/public_network_configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/relinquish_ip_block.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/relinquish_ip_block.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_netris_controller.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_netris_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             host_os (str): (Read-only) Host OS on which the Netris Controller is installed.. [optional]  # noqa: E501
-            netris_web_console_url (str): (Read-only) The URL for the Netris Controller web console. Will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            netris_web_console_url (str): (Read-only) The URL for the Netris Controller web console. It will only be returned in response to provisioning a server.. [optional]  # noqa: E501
             netris_user_password (str): (Read-only) Auto-generated password set for user 'netris' in the web console.<br>  The password is not stored and therefore will only be returned in response to provisioning a server. Copy and save it for future reference.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -227,15 +227,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             host_os (str): (Read-only) Host OS on which the Netris Controller is installed.. [optional]  # noqa: E501
-            netris_web_console_url (str): (Read-only) The URL for the Netris Controller web console. Will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            netris_web_console_url (str): (Read-only) The URL for the Netris Controller web console. It will only be returned in response to provisioning a server.. [optional]  # noqa: E501
             netris_user_password (str): (Read-only) Auto-generated password set for user 'netris' in the web console.<br>  The password is not stored and therefore will only be returned in response to provisioning a server. Copy and save it for future reference.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_patch.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_patch.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_map.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/tag_assignment.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/tag_assignment.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,19 @@
 )
 from pnap_bmc_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from pnap_bmc_api.model.network_configuration import NetworkConfiguration
     from pnap_bmc_api.model.os_configuration import OsConfiguration
+    from pnap_bmc_api.model.storage_configuration import StorageConfiguration
     from pnap_bmc_api.model.tag_assignment import TagAssignment
     globals()['NetworkConfiguration'] = NetworkConfiguration
     globals()['OsConfiguration'] = OsConfiguration
+    globals()['StorageConfiguration'] = StorageConfiguration
     globals()['TagAssignment'] = TagAssignment
 
 
 class Server(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -128,14 +130,15 @@
             'cores_per_cpu': (int,),  # noqa: E501
             'cpu_frequency': (float,),  # noqa: E501
             'ram': (str,),  # noqa: E501
             'storage': (str,),  # noqa: E501
             'private_ip_addresses': ([str],),  # noqa: E501
             'pricing_model': (str,),  # noqa: E501
             'network_configuration': (NetworkConfiguration,),  # noqa: E501
+            'storage_configuration': (StorageConfiguration,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'public_ip_addresses': ([str],),  # noqa: E501
             'reservation_id': (str,),  # noqa: E501
             'password': (str,),  # noqa: E501
             'network_type': (str,),  # noqa: E501
             'cluster_id': (str,),  # noqa: E501
             'tags': ([TagAssignment],),  # noqa: E501
@@ -160,14 +163,15 @@
         'cores_per_cpu': 'coresPerCpu',  # noqa: E501
         'cpu_frequency': 'cpuFrequency',  # noqa: E501
         'ram': 'ram',  # noqa: E501
         'storage': 'storage',  # noqa: E501
         'private_ip_addresses': 'privateIpAddresses',  # noqa: E501
         'pricing_model': 'pricingModel',  # noqa: E501
         'network_configuration': 'networkConfiguration',  # noqa: E501
+        'storage_configuration': 'storageConfiguration',  # noqa: E501
         'description': 'description',  # noqa: E501
         'public_ip_addresses': 'publicIpAddresses',  # noqa: E501
         'reservation_id': 'reservationId',  # noqa: E501
         'password': 'password',  # noqa: E501
         'network_type': 'networkType',  # noqa: E501
         'cluster_id': 'clusterId',  # noqa: E501
         'tags': 'tags',  # noqa: E501
@@ -178,32 +182,33 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, status, hostname, os, type, location, cpu, cpu_count, cores_per_cpu, cpu_frequency, ram, storage, private_ip_addresses, network_configuration, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, status, hostname, os, type, location, cpu, cpu_count, cores_per_cpu, cpu_frequency, ram, storage, private_ip_addresses, network_configuration, storage_configuration, *args, **kwargs):  # noqa: E501
         """Server - a model defined in OpenAPI
 
         Args:
             id (str): The unique identifier of the server.
             status (str): The status of the server.
             hostname (str): Hostname of server.
             os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `esxi/esxi80`, `debian/bullseye`, `proxmox/bullseye`, `netris/controller`, `netris/softgate_1g` or `netris/softgate_10g`.
-            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.storage.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge` or `d3.m6.xlarge`.
+            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.db1.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge`, `d3.m6.xlarge` or `a1.c5.large`.
             location (str): Server location ID. Cannot be changed once a server is created. Currently this field should be set to `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` or `AUS`.
             cpu (str): A description of the machine CPU.
             cpu_count (int): The number of CPUs available in the system.
             cores_per_cpu (int): The number of physical cores present on each CPU.
             cpu_frequency (float): The CPU frequency in GHz.
             ram (str): A description of the machine RAM.
             storage (str): A description of the machine storage.
             private_ip_addresses ([str]): Private IP addresses assigned to server.
             network_configuration (NetworkConfiguration):
+            storage_configuration (StorageConfiguration):
 
         Keyword Args:
             pricing_model (str): The pricing model this server is being billed. Currently this field should be set to `HOURLY`, `ONE_MONTH_RESERVATION`, `TWELVE_MONTHS_RESERVATION`, `TWENTY_FOUR_MONTHS_RESERVATION` or `THIRTY_SIX_MONTHS_RESERVATION`.. defaults to "HOURLY"  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -233,15 +238,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): Description of server.. [optional]  # noqa: E501
             public_ip_addresses ([str]): Public IP addresses assigned to server.. [optional]  # noqa: E501
             reservation_id (str): The reservation reference id if any.. [optional]  # noqa: E501
             password (str): Auto-generated password set for user `Admin` on Windows server, user `root` on ESXi servers, user `root` on Proxmox server and user `netris` on Netris servers.<br> The password is not stored and therefore will only be returned in response to provisioning a server. Copy and save it for future reference.. [optional]  # noqa: E501
-            network_type (str): The type of network configuration for this server. Currently this field should be set to `PUBLIC_AND_PRIVATE` or `PRIVATE_ONLY`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
+            network_type (str): The type of network configuration for this server. Currently this field should be set to `PUBLIC_AND_PRIVATE`, `PRIVATE_ONLY`, `PUBLIC_ONLY` or `NONE`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
             cluster_id (str): The cluster reference id if any.. [optional]  # noqa: E501
             tags ([TagAssignment]): The tags assigned if any.. [optional]  # noqa: E501
             provisioned_on (datetime): Date and time when server was provisioned.. [optional]  # noqa: E501
             os_configuration (OsConfiguration): [optional]  # noqa: E501
         """
 
         pricing_model = kwargs.get('pricing_model', "HOURLY")
@@ -285,14 +290,15 @@
         self.cores_per_cpu = cores_per_cpu
         self.cpu_frequency = cpu_frequency
         self.ram = ram
         self.storage = storage
         self.private_ip_addresses = private_ip_addresses
         self.pricing_model = pricing_model
         self.network_configuration = network_configuration
+        self.storage_configuration = storage_configuration
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -305,32 +311,33 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, status, hostname, os, type, location, cpu, cpu_count, cores_per_cpu, cpu_frequency, ram, storage, private_ip_addresses, network_configuration, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, status, hostname, os, type, location, cpu, cpu_count, cores_per_cpu, cpu_frequency, ram, storage, private_ip_addresses, network_configuration, storage_configuration, *args, **kwargs):  # noqa: E501
         """Server - a model defined in OpenAPI
 
         Args:
             id (str): The unique identifier of the server.
             status (str): The status of the server.
             hostname (str): Hostname of server.
             os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `esxi/esxi80`, `debian/bullseye`, `proxmox/bullseye`, `netris/controller`, `netris/softgate_1g` or `netris/softgate_10g`.
-            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.storage.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge` or `d3.m6.xlarge`.
+            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.db1.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge`, `d3.m6.xlarge` or `a1.c5.large`.
             location (str): Server location ID. Cannot be changed once a server is created. Currently this field should be set to `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` or `AUS`.
             cpu (str): A description of the machine CPU.
             cpu_count (int): The number of CPUs available in the system.
             cores_per_cpu (int): The number of physical cores present on each CPU.
             cpu_frequency (float): The CPU frequency in GHz.
             ram (str): A description of the machine RAM.
             storage (str): A description of the machine storage.
             private_ip_addresses ([str]): Private IP addresses assigned to server.
             network_configuration (NetworkConfiguration):
+            storage_configuration (StorageConfiguration):
 
         Keyword Args:
             pricing_model (str): The pricing model this server is being billed. Currently this field should be set to `HOURLY`, `ONE_MONTH_RESERVATION`, `TWELVE_MONTHS_RESERVATION`, `TWENTY_FOUR_MONTHS_RESERVATION` or `THIRTY_SIX_MONTHS_RESERVATION`.. defaults to "HOURLY"  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -360,15 +367,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): Description of server.. [optional]  # noqa: E501
             public_ip_addresses ([str]): Public IP addresses assigned to server.. [optional]  # noqa: E501
             reservation_id (str): The reservation reference id if any.. [optional]  # noqa: E501
             password (str): Auto-generated password set for user `Admin` on Windows server, user `root` on ESXi servers, user `root` on Proxmox server and user `netris` on Netris servers.<br> The password is not stored and therefore will only be returned in response to provisioning a server. Copy and save it for future reference.. [optional]  # noqa: E501
-            network_type (str): The type of network configuration for this server. Currently this field should be set to `PUBLIC_AND_PRIVATE` or `PRIVATE_ONLY`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
+            network_type (str): The type of network configuration for this server. Currently this field should be set to `PUBLIC_AND_PRIVATE`, `PRIVATE_ONLY`, `PUBLIC_ONLY` or `NONE`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
             cluster_id (str): The cluster reference id if any.. [optional]  # noqa: E501
             tags ([TagAssignment]): The tags assigned if any.. [optional]  # noqa: E501
             provisioned_on (datetime): Date and time when server was provisioned.. [optional]  # noqa: E501
             os_configuration (OsConfiguration): [optional]  # noqa: E501
         """
 
         pricing_model = kwargs.get('pricing_model', "HOURLY")
@@ -410,14 +417,15 @@
         self.cores_per_cpu = cores_per_cpu
         self.cpu_frequency = cpu_frequency
         self.ram = ram
         self.storage = storage
         self.private_ip_addresses = private_ip_addresses
         self.pricing_model = pricing_model
         self.network_configuration = network_configuration
+        self.storage_configuration = storage_configuration
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map_proxmox.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_map_proxmox.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key_update.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/ssh_key_update.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/action_result.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/action_result.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_windows.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/os_configuration_windows.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request_details.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/quota_edit_limit_request_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """QuotaEditLimitRequestDetails - a model defined in OpenAPI
 
         Keyword Args:
-            limit (int): The new limit that is requested.
+            limit (int): The new limit that is requested. Minimum allowed limit values: - 0 (Server, IPs) - 1000 (Network Storage)
             reason (str): The reason for changing the limit.
             requested_on (datetime): The point in time the request was submitted.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,15 +220,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """QuotaEditLimitRequestDetails - a model defined in OpenAPI
 
         Keyword Args:
-            limit (int): The new limit that is requested.
+            limit (int): The new limit that is requested. Minimum allowed limit values: - 0 (Server, IPs) - 1000 (Network Storage)
             reason (str): The reason for changing the limit.
             requested_on (datetime): The point in time the request was submitted.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/tag_assignment_request.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/tag_assignment_request.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/quota_edit_limit_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, limit, reason, *args, **kwargs):  # noqa: E501
         """QuotaEditLimitRequest - a model defined in OpenAPI
 
         Args:
-            limit (int): The new limit that is requested.
+            limit (int): The new limit that is requested. Minimum allowed limit values: - 0 (Server, IPs) - 1000 (Network Storage)
             reason (str): The reason for changing the limit.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -197,15 +197,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, limit, reason, *args, **kwargs):  # noqa: E501
         """QuotaEditLimitRequest - a model defined in OpenAPI
 
         Args:
-            limit (int): The new limit that is requested.
+            limit (int): The new limit that is requested. Minimum allowed limit values: - 0 (Server, IPs) - 1000 (Network Storage)
             reason (str): The reason for changing the limit.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_ip_block.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_ip_block.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_reserve.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_reserve.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_create.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,19 @@
 )
 from pnap_bmc_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from pnap_bmc_api.model.network_configuration import NetworkConfiguration
     from pnap_bmc_api.model.os_configuration import OsConfiguration
+    from pnap_bmc_api.model.storage_configuration import StorageConfiguration
     from pnap_bmc_api.model.tag_assignment_request import TagAssignmentRequest
     globals()['NetworkConfiguration'] = NetworkConfiguration
     globals()['OsConfiguration'] = OsConfiguration
+    globals()['StorageConfiguration'] = StorageConfiguration
     globals()['TagAssignmentRequest'] = TagAssignmentRequest
 
 
 class ServerCreate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -112,14 +114,15 @@
             'ssh_key_ids': ([str],),  # noqa: E501
             'reservation_id': (str,),  # noqa: E501
             'pricing_model': (str,),  # noqa: E501
             'network_type': (str,),  # noqa: E501
             'os_configuration': (OsConfiguration,),  # noqa: E501
             'tags': ([TagAssignmentRequest],),  # noqa: E501
             'network_configuration': (NetworkConfiguration,),  # noqa: E501
+            'storage_configuration': (StorageConfiguration,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -134,14 +137,15 @@
         'ssh_key_ids': 'sshKeyIds',  # noqa: E501
         'reservation_id': 'reservationId',  # noqa: E501
         'pricing_model': 'pricingModel',  # noqa: E501
         'network_type': 'networkType',  # noqa: E501
         'os_configuration': 'osConfiguration',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'network_configuration': 'networkConfiguration',  # noqa: E501
+        'storage_configuration': 'storageConfiguration',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -149,15 +153,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, hostname, os, type, location, *args, **kwargs):  # noqa: E501
         """ServerCreate - a model defined in OpenAPI
 
         Args:
             hostname (str): Hostname of server.
             os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `esxi/esxi80`, `debian/bullseye`, `proxmox/bullseye`, `netris/controller`, `netris/softgate_1g` or `netris/softgate_10g`.
-            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.storage.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge` or `d3.m6.xlarge`.
+            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.db1.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge`, `d3.m6.xlarge` or `a1.c5.large`.
             location (str): Server location ID. Cannot be changed once a server is created. Currently this field should be set to `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` or `AUS`.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -189,18 +193,19 @@
                                 _visited_composed_classes = (Animal,)
             description (str): Description of server.. [optional]  # noqa: E501
             install_default_ssh_keys (bool): Whether or not to install SSH keys marked as default in addition to any SSH keys specified in this request.. [optional] if omitted the server will use the default value of True  # noqa: E501
             ssh_keys ([str]): A list of SSH keys that will be installed on the server.. [optional]  # noqa: E501
             ssh_key_ids ([str]): A list of SSH key IDs that will be installed on the server in addition to any SSH keys specified in this request.. [optional]  # noqa: E501
             reservation_id (str): Server reservation ID.. [optional]  # noqa: E501
             pricing_model (str): Server pricing model. Currently this field should be set to `HOURLY`, `ONE_MONTH_RESERVATION`, `TWELVE_MONTHS_RESERVATION`, `TWENTY_FOUR_MONTHS_RESERVATION` or `THIRTY_SIX_MONTHS_RESERVATION`.. [optional] if omitted the server will use the default value of "HOURLY"  # noqa: E501
-            network_type (str): The type of network configuration for this server. Currently this field should be set to `PUBLIC_AND_PRIVATE` or `PRIVATE_ONLY`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
+            network_type (str): The type of network configuration for this server.<br> Currently this field should be set to `PUBLIC_AND_PRIVATE`, `PRIVATE_ONLY`, `PUBLIC_ONLY` or `USER_DEFINED`.<br> Setting the `force` query parameter to `true` allows you to configure network configuration type as `NONE`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
             os_configuration (OsConfiguration): [optional]  # noqa: E501
             tags ([TagAssignmentRequest]): Tags to set to the server. To create a new tag or list all the existing tags that you can use, refer to [Tags API](https://developers.phoenixnap.com/docs/tags/1/overview).. [optional]  # noqa: E501
             network_configuration (NetworkConfiguration): [optional]  # noqa: E501
+            storage_configuration (StorageConfiguration): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -254,15 +259,15 @@
     @convert_js_args_to_python_args
     def __init__(self, hostname, os, type, location, *args, **kwargs):  # noqa: E501
         """ServerCreate - a model defined in OpenAPI
 
         Args:
             hostname (str): Hostname of server.
             os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `esxi/esxi80`, `debian/bullseye`, `proxmox/bullseye`, `netris/controller`, `netris/softgate_1g` or `netris/softgate_10g`.
-            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.storage.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge` or `d3.m6.xlarge`.
+            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.db1.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge`, `d3.m6.xlarge` or `a1.c5.large`.
             location (str): Server location ID. Cannot be changed once a server is created. Currently this field should be set to `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` or `AUS`.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -294,18 +299,19 @@
                                 _visited_composed_classes = (Animal,)
             description (str): Description of server.. [optional]  # noqa: E501
             install_default_ssh_keys (bool): Whether or not to install SSH keys marked as default in addition to any SSH keys specified in this request.. [optional] if omitted the server will use the default value of True  # noqa: E501
             ssh_keys ([str]): A list of SSH keys that will be installed on the server.. [optional]  # noqa: E501
             ssh_key_ids ([str]): A list of SSH key IDs that will be installed on the server in addition to any SSH keys specified in this request.. [optional]  # noqa: E501
             reservation_id (str): Server reservation ID.. [optional]  # noqa: E501
             pricing_model (str): Server pricing model. Currently this field should be set to `HOURLY`, `ONE_MONTH_RESERVATION`, `TWELVE_MONTHS_RESERVATION`, `TWENTY_FOUR_MONTHS_RESERVATION` or `THIRTY_SIX_MONTHS_RESERVATION`.. [optional] if omitted the server will use the default value of "HOURLY"  # noqa: E501
-            network_type (str): The type of network configuration for this server. Currently this field should be set to `PUBLIC_AND_PRIVATE` or `PRIVATE_ONLY`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
+            network_type (str): The type of network configuration for this server.<br> Currently this field should be set to `PUBLIC_AND_PRIVATE`, `PRIVATE_ONLY`, `PUBLIC_ONLY` or `USER_DEFINED`.<br> Setting the `force` query parameter to `true` allows you to configure network configuration type as `NONE`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
             os_configuration (OsConfiguration): [optional]  # noqa: E501
             tags ([TagAssignmentRequest]): Tags to set to the server. To create a new tag or list all the existing tags that you can use, refer to [Tags API](https://developers.phoenixnap.com/docs/tags/1/overview).. [optional]  # noqa: E501
             network_configuration (NetworkConfiguration): [optional]  # noqa: E501
+            storage_configuration (StorageConfiguration): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_public_network.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/model/server_public_network.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/configuration.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/pnap_bmc_api/api_client.py` & `pnap-bmc-api-1.5.0/pnap_bmc_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.4.0/setup.py` & `pnap-bmc-api-1.5.0/setup.py`

 * *Files identical despite different names*

