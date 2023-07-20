# Comparing `tmp/types-ldap3-2.9.8.tar.gz` & `tmp/types-ldap3-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-ldap3-2.9.8.tar", last modified: Sat Apr 16 01:23:37 2022, max compression
+gzip compressed data, was "types-ldap3-2.9.9.tar", last modified: Thu May 26 15:22:59 2022, max compression
```

## Comparing `types-ldap3-2.9.8.tar` & `types-ldap3-2.9.9.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.412336 types-ldap3-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-04-16 01:23:36.000000 types-ldap3-2.9.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-16 01:23:36.000000 types-ldap3-2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-04-16 01:23:37.412336 types-ldap3-2.9.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.404336 types-ldap3-2.9.8/ldap3-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-04-16 01:23:36.000000 types-ldap3-2.9.8/ldap3-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.404336 types-ldap3-2.9.8/ldap3-stubs/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/abstract/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/abstract/attrDef.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/abstract/attribute.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/abstract/cursor.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/abstract/entry.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/abstract/objectDef.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.404336 types-ldap3-2.9.8/ldap3-stubs/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5924 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7294 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/pooling.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/rdns.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/results.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/server.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/timezone.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/tls.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/core/usage.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.404336 types-ldap3-2.9.8/ldap3-stubs/extend/
--rw-r--r--   0 runner    (1001) docker     (121)     3975 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.404336 types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/addMembersToGroups.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/dirSync.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/modifyPassword.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/persistentSearch.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/removeMembersFromGroups.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/unlockAccount.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.408336 types-ldap3-2.9.8/ldap3-stubs/extend/novell/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/addMembersToGroups.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/checkGroupsMemberships.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/endTransaction.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/getBindDn.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/listReplicas.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/nmasGetUniversalPassword.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/nmasSetUniversalPassword.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/partition_entry_count.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/removeMembersFromGroups.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/replicaInfo.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/novell/startTransaction.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/operation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.408336 types-ldap3-2.9.8/ldap3-stubs/extend/standard/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/standard/PagedSearch.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/standard/PersistentSearch.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/standard/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/standard/modifyPassword.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/extend/standard/whoAmI.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.408336 types-ldap3-2.9.8/ldap3-stubs/operation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/abandon.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/add.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/bind.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/compare.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/extended.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/modify.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/modifyDn.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/search.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/operation/unbind.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.408336 types-ldap3-2.9.8/ldap3-stubs/protocol/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/controls.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/convert.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.408336 types-ldap3-2.9.8/ldap3-stubs/protocol/formatters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/formatters/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/formatters/formatters.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/formatters/standard.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/formatters/validators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/microsoft.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/novell.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/oid.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/persistentSearch.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/rfc2696.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/rfc2849.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/rfc3062.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6048 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/rfc4511.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/rfc4512.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/rfc4527.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.408336 types-ldap3-2.9.8/ldap3-stubs/protocol/sasl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/sasl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/sasl/digestMd5.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/sasl/external.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/sasl/kerberos.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/sasl/plain.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/sasl/sasl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.412336 types-ldap3-2.9.8/ldap3-stubs/protocol/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/schemas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/schemas/ad2012R2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/schemas/ds389.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/schemas/edir888.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/schemas/edir914.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/protocol/schemas/slapd24.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.412336 types-ldap3-2.9.8/ldap3-stubs/strategy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/asyncStream.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/asynchronous.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/ldifProducer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/mockAsync.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/mockBase.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/mockSync.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/restartable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/reusable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/safeRestartable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/safeSync.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/strategy/sync.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.412336 types-ldap3-2.9.8/ldap3-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/asn1.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/ciDict.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/conv.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/dn.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/hashed.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/log.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/ntlm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/port_validators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/repr.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/tls_backport.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/utils/uri.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-04-16 01:22:12.000000 types-ldap3-2.9.8/ldap3-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-16 01:23:37.412336 types-ldap3-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4506 2022-04-16 01:23:36.000000 types-ldap3-2.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 01:23:37.412336 types-ldap3-2.9.8/types_ldap3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-04-16 01:23:37.000000 types-ldap3-2.9.8/types_ldap3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4225 2022-04-16 01:23:37.000000 types-ldap3-2.9.8/types_ldap3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-16 01:23:37.000000 types-ldap3-2.9.8/types_ldap3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-16 01:23:37.000000 types-ldap3-2.9.8/types_ldap3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:59.003727 types-ldap3-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-05-26 15:22:58.000000 types-ldap3-2.9.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-26 15:22:58.000000 types-ldap3-2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-05-26 15:22:59.003727 types-ldap3-2.9.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.975725 types-ldap3-2.9.9/ldap3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-26 15:22:58.000000 types-ldap3-2.9.9/ldap3-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.975725 types-ldap3-2.9.9/ldap3-stubs/abstract/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/abstract/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/abstract/attrDef.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/abstract/attribute.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/abstract/cursor.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/abstract/entry.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/abstract/objectDef.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.979725 types-ldap3-2.9.9/ldap3-stubs/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5924 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7294 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/pooling.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/rdns.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/results.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/timezone.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/tls.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/core/usage.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.979725 types-ldap3-2.9.9/ldap3-stubs/extend/
+-rw-r--r--   0 runner    (1001) docker     (121)     3975 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.983725 types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/addMembersToGroups.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/dirSync.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/modifyPassword.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/persistentSearch.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/removeMembersFromGroups.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/unlockAccount.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.983725 types-ldap3-2.9.9/ldap3-stubs/extend/novell/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/addMembersToGroups.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/checkGroupsMemberships.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/endTransaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/getBindDn.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/listReplicas.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/nmasGetUniversalPassword.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/nmasSetUniversalPassword.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/partition_entry_count.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/removeMembersFromGroups.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/replicaInfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/novell/startTransaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/operation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.987725 types-ldap3-2.9.9/ldap3-stubs/extend/standard/
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/standard/PagedSearch.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/standard/PersistentSearch.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/standard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/standard/modifyPassword.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/extend/standard/whoAmI.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.987725 types-ldap3-2.9.9/ldap3-stubs/operation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/abandon.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/add.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/bind.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/compare.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/delete.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/extended.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/modify.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/modifyDn.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/operation/unbind.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.991726 types-ldap3-2.9.9/ldap3-stubs/protocol/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/controls.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/convert.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.991726 types-ldap3-2.9.9/ldap3-stubs/protocol/formatters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/formatters/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/formatters/formatters.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/formatters/standard.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/formatters/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/microsoft.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/novell.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/oid.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/persistentSearch.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/rfc2696.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/rfc2849.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/rfc3062.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6048 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/rfc4511.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/rfc4512.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/rfc4527.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.995726 types-ldap3-2.9.9/ldap3-stubs/protocol/sasl/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/sasl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/sasl/digestMd5.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/sasl/external.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/sasl/kerberos.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/sasl/plain.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/sasl/sasl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.995726 types-ldap3-2.9.9/ldap3-stubs/protocol/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/schemas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/schemas/ad2012R2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/schemas/ds389.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/schemas/edir888.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/schemas/edir914.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/protocol/schemas/slapd24.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.999726 types-ldap3-2.9.9/ldap3-stubs/strategy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/asyncStream.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/asynchronous.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/ldifProducer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/mockAsync.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/mockBase.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/mockSync.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/restartable.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/reusable.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/safeRestartable.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/safeSync.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/strategy/sync.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:58.999726 types-ldap3-2.9.9/ldap3-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/asn1.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/ciDict.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/conv.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/dn.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/hashed.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/ntlm.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/port_validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/repr.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/tls_backport.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/utils/uri.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-26 15:22:38.000000 types-ldap3-2.9.9/ldap3-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-26 15:22:59.003727 types-ldap3-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4555 2022-05-26 15:22:58.000000 types-ldap3-2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 15:22:59.003727 types-ldap3-2.9.9/types_ldap3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-05-26 15:22:58.000000 types-ldap3-2.9.9/types_ldap3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4225 2022-05-26 15:22:58.000000 types-ldap3-2.9.9/types_ldap3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 15:22:58.000000 types-ldap3-2.9.9/types_ldap3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-26 15:22:58.000000 types-ldap3-2.9.9/types_ldap3.egg-info/top_level.txt
```

### Comparing `types-ldap3-2.9.8/CHANGELOG.md` & `types-ldap3-2.9.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.9.9 (2022-05-26)
+
+Third-party stubs: fix several fictitious type aliases (#7958)
+
 ## 2.9.8 (2022-04-16)
 
 Use `TypeAlias` where possible for type aliases (#7630)
 
 ## 2.9.7 (2022-03-06)
 
 Upgrade to stubtest with dunder pos only reverted (#7442)
```

### Comparing `types-ldap3-2.9.8/PKG-INFO` & `types-ldap3-2.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: types-ldap3
-Version: 2.9.8
+Version: 2.9.9
 Summary: Typing stubs for ldap3
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ldap3.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for ldap3
 
 This is a PEP 561 type stub package for the `ldap3` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `ldap3`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/ldap3. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `740193a8fc6499287de32e24484a3cd734c20f09`.
+This package was generated from typeshed commit `466f9c2ad7bb65702b268081bcc753778f43f6a0`.
```

### Comparing `types-ldap3-2.9.8/ldap3-stubs/__init__.pyi` & `types-ldap3-2.9.9/ldap3-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/abstract/attrDef.pyi` & `types-ldap3-2.9.9/ldap3-stubs/abstract/attrDef.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/abstract/attribute.pyi` & `types-ldap3-2.9.9/ldap3-stubs/abstract/attribute.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/abstract/cursor.pyi` & `types-ldap3-2.9.9/ldap3-stubs/abstract/cursor.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/abstract/entry.pyi` & `types-ldap3-2.9.9/ldap3-stubs/abstract/entry.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/abstract/objectDef.pyi` & `types-ldap3-2.9.9/ldap3-stubs/abstract/objectDef.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/core/connection.pyi` & `types-ldap3-2.9.9/ldap3-stubs/core/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/core/exceptions.pyi` & `types-ldap3-2.9.9/ldap3-stubs/core/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/core/pooling.pyi` & `types-ldap3-2.9.9/ldap3-stubs/core/pooling.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/core/results.pyi` & `types-ldap3-2.9.9/ldap3-stubs/core/results.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/core/server.pyi` & `types-ldap3-2.9.9/ldap3-stubs/core/server.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/core/tls.pyi` & `types-ldap3-2.9.9/ldap3-stubs/core/tls.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/core/usage.pyi` & `types-ldap3-2.9.9/ldap3-stubs/core/usage.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/extend/__init__.pyi` & `types-ldap3-2.9.9/ldap3-stubs/extend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/dirSync.pyi` & `types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/dirSync.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/extend/microsoft/persistentSearch.pyi` & `types-ldap3-2.9.9/ldap3-stubs/extend/microsoft/persistentSearch.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/extend/operation.pyi` & `types-ldap3-2.9.9/ldap3-stubs/extend/operation.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/extend/standard/PagedSearch.pyi` & `types-ldap3-2.9.9/ldap3-stubs/extend/standard/PagedSearch.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/extend/standard/PersistentSearch.pyi` & `types-ldap3-2.9.9/ldap3-stubs/extend/standard/PersistentSearch.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/extend/standard/modifyPassword.pyi` & `types-ldap3-2.9.9/ldap3-stubs/extend/standard/modifyPassword.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/operation/bind.pyi` & `types-ldap3-2.9.9/ldap3-stubs/operation/bind.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/operation/search.pyi` & `types-ldap3-2.9.9/ldap3-stubs/operation/search.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/convert.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/convert.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/formatters/validators.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/formatters/validators.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/microsoft.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/microsoft.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/novell.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/novell.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/oid.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/oid.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/rfc2849.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/rfc2849.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/rfc3062.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/rfc3062.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/rfc4511.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/rfc4511.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/protocol/rfc4512.pyi` & `types-ldap3-2.9.9/ldap3-stubs/protocol/rfc4512.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/strategy/asynchronous.pyi` & `types-ldap3-2.9.9/ldap3-stubs/strategy/asynchronous.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/strategy/base.pyi` & `types-ldap3-2.9.9/ldap3-stubs/strategy/base.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/strategy/ldifProducer.pyi` & `types-ldap3-2.9.9/ldap3-stubs/strategy/ldifProducer.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/strategy/mockBase.pyi` & `types-ldap3-2.9.9/ldap3-stubs/strategy/mockBase.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/strategy/restartable.pyi` & `types-ldap3-2.9.9/ldap3-stubs/strategy/restartable.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/strategy/reusable.pyi` & `types-ldap3-2.9.9/ldap3-stubs/strategy/reusable.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/strategy/sync.pyi` & `types-ldap3-2.9.9/ldap3-stubs/strategy/sync.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/utils/asn1.pyi` & `types-ldap3-2.9.9/ldap3-stubs/utils/asn1.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
+from typing_extensions import TypeAlias
 
 # Enable when pyasn1 gets stubs:
-# from pyasn1.codec.ber.encoder import AbstractItemEncoder, BooleanEncoder
-AbstractItemEncoder = Any
-BooleanEncoder = Any
+# from pyasn1.codec.ber.encoder import AbstractItemEncoder
+AbstractItemEncoder: TypeAlias = Any
 
 CLASSES: Any
 
 class LDAPBooleanEncoder(AbstractItemEncoder):
     supportIndefLenMode: bool
     # Requires pyasn1 > 0.3.7
     def encodeValue(self, value, asn1Spec, encodeFun, **options): ...
```

### Comparing `types-ldap3-2.9.8/ldap3-stubs/utils/ciDict.pyi` & `types-ldap3-2.9.9/ldap3-stubs/utils/ciDict.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/utils/conv.pyi` & `types-ldap3-2.9.9/ldap3-stubs/utils/conv.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/utils/log.pyi` & `types-ldap3-2.9.9/ldap3-stubs/utils/log.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/ldap3-stubs/utils/ntlm.pyi` & `types-ldap3-2.9.9/ldap3-stubs/utils/ntlm.pyi`

 * *Files identical despite different names*

### Comparing `types-ldap3-2.9.8/setup.py` & `types-ldap3-2.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `ldap3` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `ldap3`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/ldap3. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `740193a8fc6499287de32e24484a3cd734c20f09`.
+This package was generated from typeshed commit `466f9c2ad7bb65702b268081bcc753778f43f6a0`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.9.8",
+      version="2.9.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ldap3.md",
@@ -29,10 +29,11 @@
       },
       install_requires=[],
       packages=['ldap3-stubs'],
       package_data={'ldap3-stubs': ['__init__.pyi', 'abstract/__init__.pyi', 'abstract/attrDef.pyi', 'abstract/attribute.pyi', 'abstract/cursor.pyi', 'abstract/entry.pyi', 'abstract/objectDef.pyi', 'core/__init__.pyi', 'core/connection.pyi', 'core/exceptions.pyi', 'core/pooling.pyi', 'core/rdns.pyi', 'core/results.pyi', 'core/server.pyi', 'core/timezone.pyi', 'core/tls.pyi', 'core/usage.pyi', 'extend/__init__.pyi', 'extend/microsoft/__init__.pyi', 'extend/microsoft/addMembersToGroups.pyi', 'extend/microsoft/dirSync.pyi', 'extend/microsoft/modifyPassword.pyi', 'extend/microsoft/persistentSearch.pyi', 'extend/microsoft/removeMembersFromGroups.pyi', 'extend/microsoft/unlockAccount.pyi', 'extend/novell/__init__.pyi', 'extend/novell/addMembersToGroups.pyi', 'extend/novell/checkGroupsMemberships.pyi', 'extend/novell/endTransaction.pyi', 'extend/novell/getBindDn.pyi', 'extend/novell/listReplicas.pyi', 'extend/novell/nmasGetUniversalPassword.pyi', 'extend/novell/nmasSetUniversalPassword.pyi', 'extend/novell/partition_entry_count.pyi', 'extend/novell/removeMembersFromGroups.pyi', 'extend/novell/replicaInfo.pyi', 'extend/novell/startTransaction.pyi', 'extend/operation.pyi', 'extend/standard/PagedSearch.pyi', 'extend/standard/PersistentSearch.pyi', 'extend/standard/__init__.pyi', 'extend/standard/modifyPassword.pyi', 'extend/standard/whoAmI.pyi', 'operation/__init__.pyi', 'operation/abandon.pyi', 'operation/add.pyi', 'operation/bind.pyi', 'operation/compare.pyi', 'operation/delete.pyi', 'operation/extended.pyi', 'operation/modify.pyi', 'operation/modifyDn.pyi', 'operation/search.pyi', 'operation/unbind.pyi', 'protocol/__init__.pyi', 'protocol/controls.pyi', 'protocol/convert.pyi', 'protocol/formatters/__init__.pyi', 'protocol/formatters/formatters.pyi', 'protocol/formatters/standard.pyi', 'protocol/formatters/validators.pyi', 'protocol/microsoft.pyi', 'protocol/novell.pyi', 'protocol/oid.pyi', 'protocol/persistentSearch.pyi', 'protocol/rfc2696.pyi', 'protocol/rfc2849.pyi', 'protocol/rfc3062.pyi', 'protocol/rfc4511.pyi', 'protocol/rfc4512.pyi', 'protocol/rfc4527.pyi', 'protocol/sasl/__init__.pyi', 'protocol/sasl/digestMd5.pyi', 'protocol/sasl/external.pyi', 'protocol/sasl/kerberos.pyi', 'protocol/sasl/plain.pyi', 'protocol/sasl/sasl.pyi', 'protocol/schemas/__init__.pyi', 'protocol/schemas/ad2012R2.pyi', 'protocol/schemas/ds389.pyi', 'protocol/schemas/edir888.pyi', 'protocol/schemas/edir914.pyi', 'protocol/schemas/slapd24.pyi', 'strategy/__init__.pyi', 'strategy/asyncStream.pyi', 'strategy/asynchronous.pyi', 'strategy/base.pyi', 'strategy/ldifProducer.pyi', 'strategy/mockAsync.pyi', 'strategy/mockBase.pyi', 'strategy/mockSync.pyi', 'strategy/restartable.pyi', 'strategy/reusable.pyi', 'strategy/safeRestartable.pyi', 'strategy/safeSync.pyi', 'strategy/sync.pyi', 'utils/__init__.pyi', 'utils/asn1.pyi', 'utils/ciDict.pyi', 'utils/config.pyi', 'utils/conv.pyi', 'utils/dn.pyi', 'utils/hashed.pyi', 'utils/log.pyi', 'utils/ntlm.pyi', 'utils/port_validators.pyi', 'utils/repr.pyi', 'utils/tls_backport.pyi', 'utils/uri.pyi', 'version.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
+          "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-ldap3-2.9.8/types_ldap3.egg-info/PKG-INFO` & `types-ldap3-2.9.9/types_ldap3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: types-ldap3
-Version: 2.9.8
+Version: 2.9.9
 Summary: Typing stubs for ldap3
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ldap3.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for ldap3
 
 This is a PEP 561 type stub package for the `ldap3` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `ldap3`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/ldap3. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `740193a8fc6499287de32e24484a3cd734c20f09`.
+This package was generated from typeshed commit `466f9c2ad7bb65702b268081bcc753778f43f6a0`.
```

### Comparing `types-ldap3-2.9.8/types_ldap3.egg-info/SOURCES.txt` & `types-ldap3-2.9.9/types_ldap3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

