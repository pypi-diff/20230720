# Comparing `tmp/strongdm-4.0.0.zip` & `tmp/strongdm-4.1.0.zip`

## zipinfo {}

```diff
@@ -1,87 +1,95 @@
-Zip file size: 252348 bytes, number of entries: 85
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 15:29 strongdm-4.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 15:29 strongdm-4.0.0/strongdm/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 15:29 strongdm-4.0.0/strongdm.egg-info/
--rw-r--r--  2.0 unx     1908 b- defN 23-Jul-18 15:29 strongdm-4.0.0/setup.py
--rw-r--r--  2.0 unx     3957 b- defN 23-Jul-18 15:29 strongdm-4.0.0/PKG-INFO
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-18 15:29 strongdm-4.0.0/setup.cfg
--rw-r--r--  2.0 unx     2652 b- defN 23-Jul-18 15:29 strongdm-4.0.0/README.md
--rw-r--r--  2.0 unx    15880 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/spec_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/drivers_pb2_grpc.py
--rw-r--r--  2.0 unx    26113 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/nodes_pb2.py
--rw-r--r--  2.0 unx     8138 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/accounts_history_pb2.py
--rw-r--r--  2.0 unx     3111 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx     9971 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/remote_identity_groups_pb2.py
--rw-r--r--  2.0 unx     9790 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/remote_identities_pb2_grpc.py
--rw-r--r--  2.0 unx    19858 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/remote_identities_pb2.py
--rw-r--r--  2.0 unx     3388 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_resources_pb2_grpc.py
--rw-r--r--  2.0 unx   850527 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/drivers_pb2.py
--rw-r--r--  2.0 unx     7476 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/role_resources_pb2.py
--rw-r--r--  2.0 unx     7818 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/roles_history_pb2.py
--rw-r--r--  2.0 unx     3111 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/nodes_history_pb2_grpc.py
--rw-r--r--  2.0 unx   313058 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/plumbing.py
--rw-r--r--  2.0 unx     9494 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/accounts_pb2_grpc.py
--rw-r--r--  2.0 unx     8320 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/replays_pb2.py
--rw-r--r--  2.0 unx     3361 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/replays_pb2_grpc.py
--rw-r--r--  2.0 unx    16584 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_grants_pb2.py
--rw-r--r--  2.0 unx    17034 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/organization_history_pb2.py
--rw-r--r--  2.0 unx     8396 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_permissions_pb2.py
--rw-r--r--  2.0 unx    19105 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/resources_pb2.py
--rw-r--r--  2.0 unx   629518 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/models.py
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/spec_pb2_grpc.py
--rw-r--r--  2.0 unx    10693 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/resources_pb2_grpc.py
--rw-r--r--  2.0 unx     3424 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/remote_identities_history_pb2_grpc.py
--rw-r--r--  2.0 unx     4600 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/tags_pb2.py
--rw-r--r--  2.0 unx    24712 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/accounts_pb2.py
--rwxr-xr-x  2.0 unx    17673 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/constants.py
--rw-r--r--  2.0 unx     8478 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/role_resources_history_pb2.py
--rw-r--r--  2.0 unx    17817 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/queries_pb2.py
--rw-r--r--  2.0 unx     8650 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/remote_identities_history_pb2.py
--rw-r--r--  2.0 unx     8773 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_resources_history_pb2.py
--rw-r--r--  2.0 unx      808 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/__init__.py
--rw-r--r--  2.0 unx     3223 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/secret_store_types_pb2_grpc.py
--rw-r--r--  2.0 unx     7818 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/nodes_history_pb2.py
--rw-r--r--  2.0 unx     3434 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx    17037 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_attachments_pb2.py
--rw-r--r--  2.0 unx     7980 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_grants_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/tags_pb2_grpc.py
--rw-r--r--  2.0 unx     8901 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_attachments_history_pb2.py
--rw-r--r--  2.0 unx     8550 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_grants_history_pb2.py
--rw-r--r--  2.0 unx     3561 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py
--rw-r--r--  2.0 unx     4905 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/activities_pb2_grpc.py
--rw-r--r--  2.0 unx     3470 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_permissions_pb2_grpc.py
--rw-r--r--  2.0 unx     2196 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/errors.py
--rw-r--r--  2.0 unx     8102 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_attachments_pb2_grpc.py
--rw-r--r--  2.0 unx    17686 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/client.py
--rw-r--r--  2.0 unx   110921 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/svc.py
--rw-r--r--  2.0 unx     3420 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/queries_pb2_grpc.py
--rw-r--r--  2.0 unx     3322 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/secret_stores_history_pb2_grpc.py
--rw-r--r--  2.0 unx     9027 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/remote_identity_groups_history_pb2.py
--rw-r--r--  2.0 unx    16300 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/activities_pb2.py
--rw-r--r--  2.0 unx     9376 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/secret_stores_pb2_grpc.py
--rw-r--r--  2.0 unx     3295 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/role_resources_pb2_grpc.py
--rw-r--r--  2.0 unx    17214 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/secret_stores_pb2.py
--rw-r--r--  2.0 unx     6176 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/remote_identity_groups_pb2_grpc.py
--rw-r--r--  2.0 unx     9837 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/nodes_pb2_grpc.py
--rw-r--r--  2.0 unx     8901 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_resources_pb2.py
--rw-r--r--  2.0 unx     3350 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/role_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx    14750 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/options_pb2.py
--rw-r--r--  2.0 unx     8412 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/secret_stores_history_pb2.py
--rw-r--r--  2.0 unx     3198 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/accounts_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8369 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/control_panel_pb2.py
--rw-r--r--  2.0 unx    18385 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/roles_pb2.py
--rw-r--r--  2.0 unx     3493 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_attachments_history_pb2_grpc.py
--rw-r--r--  2.0 unx     9042 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/roles_pb2_grpc.py
--rw-r--r--  2.0 unx     8132 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/resources_history_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/options_pb2_grpc.py
--rw-r--r--  2.0 unx     3320 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/organization_history_pb2_grpc.py
--rw-r--r--  2.0 unx    31259 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/secret_store_types_pb2.py
--rw-r--r--  2.0 unx     4879 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/control_panel_pb2_grpc.py
--rw-r--r--  2.0 unx     3353 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm/account_grants_history_pb2_grpc.py
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm.egg-info/top_level.txt
--rw-r--r--  2.0 unx     3957 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     2581 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-18 15:29 strongdm-4.0.0/strongdm.egg-info/requires.txt
-85 files, 2529131 bytes uncompressed, 238224 bytes compressed:  90.6%
+Zip file size: 273857 bytes, number of entries: 93
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 15:57 strongdm-4.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 15:57 strongdm-4.1.0/strongdm/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 15:57 strongdm-4.1.0/strongdm.egg-info/
+-rw-r--r--  2.0 unx     1908 b- defN 23-Jul-20 15:57 strongdm-4.1.0/setup.py
+-rw-r--r--  2.0 unx     3957 b- defN 23-Jul-20 15:57 strongdm-4.1.0/PKG-INFO
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-20 15:57 strongdm-4.1.0/setup.cfg
+-rw-r--r--  2.0 unx     2652 b- defN 23-Jul-20 15:57 strongdm-4.1.0/README.md
+-rw-r--r--  2.0 unx     8167 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/peering_group_peers_pb2_grpc.py
+-rw-r--r--  2.0 unx    15880 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/spec_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/drivers_pb2_grpc.py
+-rw-r--r--  2.0 unx    26113 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/nodes_pb2.py
+-rw-r--r--  2.0 unx     8138 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/accounts_history_pb2.py
+-rw-r--r--  2.0 unx     3111 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9971 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/remote_identity_groups_pb2.py
+-rw-r--r--  2.0 unx     9790 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/remote_identities_pb2_grpc.py
+-rw-r--r--  2.0 unx    19858 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/remote_identities_pb2.py
+-rw-r--r--  2.0 unx     3388 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx   850527 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/drivers_pb2.py
+-rw-r--r--  2.0 unx     7476 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/role_resources_pb2.py
+-rw-r--r--  2.0 unx     8255 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/peering_group_nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     7818 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/roles_history_pb2.py
+-rw-r--r--  2.0 unx     3111 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/nodes_history_pb2_grpc.py
+-rw-r--r--  2.0 unx   333095 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/plumbing.py
+-rw-r--r--  2.0 unx     9494 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/accounts_pb2_grpc.py
+-rw-r--r--  2.0 unx     8320 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/replays_pb2.py
+-rw-r--r--  2.0 unx     3361 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/replays_pb2_grpc.py
+-rw-r--r--  2.0 unx    16584 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_grants_pb2.py
+-rw-r--r--  2.0 unx    17034 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/organization_history_pb2.py
+-rw-r--r--  2.0 unx     8396 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_permissions_pb2.py
+-rw-r--r--  2.0 unx    19105 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/resources_pb2.py
+-rw-r--r--  2.0 unx   650137 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/models.py
+-rw-r--r--  2.0 unx      741 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/spec_pb2_grpc.py
+-rw-r--r--  2.0 unx    10693 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/resources_pb2_grpc.py
+-rw-r--r--  2.0 unx     3424 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/remote_identities_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     4600 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/tags_pb2.py
+-rw-r--r--  2.0 unx    17096 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/peering_group_resources_pb2.py
+-rw-r--r--  2.0 unx    24712 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/accounts_pb2.py
+-rwxr-xr-x  2.0 unx    17819 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/constants.py
+-rw-r--r--  2.0 unx     8478 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/role_resources_history_pb2.py
+-rw-r--r--  2.0 unx    17817 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/queries_pb2.py
+-rw-r--r--  2.0 unx     8650 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/remote_identities_history_pb2.py
+-rw-r--r--  2.0 unx     8773 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_resources_history_pb2.py
+-rw-r--r--  2.0 unx      808 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/__init__.py
+-rw-r--r--  2.0 unx     7932 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/peering_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx     3223 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/secret_store_types_pb2_grpc.py
+-rw-r--r--  2.0 unx     7818 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/nodes_history_pb2.py
+-rw-r--r--  2.0 unx     3434 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    17037 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_attachments_pb2.py
+-rw-r--r--  2.0 unx     7980 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_grants_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/tags_pb2_grpc.py
+-rw-r--r--  2.0 unx     8901 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_attachments_history_pb2.py
+-rw-r--r--  2.0 unx     8550 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_grants_history_pb2.py
+-rw-r--r--  2.0 unx     3561 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     4905 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/activities_pb2_grpc.py
+-rw-r--r--  2.0 unx     3470 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_permissions_pb2_grpc.py
+-rw-r--r--  2.0 unx     2196 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/errors.py
+-rw-r--r--  2.0 unx    15214 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/peering_groups_pb2.py
+-rw-r--r--  2.0 unx     8102 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_attachments_pb2_grpc.py
+-rw-r--r--  2.0 unx    20218 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/client.py
+-rw-r--r--  2.0 unx     8546 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/peering_group_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx   137613 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/svc.py
+-rw-r--r--  2.0 unx     3420 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/queries_pb2_grpc.py
+-rw-r--r--  2.0 unx     3322 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/secret_stores_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9027 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/remote_identity_groups_history_pb2.py
+-rw-r--r--  2.0 unx    16300 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/activities_pb2.py
+-rw-r--r--  2.0 unx     9376 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/secret_stores_pb2_grpc.py
+-rw-r--r--  2.0 unx     3295 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/role_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    17214 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/secret_stores_pb2.py
+-rw-r--r--  2.0 unx     6176 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/remote_identity_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx     9837 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     8901 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_resources_pb2.py
+-rw-r--r--  2.0 unx     3350 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/role_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    14806 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/options_pb2.py
+-rw-r--r--  2.0 unx     8412 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/secret_stores_history_pb2.py
+-rw-r--r--  2.0 unx     3198 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/accounts_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8369 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/control_panel_pb2.py
+-rw-r--r--  2.0 unx    16346 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/peering_group_peers_pb2.py
+-rw-r--r--  2.0 unx    18385 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/roles_pb2.py
+-rw-r--r--  2.0 unx     3493 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_attachments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9042 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/roles_pb2_grpc.py
+-rw-r--r--  2.0 unx     8132 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/resources_history_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/options_pb2_grpc.py
+-rw-r--r--  2.0 unx     3320 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/organization_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    16303 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/peering_group_nodes_pb2.py
+-rw-r--r--  2.0 unx    31259 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/secret_store_types_pb2.py
+-rw-r--r--  2.0 unx     4879 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/control_panel_pb2_grpc.py
+-rw-r--r--  2.0 unx     3353 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm/account_grants_history_pb2_grpc.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     3957 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     2887 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-20 15:57 strongdm-4.1.0/strongdm.egg-info/requires.txt
+93 files, 2697378 bytes uncompressed, 258289 bytes compressed:  90.4%
```

## zipnote {}

```diff
@@ -1,256 +1,280 @@
-Filename: strongdm-4.0.0/
+Filename: strongdm-4.1.0/
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/
+Filename: strongdm-4.1.0/strongdm/
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm.egg-info/
+Filename: strongdm-4.1.0/strongdm.egg-info/
 Comment: 
 
-Filename: strongdm-4.0.0/setup.py
+Filename: strongdm-4.1.0/setup.py
 Comment: 
 
-Filename: strongdm-4.0.0/PKG-INFO
+Filename: strongdm-4.1.0/PKG-INFO
 Comment: 
 
-Filename: strongdm-4.0.0/setup.cfg
+Filename: strongdm-4.1.0/setup.cfg
 Comment: 
 
-Filename: strongdm-4.0.0/README.md
+Filename: strongdm-4.1.0/README.md
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/spec_pb2.py
+Filename: strongdm-4.1.0/strongdm/peering_group_peers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/drivers_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/spec_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/nodes_pb2.py
+Filename: strongdm-4.1.0/strongdm/drivers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/accounts_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/nodes_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/roles_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/accounts_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/remote_identity_groups_pb2.py
+Filename: strongdm-4.1.0/strongdm/roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/remote_identities_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/remote_identity_groups_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/remote_identities_pb2.py
+Filename: strongdm-4.1.0/strongdm/remote_identities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_resources_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/remote_identities_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/drivers_pb2.py
+Filename: strongdm-4.1.0/strongdm/account_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/role_resources_pb2.py
+Filename: strongdm-4.1.0/strongdm/drivers_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/roles_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/role_resources_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/nodes_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/peering_group_nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/plumbing.py
+Filename: strongdm-4.1.0/strongdm/roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/accounts_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/nodes_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/replays_pb2.py
+Filename: strongdm-4.1.0/strongdm/plumbing.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/replays_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/accounts_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_grants_pb2.py
+Filename: strongdm-4.1.0/strongdm/replays_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/organization_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/replays_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_permissions_pb2.py
+Filename: strongdm-4.1.0/strongdm/account_grants_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/resources_pb2.py
+Filename: strongdm-4.1.0/strongdm/organization_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/models.py
+Filename: strongdm-4.1.0/strongdm/account_permissions_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/spec_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/resources_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/resources_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/models.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/remote_identities_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/spec_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/tags_pb2.py
+Filename: strongdm-4.1.0/strongdm/resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/accounts_pb2.py
+Filename: strongdm-4.1.0/strongdm/remote_identities_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/constants.py
+Filename: strongdm-4.1.0/strongdm/tags_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/role_resources_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/peering_group_resources_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/queries_pb2.py
+Filename: strongdm-4.1.0/strongdm/accounts_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/remote_identities_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/constants.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_resources_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/role_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/__init__.py
+Filename: strongdm-4.1.0/strongdm/queries_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/resources_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/remote_identities_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/secret_store_types_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/account_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/nodes_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/__init__.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_resources_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/peering_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_attachments_pb2.py
+Filename: strongdm-4.1.0/strongdm/resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_grants_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/secret_store_types_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/tags_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/nodes_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_attachments_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/account_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_grants_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/account_attachments_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/account_grants_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/activities_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/tags_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_permissions_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/account_attachments_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/errors.py
+Filename: strongdm-4.1.0/strongdm/account_grants_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_attachments_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/client.py
+Filename: strongdm-4.1.0/strongdm/activities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/svc.py
+Filename: strongdm-4.1.0/strongdm/account_permissions_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/queries_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/errors.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/secret_stores_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/peering_groups_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/remote_identity_groups_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/account_attachments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/activities_pb2.py
+Filename: strongdm-4.1.0/strongdm/client.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/secret_stores_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/peering_group_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/role_resources_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/svc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/secret_stores_pb2.py
+Filename: strongdm-4.1.0/strongdm/queries_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/remote_identity_groups_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/secret_stores_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/nodes_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/remote_identity_groups_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_resources_pb2.py
+Filename: strongdm-4.1.0/strongdm/activities_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/role_resources_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/secret_stores_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/options_pb2.py
+Filename: strongdm-4.1.0/strongdm/role_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/secret_stores_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/secret_stores_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/accounts_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/remote_identity_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/control_panel_pb2.py
+Filename: strongdm-4.1.0/strongdm/nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/roles_pb2.py
+Filename: strongdm-4.1.0/strongdm/account_resources_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_attachments_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/role_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/roles_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/options_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/resources_history_pb2.py
+Filename: strongdm-4.1.0/strongdm/secret_stores_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/options_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/accounts_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/organization_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/control_panel_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/secret_store_types_pb2.py
+Filename: strongdm-4.1.0/strongdm/peering_group_peers_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/control_panel_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/roles_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm/account_grants_history_pb2_grpc.py
+Filename: strongdm-4.1.0/strongdm/account_attachments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm.egg-info/dependency_links.txt
+Filename: strongdm-4.1.0/strongdm/roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm.egg-info/top_level.txt
+Filename: strongdm-4.1.0/strongdm/resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm.egg-info/PKG-INFO
+Filename: strongdm-4.1.0/strongdm/options_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm.egg-info/SOURCES.txt
+Filename: strongdm-4.1.0/strongdm/organization_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-4.0.0/strongdm.egg-info/requires.txt
+Filename: strongdm-4.1.0/strongdm/peering_group_nodes_pb2.py
+Comment: 
+
+Filename: strongdm-4.1.0/strongdm/secret_store_types_pb2.py
+Comment: 
+
+Filename: strongdm-4.1.0/strongdm/control_panel_pb2_grpc.py
+Comment: 
+
+Filename: strongdm-4.1.0/strongdm/account_grants_history_pb2_grpc.py
+Comment: 
+
+Filename: strongdm-4.1.0/strongdm.egg-info/dependency_links.txt
+Comment: 
+
+Filename: strongdm-4.1.0/strongdm.egg-info/top_level.txt
+Comment: 
+
+Filename: strongdm-4.1.0/strongdm.egg-info/PKG-INFO
+Comment: 
+
+Filename: strongdm-4.1.0/strongdm.egg-info/SOURCES.txt
+Comment: 
+
+Filename: strongdm-4.1.0/strongdm.egg-info/requires.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `strongdm-4.0.0/setup.py` & `strongdm-4.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 from setuptools import setup
 setup(
     name='strongdm',
     packages=['strongdm'],
-    version='4.0.0',
+    version='4.1.0',
     license='apache-2.0',
     description='strongDM SDK for the Python programming language.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='strongDM Team',
     author_email='sdk-feedback@strongdm.com',
     url='https://github.com/strongdm/strongdm-sdk-python',
     download_url=
-    'https://github.com/strongdm/strongdm-sdk-python/archive/v4.0.0.tar.gz',
+    'https://github.com/strongdm/strongdm-sdk-python/archive/v4.1.0.tar.gz',
     keywords=[
         'strongDM', 'sdm', 'api', 'automation', 'security', 'audit',
         'database', 'server', 'ssh', 'rdp'
     ],
     install_requires=[
         'grpcio>=1.42.0',
         'googleapis-common-protos>1.56.2,<2',
```

## Comparing `strongdm-4.0.0/PKG-INFO` & `strongdm-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 4.0.0
+Version: 4.1.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v4.0.0.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v4.1.0.tar.gz
 Description: # strongDM SDK for Python
         
         This is the official [strongDM](https://www.strongdm.com/) SDK for the Python
         programming language.
         
         Learn more with our [📚strongDM API docs](https://www.strongdm.com/docs/api/) or
         [📓browse the SDK
```

## Comparing `strongdm-4.0.0/README.md` & `strongdm-4.1.0/README.md`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/spec_pb2.py` & `strongdm-4.1.0/strongdm/spec_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/drivers_pb2_grpc.py` & `strongdm-4.1.0/strongdm/drivers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/nodes_pb2.py` & `strongdm-4.1.0/strongdm/nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/accounts_history_pb2.py` & `strongdm-4.1.0/strongdm/accounts_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/roles_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/remote_identity_groups_pb2.py` & `strongdm-4.1.0/strongdm/remote_identity_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/remote_identities_pb2_grpc.py` & `strongdm-4.1.0/strongdm/remote_identities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/remote_identities_pb2.py` & `strongdm-4.1.0/strongdm/remote_identities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_resources_pb2_grpc.py` & `strongdm-4.1.0/strongdm/account_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/drivers_pb2.py` & `strongdm-4.1.0/strongdm/drivers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/role_resources_pb2.py` & `strongdm-4.1.0/strongdm/role_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/roles_history_pb2.py` & `strongdm-4.1.0/strongdm/roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/nodes_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/nodes_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/plumbing.py` & `strongdm-4.1.0/strongdm/plumbing.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 from .accounts_history_pb2 import *
 from .activities_pb2 import *
 from .control_panel_pb2 import *
 from .drivers_pb2 import *
 from .nodes_pb2 import *
 from .nodes_history_pb2 import *
 from .organization_history_pb2 import *
+from .peering_group_nodes_pb2 import *
+from .peering_group_peers_pb2 import *
+from .peering_group_resources_pb2 import *
+from .peering_groups_pb2 import *
 from .queries_pb2 import *
 from .remote_identities_pb2 import *
 from .remote_identities_history_pb2 import *
 from .remote_identity_groups_pb2 import *
 from .remote_identity_groups_history_pb2 import *
 from .replays_pb2 import *
 from .resources_pb2 import *
@@ -5273,14 +5277,623 @@
 def convert_repeated_organization_history_record_to_porcelain(plumbings):
     return [
         convert_organization_history_record_to_porcelain(plumbing)
         for plumbing in plumbings
     ]
 
 
+def convert_peering_group_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroup()
+    porcelain.id = (plumbing.id)
+    porcelain.name = (plumbing.name)
+    return porcelain
+
+
+def convert_peering_group_to_plumbing(porcelain):
+    plumbing = PeeringGroup()
+    if porcelain is None:
+        return plumbing
+    plumbing.id = (porcelain.id)
+    plumbing.name = (porcelain.name)
+    return plumbing
+
+
+def convert_repeated_peering_group_to_plumbing(porcelains):
+    return [
+        convert_peering_group_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_to_porcelain(plumbings):
+    return [
+        convert_peering_group_to_porcelain(plumbing) for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_create_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupCreateResponse()
+    porcelain.meta = convert_create_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.peering_group = convert_peering_group_to_porcelain(
+        plumbing.peering_group)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_create_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupCreateResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_create_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.peering_group.CopyFrom(
+        convert_peering_group_to_plumbing(porcelain.peering_group))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_create_response_to_plumbing(porcelains):
+    return [
+        convert_peering_group_create_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_create_response_to_porcelain(plumbings):
+    return [
+        convert_peering_group_create_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_delete_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupDeleteResponse()
+    porcelain.meta = convert_delete_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_delete_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupDeleteResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_delete_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_delete_response_to_plumbing(porcelains):
+    return [
+        convert_peering_group_delete_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_delete_response_to_porcelain(plumbings):
+    return [
+        convert_peering_group_delete_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_get_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupGetResponse()
+    porcelain.meta = convert_get_response_metadata_to_porcelain(plumbing.meta)
+    porcelain.peering_group = convert_peering_group_to_porcelain(
+        plumbing.peering_group)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_get_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupGetResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_get_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.peering_group.CopyFrom(
+        convert_peering_group_to_plumbing(porcelain.peering_group))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_get_response_to_plumbing(porcelains):
+    return [
+        convert_peering_group_get_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_get_response_to_porcelain(plumbings):
+    return [
+        convert_peering_group_get_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_node_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupNode()
+    porcelain.group_id = (plumbing.group_id)
+    porcelain.id = (plumbing.id)
+    porcelain.node_id = (plumbing.node_id)
+    return porcelain
+
+
+def convert_peering_group_node_to_plumbing(porcelain):
+    plumbing = PeeringGroupNode()
+    if porcelain is None:
+        return plumbing
+    plumbing.group_id = (porcelain.group_id)
+    plumbing.id = (porcelain.id)
+    plumbing.node_id = (porcelain.node_id)
+    return plumbing
+
+
+def convert_repeated_peering_group_node_to_plumbing(porcelains):
+    return [
+        convert_peering_group_node_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_node_to_porcelain(plumbings):
+    return [
+        convert_peering_group_node_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_node_create_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupNodeCreateResponse()
+    porcelain.meta = convert_create_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.peering_group_node = convert_peering_group_node_to_porcelain(
+        plumbing.peering_group_node)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_node_create_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupNodeCreateResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_create_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.peering_group_node.CopyFrom(
+        convert_peering_group_node_to_plumbing(porcelain.peering_group_node))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_node_create_response_to_plumbing(
+        porcelains):
+    return [
+        convert_peering_group_node_create_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_node_create_response_to_porcelain(
+        plumbings):
+    return [
+        convert_peering_group_node_create_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_node_delete_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupNodeDeleteResponse()
+    porcelain.meta = convert_delete_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_node_delete_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupNodeDeleteResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_delete_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_node_delete_response_to_plumbing(
+        porcelains):
+    return [
+        convert_peering_group_node_delete_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_node_delete_response_to_porcelain(
+        plumbings):
+    return [
+        convert_peering_group_node_delete_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_node_get_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupNodeGetResponse()
+    porcelain.meta = convert_get_response_metadata_to_porcelain(plumbing.meta)
+    porcelain.peering_group_node = convert_peering_group_node_to_porcelain(
+        plumbing.peering_group_node)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_node_get_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupNodeGetResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_get_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.peering_group_node.CopyFrom(
+        convert_peering_group_node_to_plumbing(porcelain.peering_group_node))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_node_get_response_to_plumbing(porcelains):
+    return [
+        convert_peering_group_node_get_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_node_get_response_to_porcelain(plumbings):
+    return [
+        convert_peering_group_node_get_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_peer_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupPeer()
+    porcelain.group_id = (plumbing.group_id)
+    porcelain.id = (plumbing.id)
+    porcelain.peers_with_group_id = (plumbing.peers_with_group_id)
+    return porcelain
+
+
+def convert_peering_group_peer_to_plumbing(porcelain):
+    plumbing = PeeringGroupPeer()
+    if porcelain is None:
+        return plumbing
+    plumbing.group_id = (porcelain.group_id)
+    plumbing.id = (porcelain.id)
+    plumbing.peers_with_group_id = (porcelain.peers_with_group_id)
+    return plumbing
+
+
+def convert_repeated_peering_group_peer_to_plumbing(porcelains):
+    return [
+        convert_peering_group_peer_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_peer_to_porcelain(plumbings):
+    return [
+        convert_peering_group_peer_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_peer_create_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupPeerCreateResponse()
+    porcelain.meta = convert_create_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.peering_group_peer = convert_peering_group_peer_to_porcelain(
+        plumbing.peering_group_peer)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_peer_create_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupPeerCreateResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_create_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.peering_group_peer.CopyFrom(
+        convert_peering_group_peer_to_plumbing(porcelain.peering_group_peer))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_peer_create_response_to_plumbing(
+        porcelains):
+    return [
+        convert_peering_group_peer_create_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_peer_create_response_to_porcelain(
+        plumbings):
+    return [
+        convert_peering_group_peer_create_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_peer_delete_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupPeerDeleteResponse()
+    porcelain.meta = convert_delete_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_peer_delete_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupPeerDeleteResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_delete_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_peer_delete_response_to_plumbing(
+        porcelains):
+    return [
+        convert_peering_group_peer_delete_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_peer_delete_response_to_porcelain(
+        plumbings):
+    return [
+        convert_peering_group_peer_delete_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_peer_get_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupPeerGetResponse()
+    porcelain.meta = convert_get_response_metadata_to_porcelain(plumbing.meta)
+    porcelain.peering_group_peer = convert_peering_group_peer_to_porcelain(
+        plumbing.peering_group_peer)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_peer_get_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupPeerGetResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_get_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.peering_group_peer.CopyFrom(
+        convert_peering_group_peer_to_plumbing(porcelain.peering_group_peer))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_peer_get_response_to_plumbing(porcelains):
+    return [
+        convert_peering_group_peer_get_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_peer_get_response_to_porcelain(plumbings):
+    return [
+        convert_peering_group_peer_get_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_resource_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupResource()
+    porcelain.group_id = (plumbing.group_id)
+    porcelain.id = (plumbing.id)
+    porcelain.resource_id = (plumbing.resource_id)
+    return porcelain
+
+
+def convert_peering_group_resource_to_plumbing(porcelain):
+    plumbing = PeeringGroupResource()
+    if porcelain is None:
+        return plumbing
+    plumbing.group_id = (porcelain.group_id)
+    plumbing.id = (porcelain.id)
+    plumbing.resource_id = (porcelain.resource_id)
+    return plumbing
+
+
+def convert_repeated_peering_group_resource_to_plumbing(porcelains):
+    return [
+        convert_peering_group_resource_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_resource_to_porcelain(plumbings):
+    return [
+        convert_peering_group_resource_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_resource_create_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupResourceCreateResponse()
+    porcelain.meta = convert_create_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.peering_group_resource = convert_peering_group_resource_to_porcelain(
+        plumbing.peering_group_resource)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_resource_create_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupResourceCreateResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_create_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.peering_group_resource.CopyFrom(
+        convert_peering_group_resource_to_plumbing(
+            porcelain.peering_group_resource))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_resource_create_response_to_plumbing(
+        porcelains):
+    return [
+        convert_peering_group_resource_create_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_resource_create_response_to_porcelain(
+        plumbings):
+    return [
+        convert_peering_group_resource_create_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_resource_delete_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupResourceDeleteResponse()
+    porcelain.meta = convert_delete_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_resource_delete_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupResourceDeleteResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_delete_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_resource_delete_response_to_plumbing(
+        porcelains):
+    return [
+        convert_peering_group_resource_delete_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_resource_delete_response_to_porcelain(
+        plumbings):
+    return [
+        convert_peering_group_resource_delete_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_peering_group_resource_get_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.PeeringGroupResourceGetResponse()
+    porcelain.meta = convert_get_response_metadata_to_porcelain(plumbing.meta)
+    porcelain.peering_group_resource = convert_peering_group_resource_to_porcelain(
+        plumbing.peering_group_resource)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_peering_group_resource_get_response_to_plumbing(porcelain):
+    plumbing = PeeringGroupResourceGetResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_get_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.peering_group_resource.CopyFrom(
+        convert_peering_group_resource_to_plumbing(
+            porcelain.peering_group_resource))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_peering_group_resource_get_response_to_plumbing(
+        porcelains):
+    return [
+        convert_peering_group_resource_get_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_peering_group_resource_get_response_to_porcelain(
+        plumbings):
+    return [
+        convert_peering_group_resource_get_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
 def convert_postgres_to_porcelain(plumbing):
     if plumbing is None:
         return None
     porcelain = models.Postgres()
     porcelain.bind_interface = (plumbing.bind_interface)
     porcelain.database = (plumbing.database)
     porcelain.egress_filter = (plumbing.egress_filter)
```

## Comparing `strongdm-4.0.0/strongdm/accounts_pb2_grpc.py` & `strongdm-4.1.0/strongdm/accounts_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/replays_pb2.py` & `strongdm-4.1.0/strongdm/replays_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/replays_pb2_grpc.py` & `strongdm-4.1.0/strongdm/replays_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_grants_pb2.py` & `strongdm-4.1.0/strongdm/account_grants_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/organization_history_pb2.py` & `strongdm-4.1.0/strongdm/organization_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_permissions_pb2.py` & `strongdm-4.1.0/strongdm/account_permissions_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/resources_pb2.py` & `strongdm-4.1.0/strongdm/resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/models.py` & `strongdm-4.1.0/strongdm/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -12334,14 +12334,802 @@
         return cls(
             activity_id=d.get('activity_id'),
             organization=d.get('organization'),
             timestamp=d.get('timestamp'),
         )
 
 
+class PeeringGroup:
+    '''
+         PeeringGroups are the building blocks used for explicit network topology making.
+     They may be linked to other peering groups. Sets of PeeringGroupResource and PeeringGroupNode can be attached to a peering group.
+    '''
+    __slots__ = [
+        'id',
+        'name',
+    ]
+
+    def __init__(
+        self,
+        id=None,
+        name=None,
+    ):
+        self.id = id if id is not None else ''
+        '''
+         Unique identifier of the PeeringGroup.
+        '''
+        self.name = name if name is not None else ''
+        '''
+         Unique human-readable name of the PeeringGroup.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroup ' + \
+            'id: ' + repr(self.id) + ' ' +\
+            'name: ' + repr(self.name) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'id': self.id,
+            'name': self.name,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            id=d.get('id'),
+            name=d.get('name'),
+        )
+
+
+class PeeringGroupCreateResponse:
+    '''
+         PeeringGroupCreateResponse reports how the PeeringGroup was created in the system.
+    '''
+    __slots__ = [
+        'meta',
+        'peering_group',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        peering_group=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.peering_group = peering_group if peering_group is not None else None
+        '''
+         The created PeeringGroup.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupCreateResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'peering_group: ' + repr(self.peering_group) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'peering_group': self.peering_group,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            peering_group=d.get('peering_group'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupDeleteResponse:
+    '''
+         PeeringGroupDeleteResponse returns information about a PeeringGroup that was deleted.
+    '''
+    __slots__ = [
+        'meta',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupDeleteResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupGetResponse:
+    '''
+         PeeringGroupGetResponse returns a requested PeeringGroup.
+    '''
+    __slots__ = [
+        'meta',
+        'peering_group',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        peering_group=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.peering_group = peering_group if peering_group is not None else None
+        '''
+         The requested PeeringGroup.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupGetResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'peering_group: ' + repr(self.peering_group) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'peering_group': self.peering_group,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            peering_group=d.get('peering_group'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupNode:
+    '''
+         PeeringGroupNode represents the attachment between a PeeringGroup and a Node.
+    '''
+    __slots__ = [
+        'group_id',
+        'id',
+        'node_id',
+    ]
+
+    def __init__(
+        self,
+        group_id=None,
+        id=None,
+        node_id=None,
+    ):
+        self.group_id = group_id if group_id is not None else ''
+        '''
+         Peering Group ID to which the node will be attached to.
+        '''
+        self.id = id if id is not None else ''
+        '''
+         Unique identifier of the Attachment.
+        '''
+        self.node_id = node_id if node_id is not None else ''
+        '''
+         Node ID to be attached.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupNode ' + \
+            'group_id: ' + repr(self.group_id) + ' ' +\
+            'id: ' + repr(self.id) + ' ' +\
+            'node_id: ' + repr(self.node_id) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'group_id': self.group_id,
+            'id': self.id,
+            'node_id': self.node_id,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            group_id=d.get('group_id'),
+            id=d.get('id'),
+            node_id=d.get('node_id'),
+        )
+
+
+class PeeringGroupNodeCreateResponse:
+    '''
+         PeeringGroupNodeCreateResponse reports how the PeeringGroupNode was created in the system.
+    '''
+    __slots__ = [
+        'meta',
+        'peering_group_node',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        peering_group_node=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.peering_group_node = peering_group_node if peering_group_node is not None else None
+        '''
+         The created PeeringGroupNode.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupNodeCreateResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'peering_group_node: ' + repr(self.peering_group_node) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'peering_group_node': self.peering_group_node,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            peering_group_node=d.get('peering_group_node'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupNodeDeleteResponse:
+    '''
+         PeeringGroupNodeDeleteResponse returns information about a PeeringGroupNode that was deleted.
+    '''
+    __slots__ = [
+        'meta',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupNodeDeleteResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupNodeGetResponse:
+    '''
+         PeeringGroupNodeGetResponse returns a requested PeeringGroupNode.
+    '''
+    __slots__ = [
+        'meta',
+        'peering_group_node',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        peering_group_node=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.peering_group_node = peering_group_node if peering_group_node is not None else None
+        '''
+         The requested PeeringGroupNode.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupNodeGetResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'peering_group_node: ' + repr(self.peering_group_node) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'peering_group_node': self.peering_group_node,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            peering_group_node=d.get('peering_group_node'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupPeer:
+    '''
+         PeeringGroupPeer represents the link between two PeeringGroups
+    '''
+    __slots__ = [
+        'group_id',
+        'id',
+        'peers_with_group_id',
+    ]
+
+    def __init__(
+        self,
+        group_id=None,
+        id=None,
+        peers_with_group_id=None,
+    ):
+        self.group_id = group_id if group_id is not None else ''
+        '''
+         Group ID from which the link will originate.
+        '''
+        self.id = id if id is not None else ''
+        '''
+         Unique identifier of the Attachment.
+        '''
+        self.peers_with_group_id = peers_with_group_id if peers_with_group_id is not None else ''
+        '''
+         Peering Group ID to which Group ID will link.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupPeer ' + \
+            'group_id: ' + repr(self.group_id) + ' ' +\
+            'id: ' + repr(self.id) + ' ' +\
+            'peers_with_group_id: ' + repr(self.peers_with_group_id) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'group_id': self.group_id,
+            'id': self.id,
+            'peers_with_group_id': self.peers_with_group_id,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            group_id=d.get('group_id'),
+            id=d.get('id'),
+            peers_with_group_id=d.get('peers_with_group_id'),
+        )
+
+
+class PeeringGroupPeerCreateResponse:
+    '''
+         PeeringGroupPeerCreateResponse reports how the PeeringGroupPeer was created in the system.
+    '''
+    __slots__ = [
+        'meta',
+        'peering_group_peer',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        peering_group_peer=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.peering_group_peer = peering_group_peer if peering_group_peer is not None else None
+        '''
+         The created PeeringGroupPeer.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupPeerCreateResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'peering_group_peer: ' + repr(self.peering_group_peer) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'peering_group_peer': self.peering_group_peer,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            peering_group_peer=d.get('peering_group_peer'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupPeerDeleteResponse:
+    '''
+         PeeringGroupPeerDeleteResponse returns information about a PeeringGroupPeer that was deleted.
+    '''
+    __slots__ = [
+        'meta',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupPeerDeleteResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupPeerGetResponse:
+    '''
+         PeeringGroupPeerGetResponse returns a requested PeeringGroupPeer.
+    '''
+    __slots__ = [
+        'meta',
+        'peering_group_peer',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        peering_group_peer=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.peering_group_peer = peering_group_peer if peering_group_peer is not None else None
+        '''
+         The requested PeeringGroupPeer.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupPeerGetResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'peering_group_peer: ' + repr(self.peering_group_peer) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'peering_group_peer': self.peering_group_peer,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            peering_group_peer=d.get('peering_group_peer'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupResource:
+    '''
+         PeeringGroupResource represents the attachment between a PeeringGroup and a Resource.
+    '''
+    __slots__ = [
+        'group_id',
+        'id',
+        'resource_id',
+    ]
+
+    def __init__(
+        self,
+        group_id=None,
+        id=None,
+        resource_id=None,
+    ):
+        self.group_id = group_id if group_id is not None else ''
+        '''
+         Peering Group ID to which the resource will be attached to.
+        '''
+        self.id = id if id is not None else ''
+        '''
+         Unique identifier of the Attachment.
+        '''
+        self.resource_id = resource_id if resource_id is not None else ''
+        '''
+         Resource ID to be attached.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupResource ' + \
+            'group_id: ' + repr(self.group_id) + ' ' +\
+            'id: ' + repr(self.id) + ' ' +\
+            'resource_id: ' + repr(self.resource_id) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'group_id': self.group_id,
+            'id': self.id,
+            'resource_id': self.resource_id,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            group_id=d.get('group_id'),
+            id=d.get('id'),
+            resource_id=d.get('resource_id'),
+        )
+
+
+class PeeringGroupResourceCreateResponse:
+    '''
+         PeeringGroupResourceCreateResponse reports how the attachment was created in the system.
+    '''
+    __slots__ = [
+        'meta',
+        'peering_group_resource',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        peering_group_resource=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.peering_group_resource = peering_group_resource if peering_group_resource is not None else None
+        '''
+         The created PeeringGroupResource.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupResourceCreateResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'peering_group_resource: ' + repr(self.peering_group_resource) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'peering_group_resource': self.peering_group_resource,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            peering_group_resource=d.get('peering_group_resource'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupResourceDeleteResponse:
+    '''
+         PeeringGroupResourceDeleteResponse returns information about a PeeringGroupResource that was deleted.
+    '''
+    __slots__ = [
+        'meta',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupResourceDeleteResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class PeeringGroupResourceGetResponse:
+    '''
+         PeeringGroupResourceGetResponse returns a requested PeeringGroupResource.
+    '''
+    __slots__ = [
+        'meta',
+        'peering_group_resource',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        peering_group_resource=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.peering_group_resource = peering_group_resource if peering_group_resource is not None else None
+        '''
+         The requested PeeringGroupResource.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.PeeringGroupResourceGetResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'peering_group_resource: ' + repr(self.peering_group_resource) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'peering_group_resource': self.peering_group_resource,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            peering_group_resource=d.get('peering_group_resource'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
 class Postgres:
     __slots__ = [
         'bind_interface',
         'database',
         'egress_filter',
         'healthy',
         'hostname',
```

## Comparing `strongdm-4.0.0/strongdm/spec_pb2_grpc.py` & `strongdm-4.1.0/strongdm/spec_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/resources_pb2_grpc.py` & `strongdm-4.1.0/strongdm/resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/remote_identities_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/remote_identities_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/tags_pb2.py` & `strongdm-4.1.0/strongdm/tags_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/accounts_pb2.py` & `strongdm-4.1.0/strongdm/accounts_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/constants.py` & `strongdm-4.1.0/strongdm/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,17 @@
     SECRET_STORE = "secretstore"
     REMOTE_IDENTITY_GROUP = "remote_identity_group"
     REMOTE_IDENTITY = "remote_identity"
     ACCESS_REQUEST = "access_request"
     WORKFLOW = "workflow"
     NODE = "node"
     PEERING_GROUP = "peering_group"
+    PEERING_GROUP_NODE = "peering_group_node"
+    PEERING_GROUP_RESOURCE = "peering_group_resource"
+    PEERING_GROUP_PEER = "peering_group_peer"
 
 
 # Activity Verbs, describe which kind of activity has taken place.
 class ActivityVerb:
     USER_ADDED = "user added"
     USER_DELETED = "user deleted"
     USER_UPDATED = "user updated"
```

## Comparing `strongdm-4.0.0/strongdm/role_resources_history_pb2.py` & `strongdm-4.1.0/strongdm/role_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/queries_pb2.py` & `strongdm-4.1.0/strongdm/queries_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/remote_identities_history_pb2.py` & `strongdm-4.1.0/strongdm/remote_identities_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_resources_history_pb2.py` & `strongdm-4.1.0/strongdm/account_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/__init__.py` & `strongdm-4.1.0/strongdm/__init__.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/resources_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/secret_store_types_pb2_grpc.py` & `strongdm-4.1.0/strongdm/secret_store_types_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/nodes_history_pb2.py` & `strongdm-4.1.0/strongdm/nodes_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_resources_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/account_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_attachments_pb2.py` & `strongdm-4.1.0/strongdm/account_attachments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_grants_pb2_grpc.py` & `strongdm-4.1.0/strongdm/account_grants_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/tags_pb2_grpc.py` & `strongdm-4.1.0/strongdm/tags_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_attachments_history_pb2.py` & `strongdm-4.1.0/strongdm/account_attachments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_grants_history_pb2.py` & `strongdm-4.1.0/strongdm/account_grants_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/activities_pb2_grpc.py` & `strongdm-4.1.0/strongdm/activities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_permissions_pb2_grpc.py` & `strongdm-4.1.0/strongdm/account_permissions_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/errors.py` & `strongdm-4.1.0/strongdm/errors.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_attachments_pb2_grpc.py` & `strongdm-4.1.0/strongdm/account_attachments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/client.py` & `strongdm-4.1.0/strongdm/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # These defaults are taken from AWS. Customization of these values
 # is a future step in the API.
 DEFAULT_MAX_RETRIES = 3
 DEFAULT_BASE_RETRY_DELAY = 0.0030  # 30 ms
 DEFAULT_MAX_RETRY_DELAY = 300  # 300 seconds
 API_VERSION = '2021-08-23'
-USER_AGENT = 'strongdm-sdk-python/4.0.0'
+USER_AGENT = 'strongdm-sdk-python/4.1.0'
 
 
 class Client:
     '''Client interacts with the strongDM API.'''
     def __init__(self,
                  api_access_key,
                  api_secret,
@@ -157,14 +157,38 @@
         '''
         self.organization_history = svc.OrganizationHistory(channel, self)
         '''
          OrganizationHistory records all changes to the state of an Organization.
 
         See `strongdm.svc.OrganizationHistory`.
         '''
+        self.peering_group_nodes = svc.PeeringGroupNodes(channel, self)
+        '''
+         PeeringGroupNodes provides the building blocks necessary to obtain attach a node to a peering group.
+
+        See `strongdm.svc.PeeringGroupNodes`.
+        '''
+        self.peering_group_peers = svc.PeeringGroupPeers(channel, self)
+        '''
+         PeeringGroupPeers provides the building blocks necessary to link two peering groups.
+
+        See `strongdm.svc.PeeringGroupPeers`.
+        '''
+        self.peering_group_resources = svc.PeeringGroupResources(channel, self)
+        '''
+         PeeringGroupResources provides the building blocks necessary to obtain attach a resource to a peering group.
+
+        See `strongdm.svc.PeeringGroupResources`.
+        '''
+        self.peering_groups = svc.PeeringGroups(channel, self)
+        '''
+         PeeringGroups provides the building blocks necessary to obtain explicit network topology and routing.
+
+        See `strongdm.svc.PeeringGroups`.
+        '''
         self.queries = svc.Queries(channel, self)
         '''
          A Query is a record of a single client request to a resource, such as a SQL query.
          Long-running SSH, RDP, or Kubernetes interactive sessions also count as queries.
          The Queries service is read-only.
 
         See `strongdm.svc.Queries`.
@@ -332,14 +356,21 @@
             client.channel, client)
         client.account_grants = svc.AccountGrants(client.channel, client)
         client.account_permissions = svc.AccountPermissions(
             client.channel, client)
         client.account_resources = svc.AccountResources(client.channel, client)
         client.accounts = svc.Accounts(client.channel, client)
         client.nodes = svc.Nodes(client.channel, client)
+        client.peering_group_nodes = svc.PeeringGroupNodes(
+            client.channel, client)
+        client.peering_group_peers = svc.PeeringGroupPeers(
+            client.channel, client)
+        client.peering_group_resources = svc.PeeringGroupResources(
+            client.channel, client)
+        client.peering_groups = svc.PeeringGroups(client.channel, client)
         client.remote_identities = svc.RemoteIdentities(client.channel, client)
         client.remote_identity_groups = svc.RemoteIdentityGroups(
             client.channel, client)
         client.resources = svc.Resources(client.channel, client)
         client.role_resources = svc.RoleResources(client.channel, client)
         client.roles = svc.Roles(client.channel, client)
         client.secret_stores = svc.SecretStores(client.channel, client)
@@ -390,14 +421,41 @@
         '''
          Nodes make up the strongDM network, and allow your users to connect securely to your resources. There are two types of nodes:
          - **Gateways** are the entry points into network. They listen for connection from the strongDM client, and provide access to databases and servers.
          - **Relays** are used to extend the strongDM network into segmented subnets. They provide access to databases and servers but do not listen for incoming connections.
 
         See `strongdm.svc.SnapshotNodes`.
         '''
+        self.peering_group_nodes = svc.SnapshotPeeringGroupNodes(
+            client.peering_group_nodes)
+        '''
+         PeeringGroupNodes provides the building blocks necessary to obtain attach a node to a peering group.
+
+        See `strongdm.svc.SnapshotPeeringGroupNodes`.
+        '''
+        self.peering_group_peers = svc.SnapshotPeeringGroupPeers(
+            client.peering_group_peers)
+        '''
+         PeeringGroupPeers provides the building blocks necessary to link two peering groups.
+
+        See `strongdm.svc.SnapshotPeeringGroupPeers`.
+        '''
+        self.peering_group_resources = svc.SnapshotPeeringGroupResources(
+            client.peering_group_resources)
+        '''
+         PeeringGroupResources provides the building blocks necessary to obtain attach a resource to a peering group.
+
+        See `strongdm.svc.SnapshotPeeringGroupResources`.
+        '''
+        self.peering_groups = svc.SnapshotPeeringGroups(client.peering_groups)
+        '''
+         PeeringGroups provides the building blocks necessary to obtain explicit network topology and routing.
+
+        See `strongdm.svc.SnapshotPeeringGroups`.
+        '''
         self.remote_identities = svc.SnapshotRemoteIdentities(
             client.remote_identities)
         '''
          RemoteIdentities assign a resource directly to an account, giving the account the permission to connect to that resource.
 
         See `strongdm.svc.SnapshotRemoteIdentities`.
         '''
```

## Comparing `strongdm-4.0.0/strongdm/svc.py` & `strongdm-4.1.0/strongdm/svc.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,14 +50,22 @@
 from .drivers_pb2_grpc import *
 from .nodes_pb2 import *
 from .nodes_pb2_grpc import *
 from .nodes_history_pb2 import *
 from .nodes_history_pb2_grpc import *
 from .organization_history_pb2 import *
 from .organization_history_pb2_grpc import *
+from .peering_group_nodes_pb2 import *
+from .peering_group_nodes_pb2_grpc import *
+from .peering_group_peers_pb2 import *
+from .peering_group_peers_pb2_grpc import *
+from .peering_group_resources_pb2 import *
+from .peering_group_resources_pb2_grpc import *
+from .peering_groups_pb2 import *
+from .peering_groups_pb2_grpc import *
 from .queries_pb2 import *
 from .queries_pb2_grpc import *
 from .remote_identities_pb2 import *
 from .remote_identities_pb2_grpc import *
 from .remote_identities_history_pb2 import *
 from .remote_identities_history_pb2_grpc import *
 from .remote_identity_groups_pb2 import *
@@ -1429,14 +1437,707 @@
                 if plumbing_response.meta.next_cursor == '':
                     break
                 req.meta.cursor = plumbing_response.meta.next_cursor
 
         return generator(self, req)
 
 
+class PeeringGroupNodes:
+    '''
+     PeeringGroupNodes provides the building blocks necessary to obtain attach a node to a peering group.
+    See `strongdm.models.PeeringGroupNode`.
+    '''
+    def __init__(self, channel, client):
+        self.parent = client
+        self.stub = PeeringGroupNodesStub(channel)
+
+    def create(self, peering_group_node, timeout=None):
+        '''
+         Create attaches a Node to a PeeringGroup
+        '''
+        req = PeeringGroupNodeCreateRequest()
+
+        if peering_group_node is not None:
+            req.peering_group_node.CopyFrom(
+                plumbing.convert_peering_group_node_to_plumbing(
+                    peering_group_node))
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Create(
+                    req,
+                    metadata=self.parent.get_metadata(
+                        'PeeringGroupNodes.Create', req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupNodeCreateResponse()
+        resp.meta = plumbing.convert_create_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.peering_group_node = plumbing.convert_peering_group_node_to_porcelain(
+            plumbing_response.peering_group_node)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def delete(self, id, timeout=None):
+        '''
+         Delete detaches a Node to a PeeringGroup.
+        '''
+        req = PeeringGroupNodeDeleteRequest()
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Delete(
+                    req,
+                    metadata=self.parent.get_metadata(
+                        'PeeringGroupNodes.Delete', req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupNodeDeleteResponse()
+        resp.meta = plumbing.convert_delete_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def get(self, id, timeout=None):
+        '''
+         Get reads the information of one peering group to node attachment.
+        '''
+        req = PeeringGroupNodeGetRequest()
+        if self.parent.snapshot_datetime is not None:
+            req.meta.CopyFrom(GetRequestMetadata())
+            req.meta.snapshot_at.FromDatetime(self.parent.snapshot_datetime)
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Get(
+                    req,
+                    metadata=self.parent.get_metadata('PeeringGroupNodes.Get',
+                                                      req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupNodeGetResponse()
+        resp.meta = plumbing.convert_get_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.peering_group_node = plumbing.convert_peering_group_node_to_porcelain(
+            plumbing_response.peering_group_node)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def list(self, filter, *args, timeout=None):
+        '''
+         List gets a list of peering group node attachments.
+        '''
+        req = PeeringGroupNodeListRequest()
+        req.meta.CopyFrom(ListRequestMetadata())
+        page_size_option = self.parent._test_options.get('PageSize')
+        if isinstance(page_size_option, int):
+            req.meta.limit = page_size_option
+        if self.parent.snapshot_datetime is not None:
+            req.meta.snapshot_at.FromDatetime(self.parent.snapshot_datetime)
+
+        req.filter = plumbing.quote_filter_args(filter, *args)
+
+        def generator(svc, req):
+            tries = 0
+            while True:
+                try:
+                    plumbing_response = svc.stub.List(
+                        req,
+                        metadata=svc.parent.get_metadata(
+                            'PeeringGroupNodes.List', req),
+                        timeout=timeout)
+                except Exception as e:
+                    if self.parent.shouldRetry(tries, e):
+                        tries += 1
+                        self.parent.jitterSleep(tries)
+                        continue
+                    raise plumbing.convert_error_to_porcelain(e) from e
+                tries = 0
+                for plumbing_item in plumbing_response.peering_group_nodes:
+                    yield plumbing.convert_peering_group_node_to_porcelain(
+                        plumbing_item)
+                if plumbing_response.meta.next_cursor == '':
+                    break
+                req.meta.cursor = plumbing_response.meta.next_cursor
+
+        return generator(self, req)
+
+
+class SnapshotPeeringGroupNodes:
+    '''
+    SnapshotPeeringGroupNodes exposes the read only methods of the PeeringGroupNodes
+    service for historical queries.
+    '''
+    def __init__(self, peering_group_nodes):
+        self.peering_group_nodes = peering_group_nodes
+
+    def get(self, id, timeout=None):
+        '''
+         Get reads the information of one peering group to node attachment.
+        '''
+        return self.peering_group_nodes.get(id, timeout=timeout)
+
+    def list(self, filter, *args, timeout=None):
+        '''
+         List gets a list of peering group node attachments.
+        '''
+        return self.peering_group_nodes.list(filter, *args, timeout=timeout)
+
+
+class PeeringGroupPeers:
+    '''
+     PeeringGroupPeers provides the building blocks necessary to link two peering groups.
+    See `strongdm.models.PeeringGroupPeer`.
+    '''
+    def __init__(self, channel, client):
+        self.parent = client
+        self.stub = PeeringGroupPeersStub(channel)
+
+    def create(self, peering_group_peer, timeout=None):
+        '''
+         Create links two peering groups.
+        '''
+        req = PeeringGroupPeerCreateRequest()
+
+        if peering_group_peer is not None:
+            req.peering_group_peer.CopyFrom(
+                plumbing.convert_peering_group_peer_to_plumbing(
+                    peering_group_peer))
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Create(
+                    req,
+                    metadata=self.parent.get_metadata(
+                        'PeeringGroupPeers.Create', req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupPeerCreateResponse()
+        resp.meta = plumbing.convert_create_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.peering_group_peer = plumbing.convert_peering_group_peer_to_porcelain(
+            plumbing_response.peering_group_peer)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def delete(self, id, timeout=None):
+        '''
+         Delete unlinks two peering groups.
+        '''
+        req = PeeringGroupPeerDeleteRequest()
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Delete(
+                    req,
+                    metadata=self.parent.get_metadata(
+                        'PeeringGroupPeers.Delete', req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupPeerDeleteResponse()
+        resp.meta = plumbing.convert_delete_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def get(self, id, timeout=None):
+        '''
+         Get reads the information of one peering group link.
+        '''
+        req = PeeringGroupPeerGetRequest()
+        if self.parent.snapshot_datetime is not None:
+            req.meta.CopyFrom(GetRequestMetadata())
+            req.meta.snapshot_at.FromDatetime(self.parent.snapshot_datetime)
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Get(
+                    req,
+                    metadata=self.parent.get_metadata('PeeringGroupPeers.Get',
+                                                      req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupPeerGetResponse()
+        resp.meta = plumbing.convert_get_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.peering_group_peer = plumbing.convert_peering_group_peer_to_porcelain(
+            plumbing_response.peering_group_peer)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def list(self, filter, *args, timeout=None):
+        '''
+         List gets a list of peering group links.
+        '''
+        req = PeeringGroupPeerListRequest()
+        req.meta.CopyFrom(ListRequestMetadata())
+        page_size_option = self.parent._test_options.get('PageSize')
+        if isinstance(page_size_option, int):
+            req.meta.limit = page_size_option
+        if self.parent.snapshot_datetime is not None:
+            req.meta.snapshot_at.FromDatetime(self.parent.snapshot_datetime)
+
+        req.filter = plumbing.quote_filter_args(filter, *args)
+
+        def generator(svc, req):
+            tries = 0
+            while True:
+                try:
+                    plumbing_response = svc.stub.List(
+                        req,
+                        metadata=svc.parent.get_metadata(
+                            'PeeringGroupPeers.List', req),
+                        timeout=timeout)
+                except Exception as e:
+                    if self.parent.shouldRetry(tries, e):
+                        tries += 1
+                        self.parent.jitterSleep(tries)
+                        continue
+                    raise plumbing.convert_error_to_porcelain(e) from e
+                tries = 0
+                for plumbing_item in plumbing_response.peering_group_peers:
+                    yield plumbing.convert_peering_group_peer_to_porcelain(
+                        plumbing_item)
+                if plumbing_response.meta.next_cursor == '':
+                    break
+                req.meta.cursor = plumbing_response.meta.next_cursor
+
+        return generator(self, req)
+
+
+class SnapshotPeeringGroupPeers:
+    '''
+    SnapshotPeeringGroupPeers exposes the read only methods of the PeeringGroupPeers
+    service for historical queries.
+    '''
+    def __init__(self, peering_group_peers):
+        self.peering_group_peers = peering_group_peers
+
+    def get(self, id, timeout=None):
+        '''
+         Get reads the information of one peering group link.
+        '''
+        return self.peering_group_peers.get(id, timeout=timeout)
+
+    def list(self, filter, *args, timeout=None):
+        '''
+         List gets a list of peering group links.
+        '''
+        return self.peering_group_peers.list(filter, *args, timeout=timeout)
+
+
+class PeeringGroupResources:
+    '''
+     PeeringGroupResources provides the building blocks necessary to obtain attach a resource to a peering group.
+    See `strongdm.models.PeeringGroupResource`.
+    '''
+    def __init__(self, channel, client):
+        self.parent = client
+        self.stub = PeeringGroupResourcesStub(channel)
+
+    def create(self, peering_group_resource, timeout=None):
+        '''
+         Create attaches a Resource to a PeeringGroup
+        '''
+        req = PeeringGroupResourceCreateRequest()
+
+        if peering_group_resource is not None:
+            req.peering_group_resource.CopyFrom(
+                plumbing.convert_peering_group_resource_to_plumbing(
+                    peering_group_resource))
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Create(
+                    req,
+                    metadata=self.parent.get_metadata(
+                        'PeeringGroupResources.Create', req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupResourceCreateResponse()
+        resp.meta = plumbing.convert_create_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.peering_group_resource = plumbing.convert_peering_group_resource_to_porcelain(
+            plumbing_response.peering_group_resource)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def delete(self, id, timeout=None):
+        '''
+         Delete detaches a Resource to a PeeringGroup
+        '''
+        req = PeeringGroupResourceDeleteRequest()
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Delete(
+                    req,
+                    metadata=self.parent.get_metadata(
+                        'PeeringGroupResources.Delete', req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupResourceDeleteResponse()
+        resp.meta = plumbing.convert_delete_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def get(self, id, timeout=None):
+        '''
+         Get reads the information of one peering group to resource attachment.
+        '''
+        req = PeeringGroupResourceGetRequest()
+        if self.parent.snapshot_datetime is not None:
+            req.meta.CopyFrom(GetRequestMetadata())
+            req.meta.snapshot_at.FromDatetime(self.parent.snapshot_datetime)
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Get(
+                    req,
+                    metadata=self.parent.get_metadata(
+                        'PeeringGroupResources.Get', req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupResourceGetResponse()
+        resp.meta = plumbing.convert_get_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.peering_group_resource = plumbing.convert_peering_group_resource_to_porcelain(
+            plumbing_response.peering_group_resource)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def list(self, filter, *args, timeout=None):
+        '''
+         List gets a list of peering group resource attachments.
+        '''
+        req = PeeringGroupResourceListRequest()
+        req.meta.CopyFrom(ListRequestMetadata())
+        page_size_option = self.parent._test_options.get('PageSize')
+        if isinstance(page_size_option, int):
+            req.meta.limit = page_size_option
+        if self.parent.snapshot_datetime is not None:
+            req.meta.snapshot_at.FromDatetime(self.parent.snapshot_datetime)
+
+        req.filter = plumbing.quote_filter_args(filter, *args)
+
+        def generator(svc, req):
+            tries = 0
+            while True:
+                try:
+                    plumbing_response = svc.stub.List(
+                        req,
+                        metadata=svc.parent.get_metadata(
+                            'PeeringGroupResources.List', req),
+                        timeout=timeout)
+                except Exception as e:
+                    if self.parent.shouldRetry(tries, e):
+                        tries += 1
+                        self.parent.jitterSleep(tries)
+                        continue
+                    raise plumbing.convert_error_to_porcelain(e) from e
+                tries = 0
+                for plumbing_item in plumbing_response.peering_group_resources:
+                    yield plumbing.convert_peering_group_resource_to_porcelain(
+                        plumbing_item)
+                if plumbing_response.meta.next_cursor == '':
+                    break
+                req.meta.cursor = plumbing_response.meta.next_cursor
+
+        return generator(self, req)
+
+
+class SnapshotPeeringGroupResources:
+    '''
+    SnapshotPeeringGroupResources exposes the read only methods of the PeeringGroupResources
+    service for historical queries.
+    '''
+    def __init__(self, peering_group_resources):
+        self.peering_group_resources = peering_group_resources
+
+    def get(self, id, timeout=None):
+        '''
+         Get reads the information of one peering group to resource attachment.
+        '''
+        return self.peering_group_resources.get(id, timeout=timeout)
+
+    def list(self, filter, *args, timeout=None):
+        '''
+         List gets a list of peering group resource attachments.
+        '''
+        return self.peering_group_resources.list(filter,
+                                                 *args,
+                                                 timeout=timeout)
+
+
+class PeeringGroups:
+    '''
+     PeeringGroups provides the building blocks necessary to obtain explicit network topology and routing.
+    See `strongdm.models.PeeringGroup`.
+    '''
+    def __init__(self, channel, client):
+        self.parent = client
+        self.stub = PeeringGroupsStub(channel)
+
+    def create(self, peering_group, timeout=None):
+        '''
+         Create registers a new PeeringGroup.
+        '''
+        req = PeeringGroupCreateRequest()
+
+        if peering_group is not None:
+            req.peering_group.CopyFrom(
+                plumbing.convert_peering_group_to_plumbing(peering_group))
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Create(
+                    req,
+                    metadata=self.parent.get_metadata('PeeringGroups.Create',
+                                                      req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupCreateResponse()
+        resp.meta = plumbing.convert_create_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.peering_group = plumbing.convert_peering_group_to_porcelain(
+            plumbing_response.peering_group)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def delete(self, id, timeout=None):
+        '''
+         Delete removes a PeeringGroup by ID.
+        '''
+        req = PeeringGroupDeleteRequest()
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Delete(
+                    req,
+                    metadata=self.parent.get_metadata('PeeringGroups.Delete',
+                                                      req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupDeleteResponse()
+        resp.meta = plumbing.convert_delete_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def get(self, id, timeout=None):
+        '''
+         Get reads one PeeringGroup by ID. It will load all its dependencies.
+        '''
+        req = PeeringGroupGetRequest()
+        if self.parent.snapshot_datetime is not None:
+            req.meta.CopyFrom(GetRequestMetadata())
+            req.meta.snapshot_at.FromDatetime(self.parent.snapshot_datetime)
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Get(
+                    req,
+                    metadata=self.parent.get_metadata('PeeringGroups.Get',
+                                                      req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.PeeringGroupGetResponse()
+        resp.meta = plumbing.convert_get_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.peering_group = plumbing.convert_peering_group_to_porcelain(
+            plumbing_response.peering_group)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def list(self, filter, *args, timeout=None):
+        '''
+         List gets a list of Peering Groups.
+        '''
+        req = PeeringGroupListRequest()
+        req.meta.CopyFrom(ListRequestMetadata())
+        page_size_option = self.parent._test_options.get('PageSize')
+        if isinstance(page_size_option, int):
+            req.meta.limit = page_size_option
+        if self.parent.snapshot_datetime is not None:
+            req.meta.snapshot_at.FromDatetime(self.parent.snapshot_datetime)
+
+        req.filter = plumbing.quote_filter_args(filter, *args)
+
+        def generator(svc, req):
+            tries = 0
+            while True:
+                try:
+                    plumbing_response = svc.stub.List(
+                        req,
+                        metadata=svc.parent.get_metadata(
+                            'PeeringGroups.List', req),
+                        timeout=timeout)
+                except Exception as e:
+                    if self.parent.shouldRetry(tries, e):
+                        tries += 1
+                        self.parent.jitterSleep(tries)
+                        continue
+                    raise plumbing.convert_error_to_porcelain(e) from e
+                tries = 0
+                for plumbing_item in plumbing_response.peering_groups:
+                    yield plumbing.convert_peering_group_to_porcelain(
+                        plumbing_item)
+                if plumbing_response.meta.next_cursor == '':
+                    break
+                req.meta.cursor = plumbing_response.meta.next_cursor
+
+        return generator(self, req)
+
+
+class SnapshotPeeringGroups:
+    '''
+    SnapshotPeeringGroups exposes the read only methods of the PeeringGroups
+    service for historical queries.
+    '''
+    def __init__(self, peering_groups):
+        self.peering_groups = peering_groups
+
+    def get(self, id, timeout=None):
+        '''
+         Get reads one PeeringGroup by ID. It will load all its dependencies.
+        '''
+        return self.peering_groups.get(id, timeout=timeout)
+
+    def list(self, filter, *args, timeout=None):
+        '''
+         List gets a list of Peering Groups.
+        '''
+        return self.peering_groups.list(filter, *args, timeout=timeout)
+
+
 class Queries:
     '''
      A Query is a record of a single client request to a resource, such as a SQL query.
      Long-running SSH, RDP, or Kubernetes interactive sessions also count as queries.
      The Queries service is read-only.
     See `strongdm.models.Query`.
     '''
```

## Comparing `strongdm-4.0.0/strongdm/queries_pb2_grpc.py` & `strongdm-4.1.0/strongdm/queries_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/secret_stores_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/secret_stores_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/remote_identity_groups_history_pb2.py` & `strongdm-4.1.0/strongdm/remote_identity_groups_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/activities_pb2.py` & `strongdm-4.1.0/strongdm/activities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/secret_stores_pb2_grpc.py` & `strongdm-4.1.0/strongdm/secret_stores_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/role_resources_pb2_grpc.py` & `strongdm-4.1.0/strongdm/role_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/secret_stores_pb2.py` & `strongdm-4.1.0/strongdm/secret_stores_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/remote_identity_groups_pb2_grpc.py` & `strongdm-4.1.0/strongdm/remote_identity_groups_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/nodes_pb2_grpc.py` & `strongdm-4.1.0/strongdm/nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_resources_pb2.py` & `strongdm-4.1.0/strongdm/account_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/role_resources_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/role_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/options_pb2.py` & `strongdm-4.1.0/strongdm/options_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\roptions.proto\x12\x02v1\x1a google/protobuf/descriptor.proto\"9\n\x0b\x46ileOptions\x12\x11\n\x07targets\x18\xc4\xc1v \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\x8b\x01\n\x0eServiceOptions\x12\x13\n\tmain_noun\x18\x98\xbfv \x01(\t\x12\x13\n\tid_prefix\x18\x9a\xbfv \x01(\t\x12\x11\n\x07targets\x18\x99\xbfv \x03(\t\x12#\n\x19\x64isable_snapshot_vertical\x18\x9b\xbfv \x01(\x08:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"e\n\rMethodOptions\x12\x10\n\x06method\x18\xb4\xbev \x01(\t\x12\r\n\x03url\x18\xb5\xbev \x01(\t\x12\x1a\n\x10\x64\x65precation_date\x18\xb6\xbev \x01(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xcd\x01\n\x0eMessageOptions\x12\x13\n\tporcelain\x18\xb5\xbev \x01(\x08\x12\x0f\n\x05\x65rror\x18\xb6\xbev \x01(\x05\x12\x17\n\roptions_field\x18\xb7\xbev \x01(\t\x12\x11\n\x07targets\x18\xba\xbev \x03(\t\x12+\n\x0eterraform_docs\x18\xb8\xbev \x01(\x0b\x32\x11.v1.TerraformDocs\x12#\n\x06\x63ustom\x18\xb9\xbev \x01(\x0b\x32\x11.v1.CustomOptions:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"@\n\x0cOneofOptions\x12\x17\n\rcommon_fields\x18\x85\xbfv \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xf8\x03\n\x0c\x46ieldOptions\x12\x13\n\tporcelain\x18\xb6\xbev \x01(\x08\x12\x12\n\x08iterable\x18\xb7\xbev \x01(\x08\x12\x12\n\x08required\x18\xb8\xbev \x01(\x08\x12\x14\n\nwrite_only\x18\xbd\xbev \x01(\x08\x12\x13\n\tread_only\x18\xc3\xbev \x01(\x08\x12\x17\n\ris_credential\x18\xc4\xbev \x01(\x08\x12\x11\n\x07targets\x18\xc6\xbev \x03(\t\x12\x1d\n\x13terraform_force_new\x18\xbc\xbev \x01(\x08\x12\x1d\n\x13terraform_sensitive\x18\xbe\xbev \x01(\x08\x12&\n\x1cterraform_diff_suppress_func\x18\xc7\xbev \x01(\t\x12\x1c\n\x12terraform_computed\x18\xca\xbev \x01(\x08\x12#\n\x06\x63ustom\x18\xb9\xbev \x01(\x0b\x32\x11.v1.CustomOptions\x12\x44\n\x12read_only_override\x18\xc0\xbev \x03(\x0b\x32&.v1.FieldOptions.ReadOnlyOverrideEntry\x12\x13\n\tcondition\x18\xcb\xbev \x01(\t\x1a\x37\n\x15ReadOnlyOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\x8f\x05\n\rCustomOptions\x12\x13\n\tconverter\x18\xbd\xbev \x01(\t\x12O\n\x17porcelain_type_override\x18\xbe\xbev \x03(\x0b\x32,.v1.CustomOptions.PorcelainTypeOverrideEntry\x12O\n\x17porcelain_name_override\x18\xc8\xbev \x03(\x0b\x32,.v1.CustomOptions.PorcelainNameOverrideEntry\x12\x42\n\x10\x63omment_override\x18\xd3\xbev \x03(\x0b\x32&.v1.CustomOptions.CommentOverrideEntry\x12H\n\x13\x64\x65precated_override\x18\xc0\xbev \x03(\x0b\x32).v1.CustomOptions.DeprecatedOverrideEntry\x12\x1d\n\x13terraform_elem_type\x18\xbf\xbev \x01(\t\x12\x12\n\x08unstable\x18\xc1\xbev \x01(\x08\x1a<\n\x1aPorcelainTypeOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a<\n\x1aPorcelainNameOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x36\n\x14\x43ommentOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x39\n\x17\x44\x65precatedOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"m\n\rTerraformDocs\x12\x1f\n\x15resource_example_path\x18\xb4\xbev \x01(\t\x12\"\n\x18\x64\x61ta_source_example_path\x18\xb5\xbev \x01(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway:E\n\x0c\x66ile_options\x12\x1c.google.protobuf.FileOptions\x18\xa8\xc2v \x01(\x0b\x32\x0f.v1.FileOptions:N\n\x0fservice_options\x12\x1f.google.protobuf.ServiceOptions\x18\x99\xbfv \x01(\x0b\x32\x12.v1.ServiceOptions:K\n\x0emethod_options\x12\x1e.google.protobuf.MethodOptions\x18\x90\xbfv \x01(\x0b\x32\x11.v1.MethodOptions:N\n\x0fmessage_options\x12\x1f.google.protobuf.MessageOptions\x18\x8f\xbfv \x01(\x0b\x32\x12.v1.MessageOptions:H\n\roneof_options\x12\x1d.google.protobuf.OneofOptions\x18\x85\xbfv \x01(\x0b\x32\x10.v1.OneofOptions:H\n\rfield_options\x12\x1d.google.protobuf.FieldOptions\x18\x8e\xbfv \x01(\x0b\x32\x10.v1.FieldOptionsBR\n\x19\x63om.strongdm.api.plumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\roptions.proto\x12\x02v1\x1a google/protobuf/descriptor.proto\"9\n\x0b\x46ileOptions\x12\x11\n\x07targets\x18\xc4\xc1v \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xaa\x01\n\x0eServiceOptions\x12\x13\n\tmain_noun\x18\x98\xbfv \x01(\t\x12\x13\n\tid_prefix\x18\x9a\xbfv \x01(\t\x12\x11\n\x07targets\x18\x99\xbfv \x03(\t\x12#\n\x19\x64isable_snapshot_vertical\x18\x9b\xbfv \x01(\x08\x12\x1d\n\x13skip_cli_generation\x18\x9c\xbfv \x01(\x08:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"e\n\rMethodOptions\x12\x10\n\x06method\x18\xb4\xbev \x01(\t\x12\r\n\x03url\x18\xb5\xbev \x01(\t\x12\x1a\n\x10\x64\x65precation_date\x18\xb6\xbev \x01(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xcd\x01\n\x0eMessageOptions\x12\x13\n\tporcelain\x18\xb5\xbev \x01(\x08\x12\x0f\n\x05\x65rror\x18\xb6\xbev \x01(\x05\x12\x17\n\roptions_field\x18\xb7\xbev \x01(\t\x12\x11\n\x07targets\x18\xba\xbev \x03(\t\x12+\n\x0eterraform_docs\x18\xb8\xbev \x01(\x0b\x32\x11.v1.TerraformDocs\x12#\n\x06\x63ustom\x18\xb9\xbev \x01(\x0b\x32\x11.v1.CustomOptions:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"@\n\x0cOneofOptions\x12\x17\n\rcommon_fields\x18\x85\xbfv \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xf8\x03\n\x0c\x46ieldOptions\x12\x13\n\tporcelain\x18\xb6\xbev \x01(\x08\x12\x12\n\x08iterable\x18\xb7\xbev \x01(\x08\x12\x12\n\x08required\x18\xb8\xbev \x01(\x08\x12\x14\n\nwrite_only\x18\xbd\xbev \x01(\x08\x12\x13\n\tread_only\x18\xc3\xbev \x01(\x08\x12\x17\n\ris_credential\x18\xc4\xbev \x01(\x08\x12\x11\n\x07targets\x18\xc6\xbev \x03(\t\x12\x1d\n\x13terraform_force_new\x18\xbc\xbev \x01(\x08\x12\x1d\n\x13terraform_sensitive\x18\xbe\xbev \x01(\x08\x12&\n\x1cterraform_diff_suppress_func\x18\xc7\xbev \x01(\t\x12\x1c\n\x12terraform_computed\x18\xca\xbev \x01(\x08\x12#\n\x06\x63ustom\x18\xb9\xbev \x01(\x0b\x32\x11.v1.CustomOptions\x12\x44\n\x12read_only_override\x18\xc0\xbev \x03(\x0b\x32&.v1.FieldOptions.ReadOnlyOverrideEntry\x12\x13\n\tcondition\x18\xcb\xbev \x01(\t\x1a\x37\n\x15ReadOnlyOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\x8f\x05\n\rCustomOptions\x12\x13\n\tconverter\x18\xbd\xbev \x01(\t\x12O\n\x17porcelain_type_override\x18\xbe\xbev \x03(\x0b\x32,.v1.CustomOptions.PorcelainTypeOverrideEntry\x12O\n\x17porcelain_name_override\x18\xc8\xbev \x03(\x0b\x32,.v1.CustomOptions.PorcelainNameOverrideEntry\x12\x42\n\x10\x63omment_override\x18\xd3\xbev \x03(\x0b\x32&.v1.CustomOptions.CommentOverrideEntry\x12H\n\x13\x64\x65precated_override\x18\xc0\xbev \x03(\x0b\x32).v1.CustomOptions.DeprecatedOverrideEntry\x12\x1d\n\x13terraform_elem_type\x18\xbf\xbev \x01(\t\x12\x12\n\x08unstable\x18\xc1\xbev \x01(\x08\x1a<\n\x1aPorcelainTypeOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a<\n\x1aPorcelainNameOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x36\n\x14\x43ommentOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x39\n\x17\x44\x65precatedOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"m\n\rTerraformDocs\x12\x1f\n\x15resource_example_path\x18\xb4\xbev \x01(\t\x12\"\n\x18\x64\x61ta_source_example_path\x18\xb5\xbev \x01(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway:E\n\x0c\x66ile_options\x12\x1c.google.protobuf.FileOptions\x18\xa8\xc2v \x01(\x0b\x32\x0f.v1.FileOptions:N\n\x0fservice_options\x12\x1f.google.protobuf.ServiceOptions\x18\x99\xbfv \x01(\x0b\x32\x12.v1.ServiceOptions:K\n\x0emethod_options\x12\x1e.google.protobuf.MethodOptions\x18\x90\xbfv \x01(\x0b\x32\x11.v1.MethodOptions:N\n\x0fmessage_options\x12\x1f.google.protobuf.MessageOptions\x18\x8f\xbfv \x01(\x0b\x32\x12.v1.MessageOptions:H\n\roneof_options\x12\x1d.google.protobuf.OneofOptions\x18\x85\xbfv \x01(\x0b\x32\x10.v1.OneofOptions:H\n\rfield_options\x12\x1d.google.protobuf.FieldOptions\x18\x8e\xbfv \x01(\x0b\x32\x10.v1.FieldOptionsBR\n\x19\x63om.strongdm.api.plumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
 
 
 FILE_OPTIONS_FIELD_NUMBER = 1941800
 file_options = DESCRIPTOR.extensions_by_name['file_options']
 SERVICE_OPTIONS_FIELD_NUMBER = 1941401
 service_options = DESCRIPTOR.extensions_by_name['service_options']
 METHOD_OPTIONS_FIELD_NUMBER = 1941392
@@ -189,31 +189,31 @@
   _CUSTOMOPTIONS._options = None
   _CUSTOMOPTIONS._serialized_options = b'\372\370\263\007\022\322\363\263\007\r!json_gateway'
   _TERRAFORMDOCS._options = None
   _TERRAFORMDOCS._serialized_options = b'\372\370\263\007\022\322\363\263\007\r!json_gateway'
   _FILEOPTIONS._serialized_start=55
   _FILEOPTIONS._serialized_end=112
   _SERVICEOPTIONS._serialized_start=115
-  _SERVICEOPTIONS._serialized_end=254
-  _METHODOPTIONS._serialized_start=256
-  _METHODOPTIONS._serialized_end=357
-  _MESSAGEOPTIONS._serialized_start=360
-  _MESSAGEOPTIONS._serialized_end=565
-  _ONEOFOPTIONS._serialized_start=567
-  _ONEOFOPTIONS._serialized_end=631
-  _FIELDOPTIONS._serialized_start=634
-  _FIELDOPTIONS._serialized_end=1138
-  _FIELDOPTIONS_READONLYOVERRIDEENTRY._serialized_start=1058
-  _FIELDOPTIONS_READONLYOVERRIDEENTRY._serialized_end=1113
-  _CUSTOMOPTIONS._serialized_start=1141
-  _CUSTOMOPTIONS._serialized_end=1796
-  _CUSTOMOPTIONS_PORCELAINTYPEOVERRIDEENTRY._serialized_start=1534
-  _CUSTOMOPTIONS_PORCELAINTYPEOVERRIDEENTRY._serialized_end=1594
-  _CUSTOMOPTIONS_PORCELAINNAMEOVERRIDEENTRY._serialized_start=1596
-  _CUSTOMOPTIONS_PORCELAINNAMEOVERRIDEENTRY._serialized_end=1656
-  _CUSTOMOPTIONS_COMMENTOVERRIDEENTRY._serialized_start=1658
-  _CUSTOMOPTIONS_COMMENTOVERRIDEENTRY._serialized_end=1712
-  _CUSTOMOPTIONS_DEPRECATEDOVERRIDEENTRY._serialized_start=1714
-  _CUSTOMOPTIONS_DEPRECATEDOVERRIDEENTRY._serialized_end=1771
-  _TERRAFORMDOCS._serialized_start=1798
-  _TERRAFORMDOCS._serialized_end=1907
+  _SERVICEOPTIONS._serialized_end=285
+  _METHODOPTIONS._serialized_start=287
+  _METHODOPTIONS._serialized_end=388
+  _MESSAGEOPTIONS._serialized_start=391
+  _MESSAGEOPTIONS._serialized_end=596
+  _ONEOFOPTIONS._serialized_start=598
+  _ONEOFOPTIONS._serialized_end=662
+  _FIELDOPTIONS._serialized_start=665
+  _FIELDOPTIONS._serialized_end=1169
+  _FIELDOPTIONS_READONLYOVERRIDEENTRY._serialized_start=1089
+  _FIELDOPTIONS_READONLYOVERRIDEENTRY._serialized_end=1144
+  _CUSTOMOPTIONS._serialized_start=1172
+  _CUSTOMOPTIONS._serialized_end=1827
+  _CUSTOMOPTIONS_PORCELAINTYPEOVERRIDEENTRY._serialized_start=1565
+  _CUSTOMOPTIONS_PORCELAINTYPEOVERRIDEENTRY._serialized_end=1625
+  _CUSTOMOPTIONS_PORCELAINNAMEOVERRIDEENTRY._serialized_start=1627
+  _CUSTOMOPTIONS_PORCELAINNAMEOVERRIDEENTRY._serialized_end=1687
+  _CUSTOMOPTIONS_COMMENTOVERRIDEENTRY._serialized_start=1689
+  _CUSTOMOPTIONS_COMMENTOVERRIDEENTRY._serialized_end=1743
+  _CUSTOMOPTIONS_DEPRECATEDOVERRIDEENTRY._serialized_start=1745
+  _CUSTOMOPTIONS_DEPRECATEDOVERRIDEENTRY._serialized_end=1802
+  _TERRAFORMDOCS._serialized_start=1829
+  _TERRAFORMDOCS._serialized_end=1938
 # @@protoc_insertion_point(module_scope)
```

## Comparing `strongdm-4.0.0/strongdm/secret_stores_history_pb2.py` & `strongdm-4.1.0/strongdm/secret_stores_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/accounts_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/accounts_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/control_panel_pb2.py` & `strongdm-4.1.0/strongdm/control_panel_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/roles_pb2.py` & `strongdm-4.1.0/strongdm/roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_attachments_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/account_attachments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/roles_pb2_grpc.py` & `strongdm-4.1.0/strongdm/roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/resources_history_pb2.py` & `strongdm-4.1.0/strongdm/resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/options_pb2_grpc.py` & `strongdm-4.1.0/strongdm/options_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/organization_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/organization_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/secret_store_types_pb2.py` & `strongdm-4.1.0/strongdm/secret_store_types_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/control_panel_pb2_grpc.py` & `strongdm-4.1.0/strongdm/control_panel_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm/account_grants_history_pb2_grpc.py` & `strongdm-4.1.0/strongdm/account_grants_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-4.0.0/strongdm.egg-info/PKG-INFO` & `strongdm-4.1.0/strongdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 4.0.0
+Version: 4.1.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v4.0.0.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v4.1.0.tar.gz
 Description: # strongDM SDK for Python
         
         This is the official [strongDM](https://www.strongdm.com/) SDK for the Python
         programming language.
         
         Learn more with our [📚strongDM API docs](https://www.strongdm.com/docs/api/) or
         [📓browse the SDK
```

## Comparing `strongdm-4.0.0/strongdm.egg-info/SOURCES.txt` & `strongdm-4.1.0/strongdm.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -33,14 +33,22 @@
 strongdm/nodes_history_pb2_grpc.py
 strongdm/nodes_pb2.py
 strongdm/nodes_pb2_grpc.py
 strongdm/options_pb2.py
 strongdm/options_pb2_grpc.py
 strongdm/organization_history_pb2.py
 strongdm/organization_history_pb2_grpc.py
+strongdm/peering_group_nodes_pb2.py
+strongdm/peering_group_nodes_pb2_grpc.py
+strongdm/peering_group_peers_pb2.py
+strongdm/peering_group_peers_pb2_grpc.py
+strongdm/peering_group_resources_pb2.py
+strongdm/peering_group_resources_pb2_grpc.py
+strongdm/peering_groups_pb2.py
+strongdm/peering_groups_pb2_grpc.py
 strongdm/plumbing.py
 strongdm/queries_pb2.py
 strongdm/queries_pb2_grpc.py
 strongdm/remote_identities_history_pb2.py
 strongdm/remote_identities_history_pb2_grpc.py
 strongdm/remote_identities_pb2.py
 strongdm/remote_identities_pb2_grpc.py
```

